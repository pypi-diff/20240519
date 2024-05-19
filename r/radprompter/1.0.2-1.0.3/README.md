# Comparing `tmp/radprompter-1.0.2.tar.gz` & `tmp/radprompter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.0.2.tar` & `radprompter-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.2/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.2/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.2/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.2/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.2/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.2/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.2/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      643 2024-05-19 14:19:18.563305 radprompter-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      211 2024-05-19 17:46:06.054012 radprompter-1.0.2/radprompter/__init__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.2/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3530 2024-05-14 18:54:06.476384 radprompter-1.0.2/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.2/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9912 2024-05-19 17:42:15.585415 radprompter-1.0.2/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     5653 2024-05-19 17:41:59.516230 radprompter-1.0.2/radprompter/radprompter.py
--rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.2/sample_prompt copy.toml
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.2/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.2/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.2/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.2/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.2/tutorials/.DS_Store
--rw-r--r--   0        0        0    12468 2024-05-19 17:20:45.695903 radprompter-1.0.2/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.2/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.2/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.2/tutorials/4_Using-Schemas/4_Using-Schemas.toml
--rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.2/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.2/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.2/tutorials/README.md
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 radprompter-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.3/.DS_Store
+-rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.3/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.3/Plan.md
+-rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.3/README.md
+-rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.3/demo.ipynb
+-rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.3/demo_no_CoT.ipynb
+-rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.3/demo_prompt_no_CoT.toml
+-rw-r--r--   0        0        0      643 2024-05-19 14:19:18.563305 radprompter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-05-19 17:52:23.317477 radprompter-1.0.3/radprompter/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.3/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.3/radprompter/clients/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.3/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9910 2024-05-19 17:48:35.892191 radprompter-1.0.3/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     5653 2024-05-19 17:41:59.516230 radprompter-1.0.3/radprompter/radprompter.py
+-rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.3/sample_prompt copy.toml
+-rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.3/sample_prompt.toml
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.3/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.3/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.3/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.3/tutorials/.DS_Store
+-rw-r--r--   0        0        0    12468 2024-05-19 17:20:45.695903 radprompter-1.0.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.toml
+-rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.3/tutorials/README.md
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 radprompter-1.0.3/PKG-INFO
```

### Comparing `radprompter-1.0.2/.DS_Store` & `radprompter-1.0.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/.gitignore` & `radprompter-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/LICENSE` & `radprompter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/demo.ipynb` & `radprompter-1.0.3/demo.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/demo_no_CoT.ipynb` & `radprompter-1.0.3/demo_no_CoT.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/demo_prompt_no_CoT.toml` & `radprompter-1.0.3/demo_prompt_no_CoT.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/pyproject.toml` & `radprompter-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/radprompter/clients/clients.py` & `radprompter-1.0.3/radprompter/clients/clients.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def chat_complete(self, messages, stop, max_tokens):
         completion = self.client.chat.completions.create(
             model=self.model,
             messages=messages,
             stream=False,
             seed=self.seed,
             temperature=self.temperature,
-            stop=stop,
+            stop=stop if stop!="" else None,
             top_p=self.top_p,
             frequency_penalty=self.frequency_penalty,
             max_tokens=max_tokens,
         )
         return completion.choices[0].message.content
     
 class vLLMClient(Client):
@@ -56,15 +56,15 @@
     def chat_complete(self, messages, stop, max_tokens):
         completion = self.client.chat.completions.create(
             model=self.model,
             messages=messages,
             stream=False,
             seed=self.seed,
             temperature=self.temperature,
-            stop=stop,
+            stop=stop if stop!="" else None,
             top_p=self.top_p,
             frequency_penalty=self.frequency_penalty,
             max_tokens=max_tokens,
         )
         return completion.choices[0].message.content
     
 class OllamaClient(Client):
@@ -84,13 +84,13 @@
     def chat_complete(self, messages, stop, max_tokens):
         completion = self.client.chat.completions.create(
             model=self.model,
             messages=messages,
             stream=False,
             seed=self.seed,
             temperature=self.temperature,
-            stop=stop,
+            stop=stop if stop!="" else None,
             top_p=self.top_p,
             frequency_penalty=self.frequency_penalty,
             max_tokens=max_tokens,
         )
         return completion.choices[0].message.content
```

### Comparing `radprompter-1.0.2/radprompter/prompts/prompts.py` & `radprompter-1.0.3/radprompter/prompts/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         
         self.schemas = self.get_schemas()
 
         if self.response_templates is None:
             self.response_templates = [""]*self.num_turns
             
         if self.stop_tags is None:
-            self.stop_tags = [None]*self.num_turns        
+            self.stop_tags = [""]*self.num_turns        
         
         if self.debug:
             print(self.num_turns)
         
         assert len(self.user_prompts) == len(self.response_templates) == len(self.stop_tags), "Number of user prompts, response templates, and stop tags should be the same."
     
     def process_schema(self, schema):
```

### Comparing `radprompter-1.0.2/radprompter/radprompter.py` & `radprompter-1.0.3/radprompter/radprompter.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/sample_prompt copy.toml` & `radprompter-1.0.3/sample_prompt copy.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/sample_prompt.toml` & `radprompter-1.0.3/sample_prompt.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/sample_reports/sample_report_1.txt` & `radprompter-1.0.3/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/sample_reports/sample_report_2.txt` & `radprompter-1.0.3/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/sample_reports/sample_report_3.txt` & `radprompter-1.0.3/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/tutorials/.DS_Store` & `radprompter-1.0.3/tutorials/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.0.3/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb` & `radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/tutorials/4_Using-Schemas/4_Using-Schemas.toml` & `radprompter-1.0.3/tutorials/4_Using-Schemas/4_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb` & `radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml` & `radprompter-1.0.3/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.2/PKG-INFO` & `radprompter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Home, https://github.com/BardiaKh/RadPrompter
```

