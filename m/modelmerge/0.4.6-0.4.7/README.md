# Comparing `tmp/modelmerge-0.4.6.tar.gz` & `tmp/modelmerge-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.6.tar", last modified: Fri May 17 18:13:07 2024, max compression
+gzip compressed data, was "modelmerge-0.4.7.tar", last modified: Sat May 18 17:54:17 2024, max compression
```

## Comparing `modelmerge-0.4.6.tar` & `modelmerge-0.4.7.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.324483 modelmerge-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 18:12:53.000000 modelmerge-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 18:13:07.324483 modelmerge-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 18:12:53.000000 modelmerge-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:13:07.324483 modelmerge-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 18:12:53.000000 modelmerge-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.316483 modelmerge-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.316483 modelmerge-0.4.6/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.320483 modelmerge-0.4.6/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29573 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.320483 modelmerge-0.4.6/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.320483 modelmerge-0.4.6/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.320483 modelmerge-0.4.6/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 18:12:53.000000 modelmerge-0.4.6/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.324483 modelmerge-0.4.6/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 18:13:07.000000 modelmerge-0.4.6/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 18:13:07.000000 modelmerge-0.4.6/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:13:07.000000 modelmerge-0.4.6/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 18:13:07.000000 modelmerge-0.4.6/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 18:13:07.000000 modelmerge-0.4.6/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:13:07.324483 modelmerge-0.4.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 18:12:53.000000 modelmerge-0.4.6/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.841751 modelmerge-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-18 17:54:09.000000 modelmerge-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 17:54:17.841751 modelmerge-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-18 17:54:09.000000 modelmerge-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 17:54:17.841751 modelmerge-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-18 17:54:09.000000 modelmerge-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.833751 modelmerge-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.833751 modelmerge-0.4.7/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.833751 modelmerge-0.4.7/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29998 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.837751 modelmerge-0.4.7/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/run_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.837751 modelmerge-0.4.7/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.837751 modelmerge-0.4.7/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-18 17:54:09.000000 modelmerge-0.4.7/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.841751 modelmerge-0.4.7/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 17:54:17.000000 modelmerge-0.4.7/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 17:54:17.841751 modelmerge-0.4.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_py_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-18 17:54:09.000000 modelmerge-0.4.7/test/test_whisper.py
```

### Comparing `modelmerge-0.4.6/LICENSE` & `modelmerge-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/PKG-INFO` & `modelmerge-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.6
+Version: 0.4.7
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.6/README.md` & `modelmerge-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.7/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,16 @@
                 "frequency_penalty",
                 self.frequency_penalty,
             ),
             "n": kwargs.get("n", self.reply_count),
             "user": role,
         }
         json_post_body.update(copy.deepcopy(body))
+        if all(value == False for value in PLUGINS.values()):
+            return json_post_body
         json_post_body.update(copy.deepcopy(function_call_list["base"]))
         for item in PLUGINS.keys():
             try:
                 # print(item, PLUGINS[item])
                 if PLUGINS[item]:
                     json_post_body["functions"].append(function_call_list[item])
             except:
@@ -362,15 +364,15 @@
         for line in response.iter_lines():
             if not line or line.decode("utf-8").startswith(':'):
                 continue
             # print("line.decode('utf-8')", line.decode("utf-8"))
             if line.decode("utf-8").startswith('data:'):
                 line = line.decode("utf-8")[6:]
             else:
-                print("line", line.decode("utf-8"))
+                # print("line", line.decode("utf-8"))
                 full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
                 yield full_response
                 break
             if line == "[DONE]":
                 break
             resp: dict = json.loads(line)
             # print("resp", resp)
@@ -446,14 +448,18 @@
                         "{}"
                         "</infomation>"
                     ).format(function_response)
                 if function_call_name == "generate_image":
                     prompt = json.loads(function_full_response)["prompt"]
                     function_response = eval(function_call_name)(prompt)
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
+                if function_call_name == "run_python_script":
+                    prompt = json.loads(function_full_response)["code"]
+                    function_response = eval(function_call_name)(prompt)
+                    function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_date_time_weekday":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                 if function_call_name == "get_version_info":
                     function_response = eval(function_call_name)()
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
             else:
```

### Comparing `modelmerge-0.4.6/src/ModelMerge/models/claude.py` & `modelmerge-0.4.7/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/models/config.py` & `modelmerge-0.4.7/src/ModelMerge/models/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 
 from ..utils import prompt
 
 PLUGINS = {
     "SEARCH": (os.environ.get('SEARCH', "True") == "False") == False,
     "URL": True,
+    # "CODE": False,
     "IMAGE": (os.environ.get('IMAGE', "False") == "False") == False,
     "DATE": False,
     "VERSION": False,
     "TARVEL": (os.environ.get('TARVEL', "False") == "False") == False,
 }
 
 LANGUAGE = os.environ.get('LANGUAGE', 'Simplified Chinese')
```

### Comparing `modelmerge-0.4.6/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.7/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/models/groq.py` & `modelmerge-0.4.7/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/plugins/image.py` & `modelmerge-0.4.7/src/ModelMerge/plugins/image.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.7/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.7/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.7/src/ModelMerge/tools/function_call.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,30 @@
                 }
             },
             "required": [
                 "prompt"
             ]
         }
     },
+    "CODE": {
+        "name": "run_python_script",
+        "description": "Convert the string to a Python script and return the Python execution result.",
+        "parameters": {
+            "type": "object",
+            "properties": {
+                "code": {
+                    "type": "string",
+                    "description": "the code to run"
+                }
+            },
+            "required": [
+                "code"
+            ]
+        }
+    },
 }
 def gpt2claude_tools_json(json_dict):
     import copy
     json_dict = copy.deepcopy(json_dict)
     keys_to_change = {
         "parameters": "input_schema",
         "functions": "tools",
```

### Comparing `modelmerge-0.4.6/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.7/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.7/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.7/src/modelmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.6
+Version: 0.4.7
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.6/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.7/src/modelmerge.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/ModelMerge/models/chatgpt.py
 src/ModelMerge/models/claude.py
 src/ModelMerge/models/config.py
 src/ModelMerge/models/genimi.py
 src/ModelMerge/models/groq.py
 src/ModelMerge/plugins/__init__.py
 src/ModelMerge/plugins/image.py
+src/ModelMerge/plugins/run_python.py
 src/ModelMerge/plugins/tarvel.py
 src/ModelMerge/plugins/today.py
 src/ModelMerge/plugins/version.py
 src/ModelMerge/plugins/websearch.py
 src/ModelMerge/tools/__init__.py
 src/ModelMerge/tools/function_call.py
 src/ModelMerge/utils/__init__.py
@@ -32,11 +33,12 @@
 test/test_download_pdf.py
 test/test_google_search.py
 test/test_jieba.py
 test/test_json.py
 test/test_langchain_search_old.py
 test/test_logging.py
 test/test_ollama.py
+test/test_py_run.py
 test/test_tikitoken.py
 test/test_token.py
 test/test_url.py
 test/test_whisper.py
```

### Comparing `modelmerge-0.4.6/test/test_Web_crawler.py` & `modelmerge-0.4.7/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_claude_zh_char.py` & `modelmerge-0.4.7/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_ddg_search.py` & `modelmerge-0.4.7/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_download_pdf.py` & `modelmerge-0.4.7/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_google_search.py` & `modelmerge-0.4.7/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_jieba.py` & `modelmerge-0.4.7/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_json.py` & `modelmerge-0.4.7/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_langchain_search_old.py` & `modelmerge-0.4.7/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_logging.py` & `modelmerge-0.4.7/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_ollama.py` & `modelmerge-0.4.7/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_tikitoken.py` & `modelmerge-0.4.7/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_token.py` & `modelmerge-0.4.7/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.6/test/test_url.py` & `modelmerge-0.4.7/test/test_url.py`

 * *Files identical despite different names*

