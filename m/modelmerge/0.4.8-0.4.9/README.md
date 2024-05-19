# Comparing `tmp/modelmerge-0.4.8.tar.gz` & `tmp/modelmerge-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.8.tar", last modified: Sun May 19 07:17:37 2024, max compression
+gzip compressed data, was "modelmerge-0.4.9.tar", last modified: Sun May 19 07:22:59 2024, max compression
```

## Comparing `modelmerge-0.4.8.tar` & `modelmerge-0.4.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.182568 modelmerge-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 07:17:28.000000 modelmerge-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:17:37.182568 modelmerge-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 07:17:28.000000 modelmerge-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:17:37.182568 modelmerge-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 07:17:28.000000 modelmerge-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.174568 modelmerge-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.174568 modelmerge-0.4.8/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30558 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/run_python.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.178568 modelmerge-0.4.8/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-19 07:17:28.000000 modelmerge-0.4.8/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.182568 modelmerge-0.4.8/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:17:37.000000 modelmerge-0.4.8/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:17:37.182568 modelmerge-0.4.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_py_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 07:17:28.000000 modelmerge-0.4.8/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.820585 modelmerge-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 07:22:51.000000 modelmerge-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:22:59.820585 modelmerge-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-19 07:22:51.000000 modelmerge-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:22:59.820585 modelmerge-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 07:22:51.000000 modelmerge-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.808585 modelmerge-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30492 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11699 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.812585 modelmerge-0.4.9/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.816585 modelmerge-0.4.9/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-19 07:22:51.000000 modelmerge-0.4.9/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.820585 modelmerge-0.4.9/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:22:59.000000 modelmerge-0.4.9/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.820585 modelmerge-0.4.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 07:22:51.000000 modelmerge-0.4.9/test/test_whisper.py
```

### Comparing `modelmerge-0.4.8/LICENSE` & `modelmerge-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/PKG-INFO` & `modelmerge-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.8
+Version: 0.4.9
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.8/README.md` & `modelmerge-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.9/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,17 +92,14 @@
             "default": [
                 {
                     "role": "system",
                     "content": system_prompt,
                 },
             ],
         }
-        self.tokens_usage = {
-            "default": 0,
-        }
         self.function_calls_counter = {}
         self.function_call_max_loop = 3
         # self.encode_web_text_list = []
 
         if self.get_token_count("default") > self.max_tokens:
             raise Exception("System prompt is too long")
```

### Comparing `modelmerge-0.4.8/src/ModelMerge/models/claude.py` & `modelmerge-0.4.9/src/ModelMerge/models/claude.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,22 +28,25 @@
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
         convo_id: str = "default",
         pass_history: bool = True,
+        total_tokens: int = 0,
     ) -> None:
         """
         Add a message to the conversation
         """
 
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.conversation[convo_id].append({"role": role, "content": message})
+        if total_tokens:
+            self.tokens_usage[convo_id] += total_tokens
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
         self.conversation[convo_id] = claudeConversation()
```

### Comparing `modelmerge-0.4.8/src/ModelMerge/models/config.py` & `modelmerge-0.4.9/src/ModelMerge/models/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
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
         self.function_call_max_loop = 10
 
     def add_to_conversation(
         self,
         message: list,
         role: str,
```

### Comparing `modelmerge-0.4.8/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.9/src/ModelMerge/models/genimi.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,26 @@
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
         convo_id: str = "default",
         pass_history: bool = True,
+        total_tokens: int = 0,
     ) -> None:
         """
         Add a message to the conversation
         """
 
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         # print("message", message)
         self.conversation[convo_id].append({"role": role, "parts": [{"text": message}]})
+        if total_tokens:
+            self.tokens_usage[convo_id] += total_tokens
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
         self.conversation[convo_id] = list()
```

### Comparing `modelmerge-0.4.8/src/ModelMerge/models/groq.py` & `modelmerge-0.4.9/src/ModelMerge/models/groq.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,24 @@
 
     def add_to_conversation(
         self,
         message: str,
         role: str,
         convo_id: str = "default",
         pass_history: bool = True,
+        total_tokens: int = 0,
     ) -> None:
         """
         Add a message to the conversation
         """
         if convo_id not in self.conversation or pass_history == False:
             self.reset(convo_id=convo_id)
         self.conversation[convo_id].append({"role": role, "content": message})
+        if total_tokens:
+            self.tokens_usage[convo_id] += total_tokens
 
     def reset(self, convo_id: str = "default", system_prompt: str = None) -> None:
         """
         Reset the conversation
         """
         self.conversation[convo_id] = list()
```

### Comparing `modelmerge-0.4.8/src/ModelMerge/plugins/image.py` & `modelmerge-0.4.9/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.9/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.9/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.9/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.9/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.9/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.9/src/modelmerge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.8
+Version: 0.4.9
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.8/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.9/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_Web_crawler.py` & `modelmerge-0.4.9/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_claude_zh_char.py` & `modelmerge-0.4.9/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_ddg_search.py` & `modelmerge-0.4.9/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_download_pdf.py` & `modelmerge-0.4.9/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_google_search.py` & `modelmerge-0.4.9/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_jieba.py` & `modelmerge-0.4.9/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_json.py` & `modelmerge-0.4.9/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_langchain_search_old.py` & `modelmerge-0.4.9/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_logging.py` & `modelmerge-0.4.9/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_ollama.py` & `modelmerge-0.4.9/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_py_run.py` & `modelmerge-0.4.9/test/test_py_run.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_tikitoken.py` & `modelmerge-0.4.9/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_token.py` & `modelmerge-0.4.9/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.8/test/test_url.py` & `modelmerge-0.4.9/test/test_url.py`

 * *Files identical despite different names*

