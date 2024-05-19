# Comparing `tmp/func2stream-0.0.0.tar.gz` & `tmp/func2stream-0.0.0.dev20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2stream-0.0.0.tar", last modified: Sat May 18 20:00:44 2024, max compression
+gzip compressed data, was "func2stream-0.0.0.dev20240519.tar", last modified: Sun May 19 03:43:58 2024, max compression
```

## Comparing `func2stream-0.0.0.tar` & `func2stream-0.0.0.dev20240519.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:44.474832 func2stream-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-18 20:00:40.000000 func2stream-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-18 20:00:44.474832 func2stream-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-18 20:00:40.000000 func2stream-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 20:00:44.474832 func2stream-0.0.0/func2stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-18 20:00:44.000000 func2stream-0.0.0/func2stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-18 20:00:44.000000 func2stream-0.0.0/func2stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:00:44.000000 func2stream-0.0.0/func2stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 20:00:44.000000 func2stream-0.0.0/func2stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 20:00:44.000000 func2stream-0.0.0/func2stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 20:00:44.474832 func2stream-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-18 20:00:40.000000 func2stream-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:58.482677 func2stream-0.0.0.dev20240519/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-19 03:43:54.000000 func2stream-0.0.0.dev20240519/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-19 03:43:58.482677 func2stream-0.0.0.dev20240519/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-19 03:43:54.000000 func2stream-0.0.0.dev20240519/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:58.482677 func2stream-0.0.0.dev20240519/func2stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-05-19 03:43:58.000000 func2stream-0.0.0.dev20240519/func2stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-19 03:43:58.000000 func2stream-0.0.0.dev20240519/func2stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:43:58.000000 func2stream-0.0.0.dev20240519/func2stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 03:43:58.000000 func2stream-0.0.0.dev20240519/func2stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:43:58.000000 func2stream-0.0.0.dev20240519/func2stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 03:43:54.000000 func2stream-0.0.0.dev20240519/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 03:43:58.482677 func2stream-0.0.0.dev20240519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-19 03:43:54.000000 func2stream-0.0.0.dev20240519/setup.py
```

### Comparing `func2stream-0.0.0/LICENSE` & `func2stream-0.0.0.dev20240519/LICENSE`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.0/PKG-INFO` & `func2stream-0.0.0.dev20240519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2stream
-Version: 0.0.0
+Version: 0.0.0.dev20240519
 Summary: Effortlessly transform functions into asynchronous elements for building high-performance pipelines
 Home-page: https://github.com/BICHENG/func2stream
 Author: BI CHENG
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `func2stream-0.0.0/README.md` & `func2stream-0.0.0.dev20240519/README.md`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.0/func2stream.egg-info/PKG-INFO` & `func2stream-0.0.0.dev20240519/func2stream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2stream
-Version: 0.0.0
+Version: 0.0.0.dev20240519
 Summary: Effortlessly transform functions into asynchronous elements for building high-performance pipelines
 Home-page: https://github.com/BICHENG/func2stream
 Author: BI CHENG
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `func2stream-0.0.0/setup.py` & `func2stream-0.0.0.dev20240519/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+import os
 from setuptools import setup, find_packages
+from datetime import datetime
+
+date_suffix = datetime.now().strftime("%Y%m%d") #YYYYMMDD
+base_version = '0.0.0'
+full_version = f"{base_version}.dev{date_suffix}"
 
 setup(
     name='func2stream',
-    version='0.0.0',
+    version=full_version,
     description='Effortlessly transform functions into asynchronous elements for building high-performance pipelines',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='BI CHENG',
     url='https://github.com/BICHENG/func2stream',
     packages=find_packages(),
     install_requires=[
```

