# Comparing `tmp/rest_solace-0.1.0.tar.gz` & `tmp/rest_solace-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_solace-0.1.0.tar", last modified: Sat May 18 13:21:01 2024, max compression
+gzip compressed data, was "rest_solace-0.2.0.tar", last modified: Sun May 19 20:19:35 2024, max compression
```

## Comparing `rest_solace-0.1.0.tar` & `rest_solace-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.997412 rest_solace-0.1.0/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.1.0/.gitignore
--rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.1.0/LICENSE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1260 2024-05-07 11:22:11.000000 rest_solace-0.1.0/NOTICE.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)     8300 2024-05-18 13:21:00.997412 rest_solace-0.1.0/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7390 2024-05-14 18:08:22.000000 rest_solace-0.1.0/README.rst
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.961393 rest_solace-0.1.0/docs/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.1.0/docs/development_refrences.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1288 2024-05-10 17:40:06.000000 rest_solace-0.1.0/docs/getting_started_with_solace.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.1.0/docs/index.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)      214 2024-05-14 15:11:52.000000 rest_solace-0.1.0/docs/semp_v2_endpoint_support.rst
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2136 2024-05-18 13:20:13.000000 rest_solace-0.1.0/pyproject.toml
--rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-18 13:21:00.997412 rest_solace-0.1.0/setup.cfg
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.953388 rest_solace-0.1.0/src/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.969397 rest_solace-0.1.0/src/rest_solace/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.1.0/src/rest_solace/__init__.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.981403 rest_solace-0.1.0/src/rest_solace/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/action.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/config.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/manage.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/manager.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/publish.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.1.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)     5149 2024-05-14 18:23:02.000000 rest_solace-0.1.0/src/rest_solace/consumer.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.1.0/src/rest_solace/exceptions.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     3164 2024-05-05 14:53:10.000000 rest_solace-0.1.0/src/rest_solace/http_client.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    31091 2024-05-12 17:11:18.000000 rest_solace-0.1.0/src/rest_solace/manager.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)    17246 2024-05-18 10:07:32.000000 rest_solace-0.1.0/src/rest_solace/publisher.py
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.993410 rest_solace-0.1.0/src/rest_solace.egg-info/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     8300 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/PKG-INFO
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1389 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/SOURCES.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/dependency_links.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       17 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/requires.txt
--rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-18 13:21:00.000000 rest_solace-0.1.0/src/rest_solace.egg-info/top_level.txt
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.989408 rest_solace-0.1.0/tests/
-drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-18 13:21:00.989408 rest_solace-0.1.0/tests/__pycache__/
--rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.1.0/tests/__pycache__/manager_unittest.cpython-311.pyc
--rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.1.0/tests/consumer_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.1.0/tests/empty_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.1.0/tests/manager_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)     2772 2024-05-14 18:07:29.000000 rest_solace-0.1.0/tests/pub_sub_test.py
--rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.1.0/tests/util.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.666236 rest_solace-0.2.0/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      132 2024-05-14 15:14:18.000000 rest_solace-0.2.0/.gitignore
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    10178 2024-05-07 08:54:03.000000 rest_solace-0.2.0/LICENSE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1694 2024-05-19 20:16:27.000000 rest_solace-0.2.0/NOTICE.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     9553 2024-05-19 20:19:35.666236 rest_solace-0.2.0/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     8615 2024-05-19 20:01:09.000000 rest_solace-0.2.0/README.rst
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.634236 rest_solace-0.2.0/docs/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      579 2024-05-10 11:24:36.000000 rest_solace-0.2.0/docs/development_refrences.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1288 2024-05-10 17:40:06.000000 rest_solace-0.2.0/docs/getting_started_with_solace.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      276 2024-05-10 17:58:06.000000 rest_solace-0.2.0/docs/index.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      214 2024-05-14 15:11:52.000000 rest_solace-0.2.0/docs/semp_v2_endpoint_support.rst
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2318 2024-05-19 20:14:39.000000 rest_solace-0.2.0/pyproject.toml
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       38 2024-05-19 20:19:35.666236 rest_solace-0.2.0/setup.cfg
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.630236 rest_solace-0.2.0/src/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.638236 rest_solace-0.2.0/src/rest_solace/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      520 2024-04-20 20:43:31.000000 rest_solace-0.2.0/src/rest_solace/__init__.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.654236 rest_solace-0.2.0/src/rest_solace/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      359 2024-04-20 20:55:30.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2040 2024-04-07 08:23:01.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/action.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2224 2024-04-07 06:29:02.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5734 2024-04-21 05:54:01.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4876 2024-04-22 07:47:41.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4128 2024-04-07 19:18:05.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/manage.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    20533 2024-04-22 10:02:53.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1227 2024-03-31 13:04:04.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2742 2024-04-07 20:21:55.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/publish.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4538 2024-04-21 19:21:45.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     4246 2024-04-07 18:11:44.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     7341 2024-03-31 19:33:25.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5358 2024-04-20 19:56:40.000000 rest_solace-0.2.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5927 2024-05-19 16:38:53.000000 rest_solace-0.2.0/src/rest_solace/consumer.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      125 2024-05-06 18:10:17.000000 rest_solace-0.2.0/src/rest_solace/exceptions.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     5439 2024-05-19 19:45:08.000000 rest_solace-0.2.0/src/rest_solace/http_client.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    31160 2024-05-19 19:46:54.000000 rest_solace-0.2.0/src/rest_solace/manager.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)    34588 2024-05-19 19:35:16.000000 rest_solace-0.2.0/src/rest_solace/publisher.py
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.666236 rest_solace-0.2.0/src/rest_solace.egg-info/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     9553 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/PKG-INFO
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1413 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/SOURCES.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)        1 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/dependency_links.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       32 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/requires.txt
+-rw-r--r--   0 skyler    (1000) skyler    (1000)       12 2024-05-19 20:19:35.000000 rest_solace-0.2.0/src/rest_solace.egg-info/top_level.txt
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.662236 rest_solace-0.2.0/tests/
+drwxr-xr-x   0 skyler    (1000) skyler    (1000)        0 2024-05-19 20:19:35.662236 rest_solace-0.2.0/tests/__pycache__/
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     1419 2024-04-21 18:34:05.000000 rest_solace-0.2.0/tests/__pycache__/manager_unittest.cpython-311.pyc
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      864 2024-05-06 18:46:43.000000 rest_solace-0.2.0/tests/consumer_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      654 2024-05-12 08:11:53.000000 rest_solace-0.2.0/tests/empty_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6920 2024-05-12 17:08:22.000000 rest_solace-0.2.0/tests/manager_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     2835 2024-05-19 15:56:09.000000 rest_solace-0.2.0/tests/pub_sub_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)     6499 2024-05-19 19:40:09.000000 rest_solace-0.2.0/tests/publisher_test.py
+-rw-r--r--   0 skyler    (1000) skyler    (1000)      891 2024-04-28 09:19:07.000000 rest_solace-0.2.0/tests/util.py
```

### Comparing `rest_solace-0.1.0/LICENSE.txt` & `rest_solace-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/NOTICE.txt` & `rest_solace-0.2.0/NOTICE.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Copyright 2024 Skyler Guha
 
 
 This software uses "requests" library by Kenneth Reitz.
 It is licensed under "Apache 2.0 license".
 
+This software uses "aiohttp" library by aio-libs contributors, primarily  Nikolay Kim and Andrew Svetlov.
+It is licensed under "Apache 2.0 license".
+
 This software uses "http" library by The Python Software Foundation.
 It is licensed under "The Python Software Foundation License (PSFL)"
 
 This software uses "functools" library by The Python Software Foundation.
 It is licensed under "The Python Software Foundation License (PSFL)"
 
 This software uses "datetime" library by The Python Software Foundation.
@@ -24,7 +27,13 @@
 
 This software uses "json" library by The Python Software Foundation.
 It is licensed under "The Python Software Foundation License (PSFL)"
 
 This software uses "urllib" library by The Python Software Foundation.
 It is licensed under "The Python Software Foundation License (PSFL)"
 
+This software uses "asyncio" library by The Python Software Foundation.
+It is licensed under "The Python Software Foundation License (PSFL)"
+
+This software uses "logging" library by The Python Software Foundation.
+It is licensed under "The Python Software Foundation License (PSFL)"
+
```

### Comparing `rest_solace-0.1.0/PKG-INFO` & `rest_solace-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.1.0
-Summary: REST based library for Solace Message Broker. Publish, Consume, & Manage!!
+Version: 0.2.0
+Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
 Keywords: solace,rest,REST API,rest-solace,rest_solace,rest solace,python,pythonic
@@ -14,20 +14,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: requests>=2.30.0
+Requires-Dist: aiohttp>=3.9.5
 
 rest-solace
 ===============
 
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
+It is written with the intent to be easy to understand, functional, and pythonic.
+Input and output parameters for every function is always one of int, float, str, bool, list, dict and None; 
+making them directly compatible with json data types. 
+
 | Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
 | View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
 | Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
 
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
@@ -39,42 +44,56 @@
 that you read `this <https://github.com/skyler-guha/rest-solace/blob/master/docs/getting_started_with_solace.rst/>`_ document first.
 It gives a brief explanation on the different components of solace; and that too within the context of this library.
 
 |
 
 Sending messages (for message-VPN in messaging mode):
 -----------------------------------------------------
+(Note: The single message sending functions in this example have async versions as well)
 
 .. code-block:: python
 
     from rest_solace import MessagingPublisher
 
     publish = MessagingPublisher(user_name= "admin", 
                                        password=" admin", 
                                        host= BROKER_IP, 
                                        rest_vpn_port= VPN_PORT #For 'default' VPN it is 9000
                                        )
 
-    #Publish to a queue
+    #Publish to a queue and (only confirms if the message was received by the broker)
     publish.direct_message_to_queue(queue_name= "my_queue",
                                     message= "hello world!!")
     
-    #Publish for a topic string
+    #Publish for a topic string (only confirms if the message was received by the broker)
     publish.direct_message_for_topic(topic_string= "test_topic", 
                                      message= "hello world!!")
 
 
+    #Publish to a queue and wait for confirmation on if the message was spooled into a queue
+    publish.persistent_message_to_queue(queue_name= "my_queue", 
+                                        message= "hello world!!",
+                                        request_reply= False)                               
+
+    #Publish for a topic string and wait for confirmation on if the message was spooled into a queue
+    publish.persistent_message_for_topic(topic_string= "test_topic", 
+                                         message= "hello world!!",
+                                         request_reply= False)
+
+
     #Publish to a queue and wait for reply from a consumer
     response = publish.persistent_message_to_queue(queue_name= "my_queue", 
-                                                   message= "hello world!!")                               
+                                                   message= "hello world!!",
+                                                   request_reply= True)                               
     print(response)
 
     #Publish for a topic string and wait for reply from a consumer
     response = publish.persistent_message_for_topic(topic_string= "test_topic", 
-                                                    message= "hello world!!")
+                                                    message= "hello world!!"
+                                                    request_reply= True)
     print(response)
 
 |
 
 Receiving messages and sending back a response:
 -----------------------------------------------
 (You can use your own REST server too. The one included with this library is only for simple uses and testing)
@@ -110,15 +129,15 @@
     uppercase_response= str.upper( regular_string_content ) 
     
     if regular_string_content == "kill":
         kill_function()
     
     return uppercase_response
 
-    #You can run this function on a septate thread if you want.
+    #You can run this function on a septate thread too if you want.
     consumer_obj.startConsumer(host= CONSUMER_HOST, 
                                port= CONSUMER_PORT,
                                callback_function= return_uppercase, 
                                log= True) 
 
 |
```

### Comparing `rest_solace-0.1.0/README.rst` & `rest_solace-0.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 rest-solace
 ===============
 
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
+It is written with the intent to be easy to understand, functional, and pythonic.
+Input and output parameters for every function is always one of int, float, str, bool, list, dict and None; 
+making them directly compatible with json data types. 
+
 | Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
 | View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
 | Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
 
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
@@ -18,42 +22,56 @@
 that you read `this <https://github.com/skyler-guha/rest-solace/blob/master/docs/getting_started_with_solace.rst/>`_ document first.
 It gives a brief explanation on the different components of solace; and that too within the context of this library.
 
 |
 
 Sending messages (for message-VPN in messaging mode):
 -----------------------------------------------------
+(Note: The single message sending functions in this example have async versions as well)
 
 .. code-block:: python
 
     from rest_solace import MessagingPublisher
 
     publish = MessagingPublisher(user_name= "admin", 
                                        password=" admin", 
                                        host= BROKER_IP, 
                                        rest_vpn_port= VPN_PORT #For 'default' VPN it is 9000
                                        )
 
-    #Publish to a queue
+    #Publish to a queue and (only confirms if the message was received by the broker)
     publish.direct_message_to_queue(queue_name= "my_queue",
                                     message= "hello world!!")
     
-    #Publish for a topic string
+    #Publish for a topic string (only confirms if the message was received by the broker)
     publish.direct_message_for_topic(topic_string= "test_topic", 
                                      message= "hello world!!")
 
 
+    #Publish to a queue and wait for confirmation on if the message was spooled into a queue
+    publish.persistent_message_to_queue(queue_name= "my_queue", 
+                                        message= "hello world!!",
+                                        request_reply= False)                               
+
+    #Publish for a topic string and wait for confirmation on if the message was spooled into a queue
+    publish.persistent_message_for_topic(topic_string= "test_topic", 
+                                         message= "hello world!!",
+                                         request_reply= False)
+
+
     #Publish to a queue and wait for reply from a consumer
     response = publish.persistent_message_to_queue(queue_name= "my_queue", 
-                                                   message= "hello world!!")                               
+                                                   message= "hello world!!",
+                                                   request_reply= True)                               
     print(response)
 
     #Publish for a topic string and wait for reply from a consumer
     response = publish.persistent_message_for_topic(topic_string= "test_topic", 
-                                                    message= "hello world!!")
+                                                    message= "hello world!!"
+                                                    request_reply= True)
     print(response)
 
 |
 
 Receiving messages and sending back a response:
 -----------------------------------------------
 (You can use your own REST server too. The one included with this library is only for simple uses and testing)
@@ -89,15 +107,15 @@
     uppercase_response= str.upper( regular_string_content ) 
     
     if regular_string_content == "kill":
         kill_function()
     
     return uppercase_response
 
-    #You can run this function on a septate thread if you want.
+    #You can run this function on a septate thread too if you want.
     consumer_obj.startConsumer(host= CONSUMER_HOST, 
                                port= CONSUMER_PORT,
                                callback_function= return_uppercase, 
                                log= True) 
 
 |
```

### Comparing `rest_solace-0.1.0/docs/development_refrences.rst` & `rest_solace-0.2.0/docs/development_refrences.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/docs/getting_started_with_solace.rst` & `rest_solace-0.2.0/docs/getting_started_with_solace.rst`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/pyproject.toml` & `rest_solace-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "rest-solace"
 authors = [
     {name = "Skyler Guha", email = "skylerguha@gmail.com"},
 ]
 maintainers = [
   {name = "Skyler Guha", email = "skylerguha@gmail.com"}
 ]
-description = "REST based library for Solace Message Broker. Publish, Consume, & Manage!!"
+description = "REST API library for Solace Message Broker. Publish, Consume, & Manage!!"
 readme = "README.rst"
 requires-python = ">=3.8"
 keywords = ["solace", "rest", 
             "REST API", "rest-solace", 
             "rest_solace", "rest solace", 
             "python", "pythonic"]
 license = {text = "apache 2.0"}
@@ -22,24 +22,28 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers"
 ]
 dependencies = [
     "requests>=2.30.0",
+    "aiohttp>=3.9.5",
     #"http>=0.02",      #part of the standard library
     #"functools",       #part of the standard library
     #"datetime",        #part of the standard library
     #"typing",          #part of the standard library
     #"queue",           #part of the standard library
     #"threading",       #part of the standard library
+    #"time"             #part of the standard library
     #"json",            #part of the standard library
     #"urllib"           #part of the standard library
+    #"asyncio"          #part of the standard library
+    #"logging"          #part of the standard library
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [project.urls]
 pypi = "https://pypi.org/project/rest-solace/"
 documentation = "https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst"
 repository = "https://github.com/skyler-guha/rest-solace"
 
 #Doing an editable install: pip install --editable .
```

### Comparing `rest_solace-0.1.0/src/rest_solace/__init__.py` & `rest_solace-0.2.0/src/rest_solace/__init__.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/action.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/action.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/config.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/consumer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/http_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/manage.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/manage.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/manager.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/pub_sub.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/publish.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/publish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/publisher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/semp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc` & `rest_solace-0.2.0/src/rest_solace/__pycache__/subscriber.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/src/rest_solace/consumer.py` & `rest_solace-0.2.0/src/rest_solace/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from functools import partial
 from datetime import datetime
 from typing import Callable
 from queue import Queue 
 from threading import Thread 
+import time
 
 
 
 class SolaceConsumerServer(BaseHTTPRequestHandler):  
 
     def __init__(self, killer_queue, result_queue, callback_function:Callable= None, 
                  log:bool= False, auto_stop:bool= False, *args, **kwargs):
@@ -74,29 +75,32 @@
             kill_function(event)
 
 
 class Consumer:
 
     def startConsumer(self, host:str, port:int, 
                       callback_function:Callable= None, 
-                      log:bool= True, auto_stop:bool= False)->dict:
+                      log:bool= True, 
+                      auto_stop:bool= False,
+                      timeout:int= None)->dict:
         """Start a Consumer server with a given host and port value. 
         It will receive your messages if you register it as a consumer on your Rest Delivery Point.
 
         Args:
             host (str): IP address for your new consumer server.
             port (int): Port to assign your new server.
             callback_function (Callable, optional): A function to call when a event (like POST request) happens. 
                                                     When called, it will receive a dictionary with the request details 
                                                     [event_type, headers, content], and a function to kill the server and return an output.
                                                     If your callback function returns a string, that string will be used as message response, 
                                                     otherwise any other type object is ignored and a default message is returned.
                                                     Defaults to None.
             log (bool, optional): To print logging info about incoming requests. Defaults to True.
             auto_stop (bool, optional): Stop after receiving a single message. Defaults to False.
+            timeout (int, optional): Timeout in seconds after which the consumer will automatically shutdown.
         """
 
         killer_queue = Queue(maxsize= 1)
         result_queue = Queue(maxsize= 1)
         result_queue.put(dict())
 
         server_address = (host, port)
@@ -107,22 +111,35 @@
 
         if log: print("Running Consumer Server...\n")
 
         #Creating server thread
         server_thread = Thread(target = httpd.serve_forever) 
         server_thread.start()
          
+        #Add these in a thread with sleep func in the future so that the while loops do not hog cpu.
         try:
-            while True:
-                if killer_queue.get() == 1:
-                    if log: print("\nStopping server to return output...")
-                    httpd.shutdown()
-                    httpd.server_close()
-                    if log: print("Server stopped.")
-                    break
+            if timeout==None:
+                while True:
+                    if killer_queue.get() == 1:
+                        if log: print("\nStopping server to return output...")
+                        httpd.shutdown()
+                        httpd.server_close()
+                        if log: print("Server stopped.")
+                        break
+            
+            else:
+                timeout = time.time() + timeout
+                while True:
+                    if killer_queue.get() == 1 or time.time() > timeout:
+                        if log: print("\nStopping server to return output...")
+                        httpd.shutdown()
+                        httpd.server_close()
+                        if log: print("Server stopped.")
+                        break
+
         except KeyboardInterrupt: #It is expected that the user might want to only use ctrl+c to close the server in some cases.
             if log: print("\nStopping server due to keyboard interrupt...")
             httpd.shutdown()
             httpd.server_close()
             if log: print("Server stopped.")
```

### Comparing `rest_solace-0.1.0/src/rest_solace/manager.py` & `rest_solace-0.2.0/src/rest_solace/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -603,15 +603,16 @@
         self.update_client_username(msgVpnName= msgVpnName, clientUsername= clientUsername)
 
         #step1
         self.create_queue_endpoint(queueName=queueName, msgVpnName=msgVpnName, throw_exception= False)
 
         #step2
         if subscriptionTopic != None:
-            self.subscribe_to_topic_on_queue(subscriptionTopic= subscriptionTopic,
+            self.subscribe_to_topic_on_queue(msgVpnName= msgVpnName,
+                                             subscriptionTopic= subscriptionTopic,
                                              queueName= queueName)
             
         #step3
         res = self.create_rest_delivery_point(msgVpnName= msgVpnName, 
                                               restDeliveryPointName= restDeliveryPointName, 
                                               throw_exception=False,
                                               clientProfileName= clientProfileName)
```

### Comparing `rest_solace-0.1.0/src/rest_solace.egg-info/PKG-INFO` & `rest_solace-0.2.0/src/rest_solace.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: rest-solace
-Version: 0.1.0
-Summary: REST based library for Solace Message Broker. Publish, Consume, & Manage!!
+Version: 0.2.0
+Summary: REST API library for Solace Message Broker. Publish, Consume, & Manage!!
 Author-email: Skyler Guha <skylerguha@gmail.com>
 Maintainer-email: Skyler Guha <skylerguha@gmail.com>
 License: apache 2.0
 Project-URL: pypi, https://pypi.org/project/rest-solace/
 Project-URL: documentation, https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst
 Project-URL: repository, https://github.com/skyler-guha/rest-solace
 Keywords: solace,rest,REST API,rest-solace,rest_solace,rest solace,python,pythonic
@@ -14,20 +14,25 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: requests>=2.30.0
+Requires-Dist: aiohttp>=3.9.5
 
 rest-solace
 ===============
 
 **rest-solace** is a rest based python library for Solace Message Broker that allows you to Publish, Consume, & Manage!!
 
+It is written with the intent to be easy to understand, functional, and pythonic.
+Input and output parameters for every function is always one of int, float, str, bool, list, dict and None; 
+making them directly compatible with json data types. 
+
 | Check it out at `PyPI <https://pypi.org/project/rest-solace/>`_.
 | View the code at `Github <https://github.com/skyler-guha/rest-solace/>`_.
 | Read the docs from `Here <https://github.com/skyler-guha/rest-solace/blob/master/docs/index.rst/>`_.
 
 Note: 
     | Right now the focus of this library is on the 'messaging' mode for solace message VPNs.
     | In the future I plan to add better support for 'gateway' mode as well.
@@ -39,42 +44,56 @@
 that you read `this <https://github.com/skyler-guha/rest-solace/blob/master/docs/getting_started_with_solace.rst/>`_ document first.
 It gives a brief explanation on the different components of solace; and that too within the context of this library.
 
 |
 
 Sending messages (for message-VPN in messaging mode):
 -----------------------------------------------------
+(Note: The single message sending functions in this example have async versions as well)
 
 .. code-block:: python
 
     from rest_solace import MessagingPublisher
 
     publish = MessagingPublisher(user_name= "admin", 
                                        password=" admin", 
                                        host= BROKER_IP, 
                                        rest_vpn_port= VPN_PORT #For 'default' VPN it is 9000
                                        )
 
-    #Publish to a queue
+    #Publish to a queue and (only confirms if the message was received by the broker)
     publish.direct_message_to_queue(queue_name= "my_queue",
                                     message= "hello world!!")
     
-    #Publish for a topic string
+    #Publish for a topic string (only confirms if the message was received by the broker)
     publish.direct_message_for_topic(topic_string= "test_topic", 
                                      message= "hello world!!")
 
 
+    #Publish to a queue and wait for confirmation on if the message was spooled into a queue
+    publish.persistent_message_to_queue(queue_name= "my_queue", 
+                                        message= "hello world!!",
+                                        request_reply= False)                               
+
+    #Publish for a topic string and wait for confirmation on if the message was spooled into a queue
+    publish.persistent_message_for_topic(topic_string= "test_topic", 
+                                         message= "hello world!!",
+                                         request_reply= False)
+
+
     #Publish to a queue and wait for reply from a consumer
     response = publish.persistent_message_to_queue(queue_name= "my_queue", 
-                                                   message= "hello world!!")                               
+                                                   message= "hello world!!",
+                                                   request_reply= True)                               
     print(response)
 
     #Publish for a topic string and wait for reply from a consumer
     response = publish.persistent_message_for_topic(topic_string= "test_topic", 
-                                                    message= "hello world!!")
+                                                    message= "hello world!!"
+                                                    request_reply= True)
     print(response)
 
 |
 
 Receiving messages and sending back a response:
 -----------------------------------------------
 (You can use your own REST server too. The one included with this library is only for simple uses and testing)
@@ -110,15 +129,15 @@
     uppercase_response= str.upper( regular_string_content ) 
     
     if regular_string_content == "kill":
         kill_function()
     
     return uppercase_response
 
-    #You can run this function on a septate thread if you want.
+    #You can run this function on a septate thread too if you want.
     consumer_obj.startConsumer(host= CONSUMER_HOST, 
                                port= CONSUMER_PORT,
                                callback_function= return_uppercase, 
                                log= True) 
 
 |
```

### Comparing `rest_solace-0.1.0/src/rest_solace.egg-info/SOURCES.txt` & `rest_solace-0.2.0/src/rest_solace.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -31,9 +31,10 @@
 src/rest_solace/__pycache__/semp_client.cpython-311.pyc
 src/rest_solace/__pycache__/semp_endpoint.cpython-311.pyc
 src/rest_solace/__pycache__/subscriber.cpython-311.pyc
 tests/consumer_test.py
 tests/empty_test.py
 tests/manager_test.py
 tests/pub_sub_test.py
+tests/publisher_test.py
 tests/util.py
 tests/__pycache__/manager_unittest.cpython-311.pyc
```

### Comparing `rest_solace-0.1.0/tests/__pycache__/manager_unittest.cpython-311.pyc` & `rest_solace-0.2.0/tests/__pycache__/manager_unittest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/tests/consumer_test.py` & `rest_solace-0.2.0/tests/consumer_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/tests/empty_test.py` & `rest_solace-0.2.0/tests/empty_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/tests/manager_test.py` & `rest_solace-0.2.0/tests/manager_test.py`

 * *Files identical despite different names*

### Comparing `rest_solace-0.1.0/tests/pub_sub_test.py` & `rest_solace-0.2.0/tests/pub_sub_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                                     msgVpnName= NEW_VPN_NAME)
 
 #Step4: setup publisher, publish a message, and get response
 print("\nPublishing a message and waiting for uppercase response\nSending message:", INPUT_MESSAGE)
 
 res = publish.persistent_message_to_queue(queue_name="queue_rest_consumer", 
                                           message= INPUT_MESSAGE,
+                                          request_reply= True,
                                           time_to_live= 10000 #waits 1 min
                                          )
 
 print("\nResponse:\n",res)
 
 if res.get('content') == EXPECTED_OUTPUT_MESSAGE:
     print("\nTest was a Success")
```

### Comparing `rest_solace-0.1.0/tests/util.py` & `rest_solace-0.2.0/tests/util.py`

 * *Files identical despite different names*

