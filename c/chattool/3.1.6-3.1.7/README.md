# Comparing `tmp/chattool-3.1.6.tar.gz` & `tmp/chattool-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chattool-3.1.6.tar", last modified: Tue May 14 15:58:42 2024, max compression
+gzip compressed data, was "chattool-3.1.7.tar", last modified: Sun May 19 13:07:04 2024, max compression
```

## Comparing `chattool-3.1.6.tar` & `chattool-3.1.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:58:42.293391 chattool-3.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 15:58:34.000000 chattool-3.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-14 15:58:42.293391 chattool-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-14 15:58:34.000000 chattool-3.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:58:42.293391 chattool-3.1.6/chattool/
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/asynctool.py
--rw-r--r--   0 runner    (1001) docker     (127)    20511 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/chattype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/functioncall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-14 15:58:34.000000 chattool-3.1.6/chattool/tokencalc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:58:42.293391 chattool-3.1.6/chattool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 15:58:42.000000 chattool-3.1.6/chattool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:58:42.293391 chattool-3.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-14 15:58:34.000000 chattool-3.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:07:04.125572 chattool-3.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 13:06:55.000000 chattool-3.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-19 13:07:04.125572 chattool-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-19 13:06:55.000000 chattool-3.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:07:04.121572 chattool-3.1.7/chattool/
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/asynctool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20504 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/chattype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/functioncall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-19 13:06:55.000000 chattool-3.1.7/chattool/tokencalc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:07:04.125572 chattool-3.1.7/chattool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-05-19 13:07:03.000000 chattool-3.1.7/chattool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-19 13:07:04.000000 chattool-3.1.7/chattool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:07:03.000000 chattool-3.1.7/chattool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 13:07:03.000000 chattool-3.1.7/chattool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:07:03.000000 chattool-3.1.7/chattool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 13:07:03.000000 chattool-3.1.7/chattool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 13:07:03.000000 chattool-3.1.7/chattool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:07:04.125572 chattool-3.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-19 13:06:55.000000 chattool-3.1.7/setup.py
```

### Comparing `chattool-3.1.6/LICENSE` & `chattool-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/PKG-INFO` & `chattool-3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.6
+Version: 3.1.7
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
```

### Comparing `chattool-3.1.6/README.md` & `chattool-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/__init__.py` & `chattool-3.1.7/chattool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Chattool."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '3.1.6'
+__version__ = '3.1.7'
 
 import os, sys, requests
 from .chattype import Chat, Resp
 from .checkpoint import load_chats, process_chats
 from .proxy import proxy_on, proxy_off, proxy_status
 from . import request
 from .tokencalc import model_cost_perktoken, findcost
```

### Comparing `chattool-3.1.6/chattool/asynctool.py` & `chattool-3.1.7/chattool/asynctool.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/chattype.py` & `chattool-3.1.7/chattool/chattype.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,19 +42,19 @@
         elif isinstance(msg, str):
             self._chat_log = chattool.default_prompt(msg)
         elif isinstance(msg, list):
             assert all(isinstance(m, dict) for m in msg), "msg should be a list of dict"
             self._chat_log = msg.copy() # avoid changing the original list
         else:
             raise ValueError("msg should be a list of dict, a string or None")
-        self.api_key = api_key or chattool.api_key
+        self.api_key = api_key or chattool.api_key or ''
+        self.model = model or chattool.model or ''
         # chat_url > api_base > base_url > chattool.api_base > chattool.base_url
         self.api_base = api_base or chattool.api_base
         self.base_url = base_url or chattool.base_url
-        self.model = model or chattool.model or "gpt-3.5-turbo"
         if chat_url:
             self.chat_url = chat_url
         elif api_base:
             self.chat_url = os.path.join(self.api_base, "chat/completions")
         elif base_url:
             self.chat_url = os.path.join(self.base_url, "v1/chat/completions")
         elif chattool.api_base:
```

### Comparing `chattool-3.1.6/chattool/checkpoint.py` & `chattool-3.1.7/chattool/checkpoint.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/finetune.py` & `chattool-3.1.7/chattool/finetune.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/functioncall.py` & `chattool-3.1.7/chattool/functioncall.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/proxy.py` & `chattool-3.1.7/chattool/proxy.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/request.py` & `chattool-3.1.7/chattool/request.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/response.py` & `chattool-3.1.7/chattool/response.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool/tokencalc.py` & `chattool-3.1.7/chattool/tokencalc.py`

 * *Files identical despite different names*

### Comparing `chattool-3.1.6/chattool.egg-info/PKG-INFO` & `chattool-3.1.7/chattool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chattool
-Version: 3.1.6
+Version: 3.1.7
 Summary: Toolkit for Chat API
 Home-page: https://github.com/cubenlp/chattool
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: <div align="center">
             <a href="https://pypi.python.org/pypi/chattool">
```

### Comparing `chattool-3.1.6/setup.py` & `chattool-3.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-VERSION = '3.1.6'
+VERSION = '3.1.7'
 
 requirements = [
     'Click>=7.0', 'requests>=2.20', "responses>=0.23", 'aiohttp>=3.8',
     'tqdm>=4.60', 'docstring_parser>=0.10', "python-dotenv>=0.17.0"]
 test_requirements = ['pytest>=3', 'unittest']
 
 setup(
```

