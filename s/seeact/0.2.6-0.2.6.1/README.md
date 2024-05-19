# Comparing `tmp/seeact-0.2.6.tar.gz` & `tmp/seeact-0.2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeact-0.2.6.tar", last modified: Sat May 18 19:37:04 2024, max compression
+gzip compressed data, was "seeact-0.2.6.1.tar", last modified: Sun May 19 02:42:35 2024, max compression
```

## Comparing `seeact-0.2.6.tar` & `seeact-0.2.6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.756636 seeact-0.2.6/
--rwxrwxrwx   0 demo      (1000) demo      (1000)    11495 2024-05-02 03:19:33.000000 seeact-0.2.6/LICENSE
--rwxrwxrwx   0 demo      (1000) demo      (1000)    13402 2024-05-18 19:37:04.756636 seeact-0.2.6/PKG-INFO
--rwxrwxrwx   0 demo      (1000) demo      (1000)     1157 2024-05-18 19:35:59.000000 seeact-0.2.6/pyproject.toml
-drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.284967 seeact-0.2.6/seeact/
--rwxrwxrwx   0 demo      (1000) demo      (1000)      607 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/__init__.py
--rwxrwxrwx   0 demo      (1000) demo      (1000)    32103 2024-05-18 19:01:37.000000 seeact-0.2.6/seeact/agent.py
-drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.426487 seeact-0.2.6/seeact/data_utils/
--rwxrwxrwx   0 demo      (1000) demo      (1000)      607 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/data_utils/__init__.py
--rwxrwxrwx   0 demo      (1000) demo      (1000)     4278 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/data_utils/format_prompt_utils.py
--rwxrwxrwx   0 demo      (1000) demo      (1000)     7487 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/data_utils/prompts.py
-drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.725376 seeact-0.2.6/seeact/demo_utils/
--rwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/demo_utils/__init__.py
--rwxrwxrwx   0 demo      (1000) demo      (1000)    13193 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/demo_utils/browser_helper.py
--rwxrwxrwx   0 demo      (1000) demo      (1000)     7554 2024-05-02 03:19:33.000000 seeact-0.2.6/seeact/demo_utils/format_prompt.py
--rwxrwxrwx   0 demo      (1000) demo      (1000)    12993 2024-05-18 19:01:37.000000 seeact-0.2.6/seeact/demo_utils/inference_engine.py
-drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-18 19:37:04.741011 seeact-0.2.6/seeact.egg-info/
--rwxrwxrwx   0 demo      (1000) demo      (1000)    13402 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/PKG-INFO
--rwxrwxrwx   0 demo      (1000) demo      (1000)      445 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/SOURCES.txt
--rwxrwxrwx   0 demo      (1000) demo      (1000)        1 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/dependency_links.txt
--rwxrwxrwx   0 demo      (1000) demo      (1000)       97 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/requires.txt
--rwxrwxrwx   0 demo      (1000) demo      (1000)        7 2024-05-18 19:37:04.000000 seeact-0.2.6/seeact.egg-info/top_level.txt
--rwxrwxrwx   0 demo      (1000) demo      (1000)       38 2024-05-18 19:37:04.756636 seeact-0.2.6/setup.cfg
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-19 02:42:35.661128 seeact-0.2.6.1/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    11495 2024-05-02 03:19:33.000000 seeact-0.2.6.1/LICENSE
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    13404 2024-05-19 02:42:35.654053 seeact-0.2.6.1/PKG-INFO
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     1201 2024-05-19 02:42:31.000000 seeact-0.2.6.1/pyproject.toml
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-19 02:42:35.379021 seeact-0.2.6.1/seeact/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)      607 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/__init__.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    32085 2024-05-19 02:38:13.000000 seeact-0.2.6.1/seeact/agent.py
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-19 02:42:35.525787 seeact-0.2.6.1/seeact/data_utils/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)      607 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/data_utils/__init__.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     4278 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/data_utils/format_prompt_utils.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     7487 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/data_utils/prompts.py
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-19 02:42:35.618602 seeact-0.2.6.1/seeact/demo_utils/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/demo_utils/__init__.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    13193 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/demo_utils/browser_helper.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)     7554 2024-05-02 03:19:33.000000 seeact-0.2.6.1/seeact/demo_utils/format_prompt.py
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    12993 2024-05-18 20:36:03.000000 seeact-0.2.6.1/seeact/demo_utils/inference_engine.py
+drwxrwxrwx   0 demo      (1000) demo      (1000)        0 2024-05-19 02:42:35.643348 seeact-0.2.6.1/seeact.egg-info/
+-rwxrwxrwx   0 demo      (1000) demo      (1000)    13404 2024-05-19 02:42:35.000000 seeact-0.2.6.1/seeact.egg-info/PKG-INFO
+-rwxrwxrwx   0 demo      (1000) demo      (1000)      445 2024-05-19 02:42:35.000000 seeact-0.2.6.1/seeact.egg-info/SOURCES.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)        1 2024-05-19 02:42:35.000000 seeact-0.2.6.1/seeact.egg-info/dependency_links.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)       97 2024-05-19 02:42:35.000000 seeact-0.2.6.1/seeact.egg-info/requires.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)        7 2024-05-19 02:42:35.000000 seeact-0.2.6.1/seeact.egg-info/top_level.txt
+-rwxrwxrwx   0 demo      (1000) demo      (1000)       38 2024-05-19 02:42:35.662130 seeact-0.2.6.1/setup.cfg
```

### Comparing `seeact-0.2.6/LICENSE` & `seeact-0.2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/PKG-INFO` & `seeact-0.2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.6
+Version: 0.2.6.1
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

### Comparing `seeact-0.2.6/pyproject.toml` & `seeact-0.2.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seeact"
-version = "0.2.6"
+version = "0.2.6.1"
 description = "SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents."
 authors = [
     {name = "Boyu Gou", email = "gou.43@osu.edu"},
     {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"},
     {name = "Zheng Du", email = "du.913@osu.edu"}
 ]
 license = {file="LICENSE"}
@@ -25,7 +25,10 @@
     "python-dotenv"
 ]
 
 [project.urls]
 homepage = "https://osu-nlp-group.github.io/SeeAct/"
 repository = "https://github.com/OSU-NLP-Group/SeeAct"
 documentation = "https://github.com/OSU-NLP-Group/SeeAct"
+
+[tool.setuptools]
+py-modules = ["seeact"]
```

### Comparing `seeact-0.2.6/seeact/__init__.py` & `seeact-0.2.6.1/seeact/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact/agent.py` & `seeact-0.2.6.1/seeact/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from playwright.async_api import async_playwright,Locator
 
 from .data_utils.format_prompt_utils import get_index_from_option_name, generate_new_query_prompt, \
     generate_new_referring_prompt, format_options
 from .demo_utils.browser_helper import normal_launch_async, normal_new_context_async, \
     get_interactive_elements_with_playwright, select_option, saveconfig
 from .demo_utils.format_prompt import format_choices, postprocess_action_lmm
-from .demo_utils.inference_engine import engine_factory, load_openai_api_key
+from .demo_utils.inference_engine import engine_factory
 
 
 class SeeActAgent:
     def __init__(self,
                  config_path=None,
                  save_file_dir="seeact_agent_files",
                  default_task='Find the pdf of the paper "GPT-4V(ision) is a Generalist Web Agent, if Grounded"',
@@ -78,31 +78,33 @@
                     "agent": {
                         "input_info": input_info,
                         "grounding_strategy": grounding_strategy,
                         "max_auto_op": max_auto_op,
                         "max_continuous_no_op": max_continuous_no_op,
                         "highlight": highlight
                     },
-                    "browser": {
-                        "headless": headless,
-                        "args": args,
-                        "browser_app": browser_app,
-                        "persistant": persistant,
-                        "persistant_user_path": persistant_user_path,
-                        "save_video": save_video,
-                        "viewport": viewport,
-                        "tracing": tracing,
-                        "trace": trace
-                    },
                     "openai": {
                         "rate_limit": rate_limit,
                         "model": model,
                         "temperature": temperature
                     }
                 }
+            config.update({     
+                "browser": {
+                    "headless": headless,
+                    "args": args,
+                    "browser_app": browser_app,
+                    "persistant": persistant,
+                    "persistant_user_path": persistant_user_path,
+                    "save_video": save_video,
+                    "viewport": viewport,
+                    "tracing": tracing,
+                    "trace": trace
+                }
+            })
 
         except FileNotFoundError:
             print(f"Error: File '{os.path.abspath(config_path)}' not found.")
         except toml.TomlDecodeError:
             print(f"Error: File '{os.path.abspath(config_path)}' is not a valid TOML file.")
 
         self.config = config
```

### Comparing `seeact-0.2.6/seeact/data_utils/__init__.py` & `seeact-0.2.6.1/seeact/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact/data_utils/format_prompt_utils.py` & `seeact-0.2.6.1/seeact/data_utils/format_prompt_utils.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact/data_utils/prompts.py` & `seeact-0.2.6.1/seeact/data_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact/demo_utils/browser_helper.py` & `seeact-0.2.6.1/seeact/demo_utils/browser_helper.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact/demo_utils/format_prompt.py` & `seeact-0.2.6.1/seeact/demo_utils/format_prompt.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact/demo_utils/inference_engine.py` & `seeact-0.2.6.1/seeact/demo_utils/inference_engine.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.6/seeact.egg-info/PKG-INFO` & `seeact-0.2.6.1/seeact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.6
+Version: 0.2.6.1
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

