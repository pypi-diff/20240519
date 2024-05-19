# Comparing `tmp/boto3-assume-0.1.1.tar.gz` & `tmp/boto3_assume-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-assume-0.1.1.tar", last modified: Thu Jun 29 02:11:56 2023, max compression
+gzip compressed data, was "boto3_assume-0.1.2.tar", last modified: Sun May 19 00:56:38 2024, max compression
```

## Comparing `boto3-assume-0.1.1.tar` & `boto3_assume-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-06-29 02:11:56.726931 boto3-assume-0.1.1/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      519 2023-06-29 02:09:45.000000 boto3-assume-0.1.1/CHANGELOG.md
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    11350 2023-06-24 00:55:07.000000 boto3-assume-0.1.1/LICENSE
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       55 2023-06-16 01:38:37.000000 boto3-assume-0.1.1/MANIFEST.in
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     6199 2023-06-29 02:11:56.726931 boto3-assume-0.1.1/PKG-INFO
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     4332 2023-06-29 02:10:28.000000 boto3-assume-0.1.1/README.md
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       90 2021-04-26 04:13:47.000000 boto3-assume-0.1.1/pyproject.toml
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1615 2023-06-29 02:11:56.730931 boto3-assume-0.1.1/setup.cfg
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-06-29 02:11:56.722931 boto3-assume-0.1.1/src/
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-06-29 02:11:56.726931 boto3-assume-0.1.1/src/boto3_assume/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      390 2023-06-29 02:10:59.000000 boto3-assume-0.1.1/src/boto3_assume/__init__.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1103 2023-06-28 03:21:14.000000 boto3-assume-0.1.1/src/boto3_assume/aio_assume_refresh.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1794 2023-06-27 23:25:02.000000 boto3-assume-0.1.1/src/boto3_assume/aio_core.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1047 2023-06-28 01:54:38.000000 boto3-assume-0.1.1/src/boto3_assume/assume_refresh.py
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1754 2023-06-27 23:23:23.000000 boto3-assume-0.1.1/src/boto3_assume/core.py
-drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2023-06-29 02:11:56.726931 boto3-assume-0.1.1/src/boto3_assume.egg-info/
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     6199 2023-06-29 02:11:56.000000 boto3-assume-0.1.1/src/boto3_assume.egg-info/PKG-INFO
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      423 2023-06-29 02:11:56.000000 boto3-assume-0.1.1/src/boto3_assume.egg-info/SOURCES.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        1 2023-06-29 02:11:56.000000 boto3-assume-0.1.1/src/boto3_assume.egg-info/dependency_links.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      176 2023-06-29 02:11:56.000000 boto3-assume-0.1.1/src/boto3_assume.egg-info/requires.txt
--rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       13 2023-06-29 02:11:56.000000 boto3-assume-0.1.1/src/boto3_assume.egg-info/top_level.txt
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 00:56:38.079639 boto3_assume-0.1.2/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      740 2024-05-19 00:42:42.000000 boto3_assume-0.1.2/CHANGELOG.md
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)    11350 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/LICENSE
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       55 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/MANIFEST.in
+-rw-r--r--   0 btemplep  (1000) btemplep  (1000)     6678 2024-05-19 00:56:38.079639 boto3_assume-0.1.2/PKG-INFO
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     4262 2024-05-19 00:34:10.000000 boto3_assume-0.1.2/README.md
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       90 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/pyproject.toml
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1528 2024-05-19 00:56:38.079639 boto3_assume-0.1.2/setup.cfg
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 00:56:38.071639 boto3_assume-0.1.2/src/
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 00:56:38.075639 boto3_assume-0.1.2/src/boto3_assume/
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      390 2024-05-19 00:34:48.000000 boto3_assume-0.1.2/src/boto3_assume/__init__.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1103 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/src/boto3_assume/aio_assume_refresh.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1794 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/src/boto3_assume/aio_core.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1047 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/src/boto3_assume/assume_refresh.py
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)     1754 2024-05-19 00:18:14.000000 boto3_assume-0.1.2/src/boto3_assume/core.py
+drwxrwxr-x   0 btemplep  (1000) btemplep  (1000)        0 2024-05-19 00:56:38.075639 boto3_assume-0.1.2/src/boto3_assume.egg-info/
+-rw-r--r--   0 btemplep  (1000) btemplep  (1000)     6678 2024-05-19 00:56:38.000000 boto3_assume-0.1.2/src/boto3_assume.egg-info/PKG-INFO
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)      423 2024-05-19 00:56:38.000000 boto3_assume-0.1.2/src/boto3_assume.egg-info/SOURCES.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)        1 2024-05-19 00:56:38.000000 boto3_assume-0.1.2/src/boto3_assume.egg-info/dependency_links.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       92 2024-05-19 00:56:38.000000 boto3_assume-0.1.2/src/boto3_assume.egg-info/requires.txt
+-rw-rw-r--   0 btemplep  (1000) btemplep  (1000)       13 2024-05-19 00:56:38.000000 boto3_assume-0.1.2/src/boto3_assume.egg-info/top_level.txt
```

### Comparing `boto3-assume-0.1.1/LICENSE` & `boto3_assume-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-assume-0.1.1/PKG-INFO` & `boto3_assume-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-assume
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easily create boto3/aioboto3 assume role sessions with automatic credential refreshing.
 Home-page: https://github.com/btemplep/boto3-assume
 Author: Brandon Temple Paul
 Author-email: btemplepgit@gmail.com
 License: Apache License 2.0
 Project-URL: Repository, https://github.com/btemplep/boto3-assume
 Keywords: aio,aioboto3,aiobotocore,assume,async,asyncio,aws,boto3,botocore,credentials,creds,iam,refresh,refreshable,role,sdk
@@ -18,19 +18,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: aioboto3
-Provides-Extra: boto3
-Provides-Extra: all
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: aioboto3; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: moto[server]; extra == "dev"
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytz; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # boto3-assume
 
 
 `boto3-assume` has one simple goal. Easily create `boto3`/`aioboto3` assume role sessions with automatic credential refreshing.
 
 
@@ -38,27 +45,22 @@
 
 Install with pip:
 
 ```text
 $ pip install boto3-assume
 ```
 
-It doesn't come with `boto3` or `aioboto3` by default, 
-but if you want to install them with the package it can be done as extras.
-
-```text
-$ pip install boto3-assume[aioboto,boto3]
-```
+> **NOTE** - It currently doesn't come with `boto3` or `aioboto3` , so you need install to one or both as needed.
 
 
 ## Tutorial
 
 There are only 2 functions `assume_role_session` and `assume_role_aio_session`
 
-For boto3:
+For `boto3`:
 
 ```python
 import boto3
 from boto3_assume import assume_role_session
 
 assume_session = assume_role_session(
     source_session=boto3.Session(), # You must pass in a boto3 session that automatically refreshes!
@@ -197,16 +199,26 @@
 ### Removed
 
 ### Fixed
 
 ### Security 
 -->
 
+## [0.1.2] - 2024-05-18
+
+### Removed
+    - `boto3` and `aioboto3` package extras.  They didn't work and weren't documented correctly. 
+
+### Fixed
+    - `datetime.datetime.utcnow()` deprecation in tests for python 3.12
+
+
 ## [0.1.1] - 2023-06-28
 
 ### Fixed
     - Formatting for Changelog, README
 
+
 ## [0.1.0] - 2023-06-28
 
 Initial Release.
```

### Comparing `boto3-assume-0.1.1/README.md` & `boto3_assume-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,22 @@
 
 Install with pip:
 
 ```text
 $ pip install boto3-assume
 ```
 
-It doesn't come with `boto3` or `aioboto3` by default, 
-but if you want to install them with the package it can be done as extras.
-
-```text
-$ pip install boto3-assume[aioboto,boto3]
-```
+> **NOTE** - It currently doesn't come with `boto3` or `aioboto3` , so you need install to one or both as needed.
 
 
 ## Tutorial
 
 There are only 2 functions `assume_role_session` and `assume_role_aio_session`
 
-For boto3:
+For `boto3`:
 
 ```python
 import boto3
 from boto3_assume import assume_role_session
 
 assume_session = assume_role_session(
     source_session=boto3.Session(), # You must pass in a boto3 session that automatically refreshes!
```

### Comparing `boto3-assume-0.1.1/setup.cfg` & `boto3_assume-0.1.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -52,22 +52,16 @@
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
-aioboto3 = 
-	aioboto3
-	aiobotocore
-boto3 = 
-	boto3
-	botocore
-all = boto3-assume[aioboto3, boto3]
 dev = 
+	aioboto3
 	build
 	coverage
 	moto[server]
 	nox
 	pytest
 	pytest-asyncio
 	pytest-cov
```

### Comparing `boto3-assume-0.1.1/src/boto3_assume/aio_assume_refresh.py` & `boto3_assume-0.1.2/src/boto3_assume/aio_assume_refresh.py`

 * *Files identical despite different names*

### Comparing `boto3-assume-0.1.1/src/boto3_assume/aio_core.py` & `boto3_assume-0.1.2/src/boto3_assume/aio_core.py`

 * *Files identical despite different names*

### Comparing `boto3-assume-0.1.1/src/boto3_assume/assume_refresh.py` & `boto3_assume-0.1.2/src/boto3_assume/assume_refresh.py`

 * *Files identical despite different names*

### Comparing `boto3-assume-0.1.1/src/boto3_assume/core.py` & `boto3_assume-0.1.2/src/boto3_assume/core.py`

 * *Files identical despite different names*

### Comparing `boto3-assume-0.1.1/src/boto3_assume.egg-info/PKG-INFO` & `boto3_assume-0.1.2/src/boto3_assume.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-assume
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easily create boto3/aioboto3 assume role sessions with automatic credential refreshing.
 Home-page: https://github.com/btemplep/boto3-assume
 Author: Brandon Temple Paul
 Author-email: btemplepgit@gmail.com
 License: Apache License 2.0
 Project-URL: Repository, https://github.com/btemplep/boto3-assume
 Keywords: aio,aioboto3,aiobotocore,assume,async,asyncio,aws,boto3,botocore,credentials,creds,iam,refresh,refreshable,role,sdk
@@ -18,19 +18,26 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: aioboto3
-Provides-Extra: boto3
-Provides-Extra: all
-Provides-Extra: dev
 License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: aioboto3; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: moto[server]; extra == "dev"
+Requires-Dist: nox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytz; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 # boto3-assume
 
 
 `boto3-assume` has one simple goal. Easily create `boto3`/`aioboto3` assume role sessions with automatic credential refreshing.
 
 
@@ -38,27 +45,22 @@
 
 Install with pip:
 
 ```text
 $ pip install boto3-assume
 ```
 
-It doesn't come with `boto3` or `aioboto3` by default, 
-but if you want to install them with the package it can be done as extras.
-
-```text
-$ pip install boto3-assume[aioboto,boto3]
-```
+> **NOTE** - It currently doesn't come with `boto3` or `aioboto3` , so you need install to one or both as needed.
 
 
 ## Tutorial
 
 There are only 2 functions `assume_role_session` and `assume_role_aio_session`
 
-For boto3:
+For `boto3`:
 
 ```python
 import boto3
 from boto3_assume import assume_role_session
 
 assume_session = assume_role_session(
     source_session=boto3.Session(), # You must pass in a boto3 session that automatically refreshes!
@@ -197,16 +199,26 @@
 ### Removed
 
 ### Fixed
 
 ### Security 
 -->
 
+## [0.1.2] - 2024-05-18
+
+### Removed
+    - `boto3` and `aioboto3` package extras.  They didn't work and weren't documented correctly. 
+
+### Fixed
+    - `datetime.datetime.utcnow()` deprecation in tests for python 3.12
+
+
 ## [0.1.1] - 2023-06-28
 
 ### Fixed
     - Formatting for Changelog, README
 
+
 ## [0.1.0] - 2023-06-28
 
 Initial Release.
```

