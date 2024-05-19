# Comparing `tmp/grpc_requests-0.1.7.tar.gz` & `tmp/grpc_requests-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_requests-0.1.7.tar", last modified: Fri Dec 16 16:40:39 2022, max compression
+gzip compressed data, was "grpc_requests-0.1.8.tar", last modified: Wed Jan 25 04:06:43 2023, max compression
```

## Comparing `grpc_requests-0.1.7.tar` & `grpc_requests-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2022-12-16 16:40:39.147945 grpc_requests-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/src/grpc_requests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/grpc_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17428 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/grpc_requests/aio.py
--rw-r--r--   0 runner    (1001) docker     (123)    17195 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/grpc_requests/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/grpc_requests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/src/grpc_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2022-12-16 16:40:38.000000 grpc_requests-0.1.7/src/grpc_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2022-12-16 16:40:39.000000 grpc_requests-0.1.7/src/grpc_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 16:40:38.000000 grpc_requests-0.1.7/src/grpc_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-16 16:40:38.000000 grpc_requests-0.1.7/src/grpc_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-16 16:40:38.000000 grpc_requests-0.1.7/src/grpc_requests.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/src/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:39.143945 grpc_requests-0.1.7/src/tests/deprecated_test_case/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/helloworld_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/helloworld_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_certs_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_certs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_service_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_service_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_service_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2022-12-16 16:40:18.000000 grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_service_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:43.679638 grpc_requests-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-01-25 04:06:43.679638 grpc_requests-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-25 04:06:43.679638 grpc_requests-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:43.671637 grpc_requests-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:43.675637 grpc_requests-0.1.8/src/grpc_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/grpc_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/grpc_requests/aio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17195 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/grpc_requests/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/grpc_requests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:43.675637 grpc_requests-0.1.8/src/grpc_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-01-25 04:06:43.000000 grpc_requests-0.1.8/src/grpc_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-01-25 04:06:43.000000 grpc_requests-0.1.8/src/grpc_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 04:06:43.000000 grpc_requests-0.1.8/src/grpc_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-25 04:06:43.000000 grpc_requests-0.1.8/src/grpc_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-25 04:06:43.000000 grpc_requests-0.1.8/src/grpc_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:43.671637 grpc_requests-0.1.8/src/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:43.679638 grpc_requests-0.1.8/src/tests/deprecated_test_case/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/helloworld_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/helloworld_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_certs_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_certs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_service_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_service_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_service_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-01-25 04:06:28.000000 grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_service_client.py
```

### Comparing `grpc_requests-0.1.7/LICENSE` & `grpc_requests-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/setup.cfg` & `grpc_requests-0.1.8/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [metadata]
 name = grpc_requests
-url = https://github.com/spaceone-dev/grpc_requests
+url = https://github.com/wesky93/grpc_requests
 license = Apache License 2.0
-maintainer = MEGAZONE SpaceONE Team
-maintainer_email = admin@spaceone.dev
+maintainer = wesky93
+maintainer_email = wesky93@gmail.com
 description = grpc for Humans. grpc reflection support client
-long_description = file: README.md
+long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 classifiers = 
 	Intended Audience :: Developers
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 packages = find:
 package_dir = = src
 include_package_data = true
-python_requires = >= 3.6
+python_requires = >= 3.7
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [flake8]
```

### Comparing `grpc_requests-0.1.7/src/grpc_requests/aio.py` & `grpc_requests-0.1.8/src/grpc_requests/aio.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/grpc_requests/client.py` & `grpc_requests-0.1.8/src/grpc_requests/client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/grpc_requests.egg-info/SOURCES.txt` & `grpc_requests-0.1.8/src/grpc_requests.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+CHANGELOG.md
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/grpc_requests/__init__.py
 src/grpc_requests/aio.py
 src/grpc_requests/client.py
```

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/helloworld_pb2.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/helloworld_pb2.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/helloworld_pb2_grpc.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/helloworld_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_certs_async_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_certs_async_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_certs_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_certs_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_performance.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_performance.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_async_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_async_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_service_async_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_service_async_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_reflection_service_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_reflection_service_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_async_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_async_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_service_async_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_service_async_client.py`

 * *Files identical despite different names*

### Comparing `grpc_requests-0.1.7/src/tests/deprecated_test_case/test_stub_service_client.py` & `grpc_requests-0.1.8/src/tests/deprecated_test_case/test_stub_service_client.py`

 * *Files identical despite different names*

