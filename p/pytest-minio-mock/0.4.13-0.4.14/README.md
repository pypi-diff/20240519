# Comparing `tmp/pytest_minio_mock-0.4.13.tar.gz` & `tmp/pytest_minio_mock-0.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_minio_mock-0.4.13.tar", last modified: Sat Apr 27 12:12:57 2024, max compression
+gzip compressed data, was "pytest_minio_mock-0.4.14.tar", last modified: Sun May 19 11:02:29 2024, max compression
```

## Comparing `pytest_minio_mock-0.4.13.tar` & `pytest_minio_mock-0.4.14.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.812839 pytest_minio_mock-0.4.13/pytest_minio_mock/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/pytest_minio_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49156 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/pytest_minio_mock/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-27 12:12:57.000000 pytest_minio_mock-0.4.13/pytest_minio_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 12:12:57.816839 pytest_minio_mock-0.4.13/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18517 2024-04-27 12:12:52.000000 pytest_minio_mock-0.4.13/tests/test_minio_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/pytest_minio_mock/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/pytest_minio_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49707 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/pytest_minio_mock/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:02:29.000000 pytest_minio_mock-0.4.14/pytest_minio_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:02:29.624246 pytest_minio_mock-0.4.14/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    19719 2024-05-19 11:02:26.000000 pytest_minio_mock-0.4.14/tests/test_minio_mock.py
```

### Comparing `pytest_minio_mock-0.4.13/LICENSE` & `pytest_minio_mock-0.4.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_minio_mock-0.4.13/README.md` & `pytest_minio_mock-0.4.14/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,38 @@
 `pytest-minio-mock` is a pytest plugin designed to simplify testing of applications that interact with Minio the code  S3 compatible object storage system. It is not designed to test the correnction to the minio server. It provides a fixture that mocks the `minio.Minio` class, allowing for easy testing of Minio interactions without the need for a real Minio server.
 
 The plugin supports python version 3.8 or above.
 
 ## Features
 - Mock implementation of the `minio.Minio` client.
 - Easy to use pytest fixture.
-- Supports common Minio operations such as bucket creation, file upload/download, etc.
+- Supports versioning.
+- Currently the plugin mocks the following Minio client APIs:
+
+    **Bucket Operations:**
+  
+    - `make_bucket`
+    - `list_buckets`
+    - `bucket_exists`
+    - `remove_bucket`
+    - `list_objects`
+    - `get_bucket_versioning`
+    - `set_bucket_versioning`
+    
+    **Objects Operations:**
+    
+    - `get_object`
+    - `fget_object`
+    - `put_object`
+    - `fput_object`
+    - `stat_object`
+    - `remove_object`
+    - `get_presigned_url`
+    - `presigned_put_object`
+    - `presigned_get_object`
 
 ## Installation
 
 To install `pytest-minio-mock`, run:
 
 ```bash
 pip install pytest-minio-mock
@@ -71,14 +94,15 @@
 
 A brief description of the mocked methods and their behavior, like:
 
 - `make_bucket(bucket_name, ...)` # Mocks bucket creation.
 - `fput_object(bucket_name, object_name, file_path, ...)` # Mocks file upload.
 - ...
 
+
 ## Contributing
 Contributions to pytest-minio-mock are welcome!
 
 Follow the usual path:
  - fork the repository
  - create a feature branch
  - push the branch to your forked repository
```

### Comparing `pytest_minio_mock-0.4.13/pytest_minio_mock/__init__.py` & `pytest_minio_mock-0.4.14/pytest_minio_mock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
 For more information and usage examples, please refer to the project's README.md.
 
 """
 
 __title__ = "pytest-minio-mock"
 __description__ = "A pytest plugin for mocking Minio S3 interactions"
-__version__ = "0.4.13"
+__version__ = "0.4.14"
 __status__ = "Production"
 __license__ = "MIT"
 __author__ = "Oussama Jarrousse"
 __maintainer__ = "Oussama Jarrousse"
 __email__ = "oussama@jarrousse.org"
 __credits__ = ["Gustavo Satheler", "@cottephi", "Wouter van Atteveldt"]
```

### Comparing `pytest_minio_mock-0.4.13/pytest_minio_mock/plugin.py` & `pytest_minio_mock-0.4.14/pytest_minio_mock/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 This module allows you to test file uploads, downloads, bucket creations, and other Minio operations
 by simulating the Minio environment. It's useful in scenarios where you want to ensure your
 application interacts correctly with Minio, without the overhead of connecting to an actual Minio
 server.
 """
 import copy
 import datetime
+import errno
 import io
 import logging
 import os
 from uuid import uuid4
 
 import pytest
 import validators
@@ -817,15 +818,15 @@
 
     def fget_object(
         self,
         bucket_name,
         object_name,
         file_path,
         request_headers=None,
-        sse=None,
+        ssec=None,
         version_id=None,
         extra_query_params=None,
     ):
         """
         Simulates Minio's 'fget_object' method to download an object from the mock Minio
         server and save it to a file.
 
@@ -847,26 +848,51 @@
                 Defaults to None.
 
         Raises:
             ValueError: If the specified bucket or object doesn't exist in the mock data.
             IOError: If there's an issue writing to the specified file path.
 
         Returns:
-            None: The method writes the object's data to a file and has no return value.
+            Object: Stat of the object as Object.
         """
+
+        stat = self.stat_object(
+            bucket_name,
+            object_name,
+            ssec,
+            version_id,
+        )
+
         the_object = self.get_object(
             bucket_name,
             object_name,
-            version_id=version_id,
             request_headers=request_headers,
+            ssec=ssec,
+            version_id=version_id,
             extra_query_params=extra_query_params,
         )
+
+        if os.path.isdir(file_path):
+            raise ValueError(f"file {file_path} is a directory")
+
+        # Create top level directory if needed.
+
+        dirname = os.path.dirname(file_path)
+        if dirname:
+            try:
+                os.makedirs(dirname)
+            except OSError as exc:  # Python >2.5
+                if exc.errno != errno.EEXIST:
+                    raise
+
         with open(file_path, "wb") as f:
             f.write(the_object.data)
 
+        return stat
+
     def get_object(
         self,
         bucket_name,
         object_name,
         offset: int = 0,
         length: int = 0,
         request_headers=None,
```

### Comparing `pytest_minio_mock-0.4.13/setup.py` & `pytest_minio_mock-0.4.14/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     license="MIT",
     author="Oussama Jarrousse",
     author_email="oussama@jarrousse.org",
     description="A pytest plugin for mocking Minio S3 interactions",
     long_description=open("README.md").read(),
     keywords="pytest minio mock",
     extras_require={"dev": ["pre-commit", "tox"]},
-    version="0.4.13",
+    version="0.4.14",
     long_description_content_type="text/markdown",
     classifiers=[
         "Framework :: Pytest",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
```

### Comparing `pytest_minio_mock-0.4.13/tests/test_minio_mock.py` & `pytest_minio_mock-0.4.14/tests/test_minio_mock.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 import sys
 
 import pytest
 import validators
 from minio import Minio
 from minio.commonconfig import ENABLED
 from minio.datatypes import Bucket
+from minio.datatypes import Object
 from minio.error import S3Error
 from minio.versioningconfig import OFF
 from minio.versioningconfig import SUSPENDED
 from minio.versioningconfig import VersioningConfig
 
 from pytest_minio_mock.plugin import MockMinioBucket
 from pytest_minio_mock.plugin import MockMinioObject
@@ -489,7 +491,38 @@
     objects = list(client.list_objects(bucket_name=bucket_name, include_version=True))
     object_stat = client.stat_object(
         bucket_name=bucket_name,
         object_name=object_name,
         version_id=objects[1].version_id,
     )
     assert object_stat.version_id is None
+
+
+@pytest.mark.REGRESSION
+@pytest.mark.UNIT
+def test_fget_object(minio_mock, tmp_path):
+    client = Minio("http://local.host:9000")
+
+    bucket_name = "new-bucket"
+    client.make_bucket(bucket_name)
+    objects = client.list_objects(bucket_name)
+    assert len(list(objects)) == 0
+
+    client.put_object(bucket_name, "object1", data=b"object1 data", length=12)
+
+    file_path = tmp_path  # should raise a Value error
+    with pytest.raises(ValueError):
+        _ = client.fget_object(bucket_name, "object1", file_path)
+
+    file_path = os.path.join(tmp_path, "object1.dat")
+    stat = client.fget_object(bucket_name, "object1", file_path)
+    assert isinstance(stat, Object)
+
+    # folder objects does not exist, fget_object should create it
+    file_path = os.path.join(tmp_path, "another_folder", "object1.dat")
+    stat = client.fget_object(bucket_name, "object1", file_path)
+    assert isinstance(stat, Object)
+
+    # folder objects does not exist, fget_object should create it
+    file_path = os.path.join(tmp_path, "another_folder", "object1.dat")
+    stat = client.fget_object(bucket_name, "object1", file_path)
+    assert isinstance(stat, Object)
```

