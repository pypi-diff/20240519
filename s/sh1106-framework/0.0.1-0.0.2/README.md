# Comparing `tmp/sh1106-framework-0.0.1.tar.gz` & `tmp/sh1106_framework-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh1106-framework-0.0.1.tar", last modified: Fri May 17 21:51:13 2024, max compression
+gzip compressed data, was "sh1106_framework-0.0.2.tar", last modified: Sat May 18 16:59:20 2024, max compression
```

## Comparing `sh1106-framework-0.0.1.tar` & `sh1106_framework-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 21:51:13.867484 sh1106-framework-0.0.1/
--rw-r--r--   0 dan        (501) staff       (20)    11357 2024-05-02 15:27:26.000000 sh1106-framework-0.0.1/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     1047 2024-05-17 21:51:13.867284 sh1106-framework-0.0.1/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      217 2024-05-02 15:27:26.000000 sh1106-framework-0.0.1/README.md
--rw-r--r--   0 dan        (501) staff       (20)      870 2024-05-17 16:01:49.000000 sh1106-framework-0.0.1/pyproject.toml
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-17 21:51:13.867533 sh1106-framework-0.0.1/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      596 2024-05-17 21:48:19.000000 sh1106-framework-0.0.1/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-17 21:51:13.867060 sh1106-framework-0.0.1/sh1106_framework.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     1047 2024-05-17 21:51:13.000000 sh1106-framework-0.0.1/sh1106_framework.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      201 2024-05-17 21:51:13.000000 sh1106-framework-0.0.1/sh1106_framework.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-17 21:51:13.000000 sh1106-framework-0.0.1/sh1106_framework.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-17 21:51:13.000000 sh1106-framework-0.0.1/sh1106_framework.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-18 16:59:20.177315 sh1106_framework-0.0.2/
+-rw-r--r--   0 dan        (501) staff       (20)    11357 2024-05-02 15:27:26.000000 sh1106_framework-0.0.2/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)     1047 2024-05-18 16:59:20.177117 sh1106_framework-0.0.2/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      217 2024-05-02 15:27:26.000000 sh1106_framework-0.0.2/README.md
+-rw-r--r--   0 dan        (501) staff       (20)      870 2024-05-18 16:59:08.000000 sh1106_framework-0.0.2/pyproject.toml
+-rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-18 16:59:20.177354 sh1106_framework-0.0.2/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      596 2024-05-18 16:59:15.000000 sh1106_framework-0.0.2/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-18 16:59:20.176900 sh1106_framework-0.0.2/sh1106_framework.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)     1047 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      201 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/top_level.txt
```

### Comparing `sh1106-framework-0.0.1/LICENSE` & `sh1106_framework-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sh1106-framework-0.0.1/PKG-INFO` & `sh1106_framework-0.0.2/sh1106_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh1106-framework
-Version: 0.0.1
+Version: 0.0.2
 Summary: A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 Author: Dan Convey
 Author-email: Dan Convey <author@example.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/danspage/sh1106-framework
 Project-URL: Issues, https://github.com/danspage/sh1106-framework/issues
 Classifier: Programming Language :: Python
```

### Comparing `sh1106-framework-0.0.1/pyproject.toml` & `sh1106_framework-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "sh1106-framework"
-version = "0.0.1"
+name = "sh1106_framework"
+version = "0.0.2"
 authors = [
   { name="Dan Convey", email="author@example.com" },
 ]
 license = { text = "Apache License 2.0" }
 description = "A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `sh1106-framework-0.0.1/setup.py` & `sh1106_framework-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 name='sh1106_framework',
-version='0.0.1',
+version='0.0.2',
 author='Dan Convey',
 description='A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.',
 packages=find_packages(),
 classifiers=[
 "Programming Language :: Python",
 "Programming Language :: Python :: 3",
 "License :: OSI Approved :: Apache Software License",
```

### Comparing `sh1106-framework-0.0.1/sh1106_framework.egg-info/PKG-INFO` & `sh1106_framework-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sh1106-framework
-Version: 0.0.1
+Name: sh1106_framework
+Version: 0.0.2
 Summary: A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers.
 Author: Dan Convey
 Author-email: Dan Convey <author@example.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/danspage/sh1106-framework
 Project-URL: Issues, https://github.com/danspage/sh1106-framework/issues
 Classifier: Programming Language :: Python
```

