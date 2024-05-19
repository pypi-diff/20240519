# Comparing `tmp/docugenr8_pdf-0.0.1.tar.gz` & `tmp/docugenr8_pdf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docugenr8_pdf-0.0.1.tar", last modified: Mon May  6 20:45:30 2024, max compression
+gzip compressed data, was "docugenr8_pdf-0.0.2.tar", last modified: Sun May 19 13:45:41 2024, max compression
```

## Comparing `docugenr8_pdf-0.0.1.tar` & `docugenr8_pdf-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.199011 docugenr8_pdf-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/src/docugenr8_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_content.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_font.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_page.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 20:45:30.203011 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-06 20:45:30.000000 docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-06 20:44:59.000000 docugenr8_pdf-0.0.1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:45:41.597422 docugenr8_pdf-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 13:45:41.597422 docugenr8_pdf-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:45:41.597422 docugenr8_pdf-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:45:41.593422 docugenr8_pdf-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:45:41.593422 docugenr8_pdf-0.0.2/src/docugenr8_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:45:41.597422 docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 13:45:41.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-19 13:45:41.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:45:41.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 13:45:41.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 13:45:41.000000 docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 13:45:15.000000 docugenr8_pdf-0.0.2/version.txt
```

### Comparing `docugenr8_pdf-0.0.1/LICENSE` & `docugenr8_pdf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/PKG-INFO` & `docugenr8_pdf-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-pdf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Docugenr8 add-on library for pdf operations
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
 Requires-Dist: docugenr8-pdf[build,check,test]; extra == "dev"
 
 # docugenr8-pdf Library
 
 docugenr8-pdf is a Python library add-on for pdf operations.
```

### Comparing `docugenr8_pdf-0.0.1/pyproject.toml` & `docugenr8_pdf-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 [tool.setuptools.dynamic]
 version = { file = "version.txt" }
 
 [project.optional-dependencies]
 check = ["ruff", "mypy"]
 test = ["pytest", "pytest-cov"]
-build = ["build", "setuptools", "twine", "tox"]
+build = ["build", "setuptools", "twine"]
 dev = ["docugenr8-pdf[check, test, build]"]
 
 [tool.ruff]
 extend-exclude = ["docs", "tests"]
 
 [tool.ruff.lint]
 select = ["D", "E", "F"]
```

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf/core.py` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf/core.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf.py` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_content.py` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_content.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_font.py` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_font.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_info.py` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_info.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf/pdf_page.py` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf/pdf_page.py`

 * *Files identical despite different names*

### Comparing `docugenr8_pdf-0.0.1/src/docugenr8_pdf.egg-info/PKG-INFO` & `docugenr8_pdf-0.0.2/src/docugenr8_pdf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docugenr8-pdf
-Version: 0.0.1
+Version: 0.0.2
 Summary: Docugenr8 add-on library for pdf operations
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
 Requires-Dist: docugenr8-pdf[build,check,test]; extra == "dev"
 
 # docugenr8-pdf Library
 
 docugenr8-pdf is a Python library add-on for pdf operations.
```

