# Comparing `tmp/pypinnacle-0.1.1.tar.gz` & `tmp/pypinnacle-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypinnacle-0.1.1.tar", last modified: Fri May 17 06:17:27 2024, max compression
+gzip compressed data, was "pypinnacle-0.1.3.tar", last modified: Sun May 19 15:02:58 2024, max compression
```

## Comparing `pypinnacle-0.1.1.tar` & `pypinnacle-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 06:17:27.025345 pypinnacle-0.1.1/
--rw-rw-rw-   0        0        0     2983 2024-05-17 06:17:27.025345 pypinnacle-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2282 2024-05-17 06:17:06.000000 pypinnacle-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 06:17:27.024374 pypinnacle-0.1.1/pypinnacle.egg-info/
--rw-rw-rw-   0        0        0     2983 2024-05-17 06:17:26.000000 pypinnacle-0.1.1/pypinnacle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-05-17 06:17:26.000000 pypinnacle-0.1.1/pypinnacle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 06:17:26.000000 pypinnacle-0.1.1/pypinnacle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-05-17 06:17:26.000000 pypinnacle-0.1.1/pypinnacle.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 06:17:26.000000 pypinnacle-0.1.1/pypinnacle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 06:17:27.025345 pypinnacle-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     4073 2024-05-17 06:17:17.000000 pypinnacle-0.1.1/setup.py
+drwxrwxrwx   0 javohir   (1000) javohir   (1000)        0 2024-05-19 15:02:58.114678 pypinnacle-0.1.3/
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)     2865 2024-05-19 15:02:58.114678 pypinnacle-0.1.3/PKG-INFO
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)     2282 2024-05-17 06:17:06.000000 pypinnacle-0.1.3/README.md
+drwxrwxrwx   0 javohir   (1000) javohir   (1000)        0 2024-05-19 15:02:58.108676 pypinnacle-0.1.3/pypinnacle/
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)        0 2024-05-19 14:20:50.000000 pypinnacle-0.1.3/pypinnacle/__init__.py
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)     3954 2024-05-17 05:03:50.000000 pypinnacle-0.1.3/pypinnacle/app.py
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)      714 2024-05-17 04:06:07.000000 pypinnacle-0.1.3/pypinnacle/middleware.py
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)     1023 2024-05-17 04:50:43.000000 pypinnacle-0.1.3/pypinnacle/response.py
+drwxrwxrwx   0 javohir   (1000) javohir   (1000)        0 2024-05-19 15:02:58.113677 pypinnacle-0.1.3/pypinnacle.egg-info/
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)     2865 2024-05-19 15:02:58.000000 pypinnacle-0.1.3/pypinnacle.egg-info/PKG-INFO
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)      276 2024-05-19 15:02:58.000000 pypinnacle-0.1.3/pypinnacle.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)        1 2024-05-19 15:02:58.000000 pypinnacle-0.1.3/pypinnacle.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)       98 2024-05-19 15:02:58.000000 pypinnacle-0.1.3/pypinnacle.egg-info/requires.txt
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)       11 2024-05-19 15:02:58.000000 pypinnacle-0.1.3/pypinnacle.egg-info/top_level.txt
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)       38 2024-05-19 15:02:58.114678 pypinnacle-0.1.3/setup.cfg
+-rwxrwxrwx   0 javohir   (1000) javohir   (1000)     4073 2024-05-19 14:27:09.000000 pypinnacle-0.1.3/setup.py
```

### Comparing `pypinnacle-0.1.1/PKG-INFO` & `pypinnacle-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pypinnacle
-Version: 0.1.1
-Summary: Python Web Framework for building web applications with ease
-Home-page: https://github.com/rustamovjavohir/PyPinnacle.git
-Author: Rustamov Javohir
-Author-email: rustamovj366@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-
-
 
 # PyPinnacle
 
 PyPinnacle is a powerful and flexible Python framework for building web applications quickly and efficiently.
 
 ![purpose](https://img.shields.io/badge/purpose-learning-green)
 
@@ -110,9 +91,8 @@
     def process_request(self, request):
         print("Processing request", request.url)
 
     def process_response(self, request, response):
         print("Processing response", request.url)
 
 app.add_middleware(LogMiddleware)  # add middleware
-```
-
+```
```

### Comparing `pypinnacle-0.1.1/setup.py` & `pypinnacle-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "pypinnacle"
 DESCRIPTION = "Python Web Framework for building web applications with ease"
 URL = "https://github.com/rustamovjavohir/PyPinnacle.git"
 EMAIL = "rustamovj366@gmail.com"
 AUTHOR = "Rustamov Javohir"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "0.1.1"
+VERSION = "0.1.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter",
```

