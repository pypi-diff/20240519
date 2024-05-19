# Comparing `tmp/lib_version_urlphishing-2.1.0.tar.gz` & `tmp/lib_version_urlphishing-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.1.0.tar", max compression
+gzip compressed data, was "lib_version_urlphishing-2.1.1.tar", max compression
```

## Comparing `lib_version_urlphishing-2.1.0.tar` & `lib_version_urlphishing-2.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      348 2024-05-19 14:51:19.627828 lib_version_urlphishing-2.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-19 14:51:19.627828 lib_version_urlphishing-2.1.0/lib_version_URLPhishing/__init__.py
--rw-r--r--   0        0        0       19 2024-05-19 14:51:32.903743 lib_version_urlphishing-2.1.0/lib_version_URLPhishing/version.py
--rw-r--r--   0        0        0      122 2024-05-19 14:51:19.627828 lib_version_urlphishing-2.1.0/lib_version_URLPhishing/version_util.py
--rw-r--r--   0        0        0      822 2024-05-19 14:51:32.831744 lib_version_urlphishing-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      348 2024-05-19 14:59:38.627296 lib_version_urlphishing-2.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 14:59:38.627296 lib_version_urlphishing-2.1.1/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-19 14:59:52.451231 lib_version_urlphishing-2.1.1/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      122 2024-05-19 14:59:38.627296 lib_version_urlphishing-2.1.1/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      822 2024-05-19 14:59:52.379231 lib_version_urlphishing-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.1.1/PKG-INFO
```

### Comparing `lib_version_urlphishing-2.1.0/pyproject.toml` & `lib_version_urlphishing-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-version-urlphishing"
-version = "2.1.0"
+version = "2.1.1"
 description = "A library to manage and track versions of software components"
 authors = ["Marianna Louizidou <M.Louizidou@student.tudelft.nl>"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `lib_version_urlphishing-2.1.0/PKG-INFO` & `lib_version_urlphishing-2.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-version-urlphishing
-Version: 2.1.0
+Version: 2.1.1
 Summary: A library to manage and track versions of software components
 License: Apache-2.0
 Author: Marianna Louizidou
 Author-email: M.Louizidou@student.tudelft.nl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

