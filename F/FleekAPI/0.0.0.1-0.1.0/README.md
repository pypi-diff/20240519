# Comparing `tmp/fleekapi-0.0.0.1.tar.gz` & `tmp/fleekapi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.0.0.1.tar", last modified: Sat May 18 11:12:10 2024, max compression
+gzip compressed data, was "fleekapi-0.1.0.tar", last modified: Sun May 19 07:18:59 2024, max compression
```

## Comparing `fleekapi-0.0.0.1.tar` & `fleekapi-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-18 11:12:10.630194 fleekapi-0.0.0.1/
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-18 11:12:10.626194 fleekapi-0.0.0.1/FleekAPI.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)      752 2024-05-18 11:12:10.000000 fleekapi-0.0.0.1/FleekAPI.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      177 2024-05-18 11:12:10.000000 fleekapi-0.0.0.1/FleekAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-18 11:12:10.000000 fleekapi-0.0.0.1/FleekAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       90 2024-05-18 11:12:10.000000 fleekapi-0.0.0.1/FleekAPI.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-18 11:12:10.000000 fleekapi-0.0.0.1/FleekAPI.egg-info/top_level.txt
--rw-r--r--   0 hasan     (1002) hasan     (1002)      752 2024-05-18 11:12:10.626194 fleekapi-0.0.0.1/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       11 2024-05-18 10:33:36.000000 fleekapi-0.0.0.1/README.md
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-18 11:12:10.630194 fleekapi-0.0.0.1/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3969 2024-05-18 10:58:04.000000 fleekapi-0.0.0.1/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:18:59.689878 fleekapi-0.1.0/
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:18:59.685878 fleekapi-0.1.0/FleekAPI/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:05:58.000000 fleekapi-0.1.0/FleekAPI/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.0/FleekAPI/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.0/FleekAPI/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.0/FleekAPI/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:18:59.689878 fleekapi-0.1.0/FleekAPI.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)      872 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/top_level.txt
+-rw-r--r--   0 hasan     (1002) hasan     (1002)      872 2024-05-19 07:18:59.689878 fleekapi-0.1.0/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       11 2024-05-18 10:33:36.000000 fleekapi-0.1.0/README.md
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 07:18:59.693878 fleekapi-0.1.0/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3979 2024-05-19 07:18:56.000000 fleekapi-0.1.0/setup.py
```

### Comparing `fleekapi-0.0.0.1/FleekAPI.egg-info/PKG-INFO` & `fleekapi-0.1.0/FleekAPI.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.0.0.1
+Version: 0.1.0
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: gunicornwebobparseicecreampytestrequests-wsgi-adapterpytest-covJinja2whitenoisesetuptools
+Requires-Dist: gunicorn==22.0.0
+Requires-Dist: Jinja2==3.1.4
+Requires-Dist: parse==1.20.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-wsgi-adapter==0.4.1
+Requires-Dist: WebOb==1.8.7
+Requires-Dist: whitenoise==6.6.0
 
 
 # FleekAPI
```

### Comparing `fleekapi-0.0.0.1/PKG-INFO` & `fleekapi-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: FleekAPI
-Version: 0.0.0.1
+Version: 0.1.0
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
-Requires-Dist: gunicornwebobparseicecreampytestrequests-wsgi-adapterpytest-covJinja2whitenoisesetuptools
+Requires-Dist: gunicorn==22.0.0
+Requires-Dist: Jinja2==3.1.4
+Requires-Dist: parse==1.20.1
+Requires-Dist: requests==2.31.0
+Requires-Dist: requests-wsgi-adapter==0.4.1
+Requires-Dist: WebOb==1.8.7
+Requires-Dist: whitenoise==6.6.0
 
 
 # FleekAPI
```

### Comparing `fleekapi-0.0.0.1/setup.py` & `fleekapi-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,29 +14,26 @@
 # Package meta-data.
 NAME = 'FleekAPI'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.0.0.1'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
-    "gunicorn"
-    "webob"
-    "parse"
-    "icecream"
-    "pytest"
-    "requests-wsgi-adapter"
-    "pytest-cov"
-    "Jinja2"
-    "whitenoise"
-    "setuptools"
+    "gunicorn==22.0.0",
+    "Jinja2==3.1.4",
+    "parse==1.20.1",
+    "requests==2.31.0",
+    "requests-wsgi-adapter==0.4.1",
+    "WebOb==1.8.7",
+    "whitenoise==6.6.0",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
```

