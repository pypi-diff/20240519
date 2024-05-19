# Comparing `tmp/pypomes_s3-0.3.2.tar.gz` & `tmp/pypomes_s3-0.3.3.tar.gz`

## Comparing `pypomes_s3-0.3.2.tar` & `pypomes_s3-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/__init__.py
--rw-r--r--   0        0        0    22130 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/aws_pomes.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/minio_client.py
--rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/minio_pomes.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/s3_common.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/s3_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/__init__.py
+-rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/aws_pomes.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/minio_client.py
+-rw-r--r--   0        0        0    22101 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/minio_pomes.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/s3_common.py
+-rw-r--r--   0        0        0    27222 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/src/pypomes_s3/s3_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pypomes_s3-0.3.3/PKG-INFO
```

### Comparing `pypomes_s3-0.3.2/src/pypomes_s3/__init__.py` & `pypomes_s3-0.3.3/src/pypomes_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.2/src/pypomes_s3/aws_pomes.py` & `pypomes_s3-0.3.3/src/pypomes_s3/aws_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from unidecode import unidecode
 
 from .s3_common import (
     _s3_get_param, _s3_get_params, _s3_except_msg, _s3_log
 )
 
 
-def _access(errors: list[str],
-            logger: Logger = None) -> BaseClient:
+def access(errors: list[str],
+           logger: Logger = None) -> BaseClient:
     """
     Obtain and return a *AWS* client object.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the S3 client object
     """
@@ -38,17 +38,17 @@
                        exception=e,
                        engine="aws",
                        logger=logger)
 
     return result
 
 
-def _startup(errors: list[str],
-             bucket: str,
-             logger: Logger = None) -> bool:
+def startup(errors: list[str],
+            bucket: str,
+            logger: Logger = None) -> bool:
     """
     Prepare the *AWS* client for operations.
 
     This function should be called just once, at startup,
     to make sure the interaction with the AWS service is fully functional.
 
     :param errors: incidental error messages
@@ -56,16 +56,16 @@
     :param logger: optional logger
     :return: True if service is fully functional
     """
     # initialize the return variable
     result: bool = False
 
     # obtain a AWS client
-    client: BaseClient = _access(errors=errors,
-                                 logger=logger)
+    client: BaseClient = access(errors=errors,
+                                logger=logger)
 
     # was the AWS client obtained ?
     if client:
         # yes, proceed
         try:
             if not client.bucket_exists(bucket_name=bucket):
                 client.make_bucket(bucket_name=bucket)
@@ -76,23 +76,23 @@
             _s3_except_msg(errors=errors,
                            exception=e,
                            engine="aws",
                            logger=logger)
     return result
 
 
-def _file_store(errors: list[str],
-                bucket: str,
-                basepath: Path | str,
-                identifier: str,
-                filepath: Path | str,
-                mimetype: str,
-                tags: dict = None,
-                client: BaseClient = None,
-                logger: Logger = None) -> bool:
+def file_store(errors: list[str],
+               bucket: str,
+               basepath: Path | str,
+               identifier: str,
+               filepath: Path | str,
+               mimetype: str,
+               tags: dict = None,
+               client: BaseClient = None,
+               logger: Logger = None) -> bool:
     """
     Store a file at the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
@@ -103,16 +103,16 @@
     :param logger: optional logger
     :return: True if the file was successfully stored, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # was the AWS client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         # have tags been defined ?
         if tags is None or len(tags) == 0:
             # no
@@ -138,21 +138,21 @@
             _s3_except_msg(errors=errors,
                            exception=e,
                            engine="aws",
                            logger=logger)
     return result
 
 
-def _file_retrieve(errors: list[str],
-                   bucket: str,
-                   basepath: Path | str,
-                   identifier: str,
-                   filepath: Path | str,
-                   client: BaseClient = None,
-                   logger: Logger = None) -> Any:
+def file_retrieve(errors: list[str],
+                  bucket: str,
+                  basepath: Path | str,
+                  identifier: str,
+                  filepath: Path | str,
+                  client: BaseClient = None,
+                  logger: Logger = None) -> Any:
     """
     Retrieve a file from the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
@@ -161,16 +161,16 @@
     :param logger: optional logger
     :return: information about the file retrieved
     """
     # initialize the return variable
     result: Any = None
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # was the AWS client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             result = curr_client.fget_object(bucket_name=bucket,
                                              object_name=f"{remotepath}",
@@ -182,20 +182,20 @@
                 _s3_except_msg(errors=errors,
                                exception=e,
                                engine="aws",
                                logger=logger)
     return result
 
 
-def _object_exists(errors: list[str],
-                   bucket: str,
-                   basepath: Path | str,
-                   identifier: str | None,
-                   client: BaseClient = None,
-                   logger: Logger = None) -> bool:
+def object_exists(errors: list[str],
+                  bucket: str,
+                  basepath: Path | str,
+                  identifier: str | None,
+                  client: BaseClient = None,
+                  logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to locate the object at
     :param identifier: optional object identifier
@@ -203,51 +203,51 @@
     :param logger: optional logger
     :return: True if the object was found, false otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # proceed, if the AWS client eas obtained
     if curr_client:
         # was the identifier provided ?
         if identifier is None:
             # no, object is a folder
-            objs: Iterator = _objects_list(errors=errors,
-                                           bucket=bucket,
-                                           basepath=basepath,
-                                           recursive=False,
-                                           client=curr_client,
-                                           logger=logger)
+            objs: Iterator = objects_list(errors=errors,
+                                          bucket=bucket,
+                                          basepath=basepath,
+                                          recursive=False,
+                                          client=curr_client,
+                                          logger=logger)
             result = next(objs, None) is None
         # verify the status of the object
-        elif _object_stat(errors=errors,
-                          bucket=bucket,
-                          basepath=basepath,
-                          identifier=identifier,
-                          client=curr_client,
-                          logger=logger):
+        elif object_stat(errors=errors,
+                         bucket=bucket,
+                         basepath=basepath,
+                         identifier=identifier,
+                         client=curr_client,
+                         logger=logger):
             result = True
 
         remotepath: Path = Path(basepath) / identifier
         existence: str = "exists" if result else "do not exist"
         _s3_log(logger=logger,
                 stmt=f"Object {remotepath}, bucket {bucket}, {existence}")
 
     return result
 
 
-def _object_stat(errors: list[str],
-                 bucket: str,
-                 basepath: Path | str,
-                 identifier: str,
-                 client: BaseClient = None,
-                 logger: Logger = None) -> dict:
+def object_stat(errors: list[str],
+                bucket: str,
+                basepath: Path | str,
+                identifier: str,
+                client: BaseClient = None,
+                logger: Logger = None) -> dict:
     """
     Retrieve and return the information about an object in the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
@@ -255,16 +255,16 @@
     :param logger: optional logger
     :return: metadata and information about the object
     """
     # initialize the return variable
     result: dict | None = None
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # was the AWS client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             result = curr_client.stat_object(bucket_name=bucket,
                                              object_name=f"{remotepath}")
@@ -275,22 +275,22 @@
                 _s3_except_msg(errors=errors,
                                exception=e,
                                engine="aws",
                                logger=logger)
     return result
 
 
-def _object_store(errors: list[str],
-                  bucket: str,
-                  basepath: Path | str,
-                  identifier: str,
-                  obj: Any,
-                  tags: dict = None,
-                  client: BaseClient = None,
-                  logger: Logger = None) -> bool:
+def object_store(errors: list[str],
+                 bucket: str,
+                 basepath: Path | str,
+                 identifier: str,
+                 obj: Any,
+                 tags: dict = None,
+                 client: BaseClient = None,
+                 logger: Logger = None) -> bool:
     """
     Store an object at the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
@@ -300,35 +300,35 @@
     :param logger: optional logger
     :return: True if the object was successfully stored, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # proceed, if the AWS client was obtained
     if curr_client:
         # serialize the object into a file
         temp_folder: Path = _s3_get_param("minio", "temp-folder")
         filepath: Path = temp_folder / f"{uuid.uuid4()}.pickle"
         with filepath.open("wb") as f:
             pickle.dump(obj, f)
 
         # store the file
         op_errors: list[str] = []
-        _file_store(errors=op_errors,
-                    bucket=bucket,
-                    basepath=basepath,
-                    identifier=identifier,
-                    filepath=filepath,
-                    mimetype="application/octet-stream",
-                    tags=tags,
-                    client=curr_client,
-                    logger=logger)
+        file_store(errors=op_errors,
+                   bucket=bucket,
+                   basepath=basepath,
+                   identifier=identifier,
+                   filepath=filepath,
+                   mimetype="application/octet-stream",
+                   tags=tags,
+                   client=curr_client,
+                   logger=logger)
 
         # errors ?
         if op_errors:
             # yes, report them
             errors.extend(op_errors)
             storage: str = "Unable to store"
         else:
@@ -340,20 +340,20 @@
         remotepath: Path = Path(basepath) / identifier
         _s3_log(logger=logger,
                 stmt=f"{storage} {remotepath}, bucket {bucket}")
 
     return result
 
 
-def _object_retrieve(errors: list[str],
-                     bucket: str,
-                     basepath: Path,
-                     identifier: str,
-                     client: BaseClient = None,
-                     logger: Logger = None) -> Any:
+def object_retrieve(errors: list[str],
+                    bucket: str,
+                    basepath: Path,
+                    identifier: str,
+                    client: BaseClient = None,
+                    logger: Logger = None) -> Any:
     """
     Retrieve an object from the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
@@ -361,28 +361,28 @@
     :param logger: optional logger
     :return: the object retrieved
     """
     # initialize the return variable
     result: Any = None
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # proceed, if the AWS client was obtained
     if curr_client:
         # retrieve the file containg the serialized object
         temp_folder: Path = _s3_get_param("minio", "temp-folder")
         filepath: Path = temp_folder / f"{uuid.uuid4()}.pickle"
-        stat: Any = _file_retrieve(errors=errors,
-                                   bucket=bucket,
-                                   basepath=basepath,
-                                   identifier=identifier,
-                                   filepath=filepath,
-                                   client=curr_client,
-                                   logger=logger)
+        stat: Any = file_retrieve(errors=errors,
+                                  bucket=bucket,
+                                  basepath=basepath,
+                                  identifier=identifier,
+                                  filepath=filepath,
+                                  client=curr_client,
+                                  logger=logger)
 
         # was the file retrieved ?
         if stat:
             # yes, umarshall the corresponding object
             with filepath.open("rb") as f:
                 result = pickle.load(f)
             filepath.unlink()
@@ -391,20 +391,20 @@
         remotepath: Path = Path(basepath) / identifier
         _s3_log(logger=logger,
                 stmt=f"{retrieval} {remotepath}, bucket {bucket}")
 
     return result
 
 
-def _object_delete(errors: list[str],
-                   bucket: str,
-                   basepath: str,
-                   identifier: str = None,
-                   client: BaseClient = None,
-                   logger: Logger = None) -> bool:
+def object_delete(errors: list[str],
+                  bucket: str,
+                  basepath: str,
+                  identifier: str = None,
+                  client: BaseClient = None,
+                  logger: Logger = None) -> bool:
     """
     Remove an object from the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: optional object identifier
@@ -412,26 +412,26 @@
     :param logger: optional logger
     :return: True if the object was successfully deleted, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # proceed, if the AWS client was obtained
     if curr_client:
         # was the identifier provided ?
         if identifier is None:
             # no, remove the folder
-            __folder_delete(errors=errors,
-                            bucket=bucket,
-                            basepath=basepath,
-                            client=curr_client,
-                            logger=logger)
+            _folder_delete(errors=errors,
+                           bucket=bucket,
+                           basepath=basepath,
+                           client=curr_client,
+                           logger=logger)
         else:
             # yes, remove the object
             remotepath: Path = Path(basepath) / identifier
             try:
                 curr_client.remove_object(bucket_name=bucket,
                                           object_name=f"{remotepath}")
                 result = True
@@ -442,20 +442,20 @@
                     _s3_except_msg(errors=errors,
                                    exception=e,
                                    engine="aws",
                                    logger=logger)
     return result
 
 
-def _object_tags_retrieve(errors: list[str],
-                          bucket: str,
-                          basepath: str,
-                          identifier: str,
-                          client: BaseClient = None,
-                          logger: Logger = None) -> dict:
+def object_tags_retrieve(errors: list[str],
+                         bucket: str,
+                         basepath: str,
+                         identifier: str,
+                         client: BaseClient = None,
+                         logger: Logger = None) -> dict:
     """
     Retrieve and return the metadata information for an object in the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
@@ -463,16 +463,16 @@
     :param logger: optional logger
     :return: the metadata about the object
     """
     # initialize the return variable
     result: dict | None = None
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # was the AWS client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             tags: dict = curr_client.get_object_tags(bucket_name=bucket,
                                                      object_name=f"{remotepath}")
@@ -488,20 +488,20 @@
                                exception=e,
                                engine="aws",
                                logger=logger)
 
     return result
 
 
-def _objects_list(errors: list[str],
-                  bucket: str,
-                  basepath: str,
-                  recursive: bool = False,
-                  client: BaseClient = None,
-                  logger: Logger = None) -> Iterator:
+def objects_list(errors: list[str],
+                 bucket: str,
+                 basepath: str,
+                 recursive: bool = False,
+                 client: BaseClient = None,
+                 logger: Logger = None) -> Iterator:
     """
     Retrieve and return an iterator into the list of objects at *basepath*, in the *AWS* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
@@ -509,16 +509,16 @@
     :param logger: optional logger
     :return: the iterator into the list of objects, 'None' if the folder does not exist
     """
     # initialize the return variable
     result: Iterator | None = None
 
     # make sure to have a AWS client
-    curr_client: BaseClient = client or _access(errors=errors,
-                                                logger=logger)
+    curr_client: BaseClient = client or access(errors=errors,
+                                               logger=logger)
     # was the AWS client obtained ?
     if curr_client:
         # yes, proceed
         try:
             result = curr_client.list_objects(bucket_name=bucket,
                                               prefix=basepath,
                                               recursive=recursive)
@@ -529,43 +529,44 @@
                            exception=e,
                            engine="aws",
                            logger=logger)
 
     return result
 
 
-def __folder_delete(errors: list[str],
-                    bucket: str,
-                    basepath: str,
-                    client: BaseClient,
-                    logger: Logger = None) -> None:
+def _folder_delete(errors: list[str],
+                   bucket: str,
+                   basepath: str,
+                   client: BaseClient,
+                   logger: Logger = None) -> None:
     """
     Traverse the folders recursively, removing its objects.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to delete the objects at
     :param client: the MinIO client object
     :param logger: optional logger
     """
     # obtain the list of entries in the given folder
-    objs: Iterator = _objects_list(errors=errors,
-                                   bucket=bucket,
-                                   basepath=basepath,
-                                   recursive=True,
-                                   logger=logger)
+    objs: Iterator = objects_list(errors=errors,
+                                  bucket=bucket,
+                                  basepath=basepath,
+                                  recursive=True,
+                                  logger=logger)
     # was the list obtained ?
     if objs:
         # yes, proceed
         for obj in objs:
             try:
                 client.remove_object(bucket_name=bucket,
                                      object_name=obj.object_name)
                 _s3_log(logger=logger,
                         stmt=f"Removed folder {basepath}, bucket {bucket}")
             except Exception as e:
                 # SANITY CHECK: in case of concurrent exclusion
+                # ruff: noqa: PERF203
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
                     _s3_except_msg(errors=errors,
                                    exception=e,
                                    engine="aws",
                                    logger=logger)
```

### Comparing `pypomes_s3-0.3.2/src/pypomes_s3/minio_client.py` & `pypomes_s3-0.3.3/src/pypomes_s3/minio_client.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.2/src/pypomes_s3/minio_pomes.py` & `pypomes_s3-0.3.3/src/pypomes_s3/minio_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from unidecode import unidecode
 
 from .s3_common import (
     _s3_get_param, _s3_get_params, _s3_except_msg, _s3_log
 )
 
 
-def _access(errors: list[str],
-            logger: Logger = None) -> Minio:
+def access(errors: list[str],
+           logger: Logger = None) -> Minio:
     """
     Obtain and return a *MinIO* client object.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the MinIO client object
     """
@@ -42,17 +42,17 @@
         _s3_except_msg(errors=errors,
                        exception=e,
                        engine="minio",
                        logger=logger)
     return result
 
 
-def _startup(errors: list[str],
-             bucket: str,
-             logger: Logger = None) -> bool:
+def startup(errors: list[str],
+            bucket: str,
+            logger: Logger = None) -> bool:
     """
     Prepare the *MinIO* client for operations.
 
     This function should be called just once, at startup,
     to make sure the interaction with the MinIo service is fully functional.
 
     :param errors: incidental error messages
@@ -60,16 +60,16 @@
     :param logger: optional logger
     :return: True if service is fully functional
     """
     # initialize the return variable
     result: bool = False
 
     # obtain a MinIO client
-    client: Minio = _access(errors=errors,
-                            logger=logger)
+    client: Minio = access(errors=errors,
+                           logger=logger)
 
     # was the MinIO client obtained ?
     if client:
         # yes, proceed
         try:
             if not client.bucket_exists(bucket_name=bucket):
                 client.make_bucket(bucket_name=bucket)
@@ -80,23 +80,23 @@
             _s3_except_msg(errors=errors,
                            exception=e,
                            engine="minio",
                            logger=logger)
     return result
 
 
-def _file_store(errors: list[str],
-                bucket: str,
-                basepath: Path | str,
-                identifier: str,
-                filepath: Path | str,
-                mimetype: str,
-                tags: dict = None,
-                client: Minio = None,
-                logger: Logger = None) -> bool:
+def file_store(errors: list[str],
+               bucket: str,
+               basepath: Path | str,
+               identifier: str,
+               filepath: Path | str,
+               mimetype: str,
+               tags: dict = None,
+               client: Minio = None,
+               logger: Logger = None) -> bool:
     """
     Store a file at the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
@@ -107,16 +107,16 @@
     :param logger: optional logger
     :return: True if the file was successfully stored, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         # have tags been defined ?
         if tags is None or len(tags) == 0:
             # no
@@ -142,21 +142,21 @@
             _s3_except_msg(errors=errors,
                            exception=e,
                            engine="minio",
                            logger=logger)
     return result
 
 
-def _file_retrieve(errors: list[str],
-                   bucket: str,
-                   basepath: Path | str,
-                   identifier: str,
-                   filepath: Path | str,
-                   client: Minio = None,
-                   logger: Logger = None) -> Any:
+def file_retrieve(errors: list[str],
+                  bucket: str,
+                  basepath: Path | str,
+                  identifier: str,
+                  filepath: Path | str,
+                  client: Minio = None,
+                  logger: Logger = None) -> Any:
     """
     Retrieve a file from the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
@@ -165,16 +165,16 @@
     :param logger: optional logger
     :return: information about the file retrieved
     """
     # initialize the return variable
     result: Any = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             result = curr_client.fget_object(bucket_name=bucket,
                                              object_name=f"{remotepath}",
@@ -186,20 +186,20 @@
                 _s3_except_msg(errors=errors,
                                exception=e,
                                engine="minio",
                                logger=logger)
     return result
 
 
-def _object_exists(errors: list[str],
-                   bucket: str,
-                   basepath: Path | str,
-                   identifier: str | None,
-                   client: Minio = None,
-                   logger: Logger = None) -> bool:
+def object_exists(errors: list[str],
+                  bucket: str,
+                  basepath: Path | str,
+                  identifier: str | None,
+                  client: Minio = None,
+                  logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to locate the object at
     :param identifier: optional object identifier
@@ -207,51 +207,51 @@
     :param logger: optional logger
     :return: True if the object was found, false otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # proceed, if the MinIO client eas obtained
     if curr_client:
         # was the identifier provided ?
         if identifier is None:
             # no, object is a folder
-            objs: Iterator = _objects_list(errors=errors,
-                                           bucket=bucket,
-                                           basepath=basepath,
-                                           recursive=False,
-                                           client=curr_client,
-                                           logger=logger)
+            objs: Iterator = objects_list(errors=errors,
+                                          bucket=bucket,
+                                          basepath=basepath,
+                                          recursive=False,
+                                          client=curr_client,
+                                          logger=logger)
             result = next(objs, None) is None
         # verify the status of the object
-        elif _object_stat(errors=errors,
-                          bucket=bucket,
-                          basepath=basepath,
-                          identifier=identifier,
-                          client=curr_client,
-                          logger=logger):
+        elif object_stat(errors=errors,
+                         bucket=bucket,
+                         basepath=basepath,
+                         identifier=identifier,
+                         client=curr_client,
+                         logger=logger):
             result = True
 
         remotepath: Path = Path(basepath) / identifier
         existence: str = "exists" if result else "do not exist"
         _s3_log(logger=logger,
                 stmt=f"Object {remotepath}, bucket {bucket}, {existence}")
 
     return result
 
 
-def _object_stat(errors: list[str],
-                 bucket: str,
-                 basepath: Path | str,
-                 identifier: str,
-                 client: Minio = None,
-                 logger: Logger = None) -> MinioObject:
+def object_stat(errors: list[str],
+                bucket: str,
+                basepath: Path | str,
+                identifier: str,
+                client: Minio = None,
+                logger: Logger = None) -> MinioObject:
     """
     Retrieve and return the information about an object in the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
@@ -259,16 +259,16 @@
     :param logger: optional logger
     :return: metadata and information about the object
     """
     # initialize the return variable
     result: MinioObject | None = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             result = curr_client.stat_object(bucket_name=bucket,
                                              object_name=f"{remotepath}")
@@ -279,22 +279,22 @@
                 _s3_except_msg(errors=errors,
                                exception=e,
                                engine="minio",
                                logger=logger)
     return result
 
 
-def _object_store(errors: list[str],
-                  bucket: str,
-                  basepath: Path | str,
-                  identifier: str,
-                  obj: Any,
-                  tags: dict = None,
-                  client: Minio = None,
-                  logger: Logger = None) -> bool:
+def object_store(errors: list[str],
+                 bucket: str,
+                 basepath: Path | str,
+                 identifier: str,
+                 obj: Any,
+                 tags: dict = None,
+                 client: Minio = None,
+                 logger: Logger = None) -> bool:
     """
     Store an object at the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
@@ -304,35 +304,35 @@
     :param logger: optional logger
     :return: True if the object was successfully stored, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # proceed, if the MinIO client was obtained
     if curr_client:
         # serialize the object into a file
         temp_folder: Path = _s3_get_param("minio", "temp-folder")
         filepath: Path = temp_folder / f"{uuid.uuid4()}.pickle"
         with filepath.open("wb") as f:
             pickle.dump(obj, f)
 
         # store the file
         op_errors: list[str] = []
-        _file_store(errors=op_errors,
-                    bucket=bucket,
-                    basepath=basepath,
-                    identifier=identifier,
-                    filepath=filepath,
-                    mimetype="application/octet-stream",
-                    tags=tags,
-                    client=curr_client,
-                    logger=logger)
+        file_store(errors=op_errors,
+                   bucket=bucket,
+                   basepath=basepath,
+                   identifier=identifier,
+                   filepath=filepath,
+                   mimetype="application/octet-stream",
+                   tags=tags,
+                   client=curr_client,
+                   logger=logger)
 
         # errors ?
         if op_errors:
             # yes, report them
             errors.extend(op_errors)
             storage: str = "Unable to store"
         else:
@@ -344,20 +344,20 @@
         remotepath: Path = Path(basepath) / identifier
         _s3_log(logger=logger,
                 stmt=f"{storage} {remotepath}, bucket {bucket}")
 
     return result
 
 
-def _object_retrieve(errors: list[str],
-                     bucket: str,
-                     basepath: Path,
-                     identifier: str,
-                     client: Minio = None,
-                     logger: Logger = None) -> Any:
+def object_retrieve(errors: list[str],
+                    bucket: str,
+                    basepath: Path,
+                    identifier: str,
+                    client: Minio = None,
+                    logger: Logger = None) -> Any:
     """
     Retrieve an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
@@ -365,28 +365,28 @@
     :param logger: optional logger
     :return: the object retrieved
     """
     # initialize the return variable
     result: Any = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # proceed, if the MinIO client was obtained
     if curr_client:
         # retrieve the file containg the serialized object
         temp_folder: Path = _s3_get_param("minio", "temp-folder")
         filepath: Path = temp_folder / f"{uuid.uuid4()}.pickle"
-        stat: Any = _file_retrieve(errors=errors,
-                                   bucket=bucket,
-                                   basepath=basepath,
-                                   identifier=identifier,
-                                   filepath=filepath,
-                                   client=curr_client,
-                                   logger=logger)
+        stat: Any = file_retrieve(errors=errors,
+                                  bucket=bucket,
+                                  basepath=basepath,
+                                  identifier=identifier,
+                                  filepath=filepath,
+                                  client=curr_client,
+                                  logger=logger)
 
         # was the file retrieved ?
         if stat:
             # yes, umarshall the corresponding object
             with filepath.open("rb") as f:
                 result = pickle.load(f)
             filepath.unlink()
@@ -395,20 +395,20 @@
         remotepath: Path = Path(basepath) / identifier
         _s3_log(logger=logger,
                 stmt=f"{retrieval} {remotepath}, bucket {bucket}")
 
     return result
 
 
-def _object_delete(errors: list[str],
-                   bucket: str,
-                   basepath: str,
-                   identifier: str = None,
-                   client: Minio = None,
-                   logger: Logger = None) -> bool:
+def object_delete(errors: list[str],
+                  bucket: str,
+                  basepath: str,
+                  identifier: str = None,
+                  client: Minio = None,
+                  logger: Logger = None) -> bool:
     """
     Remove an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: optional object identifier
@@ -416,26 +416,26 @@
     :param logger: optional logger
     :return: True if the object was successfully deleted, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # proceed, if the MinIO client was obtained
     if curr_client:
         # was the identifier provided ?
         if identifier is None:
             # no, remove the folder
-            __folder_delete(errors=errors,
-                            bucket=bucket,
-                            basepath=basepath,
-                            client=curr_client,
-                            logger=logger)
+            _folder_delete(errors=errors,
+                           bucket=bucket,
+                           basepath=basepath,
+                           client=curr_client,
+                           logger=logger)
         else:
             # yes, remove the object
             remotepath: Path = Path(basepath) / identifier
             try:
                 curr_client.remove_object(bucket_name=bucket,
                                           object_name=f"{remotepath}")
                 result = True
@@ -446,20 +446,20 @@
                     _s3_except_msg(errors=errors,
                                    exception=e,
                                    engine="minio",
                                    logger=logger)
     return result
 
 
-def _object_tags_retrieve(errors: list[str],
-                          bucket: str,
-                          basepath: str,
-                          identifier: str,
-                          client: Minio = None,
-                          logger: Logger = None) -> dict:
+def object_tags_retrieve(errors: list[str],
+                         bucket: str,
+                         basepath: str,
+                         identifier: str,
+                         client: Minio = None,
+                         logger: Logger = None) -> dict:
     """
     Retrieve and return the metadata information for an object in the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
@@ -467,16 +467,16 @@
     :param logger: optional logger
     :return: the metadata about the object
     """
     # initialize the return variable
     result: dict | None = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             tags: Tags = curr_client.get_object_tags(bucket_name=bucket,
                                                      object_name=f"{remotepath}")
@@ -492,20 +492,20 @@
                                exception=e,
                                engine="minio",
                                logger=logger)
 
     return result
 
 
-def _objects_list(errors: list[str],
-                  bucket: str,
-                  basepath: str,
-                  recursive: bool = False,
-                  client: Minio = None,
-                  logger: Logger = None) -> Iterator:
+def objects_list(errors: list[str],
+                 bucket: str,
+                 basepath: str,
+                 recursive: bool = False,
+                 client: Minio = None,
+                 logger: Logger = None) -> Iterator:
     """
     Retrieve and return an iterator into the list of objects at *basepath*, in the *MinIO* store.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
@@ -513,16 +513,16 @@
     :param logger: optional logger
     :return: the iterator into the list of objects, 'None' if the folder does not exist
     """
     # initialize the return variable
     result: Iterator | None = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or _access(errors=errors,
-                                           logger=logger)
+    curr_client: Minio = client or access(errors=errors,
+                                          logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         try:
             result = curr_client.list_objects(bucket_name=bucket,
                                               prefix=basepath,
                                               recursive=recursive)
@@ -533,43 +533,44 @@
                            exception=e,
                            engine="minio",
                            logger=logger)
 
     return result
 
 
-def __folder_delete(errors: list[str],
-                    bucket: str,
-                    basepath: str,
-                    client: Minio,
-                    logger: Logger = None) -> None:
+def _folder_delete(errors: list[str],
+                   bucket: str,
+                   basepath: str,
+                   client: Minio,
+                   logger: Logger = None) -> None:
     """
     Traverse the folders recursively, removing its objects.
 
     :param errors: incidental error messages
     :param bucket: the bucket to use
     :param basepath: the path specifying the location to delete the objects at
     :param client: the MinIO client object
     :param logger: optional logger
     """
     # obtain the list of entries in the given folder
-    objs: Iterator = _objects_list(errors=errors,
-                                   bucket=bucket,
-                                   basepath=basepath,
-                                   recursive=True,
-                                   logger=logger)
+    objs: Iterator = objects_list(errors=errors,
+                                  bucket=bucket,
+                                  basepath=basepath,
+                                  recursive=True,
+                                  logger=logger)
     # was the list obtained ?
     if objs:
         # yes, proceed
         for obj in objs:
             try:
                 client.remove_object(bucket_name=bucket,
                                      object_name=obj.object_name)
                 _s3_log(logger=logger,
                         stmt=f"Removed folder {basepath}, bucket {bucket}")
             except Exception as e:
                 # SANITY CHECK: in case of concurrent exclusion
+                # ruff: noqa: PERF203
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
                     _s3_except_msg(errors=errors,
                                    exception=e,
                                    engine="minio",
                                    logger=logger)
```

### Comparing `pypomes_s3-0.3.2/src/pypomes_s3/s3_common.py` & `pypomes_s3-0.3.3/src/pypomes_s3/s3_common.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -159,8 +159,8 @@
     """
     if err_msg:
         if logger:
             logger.log(level, err_msg)
         if isinstance(errors, list):
             errors.append(err_msg)
     if logger and stmt:
-        logger.log(level, stmt)
+        logger.log(level, stmt)
```

### Comparing `pypomes_s3-0.3.2/src/pypomes_s3/s3_pomes.py` & `pypomes_s3-0.3.3/src/pypomes_s3/s3_pomes.py`

 * *Files 14% similar despite different names*

```diff
@@ -143,22 +143,20 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._access(errors=op_errors,
-                                   logger=logger)
+        result = aws_pomes.access(errors=op_errors,
+                                  logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._access(errors=op_errors,
-                                     logger=logger)
+        result = minio_pomes.access(errors=op_errors,
+                                    logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -185,24 +183,22 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._startup(errors=op_errors,
-                                    bucket=bucket,
-                                    logger=logger)
+        result = aws_pomes.startup(errors=op_errors,
+                                   bucket=bucket,
+                                   logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._startup(errors=op_errors,
-                                      bucket=bucket,
-                                      logger=logger)
+        result = minio_pomes.startup(errors=op_errors,
+                                     bucket=bucket,
+                                     logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -238,36 +234,34 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._file_store(errors=op_errors,
-                                       bucket=bucket,
-                                       basepath=basepath,
-                                       identifier=identifier,
-                                       filepath=filepath,
-                                       mimetype=mimetype,
-                                       tags=tags,
-                                       client=client,
-                                       logger=logger)
+        result = aws_pomes.file_store(errors=op_errors,
+                                      bucket=bucket,
+                                      basepath=basepath,
+                                      identifier=identifier,
+                                      filepath=filepath,
+                                      mimetype=mimetype,
+                                      tags=tags,
+                                      client=client,
+                                      logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._file_store(errors=op_errors,
-                                         bucket=bucket,
-                                         basepath=basepath,
-                                         identifier=identifier,
-                                         filepath=filepath,
-                                         mimetype=mimetype,
-                                         tags=tags,
-                                         client=client,
-                                         logger=logger)
+        result = minio_pomes.file_store(errors=op_errors,
+                                        bucket=bucket,
+                                        basepath=basepath,
+                                        identifier=identifier,
+                                        filepath=filepath,
+                                        mimetype=mimetype,
+                                        tags=tags,
+                                        client=client,
+                                        logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -299,32 +293,30 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._file_retrieve(errors=op_errors,
-                                          bucket=bucket,
-                                          basepath=basepath,
-                                          identifier=identifier,
-                                          filepath=filepath,
-                                          client=client,
-                                          logger=logger)
+        result = aws_pomes.file_retrieve(errors=op_errors,
+                                         bucket=bucket,
+                                         basepath=basepath,
+                                         identifier=identifier,
+                                         filepath=filepath,
+                                         client=client,
+                                         logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._file_retrieve(errors=op_errors,
-                                            bucket=bucket,
-                                            basepath=basepath,
-                                            identifier=identifier,
-                                            filepath=filepath,
-                                            client=client,
-                                            logger=logger)
+        result = minio_pomes.file_retrieve(errors=op_errors,
+                                           bucket=bucket,
+                                           basepath=basepath,
+                                           identifier=identifier,
+                                           filepath=filepath,
+                                           client=client,
+                                           logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -354,30 +346,28 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._object_exists(errors=op_errors,
-                                          bucket=bucket,
-                                          basepath=basepath,
-                                          identifier=identifier,
-                                          client=client,
-                                          logger=logger)
+        result = aws_pomes.object_exists(errors=op_errors,
+                                         bucket=bucket,
+                                         basepath=basepath,
+                                         identifier=identifier,
+                                         client=client,
+                                         logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._object_exists(errors=op_errors,
-                                            bucket=bucket,
-                                            basepath=basepath,
-                                            identifier=identifier,
-                                            client=client,
-                                            logger=logger)
+        result = minio_pomes.object_exists(errors=op_errors,
+                                           bucket=bucket,
+                                           basepath=basepath,
+                                           identifier=identifier,
+                                           client=client,
+                                           logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -407,30 +397,28 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._object_stat(errors=op_errors,
-                                        bucket=bucket,
-                                        basepath=basepath,
-                                        identifier=identifier,
-                                        client=client,
-                                        logger=logger)
+        result = aws_pomes.object_stat(errors=op_errors,
+                                       bucket=bucket,
+                                       basepath=basepath,
+                                       identifier=identifier,
+                                       client=client,
+                                       logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._object_stat(errors=op_errors,
-                                          bucket=bucket,
-                                          basepath=basepath,
-                                          identifier=identifier,
-                                          client=client,
-                                          logger=logger)
+        result = minio_pomes.object_stat(errors=op_errors,
+                                         bucket=bucket,
+                                         basepath=basepath,
+                                         identifier=identifier,
+                                         client=client,
+                                         logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -464,34 +452,32 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._object_store(errors=op_errors,
-                                         bucket=bucket,
-                                         basepath=basepath,
-                                         identifier=identifier,
-                                         obj=obj,
-                                         tags=tags,
-                                         client=client,
-                                         logger=logger)
+        result = aws_pomes.object_store(errors=op_errors,
+                                        bucket=bucket,
+                                        basepath=basepath,
+                                        identifier=identifier,
+                                        obj=obj,
+                                        tags=tags,
+                                        client=client,
+                                        logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._object_store(errors=op_errors,
-                                           bucket=bucket,
-                                           basepath=basepath,
-                                           identifier=identifier,
-                                           obj=obj,
-                                           tags=tags,
-                                           client=client,
-                                           logger=logger)
+        result = minio_pomes.object_store(errors=op_errors,
+                                          bucket=bucket,
+                                          basepath=basepath,
+                                          identifier=identifier,
+                                          obj=obj,
+                                          tags=tags,
+                                          client=client,
+                                          logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -521,30 +507,28 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._object_retrieve(errors=op_errors,
-                                            bucket=bucket,
-                                            basepath=basepath,
-                                            identifier=identifier,
-                                            client=client,
-                                            logger=logger)
-    elif curr_engine == "minio":
-        from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._object_retrieve(errors=op_errors,
-                                              bucket=bucket,
-                                              basepath=basepath,
-                                              identifier=identifier,
-                                              client=client,
-                                              logger=logger)
+        result = aws_pomes.object_retrieve(errors=op_errors,
+                                           bucket=bucket,
+                                           basepath=basepath,
+                                           identifier=identifier,
+                                           client=client,
+                                           logger=logger)
+    elif curr_engine == "minio":
+        from . import minio_pomes
+        result = minio_pomes.object_retrieve(errors=op_errors,
+                                             bucket=bucket,
+                                             basepath=basepath,
+                                             identifier=identifier,
+                                             client=client,
+                                             logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -574,30 +558,28 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._object_delete(errors=op_errors,
-                                          bucket=bucket,
-                                          basepath=basepath,
-                                          identifier=identifier,
-                                          client=client,
-                                          logger=logger)
+        result = aws_pomes.object_delete(errors=op_errors,
+                                         bucket=bucket,
+                                         basepath=basepath,
+                                         identifier=identifier,
+                                         client=client,
+                                         logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._object_delete(errors=op_errors,
-                                            bucket=bucket,
-                                            basepath=basepath,
-                                            identifier=identifier,
-                                            client=client,
-                                            logger=logger)
+        result = minio_pomes.object_delete(errors=op_errors,
+                                           bucket=bucket,
+                                           basepath=basepath,
+                                           identifier=identifier,
+                                           client=client,
+                                           logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -627,30 +609,28 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._object_tags_retrieve(errors=op_errors,
-                                                 bucket=bucket,
-                                                 basepath=basepath,
-                                                 identifier=identifier,
-                                                 client=client,
-                                                 logger=logger)
-    elif curr_engine == "minio":
-        from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._object_tags_retrieve(errors=op_errors,
-                                                   bucket=bucket,
-                                                   basepath=basepath,
-                                                   identifier=identifier,
-                                                   client=client,
-                                                   logger=logger)
+        result = aws_pomes.object_tags_retrieve(errors=op_errors,
+                                                bucket=bucket,
+                                                basepath=basepath,
+                                                identifier=identifier,
+                                                client=client,
+                                                logger=logger)
+    elif curr_engine == "minio":
+        from . import minio_pomes
+        result = minio_pomes.object_tags_retrieve(errors=op_errors,
+                                                  bucket=bucket,
+                                                  basepath=basepath,
+                                                  identifier=identifier,
+                                                  client=client,
+                                                  logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -680,28 +660,26 @@
     op_errors: list[str] = []
 
     # determine the S3 engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "aws":
         from . import aws_pomes
-        # noinspection PyProtectedMember
-        result = aws_pomes._objects_list(errors=op_errors,
-                                         bucket=bucket,
-                                         basepath=basepath,
-                                         recursive=recursive,
-                                         client=client,
-                                         logger=logger)
+        result = aws_pomes.objects_list(errors=op_errors,
+                                        bucket=bucket,
+                                        basepath=basepath,
+                                        recursive=recursive,
+                                        client=client,
+                                        logger=logger)
     elif curr_engine == "minio":
         from . import minio_pomes
-        # noinspection PyProtectedMember
-        result = minio_pomes._objects_list(errors=op_errors,
-                                           bucket=bucket,
-                                           basepath=basepath,
-                                           recursive=recursive,
-                                           client=client,
-                                           logger=logger)
+        result = minio_pomes.objects_list(errors=op_errors,
+                                          bucket=bucket,
+                                          basepath=basepath,
+                                          recursive=recursive,
+                                          client=client,
+                                          logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
-    return result
+    return result
```

### Comparing `pypomes_s3-0.3.2/LICENSE` & `pypomes_s3-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.2/pyproject.toml` & `pypomes_s3-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_s3"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (S3 storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_s3-0.3.2/PKG-INFO` & `pypomes_s3-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_s3
-Version: 0.3.2
+Version: 0.3.3
 Summary: A collection of Python pomes, pennyeach (S3 storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-S3
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-S3/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

