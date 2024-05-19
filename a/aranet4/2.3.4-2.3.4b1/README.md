# Comparing `tmp/aranet4-2.3.4.tar.gz` & `tmp/aranet4-2.3.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aranet4-2.3.4.tar", last modified: Sun May 19 16:59:27 2024, max compression
+gzip compressed data, was "aranet4-2.3.4b1.tar", last modified: Wed May  1 05:41:17 2024, max compression
```

## Comparing `aranet4-2.3.4.tar` & `aranet4-2.3.4b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-19 16:59:27.293001 aranet4-2.3.4/
--rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.4/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     6927 2024-05-19 16:59:27.289001 aranet4-2.3.4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     6542 2024-04-29 07:47:15.000000 aranet4-2.3.4/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-19 16:59:27.269001 aranet4-2.3.4/aranet4/
--rw-r--r--   0 pi        (1000) pi        (1000)      131 2024-05-01 05:40:47.000000 aranet4-2.3.4/aranet4/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     9078 2024-05-01 05:40:58.000000 aranet4-2.3.4/aranet4/aranetctl.py
--rw-r--r--   0 pi        (1000) pi        (1000)    40171 2024-05-01 05:40:42.000000 aranet4-2.3.4/aranet4/client.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-19 16:59:27.285001 aranet4-2.3.4/aranet4.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     6927 2024-05-19 16:59:26.000000 aranet4-2.3.4/aranet4.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-05-19 16:59:26.000000 aranet4-2.3.4/aranet4.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-19 16:59:26.000000 aranet4-2.3.4/aranet4.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-05-19 16:59:26.000000 aranet4-2.3.4/aranet4.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-05-19 16:59:26.000000 aranet4-2.3.4/aranet4.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-05-19 16:59:26.000000 aranet4-2.3.4/aranet4.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-19 16:59:27.293001 aranet4-2.3.4/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      746 2024-05-19 16:57:46.000000 aranet4-2.3.4/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-01 05:41:17.819982 aranet4-2.3.4b1/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1071 2023-12-06 11:57:48.000000 aranet4-2.3.4b1/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     6929 2024-05-01 05:41:17.819982 aranet4-2.3.4b1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     6542 2024-04-29 07:47:15.000000 aranet4-2.3.4b1/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-01 05:41:17.799982 aranet4-2.3.4b1/aranet4/
+-rw-r--r--   0 pi        (1000) pi        (1000)      131 2024-05-01 05:40:47.000000 aranet4-2.3.4b1/aranet4/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     9078 2024-05-01 05:40:58.000000 aranet4-2.3.4b1/aranet4/aranetctl.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    40171 2024-05-01 05:40:42.000000 aranet4-2.3.4b1/aranet4/client.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-05-01 05:41:17.815982 aranet4-2.3.4b1/aranet4.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     6929 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      273 2024-05-01 05:41:17.000000 aranet4-2.3.4b1/aranet4.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       60 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-05-01 05:41:16.000000 aranet4-2.3.4b1/aranet4.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-05-01 05:41:17.823982 aranet4-2.3.4b1/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      748 2024-05-01 05:40:47.000000 aranet4-2.3.4b1/setup.py
```

### Comparing `aranet4-2.3.4/LICENSE` & `aranet4-2.3.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.4/PKG-INFO` & `aranet4-2.3.4b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.4
+Version: 2.3.4b1
 Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.3.4/README.md` & `aranet4-2.3.4b1/README.md`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.4/aranet4/aranetctl.py` & `aranet4-2.3.4b1/aranet4/aranetctl.py`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.4/aranet4/client.py` & `aranet4-2.3.4b1/aranet4/client.py`

 * *Files identical despite different names*

### Comparing `aranet4-2.3.4/aranet4.egg-info/PKG-INFO` & `aranet4-2.3.4b1/aranet4.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aranet4
-Version: 2.3.4
+Version: 2.3.4b1
 Summary: Aranet Python client
 Home-page: https://github.com/Anrijs/Aranet4-Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `aranet4-2.3.4/setup.py` & `aranet4-2.3.4b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aranet4",
-    version="2.3.4",
+    version="2.3.4b1",
     description="Aranet Python client",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Anrijs/Aranet4-Python",
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python',
```

