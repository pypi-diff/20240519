# Comparing `tmp/datayoga-1.98.0.tar.gz` & `tmp/datayoga-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga-1.98.0.tar", max compression
+gzip compressed data, was "datayoga-1.99.0.tar", max compression
```

## Comparing `datayoga-1.98.0.tar` & `datayoga-1.99.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      633 2023-10-31 10:08:01.960775 datayoga-1.98.0/README.md
--rw-r--r--   0        0        0     1284 2023-10-31 10:08:21.584946 datayoga-1.98.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.960775 datayoga-1.98.0/src/datayoga/__init__.py
--rw-r--r--   0        0        0     5623 2023-10-31 10:08:01.960775 datayoga-1.98.0/src/datayoga/__main__.py
--rw-r--r--   0        0        0     3280 2023-10-31 10:08:01.960775 datayoga-1.98.0/src/datayoga/cli_helpers.py
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 datayoga-1.98.0/PKG-INFO
+-rw-r--r--   0        0        0      633 2023-10-31 12:57:35.748486 datayoga-1.99.0/README.md
+-rw-r--r--   0        0        0     1284 2023-10-31 12:57:54.032582 datayoga-1.99.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.748486 datayoga-1.99.0/src/datayoga/__init__.py
+-rw-r--r--   0        0        0     5623 2023-10-31 12:57:35.748486 datayoga-1.99.0/src/datayoga/__main__.py
+-rw-r--r--   0        0        0     3280 2023-10-31 12:57:35.748486 datayoga-1.99.0/src/datayoga/cli_helpers.py
+-rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 datayoga-1.99.0/PKG-INFO
```

### Comparing `datayoga-1.98.0/README.md` & `datayoga-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `datayoga-1.98.0/pyproject.toml` & `datayoga-1.99.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datayoga"
-version = "1.98.0"
+version = "1.99.0"
 description = "DataYoga command line interface"
 authors = ["DataYoga <admin@datayoga.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
 ]
```

### Comparing `datayoga-1.98.0/src/datayoga/__main__.py` & `datayoga-1.99.0/src/datayoga/__main__.py`

 * *Files identical despite different names*

### Comparing `datayoga-1.98.0/src/datayoga/cli_helpers.py` & `datayoga-1.99.0/src/datayoga/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `datayoga-1.98.0/PKG-INFO` & `datayoga-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datayoga
-Version: 1.98.0
+Version: 1.99.0
 Summary: DataYoga command line interface
 License: Apache-2.0
 Author: DataYoga
 Author-email: admin@datayoga.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

