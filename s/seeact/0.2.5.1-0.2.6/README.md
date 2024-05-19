# Comparing `tmp/seeact-0.2.5.1.tar.gz` & `tmp/seeact-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeact-0.2.5.1.tar", last modified: Wed May  1 01:20:55 2024, max compression
+gzip compressed data, was "seeact-0.2.6.tar", last modified: Sat May 18 19:37:04 2024, max compression
```

## Comparing `seeact-0.2.5.1.tar` & `seeact-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.034831 seeact-0.2.5.1/
--rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.5.1/LICENSE
--rw-r--r--   0 geminigby   (501) staff       (20)    13354 2024-05-01 01:20:55.034534 seeact-0.2.5.1/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)     1125 2024-05-01 01:20:06.000000 seeact-0.2.5.1/pyproject.toml
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.031171 seeact-0.2.5.1/seeact/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    32246 2024-04-29 22:20:31.000000 seeact-0.2.5.1/seeact/agent.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.032922 seeact-0.2.5.1/seeact/data_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/data_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-05-01 01:16:18.000000 seeact-0.2.5.1/seeact/data_utils/format_prompt_utils.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/data_utils/prompts.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.033893 seeact-0.2.5.1/seeact/demo_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/demo_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    13193 2024-04-29 00:45:49.000000 seeact-0.2.5.1/seeact/demo_utils/browser_helper.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7554 2024-05-01 01:16:18.000000 seeact-0.2.5.1/seeact/demo_utils/format_prompt.py
--rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/demo_utils/inference_engine.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.034236 seeact-0.2.5.1/seeact.egg-info/
--rw-r--r--   0 geminigby   (501) staff       (20)    13354 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/SOURCES.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/dependency_links.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/requires.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/top_level.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-05-01 01:20:55.034879 seeact-0.2.5.1/setup.cfg
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.756636 seeact-0.2.6/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    11495 2024-05-02 03:19:33.000000 seeact-0.2.6/LICENSE
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    13402 2024-05-18 19:37:04.756636 seeact-0.2.6/PKG-INFO
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     1157 2024-05-18 19:35:59.000000 seeact-0.2.6/pyproject.toml
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.284967 seeact-0.2.6/seeact/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)      607 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/__init__.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    32103 2024-05-18 19:01:37.000000 seeact-0.2.6/seeact/agent.py
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.426487 seeact-0.2.6/seeact/data_utils/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)      607 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/data_utils/__init__.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     4278 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/data_utils/format_prompt_utils.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     7487 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/data_utils/prompts.py
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.725376 seeact-0.2.6/seeact/demo_utils/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/demo_utils/__init__.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    13193 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/demo_utils/browser_helper.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     7554 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/demo_utils/format_prompt.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    12993 2024-05-18 19:01:37.000000 seeact-0.2.6/seeact/demo_utils/inference_engine.py
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.741011 seeact-0.2.6/seeact.egg-info/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    13402 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/PKG-INFO
+-rwxrwxrwx   0 demo      (1000) demo      (1000)      445 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/SOURCES.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)        1 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/dependency_links.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)       97 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/requires.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)        7 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/top_level.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)       38 2024-05-18 19:37:04.756636 seeact-0.2.6/setup.cfg
```

### Comparing `seeact-0.2.5.1/LICENSE` & `seeact-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/PKG-INFO` & `seeact-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.5.1
+Version: 0.2.6
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
-Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
+Author-email: Boyu Gou <gou.43@osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
         
         Copyright (c) 2024 OSU Natural Language Processing Group
         
@@ -121,9 +121,11 @@
 Project-URL: documentation, https://github.com/OSU-NLP-Group/SeeAct
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff
 Requires-Dist: playwright
 Requires-Dist: toml
-Requires-Dist: openai==0.27.8
+Requires-Dist: openai==1.24.0
+Requires-Dist: litellm==1.35.32
+Requires-Dist: google-generativeai==0.5.2
 Requires-Dist: python-dotenv
```

### Comparing `seeact-0.2.5.1/pyproject.toml` & `seeact-0.2.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seeact"
-version = "0.2.5.1"
+version = "0.2.6"
 description = "SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents."
 authors = [
-    {name = "Boyu Gou", email = "gou.43@buckeyemail.osu.edu"},
+    {name = "Boyu Gou", email = "gou.43@osu.edu"},
     {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"},
-    {name = "Zheng Du", email = "du.913@buckeyemail.osu.edu"}
+    {name = "Zheng Du", email = "du.913@osu.edu"}
 ]
 license = {file="LICENSE"}
 readme = "https://github.com/OSU-NLP-Group/SeeAct/blob/main/README.md"
 requires-python = ">=3.9"
 
 dependencies = [
     "backoff",
     "playwright",
     "toml",
-    "openai==0.27.8",
+    "openai==1.24.0",
+    "litellm==1.35.32",
+    "google-generativeai==0.5.2",
     "python-dotenv"
 ]
 
 [project.urls]
 homepage = "https://osu-nlp-group.github.io/SeeAct/"
 repository = "https://github.com/OSU-NLP-Group/SeeAct"
 documentation = "https://github.com/OSU-NLP-Group/SeeAct"
```

### Comparing `seeact-0.2.5.1/seeact/__init__.py` & `seeact-0.2.6/seeact/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/seeact/agent.py` & `seeact-0.2.6/seeact/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,20 @@
 from playwright.async_api import async_playwright,Locator
 
 from .data_utils.format_prompt_utils import get_index_from_option_name, generate_new_query_prompt, \
     generate_new_referring_prompt, format_options
 from .demo_utils.browser_helper import normal_launch_async, normal_new_context_async, \
     get_interactive_elements_with_playwright, select_option, saveconfig
 from .demo_utils.format_prompt import format_choices, postprocess_action_lmm
-from .demo_utils.inference_engine import OpenAIEngine, load_openai_api_key
+from .demo_utils.inference_engine import engine_factory, load_openai_api_key
 
 
 class SeeActAgent:
     def __init__(self,
                  config_path=None,
-                 openai_key=None,
                  save_file_dir="seeact_agent_files",
                  default_task='Find the pdf of the paper "GPT-4V(ision) is a Generalist Web Agent, if Grounded"',
                  default_website="https://www.google.com/",
                  input_info=["screenshot"],
                  grounding_strategy="text_choice",
                  max_auto_op=50,
                  max_continuous_no_op=5,
@@ -91,15 +90,14 @@
                         "persistant_user_path": persistant_user_path,
                         "save_video": save_video,
                         "viewport": viewport,
                         "tracing": tracing,
                         "trace": trace
                     },
                     "openai": {
-                        "api_key": load_openai_api_key() if not openai_key else openai_key,
                         "rate_limit": rate_limit,
                         "model": model,
                         "temperature": temperature
                     }
                 }
 
         except FileNotFoundError:
@@ -139,15 +137,15 @@
         self.logger = self._setup_logger(redirect_to_dev_log=False)
         # self.dev_logger = self._setup_dev_logger()
 
         # # Redirect primary logger messages to dev_logger as well
         # for handler in self.logger.handlers:
         #     self.dev_logger.addHandler(handler)
 
-        self.openai_engine = OpenAIEngine(**self.config['openai'])
+        self.engine = engine_factory(**self.config['openai'])
         self.taken_actions = []
         self.prompts = self._initialize_prompts()
         self.time_step = 0
         self.valid_op = 0
         # self.error=0
         self.continuous_no_op = 0
         self.predictions=[]
@@ -521,15 +519,15 @@
         self.logger.info(f"Step - {self.time_step}\n{'-'*terminal_width}\nAction Generation ➡️")
         # for prompt_part in prompt:
         self.logger.info("TASK: "+self.tasks[-1])
         self.logger.info("Previous:")
         for action in self.taken_actions:
             self.logger.info(action)
 
-        output0 = self.openai_engine.generate(prompt=prompt, image_path=screenshot_path, turn_number=0)
+        output0 = self.engine.generate(prompt=prompt, image_path=screenshot_path, turn_number=0)
 
         terminal_width = 10
         self.logger.info("-" * terminal_width)
         self.logger.info("🤖 Action Generation Output 🤖")
 
         for line in output0.split('\n'):
             self.logger.info(line)
@@ -540,15 +538,15 @@
         choice_text = f"Action Grounding ➡️" + "\n" + format_options(
             choices)
         choice_text = choice_text.replace("\n\n", "")
 
         for line in choice_text.split('\n'):
             self.logger.info(line)
 
-        output = self.openai_engine.generate(prompt=prompt, image_path=screenshot_path, turn_number=1,
+        output = self.engine.generate(prompt=prompt, image_path=screenshot_path, turn_number=1,
                                              ouput_0=output0)
         self.logger.info("🤖 Action Grounding Output 🤖")
         for line in output.split('\n'):
             self.logger.info(line)
 
         pred_element_label, pred_action, pred_value = postprocess_action_lmm(output)
```

### Comparing `seeact-0.2.5.1/seeact/data_utils/__init__.py` & `seeact-0.2.6/seeact/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/seeact/data_utils/format_prompt_utils.py` & `seeact-0.2.6/seeact/data_utils/format_prompt_utils.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/seeact/data_utils/prompts.py` & `seeact-0.2.6/seeact/data_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/seeact/demo_utils/browser_helper.py` & `seeact-0.2.6/seeact/demo_utils/browser_helper.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/seeact/demo_utils/format_prompt.py` & `seeact-0.2.6/seeact/demo_utils/format_prompt.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5.1/seeact/demo_utils/inference_engine.py` & `seeact-0.2.6/seeact/demo_utils/inference_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,190 +13,297 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import time
 
 import backoff
 import openai
-from openai.error import (
+from openai import (
     APIConnectionError,
     APIError,
     RateLimitError,
-    ServiceUnavailableError,
-    InvalidRequestError
 )
+import requests
 from dotenv import load_dotenv
-
+import litellm
 import base64
 
-def load_openai_api_key(api_key=None):
+EMPTY_API_KEY="Your API KEY Here"
+
+def load_openai_api_key():
     load_dotenv()
     assert (
-            os.getenv("OPENAI_API_KEY", api_key) is not None
+            os.getenv("OPENAI_API_KEY") is not None and
+            os.getenv("OPENAI_API_KEY") != EMPTY_API_KEY
     ), "must pass on the api_key or set OPENAI_API_KEY in the environment"
-    if api_key is None:
-        api_key = os.getenv("OPENAI_API_KEY", api_key)
-    if isinstance(api_key, str):
-        return [api_key]
-    elif isinstance(api_key, list):
-        return api_key
-    else:
-        raise ValueError("api_key must be a string or list")
+    return os.getenv("OPENAI_API_KEY")
+
+
+def load_gemini_api_key():
+    load_dotenv()
+    assert (
+            os.getenv("GEMINI_API_KEY") is not None and
+            os.getenv("GEMINI_API_KEY") != EMPTY_API_KEY
+    ), "must pass on the api_key or set GEMINI_API_KEY in the environment"
+    return os.getenv("GEMINI_API_KEY")
 
 def encode_image(image_path):
     with open(image_path, "rb") as image_file:
         return base64.b64encode(image_file.read()).decode('utf-8')
 
 
-class Engine:
-    def __init__(self) -> None:
-        pass
-
-    def tokenize(self, input):
-        return self.tokenizer(input)
-
+def engine_factory(api_key=None, model=None, **kwargs):
+    model = model.lower()
+    if model in ["gpt-4-vision-preview", "gpt-4-turbo", "gpt-4o"]:
+        if api_key and api_key != EMPTY_API_KEY:
+            os.environ["OPENAI_API_KEY"] = api_key
+        else:
+            load_openai_api_key()
+        return OpenAIEngine(model=model, **kwargs)
+    elif model in ["gemini-1.5-pro-latest", "gemini-1.5-flash"]:
+        if api_key and api_key != EMPTY_API_KEY:
+            os.environ["GEMINI_API_KEY"] = api_key
+        else:
+            load_gemini_api_key()
+        model=f"gemini/{model}"
+        return GeminiEngine(model=model, **kwargs)
+    elif model == "llava":
+        model="llava"
+        return OllamaEngine(model=model, **kwargs)
+    raise Exception(f"Unsupported model: {model}, currently supported models: \
+                    gpt-4-vision-preview, gpt-4-turbo, gemini-1.5-pro-latest, llava")
 
-class OpenAIEngine(Engine):
+class Engine:
     def __init__(
             self,
-            api_key=None,
             stop=["\n\n"],
             rate_limit=-1,
-            model='gpt-4-vision-preview',
-            temperature=0.9,
+            model=None,
+            temperature=0,
             **kwargs,
     ) -> None:
-        """Init an OpenAI GPT/Codex engine
+        """
+            Base class to init an engine
 
         Args:
             api_key (_type_, optional): Auth key from OpenAI. Defaults to None.
             stop (list, optional): Tokens indicate stop of sequence. Defaults to ["\n"].
             rate_limit (int, optional): Max number of requests per minute. Defaults to -1.
             model (_type_, optional): Model family. Defaults to None.
         """
-        self.api_keys = load_openai_api_key(api_key)
+        self.time_slots = [0]
         self.stop = stop
         self.temperature = temperature
         self.model = model
         # convert rate limit to minmum request interval
         self.request_interval = 0 if rate_limit == -1 else 60.0 / rate_limit
-        self.next_avil_time = [0] * len(self.api_keys)
+        self.next_avil_time = [0] * len(self.time_slots)
         self.current_key_idx = 0
-        Engine.__init__(self, **kwargs)
+        print(f"Initializing model {self.model}")        
+
+    def tokenize(self, input):
+        return self.tokenizer(input)
+
+
+class OllamaEngine(Engine):
+    def __init__(self, **kwargs) -> None:
+        """
+            Init an Ollama engine
+            To use Ollama, dowload and install Ollama from https://ollama.com/
+            After Ollama start, pull llava with command: ollama pull llava
+        """
+        super().__init__(**kwargs)
+        self.api_url = "http://localhost:11434/api/chat"
+
 
-    def encode_image(self, image_path):
-        with open(self, image_path, "rb") as image_file:
-            return base64.b64encode(image_file.read()).decode('utf-8')
-
-    # @backoff.on_exception(
-    #     backoff.expo,
-    #     (APIError, RateLimitError, APIConnectionError, ServiceUnavailableError, InvalidRequestError),
-    # )
     def generate(self, prompt: list = None, max_new_tokens=4096, temperature=None, model=None, image_path=None,
                  ouput_0=None, turn_number=0, **kwargs):
-        self.current_key_idx = (self.current_key_idx + 1) % len(self.api_keys)
+        self.current_key_idx = (self.current_key_idx + 1) % len(self.time_slots)
+        start_time = time.time()
+        if (
+                self.request_interval > 0
+                and start_time < self.next_avil_time[self.current_key_idx]
+        ):
+            wait_time = self.next_avil_time[self.current_key_idx] - start_time
+            print(f"Wait {wait_time} for rate limitting")
+            time.sleep(wait_time)
+        prompt0, prompt1, prompt2 = prompt
+
+        base64_image = encode_image(image_path)
+        if turn_number == 0:
+            # Assume one turn dialogue
+            prompt_input = [
+                {"role": "assistant", "content": prompt0},
+                {"role": "user", "content": prompt1, "images": [f"{base64_image}"]},
+            ]
+        elif turn_number == 1:
+            prompt_input = [
+                {"role": "assistant", "content": prompt0},
+                {"role": "user", "content": prompt1, "images": [f"{base64_image}"]},
+                {"role": "assistant", "content": f"\n\n{ouput_0}"},
+                {"role": "user", "content": prompt2}, 
+            ]
+
+        options = {"temperature": self.temperature, "num_predict": max_new_tokens}
+        data = {
+            "model": self.model,
+            "messages": prompt_input,
+            "options": options,
+            "stream": False,
+        }
+        _request = {
+            "url": f"{self.api_url}",
+            "json": data,
+        }
+        response = requests.post(**_request)  # type: ignore
+        if response.status_code != 200:
+            raise Exception(f"Ollama API Error: {response.status_code}, {response.text}")
+        response_json = response.json()
+        return response_json["message"]["content"]
+
+
+class GeminiEngine(Engine):
+    def __init__(self, **kwargs) -> None:
+        """
+            Init a Gemini engine
+            To use this engine, please provide the GEMINI_API_KEY in the environment
+            Supported Model             Rate Limit
+            gemini-1.5-pro-latest    	2 queries per minute, 1000 queries per day
+        """
+        super().__init__(**kwargs)
+
+
+    def generate(self, prompt: list = None, max_new_tokens=4096, temperature=None, model=None, image_path=None,
+                 ouput_0=None, turn_number=0, **kwargs):
+        self.current_key_idx = (self.current_key_idx + 1) % len(self.time_slots)
+        start_time = time.time()
+        if (
+                self.request_interval > 0
+                and start_time < self.next_avil_time[self.current_key_idx]
+        ):
+            wait_time = self.next_avil_time[self.current_key_idx] - start_time
+            print(f"Wait {wait_time} for rate limitting")
+        prompt0, prompt1, prompt2 = prompt
+        litellm.set_verbose=True
+
+        base64_image = encode_image(image_path)
+        if turn_number == 0:
+            # Assume one turn dialogue
+            prompt_input = [
+                {"role": "system", "content": prompt0},
+                {"role": "user",
+                 "content": [{"type": "text", "text": prompt1}, {"type": "image_url", "image_url": {"url": image_path,
+                                                                                                    "detail": "high"},
+                                                                }]},
+            ]
+        elif turn_number == 1:
+            prompt_input = [
+                {"role": "system", "content": prompt0},
+                {"role": "user",
+                 "content": [{"type": "text", "text": prompt1}, {"type": "image_url", "image_url": {"url": image_path,
+                                                                                                    "detail": "high"}, 
+                                                                }]},
+                {"role": "assistant", "content": [{"type": "text", "text": f"\n\n{ouput_0}"}]},
+                {"role": "user", "content": [{"type": "text", "text": prompt2}]}, 
+            ]
+        response = litellm.completion(
+            model=model if model else self.model,
+            messages=prompt_input,
+            max_tokens=max_new_tokens if max_new_tokens else 4096,
+            temperature=temperature if temperature else self.temperature,
+            **kwargs,
+        )
+        return [choice["message"]["content"] for choice in response.choices][0]
+
+
+class OpenAIEngine(Engine):
+    def __init__(self, **kwargs) -> None:
+        """
+            Init an OpenAI GPT/Codex engine
+            To find your OpenAI API key, visit https://platform.openai.com/api-keys
+        """
+        super().__init__(**kwargs)
+
+    @backoff.on_exception(
+        backoff.expo,
+        (APIError, RateLimitError, APIConnectionError),
+    )
+    def generate(self, prompt: list = None, max_new_tokens=4096, temperature=None, model=None, image_path=None,
+                 ouput_0=None, turn_number=0, **kwargs):
+        self.current_key_idx = (self.current_key_idx + 1) % len(self.time_slots)
         start_time = time.time()
         if (
                 self.request_interval > 0
                 and start_time < self.next_avil_time[self.current_key_idx]
         ):
             time.sleep(self.next_avil_time[self.current_key_idx] - start_time)
-        openai.api_key = self.api_keys[self.current_key_idx]
-        prompt0 = prompt[0]
-        prompt1 = prompt[1]
-        prompt2 = prompt[2]
+        prompt0, prompt1, prompt2 = prompt
+        # litellm.set_verbose=True
 
+        base64_image = encode_image(image_path)
         if turn_number == 0:
-            base64_image = encode_image(image_path)
             # Assume one turn dialogue
-            prompt1_input = [
+            prompt_input = [
                 {"role": "system", "content": [{"type": "text", "text": prompt0}]},
                 {"role": "user",
                  "content": [{"type": "text", "text": prompt1}, {"type": "image_url", "image_url": {"url":
                                                                                                         f"data:image/jpeg;base64,{base64_image}",
                                                                                                     "detail": "high"},
                                                                  }]},
             ]
-            response1 = openai.ChatCompletion.create(
-                model=model if model else self.model,
-                messages=prompt1_input,
-                max_tokens=max_new_tokens if max_new_tokens else 4096,
-                temperature=temperature if temperature else self.temperature,
-                **kwargs,
-            )
-            answer1 = [choice["message"]["content"] for choice in response1["choices"]][0]
-
-            return answer1
         elif turn_number == 1:
-            base64_image = encode_image(image_path)
-            prompt2_input = [
+            prompt_input = [
                 {"role": "system", "content": [{"type": "text", "text": prompt0}]},
                 {"role": "user",
                  "content": [{"type": "text", "text": prompt1}, {"type": "image_url", "image_url": {"url":
                                                                                                         f"data:image/jpeg;base64,{base64_image}",
                                                                                                     "detail": "high"}, }]},
                 {"role": "assistant", "content": [{"type": "text", "text": f"\n\n{ouput_0}"}]},
-                {"role": "user", "content": [{"type": "text", "text": prompt2}]}, ]
-            response2 = openai.ChatCompletion.create(
-                model=model if model else self.model,
-                messages=prompt2_input,
-                max_tokens=max_new_tokens if max_new_tokens else 4096,
-                temperature=temperature if temperature else self.temperature,
-                **kwargs,
-            )
-            return [choice["message"]["content"] for choice in response2["choices"]][0]
+                {"role": "user", "content": [{"type": "text", "text": prompt2}]}, 
+            ]
+        response = litellm.completion(
+            model=model if model else self.model,
+            messages=prompt_input,
+            max_tokens=max_new_tokens if max_new_tokens else 4096,
+            temperature=temperature if temperature else self.temperature,
+            **kwargs,
+        )
+        return [choice["message"]["content"] for choice in response.choices][0]
 
 
 class OpenaiEngine_MindAct(Engine):
-    def __init__(
-            self,
-            api_key=None,
-            stop=["\n\n"],
-            rate_limit=-1,
-            model=None,
-            temperature=0,
-            **kwargs,
-    ) -> None:
+    def __init__(self, **kwargs) -> None:
         """Init an OpenAI GPT/Codex engine
 
         Args:
             api_key (_type_, optional): Auth key from OpenAI. Defaults to None.
             stop (list, optional): Tokens indicate stop of sequence. Defaults to ["\n"].
             rate_limit (int, optional): Max number of requests per minute. Defaults to -1.
             model (_type_, optional): Model family. Defaults to None.
         """
-        self.api_keys = load_openai_api_key(api_key)
-        self.stop = stop
-        self.temperature = temperature
-        self.model = model
-        # convert rate limit to minmum request interval
-        self.request_interval = 0 if rate_limit == -1 else 60.0 / rate_limit
-        self.next_avil_time = [0] * len(self.api_keys)
-        self.current_key_idx = 0
-        Engine.__init__(self, **kwargs)
+        super().__init__(**kwargs)
     #
     @backoff.on_exception(
         backoff.expo,
-        (APIError, RateLimitError, APIConnectionError, ServiceUnavailableError),
+        (APIError, RateLimitError, APIConnectionError),
     )
     def generate(self, prompt, max_new_tokens=50, temperature=0, model=None, **kwargs):
-        self.current_key_idx = (self.current_key_idx + 1) % len(self.api_keys)
+        self.current_key_idx = (self.current_key_idx + 1) % len(self.time_slots)
         start_time = time.time()
         if (
                 self.request_interval > 0
                 and start_time < self.next_avil_time[self.current_key_idx]
         ):
             time.sleep(self.next_avil_time[self.current_key_idx] - start_time)
-        openai.api_key = self.api_keys[self.current_key_idx]
         if isinstance(prompt, str):
             # Assume one turn dialogue
             prompt = [
                 {"role": "user", "content": prompt},
             ]
-        response = openai.ChatCompletion.create(
+        response = litellm.completion(
             model=model if model else self.model,
             messages=prompt,
             max_tokens=max_new_tokens,
             temperature=temperature,
             **kwargs,
         )
         if self.request_interval > 0:
```

### Comparing `seeact-0.2.5.1/seeact.egg-info/PKG-INFO` & `seeact-0.2.6/seeact.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.5.1
+Version: 0.2.6
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
-Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
+Author-email: Boyu Gou <gou.43@osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
         
         Copyright (c) 2024 OSU Natural Language Processing Group
         
@@ -121,9 +121,11 @@
 Project-URL: documentation, https://github.com/OSU-NLP-Group/SeeAct
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff
 Requires-Dist: playwright
 Requires-Dist: toml
-Requires-Dist: openai==0.27.8
+Requires-Dist: openai==1.24.0
+Requires-Dist: litellm==1.35.32
+Requires-Dist: google-generativeai==0.5.2
 Requires-Dist: python-dotenv
```

