# Comparing `tmp/tinyagent-0.1.4.tar.gz` & `tmp/tinyagent-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyagent-0.1.4.tar", last modified: Sun May 19 12:21:29 2024, max compression
+gzip compressed data, was "tinyagent-0.1.5.tar", last modified: Sun May 19 15:23:11 2024, max compression
```

## Comparing `tinyagent-0.1.4.tar` & `tinyagent-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.429468 tinyagent-0.1.4/
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.423330 tinyagent-0.1.4/.github/
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.424917 tinyagent-0.1.4/.github/workflows/
--rw-r--r--   0 lan        (501) wheel        (0)      539 2024-05-19 12:09:16.000000 tinyagent-0.1.4/.github/workflows/pylint.yml
--rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-19 12:09:16.000000 tinyagent-0.1.4/.gitignore
--rw-r--r--   0 lan        (501) wheel        (0)     1069 2024-05-19 12:09:16.000000 tinyagent-0.1.4/LICENSE
--rw-r--r--   0 lan        (501) wheel        (0)     1198 2024-05-19 12:21:29.429318 tinyagent-0.1.4/PKG-INFO
--rw-r--r--   0 lan        (501) wheel        (0)      778 2024-05-19 12:09:16.000000 tinyagent-0.1.4/README.md
--rw-r--r--   0 lan        (501) wheel        (0)    32102 2024-05-19 12:09:16.000000 tinyagent-0.1.4/poetry.lock
--rw-r--r--   0 lan        (501) wheel        (0)      303 2024-05-19 12:09:16.000000 tinyagent-0.1.4/pyproject.toml
--rw-r--r--   0 lan        (501) wheel        (0)       38 2024-05-19 12:21:29.429506 tinyagent-0.1.4/setup.cfg
--rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-19 12:21:18.000000 tinyagent-0.1.4/setup.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.425621 tinyagent-0.1.4/tests/
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.425740 tinyagent-0.1.4/tests/resources/
--rw-r--r--   0 lan        (501) wheel        (0)      785 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tests/resources/test.jpg
--rw-r--r--   0 lan        (501) wheel        (0)     2188 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tests/test_claude.py
--rw-r--r--   0 lan        (501) wheel        (0)     2185 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tests/test_gpt.py
--rw-r--r--   0 lan        (501) wheel        (0)      958 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tests/test_tool.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.426633 tinyagent-0.1.4/tinyagent/
--rw-r--r--   0 lan        (501) wheel        (0)      695 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)     4015 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/base.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.427901 tinyagent-0.1.4/tinyagent/claude/
--rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/claude/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)     8992 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/claude/agent.py
--rw-r--r--   0 lan        (501) wheel        (0)     2327 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/claude/client.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.428671 tinyagent-0.1.4/tinyagent/common/
--rw-r--r--   0 lan        (501) wheel        (0)       73 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/common/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)      358 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/common/event.py
--rw-r--r--   0 lan        (501) wheel        (0)      107 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/common/time.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.429110 tinyagent-0.1.4/tinyagent/gpt/
--rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/gpt/__init__.py
--rw-r--r--   0 lan        (501) wheel        (0)     9297 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/gpt/agent.py
--rw-r--r--   0 lan        (501) wheel        (0)     2371 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/gpt/client.py
--rw-r--r--   0 lan        (501) wheel        (0)     2442 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/schema.py
--rw-r--r--   0 lan        (501) wheel        (0)     2322 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/tools.py
--rw-r--r--   0 lan        (501) wheel        (0)      337 2024-05-19 12:09:16.000000 tinyagent-0.1.4/tinyagent/utils.py
-drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 12:21:29.427450 tinyagent-0.1.4/tinyagent.egg-info/
--rw-r--r--   0 lan        (501) wheel        (0)     1198 2024-05-19 12:21:29.000000 tinyagent-0.1.4/tinyagent.egg-info/PKG-INFO
--rw-r--r--   0 lan        (501) wheel        (0)      673 2024-05-19 12:21:29.000000 tinyagent-0.1.4/tinyagent.egg-info/SOURCES.txt
--rw-r--r--   0 lan        (501) wheel        (0)        1 2024-05-19 12:21:29.000000 tinyagent-0.1.4/tinyagent.egg-info/dependency_links.txt
--rw-r--r--   0 lan        (501) wheel        (0)       33 2024-05-19 12:21:29.000000 tinyagent-0.1.4/tinyagent.egg-info/requires.txt
--rw-r--r--   0 lan        (501) wheel        (0)       10 2024-05-19 12:21:29.000000 tinyagent-0.1.4/tinyagent.egg-info/top_level.txt
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.183345 tinyagent-0.1.5/
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.177416 tinyagent-0.1.5/.github/
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.179397 tinyagent-0.1.5/.github/workflows/
+-rw-r--r--   0 lan        (501) wheel        (0)      539 2024-05-19 12:09:16.000000 tinyagent-0.1.5/.github/workflows/pylint.yml
+-rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-19 12:09:16.000000 tinyagent-0.1.5/.gitignore
+-rw-r--r--   0 lan        (501) wheel        (0)     1069 2024-05-19 12:09:16.000000 tinyagent-0.1.5/LICENSE
+-rw-r--r--   0 lan        (501) wheel        (0)     1198 2024-05-19 15:23:11.183208 tinyagent-0.1.5/PKG-INFO
+-rw-r--r--   0 lan        (501) wheel        (0)      778 2024-05-19 12:09:16.000000 tinyagent-0.1.5/README.md
+-rw-r--r--   0 lan        (501) wheel        (0)    32102 2024-05-19 12:09:16.000000 tinyagent-0.1.5/poetry.lock
+-rw-r--r--   0 lan        (501) wheel        (0)      303 2024-05-19 15:23:05.000000 tinyagent-0.1.5/pyproject.toml
+-rw-r--r--   0 lan        (501) wheel        (0)       38 2024-05-19 15:23:11.183379 tinyagent-0.1.5/setup.cfg
+-rw-r--r--   0 lan        (501) wheel        (0)      789 2024-05-19 15:23:05.000000 tinyagent-0.1.5/setup.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.180008 tinyagent-0.1.5/tests/
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.180262 tinyagent-0.1.5/tests/resources/
+-rw-r--r--   0 lan        (501) wheel        (0)      785 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tests/resources/test.jpg
+-rw-r--r--   0 lan        (501) wheel        (0)     2188 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tests/test_claude.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2185 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tests/test_gpt.py
+-rw-r--r--   0 lan        (501) wheel        (0)      958 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tests/test_tool.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.181056 tinyagent-0.1.5/tinyagent/
+-rw-r--r--   0 lan        (501) wheel        (0)      695 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     4015 2024-05-19 15:23:05.000000 tinyagent-0.1.5/tinyagent/base.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.182195 tinyagent-0.1.5/tinyagent/claude/
+-rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/claude/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     8992 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/claude/agent.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2327 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/claude/client.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.182692 tinyagent-0.1.5/tinyagent/common/
+-rw-r--r--   0 lan        (501) wheel        (0)       73 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/common/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)      358 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/common/event.py
+-rw-r--r--   0 lan        (501) wheel        (0)      107 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/common/time.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.183024 tinyagent-0.1.5/tinyagent/gpt/
+-rw-r--r--   0 lan        (501) wheel        (0)        0 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/gpt/__init__.py
+-rw-r--r--   0 lan        (501) wheel        (0)     9297 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/gpt/agent.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2371 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/gpt/client.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2442 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/schema.py
+-rw-r--r--   0 lan        (501) wheel        (0)     2322 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/tools.py
+-rw-r--r--   0 lan        (501) wheel        (0)      337 2024-05-19 12:09:16.000000 tinyagent-0.1.5/tinyagent/utils.py
+drwxr-xr-x   0 lan        (501) wheel        (0)        0 2024-05-19 15:23:11.181706 tinyagent-0.1.5/tinyagent.egg-info/
+-rw-r--r--   0 lan        (501) wheel        (0)     1198 2024-05-19 15:23:11.000000 tinyagent-0.1.5/tinyagent.egg-info/PKG-INFO
+-rw-r--r--   0 lan        (501) wheel        (0)      673 2024-05-19 15:23:11.000000 tinyagent-0.1.5/tinyagent.egg-info/SOURCES.txt
+-rw-r--r--   0 lan        (501) wheel        (0)        1 2024-05-19 15:23:11.000000 tinyagent-0.1.5/tinyagent.egg-info/dependency_links.txt
+-rw-r--r--   0 lan        (501) wheel        (0)       33 2024-05-19 15:23:11.000000 tinyagent-0.1.5/tinyagent.egg-info/requires.txt
+-rw-r--r--   0 lan        (501) wheel        (0)       10 2024-05-19 15:23:11.000000 tinyagent-0.1.5/tinyagent.egg-info/top_level.txt
```

### Comparing `tinyagent-0.1.4/.github/workflows/pylint.yml` & `tinyagent-0.1.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/.gitignore` & `tinyagent-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/LICENSE` & `tinyagent-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/PKG-INFO` & `tinyagent-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyagent
-Version: 0.1.4
+Version: 0.1.5
 Summary: A minimalistic agent framework
 Home-page: https://github.com/y-lan/tinyagent
 Author: y-lan
 Author-email: lanyuyang@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinyagent-0.1.4/README.md` & `tinyagent-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/poetry.lock` & `tinyagent-0.1.5/poetry.lock`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/setup.py` & `tinyagent-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="tinyagent",
-    version="0.1.4",
+    version="0.1.5",
     author="y-lan",
     author_email="lanyuyang@gmail.com",
     description="A minimalistic agent framework",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/y-lan/tinyagent",
     packages=find_packages(),
```

### Comparing `tinyagent-0.1.4/tests/resources/test.jpg` & `tinyagent-0.1.5/tests/resources/test.jpg`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tests/test_claude.py` & `tinyagent-0.1.5/tests/test_claude.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tests/test_gpt.py` & `tinyagent-0.1.5/tests/test_gpt.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tests/test_tool.py` & `tinyagent-0.1.5/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/__init__.py` & `tinyagent-0.1.5/tinyagent/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/base.py` & `tinyagent-0.1.5/tinyagent/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Optional, Union
 
 from tinyagent.schema import (
     BaseConfig,
     ChatResponse,
     Event,
     Message,
+    Role,
     TokenUsage,
 )
 from tinyagent.common import SimpleEventManager
 
 
 class LLMEventManager(SimpleEventManager):
     def on_new_chat_token(self, callback):
@@ -85,18 +86,18 @@
         if isinstance(content, str):
             message = Message.from_text(role, content)
         elif isinstance(content, list):
             message = Message(role, content)
         self.history.append(message)
 
     def add_ai_history(self, history_message):
-        self._add_history(self.ROLE_ASSISTANT, history_message)
+        self._add_history(Role.ASSISTANT, history_message)
 
     def add_user_history(self, history_message):
-        self._add_history(self.ROLE_USER, history_message)
+        self._add_history(Role.USER, history_message)
 
     @abstractmethod
     def _assemble_request_messages(self, user_contents):
         pass
 
     def chat(
         self,
```

### Comparing `tinyagent-0.1.4/tinyagent/claude/agent.py` & `tinyagent-0.1.5/tinyagent/claude/agent.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/claude/client.py` & `tinyagent-0.1.5/tinyagent/claude/client.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/gpt/agent.py` & `tinyagent-0.1.5/tinyagent/gpt/agent.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/gpt/client.py` & `tinyagent-0.1.5/tinyagent/gpt/client.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/schema.py` & `tinyagent-0.1.5/tinyagent/schema.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent/tools.py` & `tinyagent-0.1.5/tinyagent/tools.py`

 * *Files identical despite different names*

### Comparing `tinyagent-0.1.4/tinyagent.egg-info/PKG-INFO` & `tinyagent-0.1.5/tinyagent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyagent
-Version: 0.1.4
+Version: 0.1.5
 Summary: A minimalistic agent framework
 Home-page: https://github.com/y-lan/tinyagent
 Author: y-lan
 Author-email: lanyuyang@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tinyagent-0.1.4/tinyagent.egg-info/SOURCES.txt` & `tinyagent-0.1.5/tinyagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

