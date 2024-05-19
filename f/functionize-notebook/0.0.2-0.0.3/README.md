# Comparing `tmp/functionize-notebook-0.0.2.tar.gz` & `tmp/functionize_notebook-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "functionize-notebook-0.0.2.tar", last modified: Sun May 19 13:07:22 2024, max compression
+gzip compressed data, was "functionize_notebook-0.0.3.tar", last modified: Sun May 19 13:59:08 2024, max compression
```

## Comparing `functionize-notebook-0.0.2.tar` & `functionize_notebook-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/
--rw-rw-r--   0 tu        (1001) tu        (1001)       29 2024-05-17 06:36:21.000000 functionize-notebook-0.0.2/AUTHORS.md
--rw-rw-r--   0 tu        (1001) tu        (1001)       92 2024-05-19 13:06:57.000000 functionize-notebook-0.0.2/CHANGES.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)     1053 2024-05-17 02:14:10.000000 functionize-notebook-0.0.2/LICENSE.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)       27 2024-05-17 07:16:02.000000 functionize-notebook-0.0.2/MANIFEST.in
--rw-rw-r--   0 tu        (1001) tu        (1001)     2204 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/PKG-INFO
--rw-rw-r--   0 tu        (1001) tu        (1001)     1746 2024-05-17 07:43:18.000000 functionize-notebook-0.0.2/README.md
--rw-rw-r--   0 tu        (1001) tu        (1001)     1836 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/README.rst
-drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/functionize_notebook.egg-info/
--rw-rw-r--   0 tu        (1001) tu        (1001)     2204 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/PKG-INFO
--rw-rw-r--   0 tu        (1001) tu        (1001)      324 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/SOURCES.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)        1 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/dependency_links.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)       19 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/requires.txt
--rw-rw-r--   0 tu        (1001) tu        (1001)       17 2024-05-19 13:07:22.000000 functionize-notebook-0.0.2/functionize_notebook.egg-info/top_level.txt
-drwxrwxr-x   0 tu        (1001) tu        (1001)        0 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/notebook_wrapper/
--rw-rw-r--   0 tu        (1001) tu        (1001)     4274 2024-05-19 13:05:06.000000 functionize-notebook-0.0.2/notebook_wrapper/__init__.py
--rw-rw-r--   0 tu        (1001) tu        (1001)       38 2024-05-19 13:07:22.712188 functionize-notebook-0.0.2/setup.cfg
--rw-rw-r--   0 tu        (1001) tu        (1001)      602 2024-05-19 13:07:17.000000 functionize-notebook-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:59:08.866773 functionize_notebook-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-19 13:59:08.866773 functionize_notebook-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:59:08.866773 functionize_notebook-0.0.3/functionize_notebook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-05-19 13:59:08.000000 functionize_notebook-0.0.3/functionize_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-19 13:59:08.000000 functionize_notebook-0.0.3/functionize_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:59:08.000000 functionize_notebook-0.0.3/functionize_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 13:59:08.000000 functionize_notebook-0.0.3/functionize_notebook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 13:59:08.000000 functionize_notebook-0.0.3/functionize_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:59:08.866773 functionize_notebook-0.0.3/notebook_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/notebook_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:59:08.866773 functionize_notebook-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-19 13:59:04.000000 functionize_notebook-0.0.3/setup.py
```

### Comparing `functionize-notebook-0.0.2/LICENSE.txt` & `functionize_notebook-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.2/PKG-INFO` & `functionize_notebook-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.2
+Version: 0.0.3
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE.txt
 License-File: AUTHORS.md
+Requires-Dist: nbformat
+Requires-Dist: nbconvert
 
 functionize-notebook
 ====================
 
 ``functionize-notebook`` allows you to wrap ``jupyter-notebook`` and use
 it like a function. It allows passing input and output. It is **not**
 multi-thread safe.
@@ -76,9 +77,7 @@
 
 You can also pass other datatype. However, Any modifications made by
 notebook won’t be reflected on the object. You can still return the
 object to get the modifications.
 
 More information and code samples available in the `examples
 folder <./examples/>`__.
-
-
```

### Comparing `functionize-notebook-0.0.2/README.md` & `functionize_notebook-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.2/README.rst` & `functionize_notebook-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.2/functionize_notebook.egg-info/PKG-INFO` & `functionize_notebook-0.0.3/functionize_notebook.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: functionize-notebook
-Version: 0.0.2
+Version: 0.0.3
 Summary: run notebook like a function
 Home-page: https://github.com/BuiHoangTu/functionize-notebook/tree/release
 Author: Bui Hoang Tu
 Author-email: bhtu.work@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE.txt
 License-File: AUTHORS.md
+Requires-Dist: nbformat
+Requires-Dist: nbconvert
 
 functionize-notebook
 ====================
 
 ``functionize-notebook`` allows you to wrap ``jupyter-notebook`` and use
 it like a function. It allows passing input and output. It is **not**
 multi-thread safe.
@@ -76,9 +77,7 @@
 
 You can also pass other datatype. However, Any modifications made by
 notebook won’t be reflected on the object. You can still return the
 object to get the modifications.
 
 More information and code samples available in the `examples
 folder <./examples/>`__.
-
-
```

### Comparing `functionize-notebook-0.0.2/notebook_wrapper/__init__.py` & `functionize_notebook-0.0.3/notebook_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `functionize-notebook-0.0.2/setup.py` & `functionize_notebook-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name="functionize-notebook",
-    version="0.0.2",
+    version="0.0.3",
     author="Bui Hoang Tu",
     author_email="bhtu.work@gmail.com",
     url="https://github.com/BuiHoangTu/functionize-notebook/tree/release",
     license="MIT",
     packages=find_packages(),
     package_dir={"notebook_wrapper": "notebook_wrapper"},
     description="run notebook like a function",
```

