# Comparing `tmp/fleekapi-0.1.22.tar.gz` & `tmp/fleekapi-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.1.22.tar", last modified: Sun May 19 12:23:16 2024, max compression
+gzip compressed data, was "fleekapi-0.1.23.tar", last modified: Sun May 19 13:08:17 2024, max compression
```

## Comparing `fleekapi-0.1.22.tar` & `fleekapi-0.1.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:23:16.012002 fleekapi-0.1.22/
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:23:16.004002 fleekapi-0.1.22/FleekAPI/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:05:58.000000 fleekapi-0.1.22/FleekAPI/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.22/FleekAPI/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.22/FleekAPI/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.22/FleekAPI/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:23:16.008002 fleekapi-0.1.22/FleekAPI.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 12:23:15.000000 fleekapi-0.1.22/FleekAPI.egg-info/top_level.txt
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 12:23:16.012002 fleekapi-0.1.22/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     6861 2024-05-19 12:22:45.000000 fleekapi-0.1.22/README.md
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 12:23:16.012002 fleekapi-0.1.22/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3980 2024-05-19 12:23:11.000000 fleekapi-0.1.22/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 13:08:17.465890 fleekapi-0.1.23/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 13:08:17.465890 fleekapi-0.1.23/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     6861 2024-05-19 12:22:45.000000 fleekapi-0.1.23/README.md
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 13:08:17.457890 fleekapi-0.1.23/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       25 2024-05-19 13:07:08.000000 fleekapi-0.1.23/fleekapi/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.23/fleekapi/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.23/fleekapi/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.23/fleekapi/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 13:08:17.465890 fleekapi-0.1.23/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 13:08:17.465890 fleekapi-0.1.23/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3980 2024-05-19 13:08:12.000000 fleekapi-0.1.23/setup.py
```

### Comparing `fleekapi-0.1.22/FleekAPI/app.py` & `fleekapi-0.1.23/fleekapi/app.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.22/FleekAPI/middleware.py` & `fleekapi-0.1.23/fleekapi/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.22/FleekAPI/response.py` & `fleekapi-0.1.23/fleekapi/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.22/FleekAPI.egg-info/PKG-INFO` & `fleekapi-0.1.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FleekAPI
-Version: 0.1.22
+Name: fleekapi
+Version: 0.1.23
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.1.22/PKG-INFO` & `fleekapi-0.1.23/fleekapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: FleekAPI
-Version: 0.1.22
+Name: fleekapi
+Version: 0.1.23
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `fleekapi-0.1.22/README.md` & `fleekapi-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.22/setup.py` & `fleekapi-0.1.23/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
-NAME = 'FleekAPI'
+NAME = 'fleekapi'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.22'
+VERSION = '0.1.23'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

