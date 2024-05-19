# Comparing `tmp/remla24_team8_lib_version-0.3.0.tar.gz` & `tmp/remla24_team8_lib_version-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla24_team8_lib_version-0.3.0.tar", max compression
+gzip compressed data, was "remla24_team8_lib_version-0.3.1.tar", max compression
```

## Comparing `remla24_team8_lib_version-0.3.0.tar` & `remla24_team8_lib_version-0.3.1.tar`

### file list

```diff
@@ -1,3 +1,5 @@
--rw-r--r--   0        0        0     1082 2024-05-16 15:46:29.277451 remla24_team8_lib_version-0.3.0/README.md
--rw-r--r--   0        0        0      555 2024-05-16 16:25:16.441902 remla24_team8_lib_version-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1553 1970-01-01 00:00:00.000000 remla24_team8_lib_version-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/README.md
+-rw-r--r--   0        0        0      631 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/src/lib_version/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-19 11:21:28.973728 remla24_team8_lib_version-0.3.1/src/lib_version/versioning.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 remla24_team8_lib_version-0.3.1/PKG-INFO
```

### Comparing `remla24_team8_lib_version-0.3.0/README.md` & `remla24_team8_lib_version-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 ```
 
 ## Usage
 
 To get the current version include the following lines:
 
 ```python
-from versioning_util.versioning import Version_Util
+from lib_version import Version_Util
 util = VersionUtil()
 print(util.get_version_from_setup())
 ```
```

### Comparing `remla24_team8_lib_version-0.3.0/pyproject.toml` & `remla24_team8_lib_version-0.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "remla24-team8-lib-version"
-version = "0.3.0"
-description = ""
+version = "0.3.1"
+description = "A version-aware library that can can be asked for the version of the library"
 authors = [
     "Tip ten Brink <T.M.tenBrink@student.tudelft.nl>", 
     "Felipe Bononi Bello <bello2001felipe@gmail.com>", 
     "Dielof van Loon <d.i.vanloon@student.tudelft.nl>", 
     "Sayf El Kaddouri <sayfgmaul@gmail.com>"
 ]
 readme = "README.md"
 packages = [
     { include = "lib_version", from = "src"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.12"
 importlib-resources = "^6.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `remla24_team8_lib_version-0.3.0/PKG-INFO` & `remla24_team8_lib_version-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: remla24-team8-lib-version
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: A version-aware library that can can be asked for the version of the library
 Author: Tip ten Brink
 Author-email: T.M.tenBrink@student.tudelft.nl
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-resources (>=6.4.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # lib-version
 
 A version-aware library that can can be asked for the version of the library. This can be useful, for example, for verbose system information in log messages or data records. The library may also contain other logic.
@@ -31,15 +29,15 @@
 ```
 
 ## Usage
 
 To get the current version include the following lines:
 
 ```python
-from versioning_util.versioning import Version_Util
+from lib_version import Version_Util
 util = VersionUtil()
 print(util.get_version_from_setup())
 ```
```

