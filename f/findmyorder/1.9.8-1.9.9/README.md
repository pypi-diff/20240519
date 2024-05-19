# Comparing `tmp/findmyorder-1.9.8.tar.gz` & `tmp/findmyorder-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.9.8.tar", max compression
+gzip compressed data, was "findmyorder-1.9.9.tar", max compression
```

## Comparing `findmyorder-1.9.8.tar` & `findmyorder-1.9.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-10-29 09:59:13.343377 findmyorder-1.9.8/LICENSE
--rw-r--r--   0        0        0     2620 2023-10-29 09:59:13.343377 findmyorder-1.9.8/README.md
--rw-r--r--   0        0        0      118 2023-10-29 09:59:30.291699 findmyorder-1.9.8/findmyorder/__init__.py
--rw-r--r--   0        0        0      673 2023-10-29 09:59:13.347377 findmyorder-1.9.8/findmyorder/config.py
--rw-r--r--   0        0        0     1761 2023-10-29 09:59:13.347377 findmyorder-1.9.8/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5160 2023-10-29 09:59:13.347377 findmyorder-1.9.8/findmyorder/main.py
--rw-r--r--   0        0        0     3442 2023-10-29 09:59:30.291699 findmyorder-1.9.8/pyproject.toml
--rw-r--r--   0        0        0     3479 1970-01-01 00:00:00.000000 findmyorder-1.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-10-30 14:19:48.246743 findmyorder-1.9.9/LICENSE
+-rw-r--r--   0        0        0     2620 2023-10-30 14:19:48.246743 findmyorder-1.9.9/README.md
+-rw-r--r--   0        0        0      118 2023-10-30 14:20:05.934760 findmyorder-1.9.9/findmyorder/__init__.py
+-rw-r--r--   0        0        0      673 2023-10-30 14:19:48.254743 findmyorder-1.9.9/findmyorder/config.py
+-rw-r--r--   0        0        0     1761 2023-10-30 14:19:48.254743 findmyorder-1.9.9/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5160 2023-10-30 14:19:48.254743 findmyorder-1.9.9/findmyorder/main.py
+-rw-r--r--   0        0        0     3444 2023-10-30 14:20:05.934760 findmyorder-1.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3479 1970-01-01 00:00:00.000000 findmyorder-1.9.9/PKG-INFO
```

### Comparing `findmyorder-1.9.8/LICENSE` & `findmyorder-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.9.8/README.md` & `findmyorder-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `findmyorder-1.9.8/findmyorder/config.py` & `findmyorder-1.9.9/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.9.8/findmyorder/default_settings.toml` & `findmyorder-1.9.9/findmyorder/default_settings.toml`

 * *Files identical despite different names*

### Comparing `findmyorder-1.9.8/findmyorder/main.py` & `findmyorder-1.9.9/findmyorder/main.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.9.8/pyproject.toml` & `findmyorder-1.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.9.8"
+version = "1.9.9"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -64,27 +64,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.3.0"
 
 
 
 
 
 
 
+
```

### Comparing `findmyorder-1.9.8/PKG-INFO` & `findmyorder-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.9.8
+Version: 1.9.9
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.9.8 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.9.9 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.2.0) Requires-Dist: loguru (>=0.6.0) Requires-Dist: pyparsing
```

