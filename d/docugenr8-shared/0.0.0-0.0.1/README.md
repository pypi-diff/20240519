# Comparing `tmp/docugenr8_shared-0.0.0.tar.gz` & `tmp/docugenr8_shared-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8_shared-0.0.0.tar", last modified: Thu May  2 19:40:50 2024, max compression
+gzip compressed data, was "docugenr8_shared-0.0.1.tar", last modified: Sun May 19 13:26:18 2024, max compression
```

## Comparing `docugenr8_shared-0.0.0.tar` & `docugenr8_shared-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:50.093356 docugenr8_shared-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 19:40:50.093356 docugenr8_shared-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:40:50.093356 docugenr8_shared-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:50.089356 docugenr8_shared-0.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:50.089356 docugenr8_shared-0.0.0/src/docugenr8_shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/src/docugenr8_shared/binary_data_packet.py
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/src/docugenr8_shared/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/src/docugenr8_shared/dto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/src/docugenr8_shared/json_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:40:50.093356 docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 19:40:50.000000 docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-02 19:40:50.000000 docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:40:50.000000 docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 19:40:50.000000 docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 19:40:50.000000 docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 19:40:22.000000 docugenr8_shared-0.0.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:26:18.181441 docugenr8_shared-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-19 13:26:18.181441 docugenr8_shared-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:26:18.181441 docugenr8_shared-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:26:18.177441 docugenr8_shared-0.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:26:18.181441 docugenr8_shared-0.0.1/src/docugenr8_shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/src/docugenr8_shared/binary_data_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/src/docugenr8_shared/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/src/docugenr8_shared/dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/src/docugenr8_shared/json_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:26:18.181441 docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-19 13:26:18.000000 docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-19 13:26:18.000000 docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:26:18.000000 docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-19 13:26:18.000000 docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 13:26:18.000000 docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 13:25:54.000000 docugenr8_shared-0.0.1/version.txt
```

### Comparing `docugenr8_shared-0.0.0/LICENSE` & `docugenr8_shared-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8_shared-0.0.0/PKG-INFO` & `docugenr8_shared-0.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-shared
-Version: 0.0.0
+Version: 0.0.1
 Summary: Docugenr8 add-on library for shared objects and functions
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,14 +14,13 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: twine; extra == "build"
-Requires-Dist: tox; extra == "build"
 Provides-Extra: dev
-Requires-Dist: docugenr8-cicd[build,check,test]; extra == "dev"
+Requires-Dist: docugenr8-shared[build,check,test]; extra == "dev"
 
 # docugenr8-shared Library
 
 docugenr8-shared is a Python library add-on for shared objects and functions.
```

### Comparing `docugenr8_shared-0.0.0/pyproject.toml` & `docugenr8_shared-0.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 [tool.setuptools.dynamic]
 version = { file = "version.txt" }
 
 [project.optional-dependencies]
 check = ["ruff", "mypy"]
 test = ["pytest", "pytest-cov"]
-build = ["build", "setuptools", "twine", "tox"]
-dev = ["docugenr8-cicd[check, test, build]"]
+build = ["build", "setuptools", "twine"]
+dev = ["docugenr8-shared[check, test, build]"]
 
 [tool.ruff]
 extend-exclude = ["docs", "tests"]
 
 [tool.ruff.lint]
 select = ["D", "E", "F"]
 extend-select = ["W", "C90", "I", "N", "B", "A", "C4", "PERF", "RUF"]
```

### Comparing `docugenr8_shared-0.0.0/src/docugenr8_shared/colors.py` & `docugenr8_shared-0.0.1/src/docugenr8_shared/colors.py`

 * *Files identical despite different names*

### Comparing `docugenr8_shared-0.0.0/src/docugenr8_shared/dto.py` & `docugenr8_shared-0.0.1/src/docugenr8_shared/dto.py`

 * *Files identical despite different names*

### Comparing `docugenr8_shared-0.0.0/src/docugenr8_shared.egg-info/PKG-INFO` & `docugenr8_shared-0.0.1/src/docugenr8_shared.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-shared
-Version: 0.0.0
+Version: 0.0.1
 Summary: Docugenr8 add-on library for shared objects and functions
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,14 +14,13 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: twine; extra == "build"
-Requires-Dist: tox; extra == "build"
 Provides-Extra: dev
-Requires-Dist: docugenr8-cicd[build,check,test]; extra == "dev"
+Requires-Dist: docugenr8-shared[build,check,test]; extra == "dev"
 
 # docugenr8-shared Library
 
 docugenr8-shared is a Python library add-on for shared objects and functions.
```

