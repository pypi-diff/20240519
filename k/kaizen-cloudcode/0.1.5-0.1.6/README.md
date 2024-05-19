# Comparing `tmp/kaizen_cloudcode-0.1.5.tar.gz` & `tmp/kaizen_cloudcode-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.5.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.6.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.5.tar` & `kaizen_cloudcode-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-05-16 14:16:30.950943 kaizen_cloudcode-0.1.5/LICENSE
--rw-r--r--   0        0        0     4135 2024-05-16 14:16:30.950943 kaizen_cloudcode-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     3449 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1463 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/helpers/general.py
--rw-r--r--   0        0        0     3631 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     2470 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     3395 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1528 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     1680 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/kaizen/utils/config.py
--rw-r--r--   0        0        0      776 2024-05-16 14:16:30.954943 kaizen_cloudcode-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-18 04:12:58.826722 kaizen_cloudcode-0.1.6/LICENSE
+-rw-r--r--   0        0        0     4135 2024-05-18 04:12:58.826722 kaizen_cloudcode-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1463 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3631 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7183 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     2508 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     4067 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1528 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     2248 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/kaizen/utils/config.py
+-rw-r--r--   0        0        0      776 2024-05-18 04:12:58.830722 kaizen_cloudcode-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     5366 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.6/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.5/LICENSE` & `kaizen_cloudcode-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/README.md` & `kaizen_cloudcode-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/generator/ui.py` & `kaizen_cloudcode-0.1.6/kaizen/generator/ui.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.6/kaizen/helpers/general.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.6/kaizen/helpers/output.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.6/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.6/kaizen/llms/prompts.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.6/kaizen/llms/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import litellm
 from kaizen.llms.prompts import BASIC_SYSTEM_PROMPT
-from kaizen.utils.config import CONFIG_DATA
+from kaizen.utils.config import ConfigData
 
 
 class LLMProvider:
     DEFAULT_MODEL = "gpt-3.5-turbo-1106"
     DEFAULT_MAX_TOKENS = 2000
     DEFAULT_TEMPERATURE = 0
 
@@ -15,14 +15,16 @@
         max_tokens=DEFAULT_MAX_TOKENS,
         temperature=DEFAULT_TEMPERATURE,
     ):
         self.system_prompt = system_prompt
         self.model = model
         self.max_tokens = max_tokens
         self.temperature = temperature
+        CONFIG_DATA = ConfigData()
+        self.config = CONFIG_DATA
         if CONFIG_DATA.get("language_model", {}).get(
             "enable_observability_logging", False
         ):
             # set callbacks
             litellm.success_callback = ["supabase"]
             litellm.failure_callback = ["supabase"]
 
@@ -59,16 +61,14 @@
 
     def update_usage(self, total_usage, current_usage):
         if total_usage is not None:
             total_usage = {
                 key: total_usage[key] + current_usage[key] for key in total_usage
             }
         else:
-            total_usage = {
-                key[0]: current_usage[key[0]] for key in current_usage
-            }
+            total_usage = {key[0]: current_usage[key[0]] for key in current_usage}
         return total_usage
 
     def get_usage_cost(self, total_usage):
         return litellm.cost_per_token(
             self.model, total_usage["prompt_tokens"], total_usage["completion_tokens"]
         )
```

### Comparing `kaizen_cloudcode-0.1.5/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.6/kaizen/reviewer/code_review.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,29 @@
 from kaizen.llms.prompts import (
     CODE_REVIEW_PROMPT,
     CODE_REVIEW_SYSTEM_PROMPT,
     PR_DESCRIPTION_PROMPT,
     FILE_CODE_REVIEW_PROMPT,
 )
 import logging
+from dataclasses import dataclass
+
+
+@dataclass
+class ReviewOutput:
+    review: str
+    usage: dict
+    cost: dict
+
+
+@dataclass
+class DescOutput:
+    desc: str
+    usage: dict
+    cost: dict
 
 
 class CodeReviewer:
     def __init__(self):
         self.logger = logging.getLogger(__name__)
         self.provider = LLMProvider(system_prompt=CODE_REVIEW_SYSTEM_PROMPT)
 
@@ -50,19 +65,26 @@
                         PULL_REQUEST_DESC=pull_request_desc,
                         FILE_PATCH=patch_details,
                     )
                     resp, usage = self.provider.chat_completion(prompt, user=user)
                     total_usage = self.provider.update_usage(total_usage, usage)
                     review_json = parser.extract_json(resp)
                     reviews.extend(review_json["review"])
-        body = output.create_pr_review_from_json(reviews)
-        self.logger.debug(f"Generated Review:\n {body}")
+        review = output.create_pr_review_from_json(reviews)
+        self.logger.debug(f"Generated Review:\n {review}")
         # Share the review on pull request
+        prompt_cost, completion_cost = self.provider.get_usage_cost(
+            total_usage=total_usage
+        )
 
-        return {"review": body, "usage": total_usage}
+        return ReviewOutput(
+            review=review,
+            usage=total_usage,
+            cost={"prompt_cost": prompt_cost, "completion_cost": completion_cost},
+        )
 
     def generate_pull_request_desc(
         self,
         diff_text: str,
         pull_request_title: str,
         pull_request_desc: str,
         user: Optional[str] = None,
@@ -80,8 +102,15 @@
         resp, usage = self.provider.chat_completion(prompt, user=user)
         total_usage = None
         self.logger.debug(f"PROMPT Generate PR Desc RESP: {resp}")
         body = output.create_pr_description(
             parser.extract_json(resp), pull_request_desc
         )
         total_usage = self.provider.update_usage(total_usage, usage)
-        return {"desc": body, "usage": total_usage}
+        prompt_cost, completion_cost = self.provider.get_usage_cost(
+            total_usage=total_usage
+        )
+        return DescOutput(
+            desc=body,
+            usage=total_usage,
+            cost={"prompt_cost": prompt_cost, "completion_cost": completion_cost},
+        )
```

### Comparing `kaizen_cloudcode-0.1.5/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.1.6/kaizen/reviewer/work_summarizer.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.5/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.6/kaizen/utils/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 import json
 import os
 from pathlib import Path
 
 
-def get_config():
-    # Get the directory of the calling function
-    caller_dir = Path(os.path.dirname(os.path.abspath(__file__)))
-    config_file = f"{caller_dir}/config.json"
-    if Path(config_file).is_file():
-        with open(config_file, "r") as f:
-            config_data = json.loads(f.read())
-    else:
-        config_data = {
-            "language_model": {
-                "provider": "litellm",
-                "enable_observability_logging": False,
-            },
-            "github_app": {
-                "check_signature": False,
-                "auto_pr_review": False,
-                "edit_pr_desc": False,
-            },
-        }
-    return config_data
-
-
-def validate_config_settings(config):
-    "Make sure relvant enviorment variables are set"
-    if config.get("github_app", {}).get("check_signature", False):
-        if not os.environ.get("GITHUB_APP_WEBHOOK_SECRET"):
-            raise EnvironmentError(
-                "The environment variable 'GITHUB_APP_WEBHOOK_SECRET' is not set."
-            )
-
-    if config.get("language_model", {}).get("provider", {}) == "litellm":
-        if config.get("language_model", {}).get("enable_observability_logging", False):
-            if not os.environ.get("SUPABASE_URL"):
+class ConfigData:
+    def __init__(self, config_data=None):
+        config_file = "config.json"
+        if Path(config_file).is_file():
+            with open(config_file, "r") as f:
+                self.config_data = json.loads(f.read())
+        else:
+            print(f"Couldnt find config at {config_file} loading default vals")
+            self.config_data = {
+                "language_model": {
+                    "provider": "litellm",
+                    "enable_observability_logging": False,
+                },
+                "github_app": {
+                    "check_signature": False,
+                    "auto_pr_review": False,
+                    "edit_pr_desc": False,
+                },
+            }
+
+        if config_data:
+            self.update_config_data(config_data)
+
+    def update_config_data(self, new_config_data):
+        self.config_data.update(new_config_data)
+        self.validate_config_settings(self.config_data)
+
+    def get_config_data(self):
+        return self.config_data
+
+    def get_language_model_config(self):
+        return self.config_data["language_model"]
+
+    def get_github_app_config(self):
+        return self.config_data["github_app"]
+
+    def validate_config_settings(self):
+        "Make sure relvant enviorment variables are set"
+        if self.config_data.get("github_app", {}).get("check_signature", False):
+            if not os.environ.get("GITHUB_APP_WEBHOOK_SECRET"):
                 raise EnvironmentError(
-                    "The environment variable 'SUPABASE_URL' is not set."
+                    "The environment variable 'GITHUB_APP_WEBHOOK_SECRET' is not set."
                 )
-            if not os.environ.get("SUPABASE_KEY"):
-                raise EnvironmentError(
-                    "The environment variable 'SUPABASE_KEY' is not set."
-                )
-    return config
-
 
-CONFIG_DATA = validate_config_settings(get_config())
+        if self.config_data.get("language_model", {}).get("provider", {}) == "litellm":
+            if self.config_data.get("language_model", {}).get(
+                "enable_observability_logging", False
+            ):
+                if not os.environ.get("SUPABASE_URL"):
+                    raise EnvironmentError(
+                        "The environment variable 'SUPABASE_URL' is not set."
+                    )
+                if not os.environ.get("SUPABASE_KEY"):
+                    raise EnvironmentError(
+                        "The environment variable 'SUPABASE_KEY' is not set."
+                    )
```

### Comparing `kaizen_cloudcode-0.1.5/pyproject.toml` & `kaizen_cloudcode-0.1.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.5"
+version = "0.1.6"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.5/PKG-INFO` & `kaizen_cloudcode-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.5
+Version: 0.1.6
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
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.5 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.6 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

