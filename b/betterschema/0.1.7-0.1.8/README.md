# Comparing `tmp/betterschema-0.1.7.tar.gz` & `tmp/betterschema-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterschema-0.1.7.tar", last modified: Sun May 19 19:28:01 2024, max compression
+gzip compressed data, was "betterschema-0.1.8.tar", last modified: Sun May 19 21:18:33 2024, max compression
```

## Comparing `betterschema-0.1.7.tar` & `betterschema-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 19:28:01.976420 betterschema-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-19 19:27:56.000000 betterschema-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.972420 betterschema-0.1.7/baselib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/baselib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/attr.c
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/init.c
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/schema.c
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/watch.c
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 19:27:56.000000 betterschema-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:28:01.976420 betterschema-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-19 19:27:56.000000 betterschema-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.972420 betterschema-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/src/betterschema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:27:56.000000 betterschema-0.1.7/src/betterschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 19:27:56.000000 betterschema-0.1.7/src/betterschema/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 19:27:56.000000 betterschema-0.1.7/src/betterschema/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/src/betterschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 19:27:56.000000 betterschema-0.1.7/tests/testlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 19:27:56.000000 betterschema-0.1.7/tests/testrender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 19:27:56.000000 betterschema-0.1.7/tests/testschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.100341 betterschema-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 21:18:27.000000 betterschema-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-19 21:18:33.100341 betterschema-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-19 21:18:27.000000 betterschema-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.092341 betterschema-0.1.8/baselib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/baselib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/attr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/init.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/schema.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 21:18:27.000000 betterschema-0.1.8/baselib/src/watch.c
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 21:18:27.000000 betterschema-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:18:33.100341 betterschema-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-19 21:18:27.000000 betterschema-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.092341 betterschema-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/src/betterschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 21:18:27.000000 betterschema-0.1.8/src/betterschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 21:18:27.000000 betterschema-0.1.8/src/betterschema/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 21:18:27.000000 betterschema-0.1.8/src/betterschema/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/src/betterschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 21:18:33.000000 betterschema-0.1.8/src/betterschema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:18:33.096341 betterschema-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 21:18:27.000000 betterschema-0.1.8/tests/testlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 21:18:27.000000 betterschema-0.1.8/tests/testrender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 21:18:27.000000 betterschema-0.1.8/tests/testschema.py
```

### Comparing `betterschema-0.1.7/PKG-INFO` & `betterschema-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: betterschema
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python schema library that supports type checking and validation
 Author: Wilson Wang
 Author-email: wilsonny371@gmail.com
 Project-URL: Source, https://github.com/wilsonwang371/betterschema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: PyYAML
 Provides-Extra: dev
 Requires-Dist: unittest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
+Requires-Dist: bump2version; extra == "dev"
 
 
-# betterschema
+# BetterSchema
 
-betterschema is a schema validation and data watching framework for Python. It allows you to define data schemas, validate data against these schemas, and watch for changes in the data with custom watchers.
+BetterSchema is a schema validation and data watching framework for Python. It allows you to define data schemas, validate data against these schemas, and watch for changes in the data with custom watchers.
 
 ## Features
 
 - **Schema Definition**: Easily define data schemas using type hints and decorators.
 - **Data Validation**: Automatically validate data against the defined schemas.
 - **Nested Schemas**: Support for nested schemas within data models.
 - **Watchers**: Monitor changes to data attributes and perform custom actions.
 - **Optional Fields**: Handle optional fields within your schemas.
 - **Type Checking**: Enforce type constraints on data attributes.
 
 ## Installation
 
-You can install betterschema via pip:
+You can install BetterSchema via pip:
 
 ```sh
 pip install betterschema
 ```
 
 ## Usage
 
@@ -155,10 +157,7 @@
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.
 
 ## License
 
 This project is licensed under the MIT License.
 
----
-
-Feel free to adjust this README as per your specific requirements and add any additional sections you deem necessary.
```

### Comparing `betterschema-0.1.7/README.md` & `betterschema-0.1.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
-# betterschema
+# BetterSchema
 
-betterschema is a schema validation and data watching framework for Python. It allows you to define data schemas, validate data against these schemas, and watch for changes in the data with custom watchers.
+BetterSchema is a schema validation and data watching framework for Python. It allows you to define data schemas, validate data against these schemas, and watch for changes in the data with custom watchers.
 
 ## Features
 
 - **Schema Definition**: Easily define data schemas using type hints and decorators.
 - **Data Validation**: Automatically validate data against the defined schemas.
 - **Nested Schemas**: Support for nested schemas within data models.
 - **Watchers**: Monitor changes to data attributes and perform custom actions.
 - **Optional Fields**: Handle optional fields within your schemas.
 - **Type Checking**: Enforce type constraints on data attributes.
 
 ## Installation
 
-You can install betterschema via pip:
+You can install BetterSchema via pip:
 
 ```sh
 pip install betterschema
 ```
 
 ## Usage
 
@@ -137,10 +137,7 @@
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.
 
 ## License
 
 This project is licensed under the MIT License.
 
----
-
-Feel free to adjust this README as per your specific requirements and add any additional sections you deem necessary.
```

### Comparing `betterschema-0.1.7/baselib/src/attr.c` & `betterschema-0.1.8/baselib/src/attr.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/baselib/src/init.c` & `betterschema-0.1.8/baselib/src/init.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/baselib/src/module.c` & `betterschema-0.1.8/baselib/src/module.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/baselib/src/schema.c` & `betterschema-0.1.8/baselib/src/schema.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/baselib/src/utils.c` & `betterschema-0.1.8/baselib/src/utils.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/baselib/src/watch.c` & `betterschema-0.1.8/baselib/src/watch.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/setup.py` & `betterschema-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-"""Setup script for the betterschema package."""
+"""Setup script for the BetterSchema package."""
 
 import os
 import sys
+import re
 
 from setuptools import Extension, find_packages, setup
 
 module = Extension(
     "betterschema.baselib",
     # all c files in the lib/src directory
     sources=[
@@ -23,18 +24,33 @@
     module.extra_compile_args = ["/W4"]
 else:
     module.extra_compile_args = ["-Wextra"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
+
+def read_version():
+    """Read the version from the package __init__ file."""
+    with open(
+        os.path.join(os.path.dirname(__file__), "src", "betterschema", "__init__.py"),
+        "r",
+        encoding="utf-8",
+    ) as f:
+        version_file = f.read()
+    version_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", version_file, re.M)
+    if version_match:
+        return version_match.group(1)
+    raise RuntimeError("Unable to find version string.")
+
+
 setup(
     name="betterschema",
-    version="0.1.7",
     author="Wilson Wang",
+    version=read_version(),
     project_urls={
         "Source": "https://github.com/wilsonwang371/betterschema",
     },
     author_email="wilsonny371@gmail.com",
     description="A Python schema library that supports type checking and validation",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -48,14 +64,15 @@
     extras_require={
         "dev": [
             "unittest",
             "black",
             "build",
             "isort",
             "pylint",
+            "bump2version",
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     # only include from source directory
```

### Comparing `betterschema-0.1.7/src/betterschema/core.py` & `betterschema-0.1.8/src/betterschema/core.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/src/betterschema/render.py` & `betterschema-0.1.8/src/betterschema/render.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/src/betterschema.egg-info/PKG-INFO` & `betterschema-0.1.8/src/betterschema.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: betterschema
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python schema library that supports type checking and validation
 Author: Wilson Wang
 Author-email: wilsonny371@gmail.com
 Project-URL: Source, https://github.com/wilsonwang371/betterschema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: PyYAML
 Provides-Extra: dev
 Requires-Dist: unittest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
+Requires-Dist: bump2version; extra == "dev"
 
 
-# betterschema
+# BetterSchema
 
-betterschema is a schema validation and data watching framework for Python. It allows you to define data schemas, validate data against these schemas, and watch for changes in the data with custom watchers.
+BetterSchema is a schema validation and data watching framework for Python. It allows you to define data schemas, validate data against these schemas, and watch for changes in the data with custom watchers.
 
 ## Features
 
 - **Schema Definition**: Easily define data schemas using type hints and decorators.
 - **Data Validation**: Automatically validate data against the defined schemas.
 - **Nested Schemas**: Support for nested schemas within data models.
 - **Watchers**: Monitor changes to data attributes and perform custom actions.
 - **Optional Fields**: Handle optional fields within your schemas.
 - **Type Checking**: Enforce type constraints on data attributes.
 
 ## Installation
 
-You can install betterschema via pip:
+You can install BetterSchema via pip:
 
 ```sh
 pip install betterschema
 ```
 
 ## Usage
 
@@ -155,10 +157,7 @@
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.
 
 ## License
 
 This project is licensed under the MIT License.
 
----
-
-Feel free to adjust this README as per your specific requirements and add any additional sections you deem necessary.
```

### Comparing `betterschema-0.1.7/tests/testlib.py` & `betterschema-0.1.8/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/tests/testrender.py` & `betterschema-0.1.8/tests/testrender.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.7/tests/testschema.py` & `betterschema-0.1.8/tests/testschema.py`

 * *Files identical despite different names*

