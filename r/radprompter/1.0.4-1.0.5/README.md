# Comparing `tmp/radprompter-1.0.4.tar.gz` & `tmp/radprompter-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.0.4.tar` & `radprompter-1.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.4/.DS_Store
--rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.4/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.4/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.4/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.4/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.4/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.4/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      211 2024-05-19 18:01:09.276656 radprompter-1.0.4/radprompter/__init__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.4/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.4/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.4/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.0.4/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     5653 2024-05-19 17:41:59.516230 radprompter-1.0.4/radprompter/radprompter.py
--rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.4/sample_prompt copy.toml
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.4/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.4/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.4/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.4/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.4/tutorials/.DS_Store
--rw-r--r--   0        0        0    15182 2024-05-19 17:55:30.682856 radprompter-1.0.4/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.4/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.toml
--rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.4/tutorials/README.md
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.5/.DS_Store
+-rw-r--r--   0        0        0     3169 2024-05-19 17:32:04.647315 radprompter-1.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.5/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.5/Plan.md
+-rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.5/README.md
+-rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.5/demo.ipynb
+-rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.5/demo_no_CoT.ipynb
+-rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.5/demo_prompt_no_CoT.toml
+-rw-r--r--   0        0        0      669 2024-05-19 17:56:30.082674 radprompter-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-05-19 18:05:43.726507 radprompter-1.0.5/radprompter/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.5/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0     3596 2024-05-19 17:51:15.981258 radprompter-1.0.5/radprompter/clients/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.5/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9907 2024-05-19 18:00:58.295860 radprompter-1.0.5/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     5734 2024-05-19 18:05:34.034692 radprompter-1.0.5/radprompter/radprompter.py
+-rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.5/sample_prompt copy.toml
+-rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.5/sample_prompt.toml
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.5/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.5/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.5/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0     6148 2024-05-19 17:05:10.979296 radprompter-1.0.5/tutorials/.DS_Store
+-rw-r--r--   0        0        0    16505 2024-05-19 18:04:24.619631 radprompter-1.0.5/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      387 2024-05-19 16:52:49.209987 radprompter-1.0.5/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    16143 2024-05-19 17:20:53.184090 radprompter-1.0.5/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.5/tutorials/4_Using-Schemas/4_Using-Schemas.toml
+-rw-r--r--   0        0        0    19226 2024-05-19 17:21:00.790174 radprompter-1.0.5/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.5/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.5/tutorials/README.md
+-rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 radprompter-1.0.5/PKG-INFO
```

### Comparing `radprompter-1.0.4/.DS_Store` & `radprompter-1.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/.gitignore` & `radprompter-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/LICENSE` & `radprompter-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/demo.ipynb` & `radprompter-1.0.5/demo.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/demo_no_CoT.ipynb` & `radprompter-1.0.5/demo_no_CoT.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/demo_prompt_no_CoT.toml` & `radprompter-1.0.5/demo_prompt_no_CoT.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/pyproject.toml` & `radprompter-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/radprompter/clients/clients.py` & `radprompter-1.0.5/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/radprompter/prompts/prompts.py` & `radprompter-1.0.5/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/radprompter/radprompter.py` & `radprompter-1.0.5/radprompter/radprompter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from copy import deepcopy
 from tqdm import tqdm
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from .clients import OpenAIClient
 import csv
+from __init__ import __version__
 
 class RadPrompter():
     def __init__(self, client, prompt, output_file, hide_blocks=False, concurrency=1):
         self.client = client
         self.prompt = prompt
         self.hide_blocks = hide_blocks
         self.concurrency = concurrency
@@ -20,14 +21,15 @@
             print(f"WARNING: Output file {self.output_file} already exists. Appending to it. If you want to create a new file, please delete the existing file first or pass a new file name.")
         
         if isinstance(self.client, OpenAIClient) and self.prompt.response_templates.count("") != prompt.num_turns:
             print("WARNING: OpenAI client does not accept response templates and will be ignored.")
             self.prompt.response_templates = [""]*prompt.num_turns
         
         self.log = {
+            "RadPrompter Version": __version__,
             "Model": self.client.model,
             "Prompt TOML": self.prompt.prompt_file,
             "Prompt Version": self.prompt.version,
             "Prompt Hash": self.prompt.md5_hash,
             "Concurrency Factor": self.concurrency,
         }
```

### Comparing `radprompter-1.0.4/sample_prompt copy.toml` & `radprompter-1.0.5/sample_prompt copy.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/sample_prompt.toml` & `radprompter-1.0.5/sample_prompt.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/sample_reports/sample_report_1.txt` & `radprompter-1.0.5/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/sample_reports/sample_report_2.txt` & `radprompter-1.0.5/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/sample_reports/sample_report_3.txt` & `radprompter-1.0.5/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/tutorials/.DS_Store` & `radprompter-1.0.5/tutorials/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.0.5/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956505208972315%*

 * *Differences: {"'cells'": "{12: {'execution_count': 5, 'source': {insert: [(6, '    concurrency=2,\\n')], "*

 * *            "delete: [6]}}, 14: {'execution_count': 6, 'outputs': {0: {'execution_count': 6}}}, "*

 * *            "16: {'execution_count': 7, 'outputs': {0: {'text': ['Processing items: "*

 * *            "100%|██████████| 3/3 [00:00<00:00, 11.23it/s]\\n']}}}, 18: {'execution_count': 8, "*

 * *            "'outputs': {0: {'data': {'text/html': {insert: [(35, '    </tr>\\n'), (36, '    "*

 * *            "<tr>\\n'), (37, '      <th>0< […]*

```diff
@@ -180,50 +180,50 @@
                 "4. `concurrency`: As we are hitting a server with requests, you can batch your requests together for faster processing (Default: `1`). \n",
                 "\n",
                 "Let's instantiate the engine:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from radprompter import RadPrompter\n",
                 "\n",
                 "engine = RadPrompter(\n",
                 "    client=client,\n",
                 "    prompt=prompt, \n",
                 "    output_file=\"output_tutorial_1.csv\",\n",
-                "    concurrency=1,\n",
+                "    concurrency=2,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "To run the engine, we pass it a list of dictionaries. Each dictionary should contain keys matching the placeholders in the prompt. Any additional keys will be included in the output file. \n",
                 "\n",
                 "So let's create a list of our inputs:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "{'report': 'Clinical Information:\\n72-year-old female with sudden onset shortness of breath and hypoxia. Evaluate for pulmonary embolism.\\nTechnique:\\nCT pulmonary angiography with IV contrast was performed.\\nFindings:\\nThere is a large saddle embolus extending from the main pulmonary artery into the right and left main pulmonary arteries. Multiple filling defects are also seen within the segmental and subsegmental branches bilaterally, indicating additional pulmonary emboli.\\nThe right ventricle appears dilated at 4.6 cm, greater than the left ventricle. There is flattening of the interventricular septum, suggesting right heart strain.\\nMosaic perfusion is present within the lungs bilaterally, likely representing pulmonary infarcts.\\nSmall bilateral pleural effusions are noted.\\nImpression:\\n\\nSaddle pulmonary embolism involving the main pulmonary artery, right and left main branches, and multiple segmental/subsegmental branches.\\nFindings of right heart strain with right ventricular dilation and interventricular septal flattening.\\nBilateral pleural effusions, likely due to pulmonary infarcts.\\n\\nRecommendation:\\nEmergent anticoagulation therapy is recommended given the large burden of pulmonary arterial clot and evidence of right heart strain. Surgical or catheter-based embolectomy may need to be considered. Echocardiography can further evaluate right heart function and pulmonary pressures.',\n",
                             " 'file_name': '../../sample_reports/sample_report_2.txt'}"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import glob\n",
                 "\n",
@@ -244,22 +244,22 @@
                 "Now we have a list of 3 reports, each having a `report` key (which on every run will replace the `{{report}}` placeholder in our prompt) and a `file_name` key that will be included in the output csv file for report identification.\n",
                 "\n",
                 "Now let's run our `engine`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00,  7.20it/s]\n"
+                        "Processing items: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 3/3 [00:00<00:00, 11.23it/s]\n"
                     ]
                 }
             ],
             "source": [
                 "engine(reports)"
             ]
         },
@@ -268,15 +268,15 @@
             "metadata": {},
             "source": [
                 "The engine will process each report and save the results to `output_tutorial_1.csv`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -305,50 +305,50 @@
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "      <th></th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>Abnormal</td>\n",
-                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
-                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>Abnormal</td>\n",
                             "      <td>Here is an example radiology report describing...</td>\n",
                             "      <td>../../sample_reports/sample_report_3.txt</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
+                            "      <th>0</th>\n",
+                            "      <td>Abnormal</td>\n",
+                            "      <td>Clinical Information:\\n72-year-old female with...</td>\n",
+                            "      <td>../../sample_reports/sample_report_2.txt</td>\n",
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
-                            "0             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
                             "1             Abnormal  Here is an example radiology report describing...   \n",
+                            "0             Abnormal  Clinical Information:\\n72-year-old female with...   \n",
                             "2             Abnormal  Clinical Information:\\n67-year-old male with s...   \n",
                             "\n",
                             "                                      file_name  \n",
                             "index                                            \n",
-                            "0      ../../sample_reports/sample_report_2.txt  \n",
                             "1      ../../sample_reports/sample_report_3.txt  \n",
+                            "0      ../../sample_reports/sample_report_2.txt  \n",
                             "2      ../../sample_reports/sample_report_1.txt  "
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "import pandas as pd\n",
                 "\n",
@@ -361,19 +361,55 @@
             "metadata": {},
             "source": [
                 "We can also save a log of the run using the `save_log` method:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 38,
+            "execution_count": 9,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Model: meta-llama/Meta-Llama-3-8B-Instruct\n",
+                        "Prompt TOML: /Users/bardiakhosravi/Desktop/GitHub/RadPrompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml\n",
+                        "Prompt Version: 0.1\n",
+                        "Prompt Hash: 369eb088846feaa3e6ea0fdc3a1a40b2\n",
+                        "Concurrency Factor: 2\n",
+                        "Start Time: 2024-05-19 14:03:55\n",
+                        "End Time: 2024-05-19 14:03:56\n",
+                        "Duration: 1.0\n",
+                        "Number of Items: 3\n",
+                        "Average Processing Time: 0.3333333333333333\n",
+                        "\n",
+                        "\n",
+                        "-------------------- *** - Prompt Content - *** --------------------\n",
+                        "[METADATA]\n",
+                        "\n",
+                        "version = 0.1\n",
+                        "description = \"A sample prompt for RadPrompter\"\n",
+                        "\n",
+                        "\n",
+                        "[CONSTRUCTOR]\n",
+                        "system = \"You are an experienced radiologist that help users extract infromation from radiology reports.\"\n",
+                        "user = \"\"\"\"Does the following report indicate a normal or abnormal finding?\n",
+                        "{{report}}\n",
+                        "\n",
+                        "Just reply with \"normal\" or \"abnormal\" to indicate your answer, without any additional information.\n",
+                        "\"\"\"\n"
+                    ]
+                }
+            ],
             "source": [
-                "engine.save_log(\"log_tutorial_1.log\")"
+                "engine.save_log(\"log_tutorial_1.log\")\n",
+                "\n",
+                "with open(\"log_tutorial_1.log\", \"r\") as f:\n",
+                "    print(f.read())"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This will save detailed information about the run, including the prompt used, to the specified file.\n",
```

### Comparing `radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb` & `radprompter-1.0.5/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/tutorials/4_Using-Schemas/4_Using-Schemas.toml` & `radprompter-1.0.5/tutorials/4_Using-Schemas/4_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb` & `radprompter-1.0.5/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml` & `radprompter-1.0.5/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0.4/PKG-INFO` & `radprompter-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.0.4
+Version: 1.0.5
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: openai
 Project-URL: Home, https://github.com/BardiaKh/RadPrompter
```

