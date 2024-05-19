# Comparing `tmp/vonage-3.99.0a9.tar.gz` & `tmp/vonage-3.99.1a10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-3.99.0a9.tar", last modified: Thu May  9 15:01:57 2024, max compression
+gzip compressed data, was "vonage-3.99.1a10.tar", last modified: Sun May 19 02:52:55 2024, max compression
```

## Comparing `vonage-3.99.0a9.tar` & `vonage-3.99.1a10.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.987883 vonage-3.99.0a9/
--rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-05-09 15:01:57.987175 vonage-3.99.0a9/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-05-09 15:01:57.000000 vonage-3.99.0a9/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-05-09 15:01:57.000000 vonage-3.99.0a9/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1133 2024-05-09 15:01:57.000000 vonage-3.99.0a9/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-05-09 15:01:57.987969 vonage-3.99.0a9/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.980361 vonage-3.99.0a9/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.983589 vonage-3.99.0a9/src/vonage/
--rw-r--r--   0 mkahan     (503) staff       (20)      466 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)       25 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage/_version.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1758 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage/vonage.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:57.986415 vonage-3.99.0a9/src/vonage.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2496 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      235 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-05-09 15:01:57.000000 vonage-3.99.0a9/src/vonage.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:52:55.451872 vonage-3.99.1a10/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2538 2024-05-19 02:52:55.451297 vonage-3.99.1a10/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1429 2024-05-19 02:52:54.000000 vonage-3.99.1a10/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-05-19 02:52:54.000000 vonage-3.99.1a10/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1164 2024-05-19 02:52:54.000000 vonage-3.99.1a10/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-05-19 02:52:55.451915 vonage-3.99.1a10/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:52:55.445664 vonage-3.99.1a10/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:52:55.448123 vonage-3.99.1a10/src/vonage/
+-rw-r--r--   0 mkahan     (503) staff       (20)      466 2024-05-19 02:52:54.000000 vonage-3.99.1a10/src/vonage/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)       26 2024-05-19 02:52:54.000000 vonage-3.99.1a10/src/vonage/_version.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1758 2024-05-19 02:52:54.000000 vonage-3.99.1a10/src/vonage/vonage.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:52:55.450826 vonage-3.99.1a10/src/vonage.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2538 2024-05-19 02:52:55.000000 vonage-3.99.1a10/src/vonage.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      276 2024-05-19 02:52:55.000000 vonage-3.99.1a10/src/vonage.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-19 02:52:55.000000 vonage-3.99.1a10/src/vonage.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      261 2024-05-19 02:52:55.000000 vonage-3.99.1a10/src/vonage.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        7 2024-05-19 02:52:55.000000 vonage-3.99.1a10/src/vonage.egg-info/top_level.txt
```

### Comparing `vonage-3.99.0a9/PKG-INFO` & `vonage-3.99.1a10/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a9
+Version: 3.99.1a10
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,22 +12,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: vonage-utils>=1.1.1
 Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-application>=1.0.0
 Requires-Dist: vonage-messages>=1.1.1
 Requires-Dist: vonage-number-insight>=1.0.0
 Requires-Dist: vonage-number-insight-v2>=0.1.1b0
 Requires-Dist: vonage-sms>=1.1.1
-Requires-Dist: vonage-users>=1.1.1
+Requires-Dist: vonage-users>=1.1.2
 Requires-Dist: vonage-verify>=1.1.1
 Requires-Dist: vonage-verify-v2>=1.1.1
-Requires-Dist: vonage-voice>=1.0.2
+Requires-Dist: vonage-voice>=1.0.3
 
 # Vonage Python SDK
 
 The Vonage Python SDK Package `vonage` provides a streamlined interface for using Vonage APIs in Python projects. This package includes the `Vonage` class, which simplifies API interactions.
 
 The Vonage class in this package serves as the main entry point for using Vonage APIs. It abstracts away complexities with authentication, HTTP requests and more.
```

### Comparing `vonage-3.99.0a9/README.md` & `vonage-3.99.1a10/README.md`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a9/backend_shim.py` & `vonage-3.99.1a10/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a9/pyproject.toml` & `vonage-3.99.1a10/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 description = "Python Server SDK for using Vonage APIs"
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
   "vonage-utils>=1.1.1",
   "vonage-http-client>=1.3.1",
+  "vonage-application>=1.0.0",
   "vonage-messages>=1.1.1",
   "vonage-number-insight>=1.0.0",
   "vonage-number-insight-v2>=0.1.1b0",
   "vonage-sms>=1.1.1",
-  "vonage-users>=1.1.1",
+  "vonage-users>=1.1.2",
   "vonage-verify>=1.1.1",
   "vonage-verify-v2>=1.1.1",
-  "vonage-voice>=1.0.2",
+  "vonage-voice>=1.0.3",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage-3.99.0a9/src/vonage/vonage.py` & `vonage-3.99.1a10/src/vonage/vonage.py`

 * *Files identical despite different names*

### Comparing `vonage-3.99.0a9/src/vonage.egg-info/PKG-INFO` & `vonage-3.99.1a10/src/vonage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage
-Version: 3.99.0a9
+Version: 3.99.1a10
 Summary: Python Server SDK for using Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,22 +12,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: vonage-utils>=1.1.1
 Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-application>=1.0.0
 Requires-Dist: vonage-messages>=1.1.1
 Requires-Dist: vonage-number-insight>=1.0.0
 Requires-Dist: vonage-number-insight-v2>=0.1.1b0
 Requires-Dist: vonage-sms>=1.1.1
-Requires-Dist: vonage-users>=1.1.1
+Requires-Dist: vonage-users>=1.1.2
 Requires-Dist: vonage-verify>=1.1.1
 Requires-Dist: vonage-verify-v2>=1.1.1
-Requires-Dist: vonage-voice>=1.0.2
+Requires-Dist: vonage-voice>=1.0.3
 
 # Vonage Python SDK
 
 The Vonage Python SDK Package `vonage` provides a streamlined interface for using Vonage APIs in Python projects. This package includes the `Vonage` class, which simplifies API interactions.
 
 The Vonage class in this package serves as the main entry point for using Vonage APIs. It abstracts away complexities with authentication, HTTP requests and more.
```

