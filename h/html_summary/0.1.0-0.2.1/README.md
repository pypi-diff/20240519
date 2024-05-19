# Comparing `tmp/html_summary-0.1.0-py3-none-any.whl.zip` & `tmp/html_summary-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3496 bytes, number of entries: 8
+Zip file size: 3650 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 html_summary/__init__.py
--rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 html_summary/cli.py
--rw-r--r--  2.0 unx     1053 b- defN 80-Jan-01 00:00 html_summary/summary.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 html_summary-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      751 b- defN 80-Jan-01 00:00 html_summary-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 html_summary-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 html_summary-0.1.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 html_summary-0.1.0.dist-info/RECORD
-8 files, 4209 bytes uncompressed, 2360 bytes compressed:  43.9%
+-rw-r--r--  2.0 unx      831 b- defN 80-Jan-01 00:00 html_summary/cli.py
+-rw-r--r--  2.0 unx     1282 b- defN 80-Jan-01 00:00 html_summary/summary.py
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      751 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 html_summary-0.2.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      646 b- defN 16-Jan-01 00:00 html_summary-0.2.1.dist-info/RECORD
+8 files, 4718 bytes uncompressed, 2514 bytes compressed:  46.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: html_summary/cli.py
 Comment: 
 
 Filename: html_summary/summary.py
 Comment: 
 
-Filename: html_summary-0.1.0.dist-info/LICENSE
+Filename: html_summary-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: html_summary-0.1.0.dist-info/METADATA
+Filename: html_summary-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: html_summary-0.1.0.dist-info/WHEEL
+Filename: html_summary-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: html_summary-0.1.0.dist-info/entry_points.txt
+Filename: html_summary-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: html_summary-0.1.0.dist-info/RECORD
+Filename: html_summary-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## html_summary/cli.py

```diff
@@ -1,26 +1,37 @@
 import os
-from tempfile import gettempdir
+import tempfile
 
 import click
 import httpx
 from dotenv import find_dotenv
 from dotenv import load_dotenv
 from loguru import logger
 
 from .summary import summarize_html
 
 
+def fetch_content(path: str) -> str:
+    if path.startswith("http"):
+        resp = httpx.get(url=path)
+        resp.raise_for_status()
+
+        with tempfile.NamedTemporaryFile(delete=False) as fp:
+            fp.write(resp.content)
+            f = fp.name
+    else:
+        f = path
+    return f
+
+
 @click.command()
-@click.argument("url", type=click.STRING)
-def main(url: str) -> None:
+@click.argument("path", type=click.STRING)
+@click.option("-l", "--lang", type=click.STRING, default="English")
+def main(path: str, lang: str) -> None:
     load_dotenv(find_dotenv())
 
-    resp = httpx.get(url=url)
-    resp.raise_for_status()
+    lang = os.getenv("HTML_SUMMARY_LANG", lang)
 
-    f = os.path.join(gettempdir(), "temp.html")
-    with open(f, "wb") as fp:
-        fp.write(resp.content)
+    f = fetch_content(path)
 
-    s = summarize_html(f)
+    s = summarize_html(f, lang)
     logger.info("summarization:\n{}", s)
```

## html_summary/summary.py

```diff
@@ -1,38 +1,43 @@
 import functools
+from pathlib import Path
 
-from langchain.cache import SQLiteCache
 from langchain.chains.llm import LLMChain
 from langchain.globals import set_llm_cache
+from langchain_community.cache import SQLiteCache
 from langchain_community.document_loaders.html_bs import BSHTMLLoader
-from langchain_core.documents import Document
+from langchain_core.messages import AIMessage
 from langchain_core.prompts import PromptTemplate
+from langchain_core.runnables import RunnableSerializable
 from langchain_openai import ChatOpenAI
 from loguru import logger
 
-set_llm_cache(SQLiteCache())
+database_path = Path.home() / ".cache" / ".langchain.db"
+cache = SQLiteCache(database_path.as_posix())
+set_llm_cache(cache)
 
 
-PROMPT_TEMPLATE = """使用台灣用語的繁體中文，幫以下的文章以條列的方式，寫簡潔的摘要：
+PROMPT_TEMPLATE = """Write a concise summary in bullet points using {lang} for the following article:
 {text}
 
-摘要："""
+Summary:"""
 
 
 @functools.cache
-def get_chain() -> LLMChain:
+def get_chain() -> RunnableSerializable:
     llm = ChatOpenAI(temperature=0, model="gpt-4-turbo")
     prompt = PromptTemplate.from_template(PROMPT_TEMPLATE)
-    chain = LLMChain(llm=llm, prompt=prompt)
+    chain = prompt | llm
     return chain
 
 
-def summarize_html(f: str) -> str:
+def summarize_html(f: str, lang: str = "English") -> str:
     logger.info("summarize html: {}", f)
 
     loader = BSHTMLLoader(f)
-    docs: list[Document] = loader.load()
+    docs = loader.load()
 
     text = "\n".join([doc.page_content for doc in docs])
 
     chain = get_chain()
-    return chain.invoke({"text": text})["text"]
+    ai_message: AIMessage = chain.invoke({"text": text, "lang": lang})
+    return ai_message.pretty_repr()
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `html_summary-0.1.0.dist-info/LICENSE` & `html_summary-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `html_summary-0.1.0.dist-info/METADATA` & `html_summary-0.2.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_summary
-Version: 0.1.0
+Version: 0.2.1
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

