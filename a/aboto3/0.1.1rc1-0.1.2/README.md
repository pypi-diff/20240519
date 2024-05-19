# Comparing `tmp/aboto3-0.1.1rc1.tar.gz` & `tmp/aboto3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aboto3-0.1.1rc1.tar", last modified: Mon Jan 29 02:56:33 2024, max compression
+gzip compressed data, was "aboto3-0.1.2.tar", last modified: Sun May 19 01:14:42 2024, max compression
```

## Comparing `aboto3-0.1.1rc1.tar` & `aboto3-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-01-29 02:56:33.718671 aboto3-0.1.1rc1/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      594 2024-01-28 21:05:42.000000 aboto3-0.1.1rc1/CHANGELOG.md
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1093 2024-01-28 20:36:17.000000 aboto3-0.1.1rc1/LICENSE
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       55 2024-01-28 20:36:17.000000 aboto3-0.1.1rc1/MANIFEST.in
--rw-r--r--   0 btemplep  (1000) btemplep  (1000)     9408 2024-01-29 02:56:33.718671 aboto3-0.1.1rc1/PKG-INFO
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     7377 2024-01-28 20:51:17.000000 aboto3-0.1.1rc1/README.md
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       90 2024-01-28 20:36:17.000000 aboto3-0.1.1rc1/pyproject.toml
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1310 2024-01-29 02:56:33.718671 aboto3-0.1.1rc1/setup.cfg
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-01-29 02:56:33.714671 aboto3-0.1.1rc1/src/
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-01-29 02:56:33.714671 aboto3-0.1.1rc1/src/aboto3/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       97 2024-01-28 20:51:30.000000 aboto3-0.1.1rc1/src/aboto3/__init__.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1738 2024-01-28 20:36:17.000000 aboto3-0.1.1rc1/src/aboto3/aio_client.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      889 2024-01-28 20:36:17.000000 aboto3-0.1.1rc1/src/aboto3/aio_page_iterator.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      537 2024-01-28 20:36:17.000000 aboto3-0.1.1rc1/src/aboto3/aio_paginator.py
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-01-29 02:56:33.714671 aboto3-0.1.1rc1/src/aboto3.egg-info/
--rw-r--r--   0 btemplep  (1000) btemplep  (1000)     9408 2024-01-29 02:56:33.000000 aboto3-0.1.1rc1/src/aboto3.egg-info/PKG-INFO
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      344 2024-01-29 02:56:33.000000 aboto3-0.1.1rc1/src/aboto3.egg-info/SOURCES.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        1 2024-01-29 02:56:33.000000 aboto3-0.1.1rc1/src/aboto3.egg-info/dependency_links.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       81 2024-01-29 02:56:33.000000 aboto3-0.1.1rc1/src/aboto3.egg-info/requires.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        7 2024-01-29 02:56:33.000000 aboto3-0.1.1rc1/src/aboto3.egg-info/top_level.txt
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 01:14:42.930670 aboto3-0.1.2/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      594 2024-05-19 01:10:01.000000 aboto3-0.1.2/CHANGELOG.md
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1093 2024-05-19 01:10:01.000000 aboto3-0.1.2/LICENSE
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       55 2024-05-19 01:10:01.000000 aboto3-0.1.2/MANIFEST.in
+-rw-r--r--   0 btemplep  (1000) btemplep  (1000)     9514 2024-05-19 01:14:42.930670 aboto3-0.1.2/PKG-INFO
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     7486 2024-05-19 01:11:22.000000 aboto3-0.1.2/README.md
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       90 2024-05-19 01:10:01.000000 aboto3-0.1.2/pyproject.toml
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1310 2024-05-19 01:14:42.930670 aboto3-0.1.2/setup.cfg
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 01:14:42.926670 aboto3-0.1.2/src/
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 01:14:42.926670 aboto3-0.1.2/src/aboto3/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       94 2024-05-19 01:14:13.000000 aboto3-0.1.2/src/aboto3/__init__.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1738 2024-05-19 01:10:01.000000 aboto3-0.1.2/src/aboto3/aio_client.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      889 2024-05-19 01:10:01.000000 aboto3-0.1.2/src/aboto3/aio_page_iterator.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      537 2024-05-19 01:10:01.000000 aboto3-0.1.2/src/aboto3/aio_paginator.py
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 01:14:42.930670 aboto3-0.1.2/src/aboto3.egg-info/
+-rw-r--r--   0 btemplep  (1000) btemplep  (1000)     9514 2024-05-19 01:14:42.000000 aboto3-0.1.2/src/aboto3.egg-info/PKG-INFO
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      344 2024-05-19 01:14:42.000000 aboto3-0.1.2/src/aboto3.egg-info/SOURCES.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        1 2024-05-19 01:14:42.000000 aboto3-0.1.2/src/aboto3.egg-info/dependency_links.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       81 2024-05-19 01:14:42.000000 aboto3-0.1.2/src/aboto3.egg-info/requires.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        7 2024-05-19 01:14:42.000000 aboto3-0.1.2/src/aboto3.egg-info/top_level.txt
```

### Comparing `aboto3-0.1.1rc1/CHANGELOG.md` & `aboto3-0.1.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `aboto3-0.1.1rc1/LICENSE` & `aboto3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aboto3-0.1.1rc1/PKG-INFO` & `aboto3-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aboto3
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: Async boto3 client generator.
 Home-page: https://github.com/btemplep/aboto3
 Author: Brandon Temple Paul
 Author-email: btemplepgit@gmail.com
 License: MIT
 Keywords: aio,async,asyncio,aws,boto3,botocore,sdk
 Classifier: Development Status :: 4 - Beta
@@ -33,14 +33,16 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # `aboto3`
 
+## WARNING - This project is archived and was only a test.  Please use fully async clients like `aioboto3`!
+
 `aboto3` is an async boto3 client generator!
 
 There are other boto3-like libraries that offer asyncio but the interface can be quite different from normal `boto3` clients. 
 The goal of `aboto3` is to closely replicate the `boto3` client interface with acceptable performance from the python [`ThreadPoolExecutor`](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor)!  
 
 > **API NOTE** - `aboto3` was created with boto3 API compatibility in mind.  Because of this it does not support [`boto3` "Resources"](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/resources.html), and there is no plan to support them. New "Resources" are no longer being added to `boto3`.
```

### Comparing `aboto3-0.1.1rc1/README.md` & `aboto3-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # `aboto3`
 
+## WARNING - This project is archived and was only a test.  Please use fully async clients like `aioboto3`!
+
 `aboto3` is an async boto3 client generator!
 
 There are other boto3-like libraries that offer asyncio but the interface can be quite different from normal `boto3` clients. 
 The goal of `aboto3` is to closely replicate the `boto3` client interface with acceptable performance from the python [`ThreadPoolExecutor`](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor)!  
 
 > **API NOTE** - `aboto3` was created with boto3 API compatibility in mind.  Because of this it does not support [`boto3` "Resources"](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/resources.html), and there is no plan to support them. New "Resources" are no longer being added to `boto3`.
```

### Comparing `aboto3-0.1.1rc1/setup.cfg` & `aboto3-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aboto3-0.1.1rc1/src/aboto3/aio_client.py` & `aboto3-0.1.2/src/aboto3/aio_client.py`

 * *Files identical despite different names*

### Comparing `aboto3-0.1.1rc1/src/aboto3/aio_page_iterator.py` & `aboto3-0.1.2/src/aboto3/aio_page_iterator.py`

 * *Files identical despite different names*

### Comparing `aboto3-0.1.1rc1/src/aboto3/aio_paginator.py` & `aboto3-0.1.2/src/aboto3/aio_paginator.py`

 * *Files identical despite different names*

### Comparing `aboto3-0.1.1rc1/src/aboto3.egg-info/PKG-INFO` & `aboto3-0.1.2/src/aboto3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aboto3
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: Async boto3 client generator.
 Home-page: https://github.com/btemplep/aboto3
 Author: Brandon Temple Paul
 Author-email: btemplepgit@gmail.com
 License: MIT
 Keywords: aio,async,asyncio,aws,boto3,botocore,sdk
 Classifier: Development Status :: 4 - Beta
@@ -33,14 +33,16 @@
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # `aboto3`
 
+## WARNING - This project is archived and was only a test.  Please use fully async clients like `aioboto3`!
+
 `aboto3` is an async boto3 client generator!
 
 There are other boto3-like libraries that offer asyncio but the interface can be quite different from normal `boto3` clients. 
 The goal of `aboto3` is to closely replicate the `boto3` client interface with acceptable performance from the python [`ThreadPoolExecutor`](https://docs.python.org/3/library/concurrent.futures.html#concurrent.futures.ThreadPoolExecutor)!  
 
 > **API NOTE** - `aboto3` was created with boto3 API compatibility in mind.  Because of this it does not support [`boto3` "Resources"](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/resources.html), and there is no plan to support them. New "Resources" are no longer being added to `boto3`.
```

