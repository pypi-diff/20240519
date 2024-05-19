# Comparing `tmp/betterschema-0.1.6.tar.gz` & `tmp/betterschema-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterschema-0.1.6.tar", last modified: Sun May 19 18:44:05 2024, max compression
+gzip compressed data, was "betterschema-0.1.7.tar", last modified: Sun May 19 19:28:01 2024, max compression
```

## Comparing `betterschema-0.1.6.tar` & `betterschema-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 18:44:05.241039 betterschema-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-19 18:43:57.000000 betterschema-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.237038 betterschema-0.1.6/baselib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/baselib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/attr.c
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/init.c
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/module.c
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/schema.c
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/utils.c
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/watch.c
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 18:43:57.000000 betterschema-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:44:05.241039 betterschema-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-19 18:43:57.000000 betterschema-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.237038 betterschema-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/src/betterschema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:43:57.000000 betterschema-0.1.6/src/betterschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 18:43:57.000000 betterschema-0.1.6/src/betterschema/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 18:43:57.000000 betterschema-0.1.6/src/betterschema/render.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/src/betterschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 18:43:57.000000 betterschema-0.1.6/tests/testlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 18:43:57.000000 betterschema-0.1.6/tests/testrender.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 18:43:57.000000 betterschema-0.1.6/tests/testschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 19:28:01.976420 betterschema-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-19 19:27:56.000000 betterschema-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.972420 betterschema-0.1.7/baselib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/baselib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/attr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/init.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/schema.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 19:27:56.000000 betterschema-0.1.7/baselib/src/watch.c
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 19:27:56.000000 betterschema-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:28:01.976420 betterschema-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-19 19:27:56.000000 betterschema-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.972420 betterschema-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/src/betterschema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:27:56.000000 betterschema-0.1.7/src/betterschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 19:27:56.000000 betterschema-0.1.7/src/betterschema/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 19:27:56.000000 betterschema-0.1.7/src/betterschema/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/src/betterschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 19:28:01.000000 betterschema-0.1.7/src/betterschema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:28:01.976420 betterschema-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 19:27:56.000000 betterschema-0.1.7/tests/testlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 19:27:56.000000 betterschema-0.1.7/tests/testrender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 19:27:56.000000 betterschema-0.1.7/tests/testschema.py
```

### Comparing `betterschema-0.1.6/PKG-INFO` & `betterschema-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterschema
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python schema library that supports type checking and validation
 Author: Wilson Wang
 Author-email: wilsonny371@gmail.com
 Project-URL: Source, https://github.com/wilsonwang371/betterschema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `betterschema-0.1.6/README.md` & `betterschema-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/baselib/src/attr.c` & `betterschema-0.1.7/baselib/src/attr.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/baselib/src/init.c` & `betterschema-0.1.7/baselib/src/init.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/baselib/src/module.c` & `betterschema-0.1.7/baselib/src/module.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/baselib/src/schema.c` & `betterschema-0.1.7/baselib/src/schema.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/baselib/src/utils.c` & `betterschema-0.1.7/baselib/src/utils.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/baselib/src/watch.c` & `betterschema-0.1.7/baselib/src/watch.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/setup.py` & `betterschema-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     module.extra_compile_args = ["-Wextra"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="betterschema",
-    version="0.1.6",
+    version="0.1.7",
     author="Wilson Wang",
     project_urls={
         "Source": "https://github.com/wilsonwang371/betterschema",
     },
     author_email="wilsonny371@gmail.com",
     description="A Python schema library that supports type checking and validation",
     long_description=long_description,
```

### Comparing `betterschema-0.1.6/src/betterschema/core.py` & `betterschema-0.1.7/src/betterschema/core.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/src/betterschema/render.py` & `betterschema-0.1.7/src/betterschema/render.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/src/betterschema.egg-info/PKG-INFO` & `betterschema-0.1.7/src/betterschema.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterschema
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Python schema library that supports type checking and validation
 Author: Wilson Wang
 Author-email: wilsonny371@gmail.com
 Project-URL: Source, https://github.com/wilsonwang371/betterschema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `betterschema-0.1.6/tests/testlib.py` & `betterschema-0.1.7/tests/testlib.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/tests/testrender.py` & `betterschema-0.1.7/tests/testrender.py`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.6/tests/testschema.py` & `betterschema-0.1.7/tests/testschema.py`

 * *Files identical despite different names*

