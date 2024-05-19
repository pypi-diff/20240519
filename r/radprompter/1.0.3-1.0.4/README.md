# Comparing `tmp/radprompter-1.0.3.tar.gz` & `tmp/radprompter-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.0.3.tar` & `radprompter-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.3/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.3/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.3/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.3/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.3/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.3/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.3/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      643 2024-05-19 14:19:18.563305 radprompter-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      211 2024-05-19 17:52:23.317477 radprompter-1.0.3/radprompter/__init__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.3/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.3/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.3/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9910 2024-05-19 17:48:35.892191 radprompter-1.0.3/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     5653 2024-05-19 17:41:59.516230 radprompter-1.0.3/radprompter/radprompter.py
--rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.3/sample_prompt copy.toml
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.3/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.3/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.3/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.3/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.3/tutorials/.DS_Store
--rw-r--r--   0        0        0    12468 2024-05-19 17:20:45.695903 radprompter-1.0.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.toml
--rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.3/tutorials/README.md
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 radprompter-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.4/.DS_Store
+-rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.4/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.4/Plan.md
+-rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.4/README.md
+-rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.4/demo.ipynb
+-rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.4/demo_no_CoT.ipynb
+-rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.4/demo_prompt_no_CoT.toml
+-rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-05-19 18:01:09.276656 radprompter-1.0.4/radprompter/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.4/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.4/radprompter/clients/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.4/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.0.4/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     5653 2024-05-19 17:41:59.516230 radprompter-1.0.4/radprompter/radprompter.py
+-rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.4/sample_prompt copy.toml
+-rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.4/sample_prompt.toml
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.4/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.4/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.4/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.4/tutorials/.DS_Store
+-rw-r--r--   0        0        0    15182 2024-05-19 17:55:30.682856 radprompter-1.0.4/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.4/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.toml
+-rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.4/tutorials/README.md
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.0.4/PKG-INFO
```

### Comparing `radprompter-1.0.3/.DS_Store` & `radprompter-1.0.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/.gitignore` & `radprompter-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/LICENSE` & `radprompter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/demo.ipynb` & `radprompter-1.0.4/demo.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/demo_no_CoT.ipynb` & `radprompter-1.0.4/demo_no_CoT.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/demo_prompt_no_CoT.toml` & `radprompter-1.0.4/demo_prompt_no_CoT.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/pyproject.toml` & `radprompter-1.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 name = "radprompter"
 authors = [{name = "Bardia Khosravi", email = "bardiakhosravi95@gmail.com"}, {name = "Theo Dapamede", email = "theo.dapamede@emory.edu"}]
 maintainers = [{name = "Bardia Khosravi", email = "bardiakhosravi95@gmail.com"}, {name = "Theo Dapamede", email = "theo.dapamede@emory.edu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"]
 dynamic = ["version", "description"]
+dependencies = ["openai"]
 
 [project.urls]
 Home = "https://github.com/BardiaKh/RadPrompter"
```

### Comparing `radprompter-1.0.3/radprompter/clients/clients.py` & `radprompter-1.0.4/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/radprompter/prompts/prompts.py` & `radprompter-1.0.4/radprompter/prompts/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+import os
 import re
 import html
-import pickle
-import datetime
 import tomllib
 import hashlib
 from copy import deepcopy
 
 try: 
     from IPython.display import HTML, display
     from IPython import get_ipython
@@ -13,15 +12,15 @@
     pass
 
 class Prompt:
     def __init__(self, prompt_file, debug=False):
         self.debug = debug
 
         assert prompt_file.endswith(".toml"), "Prompt file should be a TOML file."
-        self.prompt_file = prompt_file
+        self.prompt_file = os.path.abspath(prompt_file)
         self.data, self.raw_data = self.load_toml(self.prompt_file)
         self.md5_hash = hashlib.md5(str(self.data).encode()).hexdigest()
         self.version = self.data["METADATA"]["version"]
 
         self.system_prompt = self.init_constructor_component("system")
         self.user_prompts = self.init_constructor_component("user")
         self.response_templates = self.init_constructor_component("response_templates")
```

### Comparing `radprompter-1.0.3/radprompter/radprompter.py` & `radprompter-1.0.4/radprompter/radprompter.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/sample_prompt copy.toml` & `radprompter-1.0.4/sample_prompt copy.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/sample_prompt.toml` & `radprompter-1.0.4/sample_prompt.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/sample_reports/sample_report_1.txt` & `radprompter-1.0.4/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/sample_reports/sample_report_2.txt` & `radprompter-1.0.4/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/sample_reports/sample_report_3.txt` & `radprompter-1.0.4/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/tutorials/.DS_Store` & `radprompter-1.0.4/tutorials/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb` & `radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.toml` & `radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb` & `radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml` & `radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.3/PKG-INFO` & `radprompter-1.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Dist: openai
 Project-URL: Home, https://github.com/BardiaKh/RadPrompter
 
 # RadPrompter
```

