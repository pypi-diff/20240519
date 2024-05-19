# Comparing `tmp/radprompter-1.0.8.tar.gz` & `tmp/radprompter-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.0.8.tar` & `radprompter-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.8/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.8/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.8/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.8/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.8/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.8/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.8/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.0.8/radprompter/__init__.py
--rw-r--r--   0        0        0       21 2024-05-19 18:13:07.639856 radprompter-1.0.8/radprompter/__version__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.8/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.8/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.8/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.0.8/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     5738 2024-05-19 18:13:40.081240 radprompter-1.0.8/radprompter/radprompter.py
--rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.8/sample_prompt copy.toml
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.8/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.8/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.8/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.8/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.8/tutorials/.DS_Store
--rw-r--r--   0        0        0    16505 2024-05-19 18:04:24.619631 radprompter-1.0.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.8/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.8/tutorials/4_Using-Schemas/4_Using-Schemas.toml
--rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.8/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.8/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.8/tutorials/README.md
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.9/.DS_Store
+-rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.9/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.9/Plan.md
+-rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.9/README.md
+-rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.9/demo.ipynb
+-rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.9/demo_no_CoT.ipynb
+-rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.9/demo_prompt_no_CoT.toml
+-rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      225 2024-05-19 18:13:05.689042 radprompter-1.0.9/radprompter/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-19 20:35:14.195029 radprompter-1.0.9/radprompter/__version__.py
+-rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.9/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.9/radprompter/clients/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.9/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.0.9/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     7035 2024-05-19 20:35:03.508905 radprompter-1.0.9/radprompter/radprompter.py
+-rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.9/sample_prompt.toml
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.9/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.9/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.9/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0     6148 2024-05-19 19:37:48.126029 radprompter-1.0.9/tutorials/.DS_Store
+-rw-r--r--   0        0        0    16762 2024-05-19 18:51:21.283638 radprompter-1.0.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.0.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    17583 2024-05-19 19:52:03.804859 radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
+-rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.toml
+-rw-r--r--   0        0        0    19012 2024-05-19 19:51:58.516551 radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
+-rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
+-rw-r--r--   0        0        0    26892 2024-05-19 19:51:53.847964 radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.toml
+-rw-r--r--   0        0        0    35817 2024-05-19 20:35:17.292967 radprompter-1.0.9/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     3277 2024-05-19 20:19:42.275696 radprompter-1.0.9/tutorials/05_Assistant-Prefill/05_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.9/tutorials/README.md
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.0.9/PKG-INFO
```

### Comparing `radprompter-1.0.8/.DS_Store` & `radprompter-1.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/.gitignore` & `radprompter-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/LICENSE` & `radprompter-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/demo.ipynb` & `radprompter-1.0.9/demo.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/demo_no_CoT.ipynb` & `radprompter-1.0.9/demo_no_CoT.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/demo_prompt_no_CoT.toml` & `radprompter-1.0.9/demo_prompt_no_CoT.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/pyproject.toml` & `radprompter-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/radprompter/clients/clients.py` & `radprompter-1.0.9/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/radprompter/prompts/prompts.py` & `radprompter-1.0.9/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/radprompter/radprompter.py` & `radprompter-1.0.9/radprompter/radprompter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+import pandas as pd
+import re
 from copy import deepcopy
 from tqdm import tqdm
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor, as_completed
 import csv
 from .clients import OpenAIClient
 from .__version__ import __version__
@@ -119,8 +121,38 @@
             f.write("\n\n")
             f.write("-"*20)
             f.write(" *** - Prompt Content - *** ")
             f.write("-"*20)
             f.write("\n")
             f.write(self.prompt.raw_data)
             
-            f.close()
+            f.close()
+            
+    def sanitize_json(self, variable_name="all"):
+        df = pd.read_csv(self.output_file)
+
+        if variable_name == "all":
+            for schema in self.prompt.schemas.schemas:
+                if schema["type"] == "select":
+                    column_name = f"{schema['variable_name']}_response"
+                    options = schema["options"]
+                    df[column_name] = df[column_name].apply(lambda x: self._sanitize_response(x, options))
+        else:
+            schema = next((s for s in self.prompt.schemas.schemas if s["variable_name"] == variable_name), None)
+            if schema and schema["type"] == "select":
+                column_name = f"{schema['variable_name']}_response"
+                options = schema["options"]
+                df[column_name] = df[column_name].apply(lambda x: self._sanitize_response(x, options))
+
+        return df
+
+    def _sanitize_response(self, response, options):
+        matches = []
+        for option in options:
+            pattern = r'\b' + re.escape(option) + r'\b'
+            if re.search(pattern, response, re.IGNORECASE):
+                matches.append(option)
+
+        if len(matches) == 1:
+            return matches[0]
+        else:
+            return "**RECHECK** " + response
```

### Comparing `radprompter-1.0.8/sample_prompt copy.toml` & `radprompter-1.0.9/sample_prompt.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,27 @@
 description = "A sample prompt for RadPrompter"
 
 [PROMPTS]
 
 system_prompt = "You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements."
 
 user_prompt_intro = """
-{{intro_prompt}}
+Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.
+
+Here is the report:
+<report>
+{{report}}
+</report>
+
+Please pay attention to the following details:
+- Your attention to detail is crucial for maintaining the integrity of the medical records. 
+- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.
+- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.
+- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.
+- Do not print anything else other than the provided output format.
 """
 
 user_prompt_cot = """
 I want you to extract the following data element from the report:
 {{hint}}
 
 After you provide the data element, I will ask you to provide an explanation and then the final answer.
@@ -62,58 +74,56 @@
 <json>
 {
   "{{variable_name}}" : \""""
 
 
 [CONSTRUCTOR]
 system = "rdp(system_prompt)"
-user = "rdp(user_prompt_intro + user_prompt_cot)"
+user = [
+"rdp(user_prompt_intro + user_prompt_cot)"
+,
+"rdp(user_prompt_cot_2nd_turn)"
+]
+stop_tags = [
+"</answer>"
+,
+"</json>"
+]
+response_templates = [
+"<answer>\n<initial_answer>"
+,
+"rdp(assistant_response_template)"
+]
+
 
 [SCHEMAS]
 
 [SCHEMAS.PulmonaryEmbolism]
 variable_name = "Pulmonary Embolism"
-intro_prompt = """
-Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.
-
-Here is the report:
-<report>
-{{report}}
-</report>
-
-Please pay attention to the following details:
-- Your attention to detail is crucial for maintaining the integrity of the medical records. 
-- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.
-- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.
-- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.
-- Do not print anything else other than the provided output format.
-"""
 type = "select"
 options = ["Present", "Absent"]
 hint = """"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. 
 Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved."""
 show_options_in_hint = true
 
 [SCHEMAS.Laterality]
 variable_name = "Laterality"
-intro_prompt = ""
 type = "select"
 options = ["Left", "Right", "Bilateral", "Not Mentioned"]
 hint = """
 Indicate `Left` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. 
 Indicate `Right` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. 
 Indicate `Bilateral` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.
 Indicate `Not Mentioned` if side of pulmonary embolism is not mentioned.
 """
 show_options_in_hint = true
 
 
 [SCHEMAS.Acuity]
 variable_name = "Acuity"
-intro_prompt = ""
 type = "select"
 options = ["Acute", "Chronic", "Mixed", "Not Mentioned"]
 hint = """
 Indicate `Acute` if the report explicitly mentions the patient has an acute pulmonary embolism in their CT scan. 
 Indicate `Chronic` if the report explicitly mentions the patient has a chronic pulmonary embolism in their CT scan. 
 Indicate `Mixed` if the report explicitly mentions the patient has a acute on chronic pulmonary embolism in their CT scan. 
 Indicate `Not Mentioned` if acuity of pulmonary embolism is not mentioned.
```

### Comparing `radprompter-1.0.8/sample_reports/sample_report_1.txt` & `radprompter-1.0.9/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/sample_reports/sample_report_2.txt` & `radprompter-1.0.9/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/sample_reports/sample_report_3.txt` & `radprompter-1.0.9/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.0.9/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944395390785735%*

 * *Differences: {"'cells'": "{16: {'outputs': {0: {'text': ['Processing items: 100%|██████████| 3/3 [00:00<00:00, "*

 * *            "11.13it/s]\\n']}}}, 18: {'outputs': {0: {'data': {'text/html': {insert: [(35, '    "*

 * *            "</tr>\\n'), (36, '    <tr>\\n'), (37, '      <th>1</th>\\n'), (38, '      "*

 * *            "<td>Abnormal</td>\\n'), (39, '      <td>Here is an example radiology report "*

 * *            "describing...</td>\\n'), (40, '      "*

 * *            "<td>../../sample_reports/sample_report_3.txt</td>\\n')], delete: [35, […]*

```diff
@@ -251,15 +251,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 11.23it/s]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 11.13it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "engine(reports)"
             ]
         },
@@ -305,46 +305,46 @@
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>Abnormal</td>\n",
-                            "      <td>Here is an example radiology report describing...</td>\n",
-                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>Abnormal</td>\n",
                             "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
                             "      <td>../../sample_reports/sample_report_2.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
+                            "      <th>1</th>\n",
+                            "      <td>Abnormal</td>\n",
+                            "      <td>Here is an example radiology report describing...</td>\n",
+                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>Abnormal</td>\n",
                             "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
                             "      <td>../../sample_reports/sample_report_1.txt</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "      default_response                                             report  \\\n",
                             "index                                                                       \n",
-                            "1             Abnormal  Here is an example radiology report describing...   \n",
                             "0             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
+                            "1             Abnormal  Here is an example radiology report describing...   \n",
                             "2             Abnormal  Clinical Information:\\n67-year-old male with s...   \n",
                             "\n",
                             "                                      file_name  \n",
                             "index                                            \n",
-                            "1      ../../sample_reports/sample_report_3.txt  \n",
                             "0      ../../sample_reports/sample_report_2.txt  \n",
+                            "1      ../../sample_reports/sample_report_3.txt  \n",
                             "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
@@ -356,36 +356,44 @@
                 "df"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "The column `default_response` will contain the LLM output. In future tutorials, you will learn how to use **Schemas** to further customize your output."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "We can also save a log of the run using the `save_log` method:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "RadPrompter Version: 1.0.8\n",
                         "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
                         "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml\n",
                         "Prompt Version: 0.1\n",
                         "Prompt Hash: 369eb088846feaa3e6ea0fdc3a1a40b2\n",
                         "Concurrency Factor: 2\n",
-                        "Start Time: 2024-05-19 14:03:55\n",
-                        "End Time: 2024-05-19 14:03:56\n",
-                        "Duration: 1.0\n",
+                        "Start Time: 2024-05-19 14:14:28\n",
+                        "End Time: 2024-05-19 14:14:28\n",
+                        "Duration: 0.0\n",
                         "Number of Items: 3\n",
-                        "Average Processing Time: 0.3333333333333333\n",
+                        "Average Processing Time: 0.0\n",
                         "\n",
                         "\n",
                         "-------------------- *** - Prompt Content - *** --------------------\n",
                         "[METADATA]\n",
                         "\n",
                         "version = 0.1\n",
                         "description = \"A sample prompt for RadPrompter\"\n",
```

### Comparing `radprompter-1.0.8/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb` & `radprompter-1.0.9/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8048363940746753%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'# Tutorial 2: `RDP` Templating\\n\'), (2, "In this '*

 * *            "tutorial, we'll explore some of RadPrompter's more advanced prompting features, "*

 * *            'including:\\n"), (4, \'- The `[PROMPTS]` section for defining reusable prompt '*

 * *            "components\\n'), (5, '- The `rdp` operator for composing prompts\\n'), (6, '- Using "*

 * *            "`stop_tags` to control generation')], delete: [4, 2, 0]}}, 1: {'source': ['## "*

 * *            "Prompt\\n', '\\n', ' […]*

```diff
@@ -1,274 +1,238 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Tutorial 4: Schema without Chain of Thought (CoT)\n",
+                "# Tutorial 2: `RDP` Templating\n",
                 "\n",
-                "In this tutorial, we will explore how to use RadPrompter to work with schemas without using Chain of Thought (CoT).\n",
+                "In this tutorial, we'll explore some of RadPrompter's more advanced prompting features, including:\n",
                 "\n",
-                "So let's get started!"
+                "- The `[PROMPTS]` section for defining reusable prompt components\n",
+                "- The `rdp` operator for composing prompts\n",
+                "- Using `stop_tags` to control generation"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 0. Imports"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import os\n",
-                "import pandas as pd\n",
-                "import glob\n",
-                "from radprompter import RadPrompter, Prompt, vLLMClient"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## 1. Load reports"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "report_files = glob.glob(\"../../sample_reports/*.txt\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "reports = []\n",
-                "report_ids = []\n",
-                "for report_file in report_files:\n",
-                "    report_ids.append(os.path.basename(report_file))\n",
-                "    with open(report_file, 'r') as f:\n",
-                "        reports.append(f.read())"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "# 2. Initializing Prompt"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "prompt = Prompt('4_Using-Schemas.toml')"
+                "## Prompt\n",
+                "\n",
+                "As before, we start by importing the `Prompt` class and loading our TOML file:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(255, 224, 178, 0.3);'>{{intro_prompt}}</span>I want you to extract the following data element from the report: <br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{hint}}</span><br><br>Provide a single answer:<br><br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span> </p></div></div>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/plain": []
-                    },
-                    "execution_count": 7,
-                    "metadata": {},
-                    "output_type": "execute_result"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[METADATA]\n",
+                        "\n",
+                        "version = 0.1\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
+                        "\n",
+                        "[PROMPTS]\n",
+                        "\n",
+                        "system_prompt = \"You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.\"\n",
+                        "\n",
+                        "user_prompt_intro = \"\"\"\n",
+                        "Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.\n",
+                        "\n",
+                        "Here is the report:\n",
+                        "<report>\n",
+                        "{{report}}\n",
+                        "</report>\"\"\"\n",
+                        "\n",
+                        "user_prompt_cot = \"\"\"\n",
+                        "I want you to extract the following data element from the report:\n",
+                        "'Pulmonary Embolism'\n",
+                        "Here are your options and you can explicitly use one of these:\n",
+                        "- `Present`\n",
+                        "- `Absent`\n",
+                        "\n",
+                        "Hint: \"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan.\n",
+                        "Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.\n",
+                        "\n",
+                        "After you provide the data element, I will ask you to provide an explanation and then the final answer.\n",
+                        "\n",
+                        "Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:\n",
+                        "\n",
+                        "<answer>\n",
+                        "<initial_answer>\n",
+                        "initial answer goes here\n",
+                        "</initial_answer>\n",
+                        "<explanation>\n",
+                        "1. your first explanation goes here\n",
+                        "2. your second explanation goes here (if needed)\n",
+                        "3. your third explanation goes here (if needed)\n",
+                        "</explanation>\n",
+                        "<final_answer>\n",
+                        "final answer goes here\n",
+                        "</final_answer>\n",
+                        "</answer>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "[CONSTRUCTOR]\n",
+                        "system = \"rdp(system_prompt)\"\n",
+                        "user = \"rdp(user_prompt_intro + user_prompt_cot)\"\n",
+                        "stop_tags = \"</answer>\"\n"
+                    ]
                 }
             ],
             "source": [
-                "prompt"
+                "with open(\"./02_RDP-Templating.toml\", \"r\") as f:\n",
+                "    lines = f.readlines()\n",
+                "print(\"\".join(lines))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We can look at the each schema by passing the index `i`: `prompt.schema[i]`\n",
+                "This TOML file introduces a new section, `[PROMPTS]`, which allows us to define reusable prompt components. In this example, we've defined `system_prompt`, `user_prompt_intro`, and `user_prompt_cot`.\n",
+                "\n",
+                "The `[CONSTRUCTOR]` section then uses these components to build the final prompt:\n",
+                "\n",
+                "```toml\n",
+                "[CONSTRUCTOR]\n",
+                "system = \"rdp(system_prompt)\"\n",
+                "user = \"rdp(user_prompt_intro + user_prompt_cot)\"\n",
+                "stop_tags = \"</answer>\"\n",
+                "```\n",
+                "\n",
+                "The `rdp` operator is used to reference the prompt components. If a plain string is provided instead of `rdp(...)`, that string will be used directly, just like the previous tutorial. But when `rdp` is used, RadPrompter will look up the referenced components in the `[PROMPTS]` section and concatenate them together.\n",
+                "\n",
+                "This allows for a lot of flexibility in composing complex prompts from simpler pieces.\n",
                 "\n",
-                "In this example, we see that the first schema contains the introduction prompt which contains the Radiology report.\n",
+                "The `stop_tags` parameter is used to control generation. When the model outputs the specified tag, generation will halt. This is useful for ensuring the model follows a specific format and doesn't generate irrelevant text.\n",
                 "\n",
-                "It also contains the constraints for the LLM and the first question."
+                "Let's create our prompt object:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Carefully review the provided chest CT report (in the &lt;report&gt; tag). Ensure that each data element is accurately captured.<br><br>Here is the report:<br>&lt;report&gt;<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br>&lt;/report&gt;<br><br>Please pay attention to the following details:<br>- Your attention to detail is crucial for maintaining the integrity of the medical records. <br>- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.<br>- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.<br>- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.<br>- Do not print anything else other than the provided output format.<br>I want you to extract the following data element from the report: <br>&#x27;Pulmonary Embolism&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Present`<br>  - `Absent`<br><br>Hint: Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. <br>Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.<br><br><br>Provide a single answer:<br><br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span> </p></div></div>"
+                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Carefully review the provided chest CT report (in the &lt;report&gt; tag). Ensure that each data element is accurately captured.<br><br>Here is the report:<br>&lt;report&gt;<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br>&lt;/report&gt;I want you to extract the following data element from the report:<br>&#x27;Pulmonary Embolism&#x27;<br>Here are your options and you can explicitly use one of these:<br>- `Present`<br>- `Absent`<br><br>Hint: &quot;Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan.<br>Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.<br><br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br><br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:<br><br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed)<br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/answer&gt;</p></div></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": []
                     },
-                    "execution_count": 8,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "prompt.schemas[0]"
+                "from radprompter import Prompt\n",
+                "\n",
+                "prompt = Prompt(\"./02_RDP-Templating.toml\")\n",
+                "prompt"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Subsequent schemas directly go to the question and hints, as shown below.\n",
-                "\n",
-                "This is because these schemas are not independent from the previous schema."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>I want you to extract the following data element from the report: <br>&#x27;Left&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Yes`<br>  - `No`<br><br>Hint: Indicate `Yes` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. <br>Indicate `Yes` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.<br>Indicate `No` if the report doesn&#x27;t explicitly mentions the patient has a left-sided or bilateral pulmonary embolism in their CT scan. <br><br><br>Provide a single answer:<br><br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span> </p></div></div>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/plain": []
-                    },
-                    "execution_count": 9,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "prompt.schemas[1]"
+                "Notice `</answer>` tag after the model's `[... response ...]` generation. "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 3. Initializing LLM Client and RadPrompter Engine"
+                "## Client & Engine\n",
+                "\n",
+                "We'll use the `vLLMClient` and `RadPrompter` engine as in previous tutorials:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from radprompter import RadPrompter, vLLMClient\n",
+                "\n",
                 "client = vLLMClient(\n",
                 "    model = \"meta-llama/Meta-Llama-3-8B-Instruct\",\n",
                 "    base_url = \"http://localhost:9999/v1\",\n",
                 "    temperature = 0.0,\n",
                 "    seed=42\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                ")\n",
+                "\n",
                 "engine = RadPrompter(\n",
                 "    client=client,\n",
-                "    prompt=prompt,\n",
-                "    concurrency=12,\n",
-                "    hide_blocks=False,\n",
-                "    output_file=\"output_tutorial_4.csv\",\n",
+                "    prompt=prompt, \n",
+                "    output_file=\"output_tutorial_2.csv\",\n",
+                "    concurrency=2,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 4. Run Inference"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "sample = [{'report': sample_report, 'report_id': report_id} for sample_report, report_id in zip(reports, report_ids)]"
+                "And we run it on our sample reports:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items:   0%|          | 0/3 [00:00<?, ?it/s]"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:01<00:00,  1.80it/s]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:06<00:00,  2.11s/it]\n"
                     ]
                 }
             ],
             "source": [
-                "engine(sample)"
+                "import glob\n",
+                "\n",
+                "report_files = glob.glob(\"../../sample_reports/*.txt\")\n",
+                "\n",
+                "reports = []\n",
+                "for file in report_files:\n",
+                "    with open(file, \"r\") as f:\n",
+                "        reports.append({\"report\": f.read(), \"file_name\": file})\n",
+                "\n",
+                "engine(reports)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The engine will process each report using our advanced prompt and save the results to `output_tutorial_2.csv`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -284,146 +248,207 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>Pulmonary Embolism_response</th>\n",
-                            "      <th>Left_response</th>\n",
-                            "      <th>Right_response</th>\n",
-                            "      <th>Acute_response</th>\n",
-                            "      <th>Chronic_response</th>\n",
-                            "      <th>RightHeartStrain_response</th>\n",
-                            "      <th>PulmonaryArteryHypertension_response</th>\n",
+                            "      <th>default_response</th>\n",
                             "      <th>report</th>\n",
-                            "      <th>report_id</th>\n",
+                            "      <th>file_name</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>index</th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
-                            "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>Present</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>No</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>No</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
-                            "      <td>sample_report_1.txt</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>Present</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>No</td>\n",
-                            "      <td>No</td>\n",
-                            "      <td>No</td>\n",
-                            "      <td>No</td>\n",
+                            "      <th>1</th>\n",
+                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nPresent\\n&lt;/initial...</td>\n",
                             "      <td>Here is an example radiology report describing...</td>\n",
-                            "      <td>sample_report_3.txt</td>\n",
+                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>Present</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>No</td>\n",
-                            "      <td>Yes</td>\n",
-                            "      <td>No</td>\n",
+                            "      <th>0</th>\n",
+                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nPresent\\n&lt;/initial...</td>\n",
                             "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
-                            "      <td>sample_report_2.txt</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nPresent\\n&lt;/initial...</td>\n",
+                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
+                            "      <td>../../sample_reports/sample_report_1.txt</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "      Pulmonary Embolism_response Left_response Right_response Acute_response  \\\n",
-                            "index                                                                           \n",
-                            "0                         Present           Yes            Yes             No   \n",
-                            "2                         Present           Yes            Yes             No   \n",
-                            "1                         Present           Yes            Yes            Yes   \n",
-                            "\n",
-                            "      Chronic_response RightHeartStrain_response  \\\n",
-                            "index                                              \n",
-                            "0                  Yes                        No   \n",
-                            "2                   No                        No   \n",
-                            "1                   No                       Yes   \n",
+                            "                                        default_response  \\\n",
+                            "index                                                      \n",
+                            "1      <answer>\\n<initial_answer>\\nPresent\\n</initial...   \n",
+                            "0      <answer>\\n<initial_answer>\\nPresent\\n</initial...   \n",
+                            "2      <answer>\\n<initial_answer>\\nPresent\\n</initial...   \n",
                             "\n",
-                            "      PulmonaryArteryHypertension_response  \\\n",
-                            "index                                        \n",
-                            "0                                      Yes   \n",
-                            "2                                       No   \n",
-                            "1                                       No   \n",
+                            "                                                  report  \\\n",
+                            "index                                                      \n",
+                            "1      Here is an example radiology report describing...   \n",
+                            "0      Clinical Information:\\n72-year-old female with...   \n",
+                            "2      Clinical Information:\\n67-year-old male with s...   \n",
                             "\n",
-                            "                                                  report            report_id  \n",
-                            "index                                                                          \n",
-                            "0      Clinical Information:\\n67-year-old male with s...  sample_report_1.txt  \n",
-                            "2      Here is an example radiology report describing...  sample_report_3.txt  \n",
-                            "1      Clinical Information:\\n72-year-old female with...  sample_report_2.txt  "
+                            "                                      file_name  \n",
+                            "index                                            \n",
+                            "1      ../../sample_reports/sample_report_3.txt  \n",
+                            "0      ../../sample_reports/sample_report_2.txt  \n",
+                            "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "results = pd.read_csv(\"output_tutorial_4.csv\", index_col=0)\n",
-                "results"
+                "import pandas as pd\n",
+                "\n",
+                "df = pd.read_csv(\"output_tutorial_2.csv\", index_col='index')\n",
+                "df"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 15,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "engine.save_log(\"log_tutorial_4.log\")"
+                "**Note**: The `stop_tag` is not returned in the LLM response. If you want that in your csv, you have to include it as a post-hoc measure:\n",
+                "\n",
+                "```python\n",
+                "\n",
+                "df['default_response'] = df['default_response'].apply(lambda x: x+\"</answer>\")\n",
+                "\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "\n",
+                "Finally, we save the log:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 6,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "RadPrompter Version: 1.0.8\n",
+                        "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
+                        "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/02_RDP-Templating/02_RDP-Templating.toml\n",
+                        "Prompt Version: 0.1\n",
+                        "Prompt Hash: b5b6e7cc73163ad0c3024020aa06a0a7\n",
+                        "Concurrency Factor: 2\n",
+                        "Start Time: 2024-05-19 14:36:49\n",
+                        "End Time: 2024-05-19 14:36:55\n",
+                        "Duration: 6.0\n",
+                        "Number of Items: 3\n",
+                        "Average Processing Time: 2.0\n",
+                        "\n",
+                        "\n",
+                        "-------------------- *** - Prompt Content - *** --------------------\n",
+                        "[METADATA]\n",
+                        "\n",
+                        "version = 0.1\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
+                        "\n",
+                        "[PROMPTS]\n",
+                        "\n",
+                        "system_prompt = \"You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.\"\n",
+                        "\n",
+                        "user_prompt_intro = \"\"\"\n",
+                        "Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured.\n",
+                        "\n",
+                        "Here is the report:\n",
+                        "<report>\n",
+                        "{{report}}\n",
+                        "</report>\"\"\"\n",
+                        "\n",
+                        "user_prompt_cot = \"\"\"\n",
+                        "I want you to extract the following data element from the report:\n",
+                        "'Pulmonary Embolism'\n",
+                        "Here are your options and you can explicitly use one of these:\n",
+                        "- `Present`\n",
+                        "- `Absent`\n",
+                        "\n",
+                        "Hint: \"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan.\n",
+                        "Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.\n",
+                        "\n",
+                        "After you provide the data element, I will ask you to provide an explanation and then the final answer.\n",
+                        "\n",
+                        "Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:\n",
+                        "\n",
+                        "<answer>\n",
+                        "<initial_answer>\n",
+                        "initial answer goes here\n",
+                        "</initial_answer>\n",
+                        "<explanation>\n",
+                        "1. your first explanation goes here\n",
+                        "2. your second explanation goes here (if needed)\n",
+                        "3. your third explanation goes here (if needed)\n",
+                        "</explanation>\n",
+                        "<final_answer>\n",
+                        "final answer goes here\n",
+                        "</final_answer>\n",
+                        "</answer>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "[CONSTRUCTOR]\n",
+                        "system = \"rdp(system_prompt)\"\n",
+                        "user = \"rdp(user_prompt_intro + user_prompt_cot)\"\n",
+                        "stop_tags = \"</answer>\"\n"
+                    ]
+                }
+            ],
+            "source": [
+                "engine.save_log(\"log_tutorial_2.log\")\n",
+                "\n",
+                "with open(\"log_tutorial_2.log\", \"r\") as f:\n",
+                "    print(f.read())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "In this tutorial, we've seen how RadPrompter's `[PROMPTS]` section and `rdp` operator allow us to compose complex prompts from simpler components, and how `stop_tags` can be used to control generation. These features provide a lot of power and flexibility in designing prompts for specific tasks."
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "VLLM",
+            "display_name": "Python 3",
             "language": "python",
-            "name": "vllm"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `radprompter-1.0.8/tutorials/4_Using-Schemas/4_Using-Schemas.toml` & `radprompter-1.0.9/tutorials/04_Using-Schemas/04_Using-Schemas.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 [METADATA]
 
 version = 0.1
-description = "A sample prompt for RadPrompter with no CoT"
+description = "A sample prompt for RadPrompter"
 
 [PROMPTS]
 
 system_prompt = "You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements."
 
-user_prompt_intro = "{{intro_prompt}}"
+user_prompt_intro = "{{intro_prompt}}\n"
 
 user_prompt_no_cot = """
 I want you to extract the following data element from the report: 
 {{hint}}
 
 Provide a single answer:
```

### Comparing `radprompter-1.0.8/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb` & `radprompter-1.0.9/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.800218253968254%*

 * *Differences: {"'cells'": '{0: {\'source\': {insert: [(0, \'# Tutorial 3: Multi-turn Prompting\\n\'), (2, "In '*

 * *            "this tutorial, we'll explore RadPrompter's support for multi-turn prompting. This "*

 * *            "allows for more complex interactions with the model, where the model's output from "*

 * *            'one turn can inform the prompt for the next turn.")], delete: [7, 5, 4, 3, 2, 1, '*

 * *            "0]}}, 1: {'source': ['## Prompt\\n', '\\n', 'As usual, we start by importing the "*

 * *            "`Prompt` class […]*

```diff
@@ -1,286 +1,222 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Tutorial 5: Prefill\n",
+                "# Tutorial 3: Multi-turn Prompting\n",
                 "\n",
-                "In this tutorial, we will explore how to use prefils in RadPrompter.\n",
-                "\n",
-                "\n",
-                "Prefils in LLMS (Language Model-based Medical Systems) refer to pre-filled information or context that is provided to the model before generating responses. These prefils can be used to guide the model's behavior and ensure that it generates more accurate and relevant responses.\n",
-                "\n",
-                "By providing prefils, LLMS can be customized to generate responses that align with specific requirements or scenarios. Prefils help in fine-tuning the model's behavior and improving the quality of generated responses."
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## 0. Imports"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import os\n",
-                "import pandas as pd\n",
-                "import glob\n",
-                "from radprompter import RadPrompter, Prompt, vLLMClient"
+                "In this tutorial, we'll explore RadPrompter's support for multi-turn prompting. This allows for more complex interactions with the model, where the model's output from one turn can inform the prompt for the next turn."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 1. Load reports"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "report_files = glob.glob(\"../../sample_reports/*.txt\")"
+                "## Prompt\n",
+                "\n",
+                "As usual, we start by importing the `Prompt` class and loading our TOML file:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "reports = []\n",
-                "report_ids = []\n",
-                "for report_file in report_files:\n",
-                "    report_ids.append(os.path.basename(report_file))\n",
-                "    with open(report_file, 'r') as f:\n",
-                "        reports.append(f.read())"
-            ]
-        },
-        {
-            "cell_type": "markdown",
+            "execution_count": 1,
             "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "[METADATA]\n",
+                        "version = 0.1\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
+                        "\n",
+                        "[PROMPTS]\n",
+                        "system_prompt = \"You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.\"\n",
+                        "\n",
+                        "user_prompt_intro = \"\"\"\n",
+                        "Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured. Here is the report:\n",
+                        "<report>\n",
+                        "{{report}}\n",
+                        "</report>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "user_prompt_cot = \"\"\"\n",
+                        "I want you to extract the following data element from the report: 'Pulmonary Embolism'\n",
+                        "Here are your options and you can explicitly use one of these:\n",
+                        "  - `Present`\n",
+                        "  - `Absent`\n",
+                        "Hint: \"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.\n",
+                        "After you provide the data element, I will ask you to provide an explanation and then the final answer.\n",
+                        "Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer.\n",
+                        "Format your answers with this format as:\n",
+                        "<answer>\n",
+                        "<initial_answer>\n",
+                        "initial answer goes here\n",
+                        "</initial_answer>\n",
+                        "<explanation>\n",
+                        "1. your first explanation goes here\n",
+                        "2. your second explanation goes here (if needed)\n",
+                        "3. your third explanation goes here (if needed) \n",
+                        "</explanation>\n",
+                        "<final_answer>\n",
+                        "final answer goes here\n",
+                        "</final_answer>\n",
+                        "</answer>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "user_prompt_format = \"\"\"\n",
+                        "Great. Now please format your response in JSON format like this:\n",
+                        "{\n",
+                        "    \"answer\": \"your final answer\"\n",
+                        "}\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "[CONSTRUCTOR]\n",
+                        "system = \"rdp(system_prompt)\"\n",
+                        "user = [\"rdp(user_prompt_intro + user_prompt_cot)\", \"rdp(user_prompt_format)\"]\n",
+                        "stop_tags = [\"</answer>\", \"}\"]\n"
+                    ]
+                }
+            ],
             "source": [
-                "# 2. Initializing Prompt"
+                "with open(\"./03_Multiturn-Prompting.toml\", \"r\") as f:\n",
+                "    lines = f.readlines()\n",
+                "print(\"\".join(lines))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Here we load `5_Assistant-Prefill.toml`\n",
-                "\n",
-                "The section to be noted is the following:\n",
-                "\n",
-                "```toml\n",
-                "assistant_response_template = \"\"\"\n",
-                "<json>\n",
-                "{\n",
-                "  \"{{variable_name}}\" : \\\"\"\"\"\n",
-                "```\n",
-                "\n",
-                "This prefill requires the model to generate the outputs with that json syntax.\n",
-                "\n",
-                "We also add a stop tag in the `CONSTRUCTOR` section:\n",
+                "In this TOML file, we've defined our prompt components in the `[PROMPTS]` section as before. The key difference is in the `[CONSTRUCTOR]` section:\n",
                 "\n",
                 "```toml\n",
                 "[CONSTRUCTOR]\n",
                 "system = \"rdp(system_prompt)\"\n",
-                "user = \"rdp(user_prompt_intro + user_prompt_cot)\"\n",
-                "stop_tags = \"</json>\"\n",
+                "user = [\"rdp(user_prompt_intro + user_prompt_cot)\", \"rdp(user_prompt_format)\"]\n",
+                "stop_tags = [\"</answer>\", \"}\"]\n",
                 "```\n",
                 "\n",
-                "This will tell the LLM to stop generating response once it reaches those tags."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 6,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "prompt = Prompt('5_Assistant-Prefill.toml')"
+                "Instead of a single user prompt, we now have a list of two prompts. The first prompt asks the model to extract a data element from the report and provide an explanation, just like in the previous tutorial. The second prompt then asks the model to format its response as JSON.\n",
+                "\n",
+                "We've also updated the `stop_tags` to include both the `</answer>` tag from the first prompt and the `}` character that will end the JSON object in the second prompt.\n",
+                "\n",
+                "Let's create our prompt object:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(255, 224, 178, 0.3);'>{{intro_prompt}}</span><br>I want you to extract the following data element from the report:<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{hint}}</span><br><br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br><br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:<br><br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed)<br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
+                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Carefully review the provided chest CT report (in the &lt;report&gt; tag). Ensure that each data element is accurately captured. Here is the report:<br>&lt;report&gt;<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br>&lt;/report&gt;<br>I want you to extract the following data element from the report: &#x27;Pulmonary Embolism&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Present`<br>  - `Absent`<br>Hint: &quot;Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.<br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer.<br>Format your answers with this format as:<br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed) <br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/answer&gt;</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Great. Now please format your response in JSON format like this:<br>{<br>    &quot;answer&quot;: &quot;your final answer&quot;<br>}<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>}</p></div></div>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": []
                     },
-                    "execution_count": 7,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "from radprompter import Prompt\n",
+                "\n",
+                "prompt = Prompt(\"./03_Multiturn-Prompting.toml\")\n",
                 "prompt"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'>Carefully review the provided chest CT report (in the &lt;report&gt; tag). Ensure that each data element is accurately captured.<br><br>Here is the report:<br>&lt;report&gt;<br><span style='background-color: rgb(255, 224, 178, 0.3);'>{{report}}</span><br>&lt;/report&gt;<br><br>Please pay attention to the following details:<br>- Your attention to detail is crucial for maintaining the integrity of the medical records. <br>- You should not confabulate information, and if something is not mentioned, you should assume that it is `Absent` unless otherwise stated.<br>- The report may contain additional information that is not relevant to the requested data elements. Please ignore that information.<br>- We are interested at findings at the time of scan, not the previous ones, so only consider the impression and findings sections of the report.<br>- Do not print anything else other than the provided output format.<br><br>I want you to extract the following data element from the report:<br>&#x27;Pulmonary Embolism&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Present`<br>  - `Absent`<br><br>Hint: &quot;Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. <br>Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.<br><br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br><br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:<br><br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed)<br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/plain": []
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "prompt.schemas[0]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div style='padding: 0; border-radius: 5px; font-family: Arial; line-height: 1.2rem; border: 1px solid currentColor'><div style='display: flex; align-items: top; padding: 0; border-right-width: 1px'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px; '>System:</h4><p style='margin: 0; padding: 8px; border-left: 1px solid currentColor;'>You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.</p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>User:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><br>I want you to extract the following data element from the report:<br>&#x27;Laterality&#x27;<br>Here are your options and you can explicitly use one of these:<br>  - `Left`<br>  - `Right`<br>  - `Bilateral`<br>  - `Not Mentioned`<br><br>Hint: Indicate `Left` if the report explicitly mentions the patient has a left-sided pulmonary embolism in their CT scan. <br>Indicate `Right` if the report explicitly mentions the patient has a right-sided pulmonary embolism in their CT scan. <br>Indicate `Bilateral` if the report explicitly mentions the patient has a bilateral pulmonary embolism in their CT scan or if patient has both left and right sided pulmonary embolism.<br>Indicate `Not Mentioned` if side of pulmonary embolism is not mentioned.<br><br><br>After you provide the data element, I will ask you to provide an explanation and then the final answer.<br><br>Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer. Format your answers with this format as:<br><br>&lt;answer&gt;<br>&lt;initial_answer&gt;<br>initial answer goes here<br>&lt;/initial_answer&gt;<br>&lt;explanation&gt;<br>1. your first explanation goes here<br>2. your second explanation goes here (if needed)<br>3. your third explanation goes here (if needed)<br>&lt;/explanation&gt;<br>&lt;final_answer&gt;<br>final answer goes here<br>&lt;/final_answer&gt;<br>&lt;/answer&gt;<br></p></div><div style='display: flex; align-items: top; padding: 0;'><h4 style='margin: 0; padding: 8px; flex: 0 0 100px;'>Assistant:</h4><p style='margin: 0; padding: 8px; flex-grow: 1; border-left: 1px solid currentColor;border-top: 1px solid currentColor;'><span style='background-color: rgb(178, 219, 255, 0.3);'>[... response ...]</span>&lt;/json&gt;</p></div></div>"
-                        ],
-                        "text/plain": [
-                            "<IPython.core.display.HTML object>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/plain": []
-                    },
-                    "execution_count": 9,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "prompt.schemas[1]"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 3. Initializing LLM Client and RadPrompter Engine"
+                "## Client & Engine\n",
+                "\n",
+                "We'll use the `vLLMClient` and `RadPrompter` engine as in previous tutorials:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
+                "from radprompter import RadPrompter, vLLMClient\n",
+                "\n",
                 "client = vLLMClient(\n",
                 "    model = \"meta-llama/Meta-Llama-3-8B-Instruct\",\n",
                 "    base_url = \"http://localhost:9999/v1\",\n",
                 "    temperature = 0.0,\n",
                 "    seed=42\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 11,
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                ")\n",
+                "\n",
                 "engine = RadPrompter(\n",
                 "    client=client,\n",
-                "    prompt=prompt,\n",
-                "    concurrency=12,\n",
-                "    hide_blocks=False,\n",
-                "    output_file=\"output_tutorial_5.csv\",\n",
+                "    prompt=prompt, \n",
+                "    output_file=\"output_tutorial_3.csv\",\n",
+                "    concurrency=2,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## 4. Run Inference"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 12,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "sample = [{'report': sample_report, 'report_id': report_id} for sample_report, report_id in zip(reports, report_ids)]"
+                "And we run it on our sample reports:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items:   0%|          | 0/3 [00:00<?, ?it/s]"
-                    ]
-                },
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:09<00:00,  3.01s/it]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:13<00:00,  4.47s/it]\n"
                     ]
                 }
             ],
             "source": [
-                "engine(sample)"
+                "import glob\n",
+                "\n",
+                "report_files = glob.glob(\"../../sample_reports/*.txt\")\n",
+                "\n",
+                "reports = []\n",
+                "for file in report_files:\n",
+                "    with open(file, \"r\") as f:\n",
+                "        reports.append({\"report\": f.read(), \"file_name\": file})\n",
+                "\n",
+                "engine(reports)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The engine will process each report using our multi-turn prompt and save the results to `output_tutorial_3.csv`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -296,126 +232,212 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>Pulmonary Embolism_response</th>\n",
-                            "      <th>Laterality_response</th>\n",
-                            "      <th>Acuity_response</th>\n",
+                            "      <th>default_response_0</th>\n",
+                            "      <th>default_response_1</th>\n",
                             "      <th>report</th>\n",
-                            "      <th>report_id</th>\n",
+                            "      <th>file_name</th>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>index</th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
-                            "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;Present&lt;/Present&gt;\\n&lt;initial_answer&gt;...</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nBilateral\\n&lt;/initi...</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nAcute\\n&lt;/initial_a...</td>\n",
-                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
-                            "      <td>sample_report_1.txt</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
                             "      <td>&lt;answer&gt;\\n&lt;Present&lt;/Present&gt;\\n_initial_answer_...</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nBilateral&lt;/initial...</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nAcute&lt;/initial_ans...</td>\n",
+                            "      <td>{\\n    \"answer\": {\\n        \"data_element\": \"P...</td>\n",
                             "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
-                            "      <td>sample_report_2.txt</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2</th>\n",
+                            "      <th>1</th>\n",
                             "      <td>&lt;answer&gt;\\n&lt;Present&gt;\\n&lt;initial_answer&gt;\\nBased o...</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nBased on the repor...</td>\n",
-                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nBased on the repor...</td>\n",
+                            "      <td>{\\n    \"answer\": {\\n        \"Present\",\\n      ...</td>\n",
                             "      <td>Here is an example radiology report describing...</td>\n",
-                            "      <td>sample_report_3.txt</td>\n",
+                            "      <td>../../sample_reports/sample_report_3.txt</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th>2</th>\n",
+                            "      <td>&lt;answer&gt;\\n&lt;initial_answer&gt;\\nPresent\\n&lt;/initial...</td>\n",
+                            "      <td>{\\n    \"answer\": {\\n        \"initial_answer\": ...</td>\n",
+                            "      <td>Clinical Information:\\n67-year-old male with s...</td>\n",
+                            "      <td>../../sample_reports/sample_report_1.txt</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "                             Pulmonary Embolism_response  \\\n",
+                            "                                      default_response_0  \\\n",
                             "index                                                      \n",
-                            "0      <answer>\\n<Present</Present>\\n<initial_answer>...   \n",
-                            "1      <answer>\\n<Present</Present>\\n_initial_answer_...   \n",
-                            "2      <answer>\\n<Present>\\n<initial_answer>\\nBased o...   \n",
+                            "0      <answer>\\n<Present</Present>\\n_initial_answer_...   \n",
+                            "1      <answer>\\n<Present>\\n<initial_answer>\\nBased o...   \n",
+                            "2      <answer>\\n<initial_answer>\\nPresent\\n</initial...   \n",
                             "\n",
-                            "                                     Laterality_response  \\\n",
+                            "                                      default_response_1  \\\n",
                             "index                                                      \n",
-                            "0      <answer>\\n<initial_answer>\\nBilateral\\n</initi...   \n",
-                            "1      <answer>\\n<initial_answer>\\nBilateral</initial...   \n",
-                            "2      <answer>\\n<initial_answer>\\nBased on the repor...   \n",
+                            "0      {\\n    \"answer\": {\\n        \"data_element\": \"P...   \n",
+                            "1      {\\n    \"answer\": {\\n        \"Present\",\\n      ...   \n",
+                            "2      {\\n    \"answer\": {\\n        \"initial_answer\": ...   \n",
                             "\n",
-                            "                                         Acuity_response  \\\n",
+                            "                                                  report  \\\n",
                             "index                                                      \n",
-                            "0      <answer>\\n<initial_answer>\\nAcute\\n</initial_a...   \n",
-                            "1      <answer>\\n<initial_answer>\\nAcute</initial_ans...   \n",
-                            "2      <answer>\\n<initial_answer>\\nBased on the repor...   \n",
+                            "0      Clinical Information:\\n72-year-old female with...   \n",
+                            "1      Here is an example radiology report describing...   \n",
+                            "2      Clinical Information:\\n67-year-old male with s...   \n",
                             "\n",
-                            "                                                  report            report_id  \n",
-                            "index                                                                          \n",
-                            "0      Clinical Information:\\n67-year-old male with s...  sample_report_1.txt  \n",
-                            "1      Clinical Information:\\n72-year-old female with...  sample_report_2.txt  \n",
-                            "2      Here is an example radiology report describing...  sample_report_3.txt  "
+                            "                                      file_name  \n",
+                            "index                                            \n",
+                            "0      ../../sample_reports/sample_report_2.txt  \n",
+                            "1      ../../sample_reports/sample_report_3.txt  \n",
+                            "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "results = pd.read_csv(\"output_tutorial_5.csv\", index_col=0)\n",
-                "results"
+                "import pandas as pd\n",
+                "\n",
+                "df = pd.read_csv(\"output_tutorial_3.csv\", index_col='index')\n",
+                "df"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 15,
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "As you can see, the `default_response_0` and `default_response_1` columns hold the LLM response to first and second question, respectively. Please note that the `stop_tag` is not returned in the LLM response (see Tutorial 02)."
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "engine.save_log(\"log_tutorial_5.log\")"
+                "Finally, we save the log:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 6,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "RadPrompter Version: 1.0.8\n",
+                        "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
+                        "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml\n",
+                        "Prompt Version: 0.1\n",
+                        "Prompt Hash: 06f66066098813d66e786cbc2d86e6fa\n",
+                        "Concurrency Factor: 2\n",
+                        "Start Time: 2024-05-19 15:10:58\n",
+                        "End Time: 2024-05-19 15:11:11\n",
+                        "Duration: 13.0\n",
+                        "Number of Items: 3\n",
+                        "Average Processing Time: 4.333333333333333\n",
+                        "\n",
+                        "\n",
+                        "-------------------- *** - Prompt Content - *** --------------------\n",
+                        "[METADATA]\n",
+                        "version = 0.1\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
+                        "\n",
+                        "[PROMPTS]\n",
+                        "system_prompt = \"You are a helpful assistant that has 20 years of experience in reading radiology reports and extracting data elements.\"\n",
+                        "\n",
+                        "user_prompt_intro = \"\"\"\n",
+                        "Carefully review the provided chest CT report (in the <report> tag). Ensure that each data element is accurately captured. Here is the report:\n",
+                        "<report>\n",
+                        "{{report}}\n",
+                        "</report>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "user_prompt_cot = \"\"\"\n",
+                        "I want you to extract the following data element from the report: 'Pulmonary Embolism'\n",
+                        "Here are your options and you can explicitly use one of these:\n",
+                        "  - `Present`\n",
+                        "  - `Absent`\n",
+                        "Hint: \"Indicate `Present` if the report explicitly mentions the patient has pulmonary embolism in their CT scan. Indicate `Absent` if pulmonary embolism is not seen or if a previously observed pulmonary embolism is mentioned as resolved.\n",
+                        "After you provide the data element, I will ask you to provide an explanation and then the final answer.\n",
+                        "Now give your initial answer. Then provide a step-by-step explanation based on the information in the report, using no more than three short sentences. You can use less sentences if needed.Try to critically appraise your initial answer, which MIGHT be wrong. Then give me your final answer.\n",
+                        "Format your answers with this format as:\n",
+                        "<answer>\n",
+                        "<initial_answer>\n",
+                        "initial answer goes here\n",
+                        "</initial_answer>\n",
+                        "<explanation>\n",
+                        "1. your first explanation goes here\n",
+                        "2. your second explanation goes here (if needed)\n",
+                        "3. your third explanation goes here (if needed) \n",
+                        "</explanation>\n",
+                        "<final_answer>\n",
+                        "final answer goes here\n",
+                        "</final_answer>\n",
+                        "</answer>\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "user_prompt_format = \"\"\"\n",
+                        "Great. Now please format your response in JSON format like this:\n",
+                        "{\n",
+                        "    \"answer\": \"your final answer\"\n",
+                        "}\n",
+                        "\"\"\"\n",
+                        "\n",
+                        "[CONSTRUCTOR]\n",
+                        "system = \"rdp(system_prompt)\"\n",
+                        "user = [\"rdp(user_prompt_intro + user_prompt_cot)\", \"rdp(user_prompt_format)\"]\n",
+                        "stop_tags = [\"</answer>\", \"}\"]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "engine.save_log(\"log_tutorial_3.log\")\n",
+                "\n",
+                "with open(\"log_tutorial_3.log\", \"r\") as f:\n",
+                "    print(f.read())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "This tutorial introduces the concept of multi-turn prompting, where the `user` parameter in the `[CONSTRUCTOR]` section is a list of prompts instead of a single prompt. The model's output from each prompt is used as context for the next prompt, allowing for more complex interactions.\n",
+                "\n",
+                "The provided TOML file shows an example of a two-turn prompt, where the first turn asks the model to extract a data element and provide an explanation, and the second turn asks the model to format this response as JSON."
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "VLLM",
+            "display_name": "Python 3",
             "language": "python",
-            "name": "vllm"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.8"
+            "version": "3.11.9"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 2
 }
```

### Comparing `radprompter-1.0.8/PKG-INFO` & `radprompter-1.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: openai
 Project-URL: Home, https://github.com/BardiaKh/RadPrompter
```

