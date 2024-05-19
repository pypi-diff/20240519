# Comparing `tmp/pypomes_s3-0.3.4.tar.gz` & `tmp/pypomes_s3-0.3.5.tar.gz`

## Comparing `pypomes_s3-0.3.4.tar` & `pypomes_s3-0.3.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/__init__.py
--rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/aws_pomes.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/minio_client.py
--rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/minio_pomes.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/s3_common.py
--rw-r--r--   0        0        0    27222 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/src/pypomes_s3/s3_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/__init__.py
+-rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/aws_pomes.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/minio_client.py
+-rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/minio_pomes.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/s3_common.py
+-rw-r--r--   0        0        0    29382 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/src/pypomes_s3/s3_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.5/PKG-INFO
```

### Comparing `pypomes_s3-0.3.4/src/pypomes_s3/__init__.py` & `pypomes_s3-0.3.5/src/pypomes_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.4/src/pypomes_s3/aws_pomes.py` & `pypomes_s3-0.3.5/src/pypomes_s3/aws_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.4/src/pypomes_s3/minio_client.py` & `pypomes_s3-0.3.5/src/pypomes_s3/minio_client.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.4/src/pypomes_s3/minio_pomes.py` & `pypomes_s3-0.3.5/src/pypomes_s3/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.4/src/pypomes_s3/s3_common.py` & `pypomes_s3-0.3.5/src/pypomes_s3/s3_common.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.4/src/pypomes_s3/s3_pomes.py` & `pypomes_s3-0.3.5/src/pypomes_s3/s3_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import Iterator
 from logging import Logger
 from pathlib import Path
 from typing import Any
 
 from .s3_common import (
-    _S3_ENGINES, _S3_ACCESS_DATA, _assert_engine
+    _S3_ENGINES, _S3_ACCESS_DATA,
+    _assert_engine, _s3_get_param
 )
 
 
 def s3_setup(engine: str,
              access_key: str,
              access_secret: str,
              bucket_name: str,
@@ -157,38 +158,42 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_startup(errors: list[str],
-               bucket: str,
+               bucket: str = None,
                engine: str = None,
                logger: Logger = None) -> bool:
     """
     Prepare the S3 *client* for operations.
 
     This function should be called just once, at startup,
     to make sure the interaction with the MinIo service is fully functional.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param logger: optional logger
     :return: True if service is fully functional
     """
     # initialize the return variable
     result: bool = False
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.startup(errors=op_errors,
                                    bucket=bucket,
                                    logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
@@ -199,47 +204,51 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_file_store(errors: list[str],
-                  bucket: str,
                   basepath: Path | str,
                   identifier: str,
                   filepath: Path | str,
                   mimetype: str,
                   tags: dict = None,
+                  bucket: str = None,
                   engine: Any = None,
                   client: Any = None,
                   logger: Logger = None) -> bool:
     """
     Store a file at the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
     :param mimetype: the file mimetype
     :param tags: optional metadata describing the file
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the file was successfully stored, False otherwise
     """
     # initialize the return variable
     result: bool | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.file_store(errors=op_errors,
                                       bucket=bucket,
                                       basepath=basepath,
                                       identifier=identifier,
                                       filepath=filepath,
@@ -262,43 +271,47 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_file_retrieve(errors: list[str],
-                     bucket: str,
                      basepath: Path | str,
                      identifier: str,
                      filepath: Path | str,
+                     bucket: str = None,
                      engine: str = None,
                      client: Any = None,
                      logger: Logger = None) -> Any:
     """
     Retrieve a file from the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path to save the retrieved file at
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: information about the file retrieved
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.file_retrieve(errors=op_errors,
                                          bucket=bucket,
                                          basepath=basepath,
                                          identifier=identifier,
                                          filepath=filepath,
@@ -317,41 +330,45 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_exists(errors: list[str],
-                     bucket: str,
                      basepath: Path | str,
                      identifier: str | None,
+                     bucket: str = None,
                      engine: str = None,
                      client: Any = None,
                      logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to locate the object at
     :param identifier: optional object identifier
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the object was found, false otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.object_exists(errors=op_errors,
                                          bucket=bucket,
                                          basepath=basepath,
                                          identifier=identifier,
                                          client=client,
@@ -368,41 +385,45 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_stat(errors: list[str],
-                   bucket: str,
                    basepath: Path | str,
                    identifier: str,
+                   bucket: str = None,
                    engine: str = None,
                    client: Any = None,
                    logger: Logger = None) -> Any:
     """
     Retrieve and return the information about an object in the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: metadata and information about the object
     """
     # initialize the return variable
     result: Any | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.object_stat(errors=op_errors,
                                        bucket=bucket,
                                        basepath=basepath,
                                        identifier=identifier,
                                        client=client,
@@ -419,45 +440,49 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_store(errors: list[str],
-                    bucket: str,
                     basepath: Path | str,
                     identifier: str,
                     obj: Any,
                     tags: dict = None,
+                    bucket: str = None,
                     engine: str = None,
                     client: Any = None,
                     logger: Logger = None) -> bool:
     """
     Store an object at the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
     :param obj: object to be stored
     :param tags: optional metadata describing the object
     :param engine: the S3 engine to use (uses the default engine, if not provided)
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the object was successfully stored, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.object_store(errors=op_errors,
                                         bucket=bucket,
                                         basepath=basepath,
                                         identifier=identifier,
                                         obj=obj,
@@ -478,41 +503,45 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_retrieve(errors: list[str],
-                       bucket: str,
                        basepath: Path,
                        identifier: str,
+                       bucket: str = None,
                        engine: str = None,
                        client: Any = None,
                        logger: Logger = None) -> Any:
     """
     Retrieve an object from the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the object retrieved
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.object_retrieve(errors=op_errors,
                                            bucket=bucket,
                                            basepath=basepath,
                                            identifier=identifier,
                                            client=client,
@@ -529,41 +558,45 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_delete(errors: list[str],
-                     bucket: str,
                      basepath: str,
                      identifier: str = None,
+                     bucket: str = None,
                      engine: str = None,
                      client: Any = None,
                      logger: Logger = None) -> bool:
     """
     Remove an object from the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: optional object identifier
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if the object was successfully deleted, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.object_delete(errors=op_errors,
                                          bucket=bucket,
                                          basepath=basepath,
                                          identifier=identifier,
                                          client=client,
@@ -580,41 +613,45 @@
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
 def s3_object_tags_retrieve(errors: list[str],
-                            bucket: str,
                             basepath: str,
                             identifier: str,
+                            bucket: str = None,
                             engine: str = None,
                             client: Any = None,
                             logger: Logger = None) -> dict:
     """
     Retrieve and return the metadata information for an object in the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the metadata about the object
     """
     # initialize the return variable
     result: dict | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.object_tags_retrieve(errors=op_errors,
                                                 bucket=bucket,
                                                 basepath=basepath,
                                                 identifier=identifier,
                                                 client=client,
@@ -632,40 +669,44 @@
     errors.extend(op_errors)
 
     return result
 
 
 def s3_objects_list(errors: list[str],
                     basepath: str,
-                    bucket: str,
                     recursive: bool = False,
+                    bucket: str = None,
                     engine: str = None,
                     client: Any = None,
                     logger: Logger = None) -> Iterator:
     """
     Retrieve and return an iterator into the list of objects at *basepath*, in the S3 store.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
+    :param bucket: the bucket to use (uses the default bucket, if not provided)
     :param engine: the S3 engine to use (uses the default engine, if not provided)
     :param client: optional S3 client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the iterator into the list of objects, 'None' if the folder does not exist
     """
     # initialize the return variable
     result: Iterator | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
+    # make sure to have a bucket name
+    if not bucket:
+        bucket = _s3_get_param(engine=curr_engine,
+                               param="bucket-name")
     if curr_engine == "aws":
         from . import aws_pomes
         result = aws_pomes.objects_list(errors=op_errors,
                                         bucket=bucket,
                                         basepath=basepath,
                                         recursive=recursive,
                                         client=client,
```

### Comparing `pypomes_s3-0.3.4/LICENSE` & `pypomes_s3-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.4/pyproject.toml` & `pypomes_s3-0.3.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_s3"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (S3 storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_s3-0.3.4/PKG-INFO` & `pypomes_s3-0.3.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_s3
-Version: 0.3.4
+Version: 0.3.5
 Summary: A collection of Python pomes, pennyeach (S3 storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-S3
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-S3/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

