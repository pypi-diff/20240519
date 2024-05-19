# Comparing `tmp/docugenr8_core-0.0.4.tar.gz` & `tmp/docugenr8_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8_core-0.0.4.tar", last modified: Fri May 10 19:57:44 2024, max compression
+gzip compressed data, was "docugenr8_core-0.0.5.tar", last modified: Sun May 19 11:13:58 2024, max compression
```

## Comparing `docugenr8_core-0.0.4.tar` & `docugenr8_core-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.089646 docugenr8_core-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.093647 docugenr8_core-0.0.4/src/docugenr8_core/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/build_dto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/font.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/src/docugenr8_core/text_area/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/paragraph.py
--rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/textline.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/word.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/src/docugenr8_core/text_area/words_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 19:57:44.000000 docugenr8_core-0.0.4/src/docugenr8_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:57:44.097647 docugenr8_core-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/tests/test_1.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 19:57:14.000000 docugenr8_core-0.0.4/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:58.616553 docugenr8_core-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 11:13:58.616553 docugenr8_core-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:13:58.616553 docugenr8_core-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:58.608553 docugenr8_core-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:58.612553 docugenr8_core-0.0.5/src/docugenr8_core/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/build_dto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:58.616553 docugenr8_core-0.0.5/src/docugenr8_core/text_area/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/paragraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16389 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14263 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/textline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/src/docugenr8_core/text_area/words_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:58.616553 docugenr8_core-0.0.5/src/docugenr8_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 11:13:58.000000 docugenr8_core-0.0.5/src/docugenr8_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-19 11:13:58.000000 docugenr8_core-0.0.5/src/docugenr8_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:13:58.000000 docugenr8_core-0.0.5/src/docugenr8_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 11:13:58.000000 docugenr8_core-0.0.5/src/docugenr8_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 11:13:58.000000 docugenr8_core-0.0.5/src/docugenr8_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:13:58.616553 docugenr8_core-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/tests/test_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 11:13:34.000000 docugenr8_core-0.0.5/version.txt
```

### Comparing `docugenr8_core-0.0.4/LICENSE` & `docugenr8_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/PKG-INFO` & `docugenr8_core-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,13 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: twine; extra == "build"
-Requires-Dist: tox; extra == "build"
 Provides-Extra: dev
 Requires-Dist: docugenr8-core[build,check,test]; extra == "dev"
 
 # docugenr8 Library
 
 docugenr8 is a Python library for document creation.
```

### Comparing `docugenr8_core-0.0.4/pyproject.toml` & `docugenr8_core-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.setuptools.dynamic]
 version = { file = "version.txt" }
 
 [project.optional-dependencies]
 check = ["ruff", "mypy"]
 test = ["pytest", "pytest-cov"]
-build = ["build", "setuptools", "twine", "tox"]
+build = ["build", "setuptools", "twine"]
 dev = ["docugenr8-core[check, test, build]"]
 
 [tool.ruff]
 line-length = 120
 extend-exclude = ["docs", "tests"]
 
 [tool.ruff.lint]
```

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/__init__.py` & `docugenr8_core-0.0.5/src/docugenr8_core/__init__.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/build_dto.py` & `docugenr8_core-0.0.5/src/docugenr8_core/build_dto.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/document.py` & `docugenr8_core-0.0.5/src/docugenr8_core/document.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/font.py` & `docugenr8_core-0.0.5/src/docugenr8_core/font.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/settings.py` & `docugenr8_core-0.0.5/src/docugenr8_core/settings.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/text_area/fragment.py` & `docugenr8_core-0.0.5/src/docugenr8_core/text_area/fragment.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/text_area/paragraph.py` & `docugenr8_core-0.0.5/src/docugenr8_core/text_area/paragraph.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/text_area/textarea.py` & `docugenr8_core-0.0.5/src/docugenr8_core/text_area/textarea.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/text_area/textline.py` & `docugenr8_core-0.0.5/src/docugenr8_core/text_area/textline.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/text_area/word.py` & `docugenr8_core-0.0.5/src/docugenr8_core/text_area/word.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core/text_area/words_creation.py` & `docugenr8_core-0.0.5/src/docugenr8_core/text_area/words_creation.py`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core.egg-info/PKG-INFO` & `docugenr8_core-0.0.5/src/docugenr8_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library for document creating
 Author-email: Vladimir Jovanovic <vladimirjo@protonmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,14 +16,13 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: setuptools; extra == "build"
 Requires-Dist: twine; extra == "build"
-Requires-Dist: tox; extra == "build"
 Provides-Extra: dev
 Requires-Dist: docugenr8-core[build,check,test]; extra == "dev"
 
 # docugenr8 Library
 
 docugenr8 is a Python library for document creation.
```

### Comparing `docugenr8_core-0.0.4/src/docugenr8_core.egg-info/SOURCES.txt` & `docugenr8_core-0.0.5/src/docugenr8_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docugenr8_core-0.0.4/tests/test_1.py` & `docugenr8_core-0.0.5/tests/test_1.py`

 * *Files identical despite different names*

