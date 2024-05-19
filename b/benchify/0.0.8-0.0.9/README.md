# Comparing `tmp/benchify-0.0.8.tar.gz` & `tmp/benchify-0.0.9.tar.gz`

## Comparing `benchify-0.0.8.tar` & `benchify-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 benchify-0.0.8/Makefile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.8/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.8/src/benchify/__init__.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 benchify-0.0.8/src/benchify/main.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 benchify-0.0.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 benchify-0.0.8/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 benchify-0.0.8/README.md
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 benchify-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 benchify-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 benchify-0.0.9/Makefile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 benchify-0.0.9/src/benchify/__init__.py
+-rw-r--r--   0        0        0     7025 2020-02-02 00:00:00.000000 benchify-0.0.9/src/benchify/main.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 benchify-0.0.9/src/benchify/source_manipulation.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 benchify-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 benchify-0.0.9/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 benchify-0.0.9/README.md
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 benchify-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 benchify-0.0.9/PKG-INFO
```

### Comparing `benchify-0.0.8/LICENSE` & `benchify-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `benchify-0.0.8/pyproject.toml` & `benchify-0.0.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "benchify"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Max von Hippel", email="max@benchify.ai" },
   { name="Juan Castaño", email="juan@benchify.ai" },
   { name="Tyler Gabb", email="tylerjgabb@gmail.com" },
 ]
 description = "Formal code intelligence"
 readme = "README.md"
```

### Comparing `benchify-0.0.8/PKG-INFO` & `benchify-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: benchify
-Version: 0.0.8
+Version: 0.0.9
 Summary: Formal code intelligence
 Project-URL: Homepage, https://github.com/Benchify/benchify-api
 Project-URL: Issues, https://github.com/Benchify/benchify-api/issues
 Author-email: Max von Hippel <max@benchify.ai>, Juan Castaño <juan@benchify.ai>, Tyler Gabb <tylerjgabb@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

