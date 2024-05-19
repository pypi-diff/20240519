# Comparing `tmp/modelmerge-0.4.7.tar.gz` & `tmp/modelmerge-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.7.tar", last modified: Sat May 18 17:54:17 2024, max compression
+gzip compressed data, was "modelmerge-0.4.8.tar", last modified: Sun May 19 07:17:37 2024, max compression
```

## Comparing `modelmerge-0.4.7.tar` & `modelmerge-0.4.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.841751 modelmerge-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-18 17:54:09.000000 modelmerge-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 17:54:17.841751 modelmerge-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-18 17:54:09.000000 modelmerge-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 17:54:17.841751 modelmerge-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-18 17:54:09.000000 modelmerge-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.833751 modelmerge-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.833751 modelmerge-0.4.7/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.833751 modelmerge-0.4.7/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29998 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.837751 modelmerge-0.4.7/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.837751 modelmerge-0.4.7/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.837751 modelmerge-0.4.7/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.841751 modelmerge-0.4.7/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.841751 modelmerge-0.4.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.182568 modelmerge-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 07:17:28.000000 modelmerge-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:17:37.182568 modelmerge-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 07:17:28.000000 modelmerge-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:17:37.182568 modelmerge-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 07:17:28.000000 modelmerge-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.174568 modelmerge-0.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.174568 modelmerge-0.4.8/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30558 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.182568 modelmerge-0.4.8/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.182568 modelmerge-0.4.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_whisper.py
```

### Comparing `modelmerge-0.4.7/LICENSE` & `modelmerge-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/PKG-INFO` & `modelmerge-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.7
+Version: 0.4.8
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.7/README.md` & `modelmerge-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.8/src/ModelMerge/models/chatgpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,27 +92,31 @@
             "default": [
                 {
                     "role": "system",
                     "content": system_prompt,
                 },
             ],
         }
+        self.tokens_usage = {
+            "default": 0,
+        }
         self.function_calls_counter = {}
         self.function_call_max_loop = 3
         # self.encode_web_text_list = []
 
         if self.get_token_count("default") > self.max_tokens:
             raise Exception("System prompt is too long")
 
     def add_to_conversation(
         self,
         message: list,
         role: str,
         convo_id: str = "default",
         function_name: str = "",
+        total_tokens: int = 0,
     ) -> None:
         """
         Add a message to the conversation
         """
         if convo_id not in self.conversation:
             self.reset(convo_id=convo_id)
         if function_name == "" and message and message != None:
@@ -120,14 +124,16 @@
         elif function_name != "" and message and message != None:
             self.conversation[convo_id].append({"role": role, "name": function_name, "content": message})
         else:
             print('\033[31m')
             print("error: add_to_conversation message is None or empty")
             print("role", role, "function_name", function_name, "message", message)
             print('\033[0m')
+        if total_tokens:
+            self.tokens_usage[convo_id] += total_tokens
 
     def __truncate_conversation(self, convo_id: str = "default") -> None:
         """
         Truncate the conversation
         """
         while True:
             if (
@@ -309,23 +315,24 @@
         self,
         prompt: list,
         role: str = "user",
         convo_id: str = "default",
         model: str = None,
         pass_history: bool = True,
         function_name: str = "",
+        total_tokens: int = 0,
         **kwargs,
     ):
         """
         Ask a question
         """
         # Make conversation if it doesn't exist
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id, system_prompt=self.system_prompt)
-        self.add_to_conversation(prompt, role, convo_id=convo_id, function_name=function_name)
+        self.add_to_conversation(prompt, role, convo_id=convo_id, function_name=function_name, total_tokens=total_tokens)
         json_post, message_token = self.truncate_conversation(prompt, role, convo_id, model, pass_history, **kwargs)
         # print(self.conversation[convo_id])
         model_max_tokens = kwargs.get("max_tokens", self.max_tokens)
         print("model_max_tokens", model_max_tokens)
         json_post["max_tokens"] = model_max_tokens
         print("api_url", self.api_url.chat_url)
         for _ in range(2):
@@ -357,14 +364,15 @@
         if response.status_code != 200:
             raise Exception(f"{response.status_code} {response.reason} {response.text}")
         response_role: str = None
         full_response: str = ""
         function_full_response: str = ""
         function_call_name: str = ""
         need_function_call: bool = False
+        total_tokens = 0
         for line in response.iter_lines():
             if not line or line.decode("utf-8").startswith(':'):
                 continue
             # print("line.decode('utf-8')", line.decode("utf-8"))
             if line.decode("utf-8").startswith('data:'):
                 line = line.decode("utf-8")[6:]
             else:
@@ -372,28 +380,33 @@
                 full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
                 yield full_response
                 break
             if line == "[DONE]":
                 break
             resp: dict = json.loads(line)
             # print("resp", resp)
+            usage = resp.get("usage")
+            if usage:
+                total_tokens = usage.get("total_tokens") or 0
+                print("total_tokens", total_tokens)
             choices = resp.get("choices")
             if not choices:
                 continue
             delta = choices[0].get("delta")
             if not delta:
                 continue
             if "role" in delta and response_role == None:
                 response_role = delta["role"]
             if "content" in delta and delta["content"]:
                 need_function_call = False
                 content = delta["content"]
                 full_response += content
                 yield content
             if "function_call" in delta:
+                # print(delta["function_call"]["arguments"], end="")
                 need_function_call = True
                 function_call_content = delta["function_call"]["arguments"]
                 if "name" in delta["function_call"]:
                     function_call_name = delta["function_call"]["name"]
                 function_full_response += function_call_content
                 if function_full_response.count("\\n") > 2 or "}" in function_full_response:
                     break
@@ -449,15 +462,15 @@
                         "</infomation>"
                     ).format(function_response)
                 if function_call_name == "generate_image":
                     prompt = json.loads(function_full_response)["prompt"]
                     function_response = eval(function_call_name)(prompt)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "run_python_script":
-                    prompt = json.loads(function_full_response)["code"]
+                    prompt = json.loads(function_full_response)["prompt"]
                     function_response = eval(function_call_name)(prompt)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_version_info":
                     function_response = eval(function_call_name)()
@@ -465,19 +478,19 @@
             else:
                 function_response = "无法找到相关信息，停止使用 tools"
             response_role = "function"
             # print(self.conversation[convo_id][-1])
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
                 # print("Truncate message:", mess)
-            yield from self.ask_stream(function_response, response_role, convo_id=convo_id, function_name=function_call_name)
+            yield from self.ask_stream(function_response, response_role, convo_id=convo_id, function_name=function_call_name, total_tokens=total_tokens)
         else:
             if self.conversation[convo_id][-1]["role"] == "function" and self.conversation[convo_id][-1]["name"] == "get_search_results":
                 mess = self.conversation[convo_id].pop(-1)
-            self.add_to_conversation(full_response, response_role, convo_id=convo_id)
+            self.add_to_conversation(full_response, response_role, convo_id=convo_id, total_tokens=total_tokens)
             self.function_calls_counter = {}
             # self.clear_function_call(convo_id=convo_id)
             # self.encode_web_text_list = []
             # total_tokens = self.get_token_count(convo_id)
 
     async def ask_stream_async(
         self,
```

### Comparing `modelmerge-0.4.7/src/ModelMerge/models/claude.py` & `modelmerge-0.4.8/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/models/config.py` & `modelmerge-0.4.8/src/ModelMerge/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 from ..utils import prompt
 
 PLUGINS = {
     "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
-    # "CODE": False,
+    "CODE": True,
     "IMAGE": (os.environ.get('IMAGE', "False") == "False") == False,
     "DATE": False,
     "VERSION": False,
     "TARVEL": (os.environ.get('TARVEL', "False") == "False") == False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
```

### Comparing `modelmerge-0.4.7/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.8/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/models/groq.py` & `modelmerge-0.4.8/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/plugins/image.py` & `modelmerge-0.4.8/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.8/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.8/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.8/src/ModelMerge/tools/function_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -105,25 +105,25 @@
             "required": [
                 "prompt"
             ]
         }
     },
     "CODE": {
         "name": "run_python_script",
-        "description": "Convert the string to a Python script and return the Python execution result.",
+        "description": "Convert the string to a Python script and return the Python execution result. Assign the result to the variable result. Directly output the code, without using quotation marks or other symbols to enclose the code.",
         "parameters": {
             "type": "object",
             "properties": {
-                "code": {
+                "prompt": {
                     "type": "string",
                     "description": "the code to run"
                 }
             },
             "required": [
-                "code"
+                "prompt"
             ]
         }
     },
 }
 def gpt2claude_tools_json(json_dict):
     import copy
     json_dict = copy.deepcopy(json_dict)
```

### Comparing `modelmerge-0.4.7/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.8/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.8/src/ModelMerge/utils/scripts.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     return encoding, encode_text
 
 def get_text_token_len(text, model_name):
     encoding, encode_text = get_encode_text(text, model_name)
     return len(encode_text)
 
 def cut_message(message: str, max_tokens: int, model_name: str):
+    if type(message) != str:
+        message = str(message)
     encoding, encode_text = get_encode_text(message, model_name)
     if len(encode_text) > max_tokens:
         encode_text = encode_text[:max_tokens]
         message = encoding.decode(encode_text)
     encode_text = encoding.encode(message)
     return message, len(encode_text)
 
@@ -73,14 +75,16 @@
             if "Invalid control character" in str(e):
                 json_data = json_data.replace("\n", "\\n")
             if "Unterminated string starting" in str(e):
                 json_data += '"}'
             if "Expecting ',' delimiter" in str(e):
                 json_data += '}'
             if "Expecting value: line 1 column 1" in str(e):
+                if json_data.startswith("prompt: "):
+                    json_data = json_data.replace("prompt: ", "")
                 json_data = '{"prompt": ' + json.dumps(json_data) + '}'
     return json_data
 
 def is_surrounded_by_chinese(text, index):
     left_char = text[index - 1]
     if 0 < index < len(text) - 1:
         right_char = text[index + 1]
```

### Comparing `modelmerge-0.4.7/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.8/src/modelmerge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.7
+Version: 0.4.8
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.7/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.8/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_Web_crawler.py` & `modelmerge-0.4.8/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_claude_zh_char.py` & `modelmerge-0.4.8/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_ddg_search.py` & `modelmerge-0.4.8/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_download_pdf.py` & `modelmerge-0.4.8/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_google_search.py` & `modelmerge-0.4.8/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_jieba.py` & `modelmerge-0.4.8/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_json.py` & `modelmerge-0.4.8/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_langchain_search_old.py` & `modelmerge-0.4.8/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_logging.py` & `modelmerge-0.4.8/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_ollama.py` & `modelmerge-0.4.8/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_tikitoken.py` & `modelmerge-0.4.8/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_token.py` & `modelmerge-0.4.8/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.7/test/test_url.py` & `modelmerge-0.4.8/test/test_url.py`

 * *Files identical despite different names*

