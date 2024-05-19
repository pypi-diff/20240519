# Comparing `tmp/kaizen_cloudcode-0.1.6.tar.gz` & `tmp/kaizen_cloudcode-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.6.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.7.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.6.tar` & `kaizen_cloudcode-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-18 04:12:58.826722 kaizen_cloudcode-0.1.6/LICENSE
--rw-r--r--   0        0        0     4135 2024-05-18 04:12:58.826722 kaizen_cloudcode-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3449 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1463 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3631 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     2508 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     4067 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1528 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     2248 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/utils/config.py
--rw-r--r--   0        0        0      776 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-19 02:39:48.374902 kaizen_cloudcode-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4135 2024-05-19 02:39:48.374902 kaizen_cloudcode-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1463 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3631 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7183 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     2526 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     4067 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1528 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     2248 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-05-19 02:39:48.378902 kaizen_cloudcode-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.7/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.6/LICENSE` & `kaizen_cloudcode-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/README.md` & `kaizen_cloudcode-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/generator/ui.py` & `kaizen_cloudcode-0.1.7/kaizen/generator/ui.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.7/kaizen/helpers/general.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.7/kaizen/helpers/output.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.7/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.7/kaizen/llms/prompts.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.7/kaizen/llms/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         temperature=DEFAULT_TEMPERATURE,
     ):
         self.system_prompt = system_prompt
         self.model = model
         self.max_tokens = max_tokens
         self.temperature = temperature
         CONFIG_DATA = ConfigData()
-        self.config = CONFIG_DATA
+        self.config = CONFIG_DATA.get_config_data()
         if CONFIG_DATA.get("language_model", {}).get(
             "enable_observability_logging", False
         ):
             # set callbacks
             litellm.success_callback = ["supabase"]
             litellm.failure_callback = ["supabase"]
```

### Comparing `kaizen_cloudcode-0.1.6/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.7/kaizen/reviewer/code_review.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.1.7/kaizen/reviewer/work_summarizer.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.7/kaizen/utils/config.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.6/pyproject.toml` & `kaizen_cloudcode-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.6"
+version = "0.1.7"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.6/PKG-INFO` & `kaizen_cloudcode-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.6
+Version: 0.1.7
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.6 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.7 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

