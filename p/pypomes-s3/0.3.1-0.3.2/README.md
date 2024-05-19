# Comparing `tmp/pypomes_s3-0.3.1.tar.gz` & `tmp/pypomes_s3-0.3.2.tar.gz`

## Comparing `pypomes_s3-0.3.1.tar` & `pypomes_s3-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/__init__.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/pypomes_s3/__init__.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/pypomes_s3/aws_pomes.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/pypomes_s3/minio_client.py
--rw-r--r--   0        0        0    23774 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/pypomes_s3/minio_pomes.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/pypomes_s3/s3_common.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/src/pypomes_s3/s3_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/README.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pypomes_s3-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/__init__.py
+-rw-r--r--   0        0        0    22130 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/aws_pomes.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/minio_client.py
+-rw-r--r--   0        0        0    22190 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/minio_pomes.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/s3_common.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/src/pypomes_s3/s3_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/README.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pypomes_s3-0.3.2/PKG-INFO
```

### Comparing `pypomes_s3-0.3.1/src/pypomes_s3/minio_client.py` & `pypomes_s3-0.3.2/src/pypomes_s3/minio_client.py`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.1/src/pypomes_s3/minio_pomes.py` & `pypomes_s3-0.3.2/src/pypomes_s3/minio_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,123 +2,121 @@
 import uuid
 from collections.abc import Iterator
 from logging import Logger
 from minio import Minio
 from minio.datatypes import Object as MinioObject
 from minio.commonconfig import Tags
 from pathlib import Path
-from pypomes_core import (
-    APP_PREFIX, TEMP_DIR,
-    env_get_bool, env_get_str, env_get_path
-)
-from typing import Final
+from typing import Any
 from unidecode import unidecode
 
-MINIO_BUCKET_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET_URL")
-MINIO_ENDPOINT_URL: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_ENDPOINT_URL")
-MINIO_ACCESS_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY")
-MINIO_SECRET_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY")
-MINIO_SECURE_ACCESS: Final[bool] = env_get_bool(f"{APP_PREFIX}_MINIO_SECURE_ACCESS")
-MINIO_TEMP_PATH: Final[Path] = env_get_path(f"{APP_PREFIX}_MINIO_TEMP_PATH", TEMP_DIR)
+from .s3_common import (
+    _s3_get_param, _s3_get_params, _s3_except_msg, _s3_log
+)
 
 
-def minio_access(errors: list[str],
-                 logger: Logger = None) -> Minio:
+def _access(errors: list[str],
+            logger: Logger = None) -> Minio:
     """
     Obtain and return a *MinIO* client object.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the MinIO client object
     """
     # initialize the return variable
     result: Minio | None = None
 
+    # retrieve the access parameters
+    access_key, secret_key, endpoint, secure = _s3_get_params("minio")
+
     # obtain the MinIO client
     try:
-        result = Minio(endpoint=MINIO_ENDPOINT_URL,
-                       access_key=MINIO_ACCESS_KEY,
-                       secret_key=MINIO_SECRET_KEY,
-                       secure=MINIO_SECURE_ACCESS)
-        if logger:
-            logger.debug("Minio client created")
+        result = Minio(access_key=access_key,
+                       secret_key=secret_key,
+                       endpoint=endpoint,
+                       secure=secure)
+        _s3_log(logger=logger,
+                stmt="Minio client created")
 
     except Exception as e:
-        __minio_except_msg(errors=errors,
-                           exception=e,
-                           logger=logger)
-
+        _s3_except_msg(errors=errors,
+                       exception=e,
+                       engine="minio",
+                       logger=logger)
     return result
 
 
-def minio_setup(errors: list[str],
-                bucket: str = MINIO_BUCKET_NAME,
-                client: Minio = None,
-                logger: Logger = None) -> bool:
+def _startup(errors: list[str],
+             bucket: str,
+             logger: Logger = None) -> bool:
     """
     Prepare the *MinIO* client for operations.
 
     This function should be called just once, at startup,
     to make sure the interaction with the MinIo service is fully functional.
 
     :param errors: incidental error messages
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
-    :param client: optional MinIO client (obtains a new one, if not provided)
+    :param bucket: the bucket to use
     :param logger: optional logger
     :return: True if service is fully functional
     """
     # initialize the return variable
     result: bool = False
 
-    # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    # obtain a MinIO client
+    client: Minio = _access(errors=errors,
+                            logger=logger)
+
     # was the MinIO client obtained ?
-    if curr_client:
+    if client:
         # yes, proceed
         try:
-            if not curr_client.bucket_exists(bucket_name=bucket):
-                curr_client.make_bucket(bucket_name=bucket)
+            if not client.bucket_exists(bucket_name=bucket):
+                client.make_bucket(bucket_name=bucket)
             result = True
-            if logger:
-                logger.debug(f"Setup MinIO, endpoint={MINIO_ENDPOINT_URL}, bucket={bucket}, "
-                             f"access key={MINIO_ACCESS_KEY}, secure={MINIO_SECURE_ACCESS}")
+            _s3_log(logger=logger,
+                    stmt=f"Started MinIO, bucket={bucket}")
         except Exception as e:
-            __minio_except_msg(errors=errors,
-                               exception=e,
-                               logger=logger)
-
+            _s3_except_msg(errors=errors,
+                           exception=e,
+                           engine="minio",
+                           logger=logger)
     return result
 
 
-def minio_file_store(errors: list[str],
-                     basepath: Path | str,
-                     identifier: str,
-                     filepath: Path | str,
-                     mimetype: str,
-                     tags: dict = None,
-                     bucket: str = MINIO_BUCKET_NAME,
-                     client: Minio = None,
-                     logger: Logger = None) -> None:
+def _file_store(errors: list[str],
+                bucket: str,
+                basepath: Path | str,
+                identifier: str,
+                filepath: Path | str,
+                mimetype: str,
+                tags: dict = None,
+                client: Minio = None,
+                logger: Logger = None) -> bool:
     """
     Store a file at the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
     :param mimetype: the file mimetype
     :param tags: optional metadata describing the file
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
+    :return: True if the file was successfully stored, False otherwise
     """
+    # initialize the return variable
+    result: bool = False
+
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         # have tags been defined ?
         if tags is None or len(tags) == 0:
             # no
@@ -132,447 +130,446 @@
         # store the file
         try:
             curr_client.fput_object(bucket_name=bucket,
                                     object_name=f"{remotepath}",
                                     file_path=filepath,
                                     content_type=mimetype,
                                     tags=doc_tags)
-            if logger:
-                logger.debug(f"Stored {remotepath}, "
-                             f"content type {mimetype}, tags {tags}, bucket {bucket}")
+            result = True
+            _s3_log(logger=logger,
+                    stmt=(f"Stored {remotepath}, bucket {bucket}, "
+                          f"content type {mimetype}, tags {tags}"))
         except Exception as e:
-            __minio_except_msg(errors=errors,
-                               exception=e,
-                               logger=logger)
+            _s3_except_msg(errors=errors,
+                           exception=e,
+                           engine="minio",
+                           logger=logger)
+    return result
 
 
-def minio_file_retrieve(errors: list[str],
-                        basepath: Path | str,
-                        identifier: str,
-                        filepath: Path | str,
-                        bucket: str = MINIO_BUCKET_NAME,
-                        client: Minio = None,
-                        logger: Logger = None) -> any:
+def _file_retrieve(errors: list[str],
+                   bucket: str,
+                   basepath: Path | str,
+                   identifier: str,
+                   filepath: Path | str,
+                   client: Minio = None,
+                   logger: Logger = None) -> Any:
     """
     Retrieve a file from the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the file from
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path to save the retrieved file at
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: information about the file retrieved
     """
     # initialize the return variable
-    result: any = None
+    result: Any = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             result = curr_client.fget_object(bucket_name=bucket,
                                              object_name=f"{remotepath}",
                                              file_path=filepath)
-            if logger:
-                logger.debug(f"Retrieved {remotepath}, bucket {bucket}")
+            _s3_log(logger=logger,
+                    stmt=f"Retrieved {remotepath}, bucket {bucket}")
         except Exception as e:
             if not hasattr(e, "code") or e.code != "NoSuchKey":
-                __minio_except_msg(errors=errors,
-                                   exception=e,
-                                   logger=logger)
-
+                _s3_except_msg(errors=errors,
+                               exception=e,
+                               engine="minio",
+                               logger=logger)
     return result
 
 
-def minio_object_exists(errors: list[str],
-                        basepath: Path | str,
-                        identifier: str = None,
-                        bucket: str = MINIO_BUCKET_NAME,
-                        client: Minio = None,
-                        logger: Logger = None) -> bool:
+def _object_exists(errors: list[str],
+                   bucket: str,
+                   basepath: Path | str,
+                   identifier: str | None,
+                   client: Minio = None,
+                   logger: Logger = None) -> bool:
     """
     Determine if a given object exists in the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to locate the object at
-    :param identifier: the object identifier
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
+    :param identifier: optional object identifier
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
-    :return: True if the object was found
+    :return: True if the object was found, false otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # proceed, if the MinIO client eas obtained
     if curr_client:
         # was the identifier provided ?
         if identifier is None:
             # no, object is a folder
-            objs: Iterator = minio_objects_list(errors=errors,
-                                                basepath=basepath,
-                                                recursive=False,
-                                                bucket=bucket,
-                                                client=curr_client,
-                                                logger=logger)
-            for _ in objs:
-                result = True
-                break
+            objs: Iterator = _objects_list(errors=errors,
+                                           bucket=bucket,
+                                           basepath=basepath,
+                                           recursive=False,
+                                           client=curr_client,
+                                           logger=logger)
+            result = next(objs, None) is None
         # verify the status of the object
-        elif minio_object_stat(errors=errors,
-                               basepath=basepath,
-                               identifier=identifier,
-                               bucket=bucket,
-                               client=curr_client,
-                               logger=logger):
+        elif _object_stat(errors=errors,
+                          bucket=bucket,
+                          basepath=basepath,
+                          identifier=identifier,
+                          client=curr_client,
+                          logger=logger):
             result = True
-        if logger:
-            remotepath: Path = Path(basepath) / identifier
-            existence: str = "exists" if result else "do not exist"
-            logger.debug(f"Object {remotepath}, bucket {bucket}, {existence}")
+
+        remotepath: Path = Path(basepath) / identifier
+        existence: str = "exists" if result else "do not exist"
+        _s3_log(logger=logger,
+                stmt=f"Object {remotepath}, bucket {bucket}, {existence}")
 
     return result
 
 
-def minio_object_stat(errors: list[str],
-                      basepath: Path | str,
-                      identifier: str,
-                      bucket: str = MINIO_BUCKET_NAME,
-                      client: Minio = None,
-                      logger: Logger = None) -> MinioObject:
+def _object_stat(errors: list[str],
+                 bucket: str,
+                 basepath: Path | str,
+                 identifier: str,
+                 client: Minio = None,
+                 logger: Logger = None) -> MinioObject:
     """
     Retrieve and return the information about an object in the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying where to locate the object
     :param identifier: the object identifier
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: metadata and information about the object
     """
     # initialize the return variable
     result: MinioObject | None = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             result = curr_client.stat_object(bucket_name=bucket,
                                              object_name=f"{remotepath}")
-            if logger:
-                logger.debug(f"Stat'ed {remotepath}, bucket {bucket}")
+            _s3_log(logger=logger,
+                    stmt=f"Stat'ed {remotepath}, bucket {bucket}")
         except Exception as e:
             if not hasattr(e, "code") or e.code != "NoSuchKey":
-                __minio_except_msg(errors=errors,
-                                   exception=e,
-                                   logger=logger)
-
+                _s3_except_msg(errors=errors,
+                               exception=e,
+                               engine="minio",
+                               logger=logger)
     return result
 
 
-def minio_object_store(errors: list[str],
-                       basepath: Path | str,
-                       identifier: str,
-                       obj: any,
-                       tags: dict = None,
-                       bucket: str = MINIO_BUCKET_NAME,
-                       client: Minio = None,
-                       logger: Logger = None) -> None:
+def _object_store(errors: list[str],
+                  bucket: str,
+                  basepath: Path | str,
+                  identifier: str,
+                  obj: Any,
+                  tags: dict = None,
+                  client: Minio = None,
+                  logger: Logger = None) -> bool:
     """
     Store an object at the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
     :param obj: object to be stored
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
+    :param tags: optional metadata describing the object
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
-    :param tags: optional metadata describing the object
+    :return: True if the object was successfully stored, False otherwise
     """
+    # initialize the return variable
+    result: bool = False
+
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # proceed, if the MinIO client was obtained
     if curr_client:
         # serialize the object into a file
-        filepath: Path = Path(MINIO_TEMP_PATH) / f"{uuid.uuid4()}.pickle"
+        temp_folder: Path = _s3_get_param("minio", "temp-folder")
+        filepath: Path = temp_folder / f"{uuid.uuid4()}.pickle"
         with filepath.open("wb") as f:
             pickle.dump(obj, f)
 
         # store the file
         op_errors: list[str] = []
-        minio_file_store(errors=op_errors,
-                         basepath=basepath,
-                         identifier=identifier,
-                         filepath=filepath,
-                         mimetype="application/octet-stream",
-                         tags=tags,
-                         bucket=bucket,
-                         client=curr_client,
-                         logger=logger)
+        _file_store(errors=op_errors,
+                    bucket=bucket,
+                    basepath=basepath,
+                    identifier=identifier,
+                    filepath=filepath,
+                    mimetype="application/octet-stream",
+                    tags=tags,
+                    client=curr_client,
+                    logger=logger)
 
         # errors ?
         if op_errors:
             # yes, report them
             errors.extend(op_errors)
             storage: str = "Unable to store"
         else:
             # no, remove the file from the file system
+            result = True
             filepath.unlink()
             storage: str = "Stored "
 
-        if logger:
-            remotepath: Path = Path(basepath) / identifier
-            logger.debug(f"{storage} {remotepath}, bucket {bucket}")
+        remotepath: Path = Path(basepath) / identifier
+        _s3_log(logger=logger,
+                stmt=f"{storage} {remotepath}, bucket {bucket}")
 
+    return result
 
-def minio_object_retrieve(errors: list[str],
-                          basepath: Path,
-                          identifier: str,
-                          bucket: str = MINIO_BUCKET_NAME,
-                          client: Minio = None,
-                          logger: Logger = None) -> any:
+
+def _object_retrieve(errors: list[str],
+                     bucket: str,
+                     basepath: Path,
+                     identifier: str,
+                     client: Minio = None,
+                     logger: Logger = None) -> Any:
     """
     Retrieve an object from the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the object retrieved
     """
     # initialize the return variable
-    result: any = None
+    result: Any = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # proceed, if the MinIO client was obtained
     if curr_client:
         # retrieve the file containg the serialized object
-        filepath: Path = Path(MINIO_TEMP_PATH) / f"{uuid.uuid4()}.pickle"
-        stat: any = minio_file_retrieve(errors=errors,
-                                        basepath=basepath,
-                                        identifier=identifier,
-                                        filepath=filepath,
-                                        bucket=bucket,
-                                        client=curr_client,
-                                        logger=logger)
+        temp_folder: Path = _s3_get_param("minio", "temp-folder")
+        filepath: Path = temp_folder / f"{uuid.uuid4()}.pickle"
+        stat: Any = _file_retrieve(errors=errors,
+                                   bucket=bucket,
+                                   basepath=basepath,
+                                   identifier=identifier,
+                                   filepath=filepath,
+                                   client=curr_client,
+                                   logger=logger)
 
         # was the file retrieved ?
         if stat:
             # yes, umarshall the corresponding object
             with filepath.open("rb") as f:
                 result = pickle.load(f)
             filepath.unlink()
 
-        if logger:
-            retrieval: str = "Retrieved" if result else "Unable to retrieve"
-            remotepath: Path = Path(basepath) / identifier
-            logger.debug(f"{retrieval} {remotepath}, bucket {bucket}")
+        retrieval: str = "Retrieved" if result else "Unable to retrieve"
+        remotepath: Path = Path(basepath) / identifier
+        _s3_log(logger=logger,
+                stmt=f"{retrieval} {remotepath}, bucket {bucket}")
 
     return result
 
 
-def minio_object_delete(errors: list[str],
-                        basepath: str,
-                        identifier: str = None,
-                        bucket: str = MINIO_BUCKET_NAME,
-                        client: Minio = None,
-                        logger: Logger = None) -> None:
+def _object_delete(errors: list[str],
+                   bucket: str,
+                   basepath: str,
+                   identifier: str = None,
+                   client: Minio = None,
+                   logger: Logger = None) -> bool:
     """
     Remove an object from the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
-    :param identifier: the object identifier
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
+    :param identifier: optional object identifier
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
+    :return: True if the object was successfully deleted, False otherwise
     """
+    # initialize the return variable
+    result: bool = False
+
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # proceed, if the MinIO client was obtained
     if curr_client:
         # was the identifier provided ?
         if identifier is None:
             # no, remove the folder
-            __minio_folder_delete(errors=errors,
-                                  client=curr_client,
-                                  basepath=basepath,
-                                  bucket=bucket,
-                                  logger=logger)
+            __folder_delete(errors=errors,
+                            bucket=bucket,
+                            basepath=basepath,
+                            client=curr_client,
+                            logger=logger)
         else:
             # yes, remove the object
             remotepath: Path = Path(basepath) / identifier
             try:
                 curr_client.remove_object(bucket_name=bucket,
                                           object_name=f"{remotepath}")
-                if logger:
-                    logger.debug(f"Deleted {remotepath}, bucket {bucket}")
+                result = True
+                _s3_log(logger=logger,
+                        stmt=f"Deleted {remotepath}, bucket {bucket}")
             except Exception as e:
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
-                    __minio_except_msg(errors=errors,
-                                       exception=e,
-                                       logger=logger)
+                    _s3_except_msg(errors=errors,
+                                   exception=e,
+                                   engine="minio",
+                                   logger=logger)
+    return result
 
 
-# recupera as tags do objeto
-def minio_object_tags_retrieve(errors: list[str],
-                               basepath: str,
-                               identifier: str,
-                               bucket: str = MINIO_BUCKET_NAME,
-                               client: Minio = None,
-                               logger: Logger = None) -> dict:
+def _object_tags_retrieve(errors: list[str],
+                          bucket: str,
+                          basepath: str,
+                          identifier: str,
+                          client: Minio = None,
+                          logger: Logger = None) -> dict:
     """
     Retrieve and return the metadata information for an object in the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the metadata about the object
     """
     # initialize the return variable
     result: dict | None = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         remotepath: Path = Path(basepath) / identifier
         try:
             tags: Tags = curr_client.get_object_tags(bucket_name=bucket,
                                                      object_name=f"{remotepath}")
-            if tags is not None and len(tags) > 0:
+            if tags and len(tags) > 0:
                 result = {}
                 for key, value in tags.items():
                     result[key] = value
-            if logger:
-                logger.debug(f"Retrieved {remotepath}, bucket {bucket}, tags {result}")
+            _s3_log(logger=logger,
+                    stmt=f"Retrieved {remotepath}, bucket {bucket}, tags {result}")
         except Exception as e:
             if not hasattr(e, "code") or e.code != "NoSuchKey":
-                __minio_except_msg(errors=errors,
-                                   exception=e,
-                                   logger=logger)
+                _s3_except_msg(errors=errors,
+                               exception=e,
+                               engine="minio",
+                               logger=logger)
 
     return result
 
 
-def minio_objects_list(errors: list[str],
-                       basepath: str,
-                       recursive: bool = False,
-                       bucket: str = MINIO_BUCKET_NAME,
-                       client: Minio = None,
-                       logger: Logger = None) -> Iterator:
+def _objects_list(errors: list[str],
+                  bucket: str,
+                  basepath: str,
+                  recursive: bool = False,
+                  client: Minio = None,
+                  logger: Logger = None) -> Iterator:
     """
     Retrieve and return an iterator into the list of objects at *basepath*, in the *MinIO* store.
 
     :param errors: incidental error messages
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to iterate from
     :param recursive: whether the location is iterated recursively
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
     :param client: optional MinIO client (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the iterator into the list of objects, 'None' if the folder does not exist
     """
     # initialize the return variable
     result: Iterator | None = None
 
     # make sure to have a MinIO client
-    curr_client: Minio = client or minio_access(errors=errors,
-                                                logger=logger)
+    curr_client: Minio = client or _access(errors=errors,
+                                           logger=logger)
     # was the MinIO client obtained ?
     if curr_client:
         # yes, proceed
         try:
             result = curr_client.list_objects(bucket_name=bucket,
                                               prefix=basepath,
                                               recursive=recursive)
-            if logger:
-                logger.debug(f"Listed {basepath}, bucket {bucket}")
+            _s3_log(logger=logger,
+                    stmt=f"Listed {basepath}, bucket {bucket}")
         except Exception as e:
-            __minio_except_msg(errors=errors,
-                               exception=e,
-                               logger=logger)
+            _s3_except_msg(errors=errors,
+                           exception=e,
+                           engine="minio",
+                           logger=logger)
 
     return result
 
 
-def __minio_folder_delete(errors: list[str],
-                          client: Minio,
-                          basepath: str,
-                          bucket: str = MINIO_BUCKET_NAME,
-                          logger: Logger = None) -> None:
+def __folder_delete(errors: list[str],
+                    bucket: str,
+                    basepath: str,
+                    client: Minio,
+                    logger: Logger = None) -> None:
     """
     Traverse the folders recursively, removing its objects.
 
     :param errors: incidental error messages
-    :param client: the MinIO client object
+    :param bucket: the bucket to use
     :param basepath: the path specifying the location to delete the objects at
-    :param bucket: the bucket to use (defaults to MINIO_BUCKET)
+    :param client: the MinIO client object
     :param logger: optional logger
     """
     # obtain the list of entries in the given folder
-    objs: Iterator = minio_objects_list(errors=errors,
-                                        basepath=basepath,
-                                        recursive=True,
-                                        bucket=bucket,
-                                        logger=logger)
+    objs: Iterator = _objects_list(errors=errors,
+                                   bucket=bucket,
+                                   basepath=basepath,
+                                   recursive=True,
+                                   logger=logger)
     # was the list obtained ?
     if objs:
         # yes, proceed
         for obj in objs:
             try:
                 client.remove_object(bucket_name=bucket,
                                      object_name=obj.object_name)
+                _s3_log(logger=logger,
+                        stmt=f"Removed folder {basepath}, bucket {bucket}")
             except Exception as e:
                 # SANITY CHECK: in case of concurrent exclusion
                 if not hasattr(e, "code") or e.code != "NoSuchKey":
-                    __minio_except_msg(errors=errors,
-                                       exception=e,
-                                       logger=logger)
-        if logger:
-            logger.debug(msg=f"Removed folder {basepath}, bucket {bucket}")
-
-
-def __minio_except_msg(errors: list[str],
-                       exception: Exception,
-                       logger: Logger) -> None:
-    """
-    Format and return an error message from *exception*.
-
-    :param errors: incidental error messages
-    :param exception: the reference exception
-    :param logger: optional logger
-    :return: the error message
-    """
-    # interaction with MinIO raised the exception "<class 'exception_class'>"
-    cls: str = str(exception.__class__)
-    exc_msg: str = f"{cls[7:-1]} - {exception}"
-    err_msg: str = f"Error accessing the object storer: {exc_msg}"
-    if errors:
-        errors.append(err_msg)
-    if logger:
-        logger.error(msg=err_msg)
+                    _s3_except_msg(errors=errors,
+                                   exception=e,
+                                   engine="minio",
+                                   logger=logger)
```

### Comparing `pypomes_s3-0.3.1/src/pypomes_s3/s3_common.py` & `pypomes_s3-0.3.2/src/pypomes_s3/s3_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from logging import DEBUG, Logger
+from pathlib import Path
 from pypomes_core import (
     APP_PREFIX,
     env_get_str, str_sanitize, str_get_positional
 )
+from typing import Any
 
 # the preferred way to specify S3 storage parameters is dynamically with 's3_setup_params'
 # specifying S3 storage parameters with environment variables can be done in two ways:
 # 1. specify the set
 #   {APP_PREFIX}_S3_ENGINE (one of 'aws', 'minio')
 #   {APP_PREFIX}_S3_ACCESS_KEY
 #   {APP_PREFIX}_S3_SECRET_KEY
 #   {APP_PREFIX}_S3_BUCKET_NAME
-#   {APP_PREFIX}_S3_TEMP_PATH
+#   {APP_PREFIX}_S3_TEMP_FOLDER
 #   {APP_PREFIX}_S3_REGION_NAME (for aws)
 #   {APP_PREFIX}_S3_ENDPOINT_URL (for minio)
 #   {APP_PREFIX}_S3_SECURE_ACCESS (for minio)
 # 2. alternatively, specify a comma-separated list of servers in
 #   {APP_PREFIX}_S3_ENGINES
 #   and for each engine, specify the set above, replacing 'S3' with
 #   'AWS' and 'MINIO', respectively for the engines listed above
 
 _S3_ACCESS_DATA: dict = {}
 _S3_ENGINES: list[str] = []
-if env_get_str(f"{APP_PREFIX}_S3_ENGINE",  None):
+_prefix: str = env_get_str(f"{APP_PREFIX}_S3_ENGINE",  None)
+if _prefix:
     _default_setup: bool = True
-    _S3_ENGINES.append(env_get_str(f"{APP_PREFIX}_S3_ENGINE"))
+    _S3_ENGINES.append(_prefix)
 else:
     _default_setup: bool = False
     _engines: str = env_get_str(f"{APP_PREFIX}_S3_ENGINES", None)
     if _engines:
         _S3_ENGINES.extend(_engines.split(sep=","))
 for engine in _S3_ENGINES:
     if _default_setup:
@@ -38,15 +41,15 @@
         _tag: str = str_get_positional(source=engine,
                                        list_origin=["aws", "minio"],
                                        list_dest=["AWS", "MINIO"])
     _s3_data = {
         "access-key":  env_get_str(f"{APP_PREFIX}_{_tag}_ACESS_KEY"),
         "secret-key": env_get_str(f"{APP_PREFIX}_{_tag}_SECRET_KEY"),
         "bucket-name": env_get_str(f"{APP_PREFIX}_{_tag}_BUCKET_NAME"),
-        "temp-path": env_get_str(f"{APP_PREFIX}_{_tag}_TEMP_PATH")
+        "temp-folder": Path(env_get_str(f"{APP_PREFIX}_{_tag}_TEMP_FOLDER"))
     }
     if engine == "aws":
         _s3_data["client"] = env_get_str(f"{APP_PREFIX}_{_tag}_REGION_NAME")
     elif engine == "minio":
         _s3_data["endpoit-url"] = env_get_str(f"{APP_PREFIX}_{_tag}_ENDPOINT_URL")
         _s3_data["secure-access"] = env_get_str(f"{APP_PREFIX}_{_tag}_SECURE_ACCESS")
     _S3_ACCESS_DATA[engine] = _s3_data
@@ -74,56 +77,74 @@
     else:
         err_msg = f"S3 engine '{engine}' unknown or not configured"
         errors.append(err_msg)
 
     return result
 
 
+def _s3_get_param(engine: str,
+                  param: str) -> Any:
+    """
+    Return the current value of *param* being used by *engine*.
+
+    :param engine: the reference S3 engine
+    :param param: the reference parameter
+    :return: the parameter's current value
+    """
+    return _S3_ACCESS_DATA[engine].get(param)
+
+
 def _s3_get_params(engine: str) -> tuple:
     """
     Return the current parameters being used for *engine*.
 
     The parameters are returned as a *tuple*, with the elements
-    *access-key*, *secret-key*, *bucket-name*, *temp-path*.
+    *access-key*, *secret-key*, *bucket-name*, *temp-folder*.
     For *aws* engines, the extra element *region-name* is returned.
     for *minio* engines, the elements *endpoint-url* and *secure-access are returned.
     The meaning of some parameters may vary between different S3 engines.
 
     :param engine: the reference database engine
     :return: the current parameters for the engine
     """
-    access_key: str = _S3_ACCESS_DATA[engine]["access-key"]
-    secret_key: str = _S3_ACCESS_DATA[engine]["secret-key"]
-    bucket_name: str = _S3_ACCESS_DATA[engine]["bucket-name"]
-    temp_path = _S3_ACCESS_DATA[engine]["temp-path"]
+    access_key: str = _S3_ACCESS_DATA[engine].get("access-key")
+    secret_key: str = _S3_ACCESS_DATA[engine].get("secret-key")
 
     result: tuple | None = None
     if engine == "aws":
-        region_name: str = _S3_ACCESS_DATA[engine]["region-name"]
-        result = (access_key, secret_key, bucket_name, temp_path, region_name)
+        region_name: str = _S3_ACCESS_DATA[engine].get("region-name")
+        result = (access_key, secret_key, region_name)
     elif engine == "minio":
-        endpoint_url: str = _S3_ACCESS_DATA[engine]["endpoint-url"]
-        secure_access: bool = _S3_ACCESS_DATA[engine]["secure-access"]
-        result = (access_key, secret_key, bucket_name, temp_path, endpoint_url, secure_access)
+        endpoint_url: str = _S3_ACCESS_DATA[engine].get("endpoint-url")
+        secure_access: bool = _S3_ACCESS_DATA[engine].get("secure-access")
+        result = (access_key, secret_key, endpoint_url, secure_access)
 
     return result
 
 
-def _db_except_msg(exception: Exception,
-                   engine: str) -> str:
+def _s3_except_msg(errors: list[str],
+                   exception: Exception,
+                   engine: str,
+                   logger: Logger) -> None:
     """
-    Format and return the error message corresponding to the exception raised while accessing the database.
+    Format and log the error message corresponding to the exception raised while accessing the S3 store.
 
+    :param errors: incidental error messages
     :param exception: the exception raised
+    :param logger: the logger object
     :param engine: the reference database engine
     :return: the formatted error message
     """
     endpoint: str = _S3_ACCESS_DATA[engine].get("region-name") if engine == "aws" else \
                     _S3_ACCESS_DATA[engine].get("endpoint-url")
-    return f"Error accessing '{engine}' at '{endpoint}': {str_sanitize(f'{exception}')}"
+    err_msg: str = f"Error accessing '{engine}' at '{endpoint}': {str_sanitize(f'{exception}')}"
+    if errors:
+        errors.append(err_msg)
+    if logger:
+        logger.error(err_msg)
 
 
 def _s3_log(logger: Logger,
             err_msg: str = None,
             level: int = DEBUG,
             errors: list[str] = None,
             stmt: str = None) -> None:
```

### Comparing `pypomes_s3-0.3.1/LICENSE` & `pypomes_s3-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_s3-0.3.1/pyproject.toml` & `pypomes_s3-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_s3"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (S3 storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "boto3>=1.34.108",
-    "minio>=7.2.5",
+    "minio>=7.2.7",
     "pip>=24.0",
     "pypomes_core>=1.0.4",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.42.0"
 ]
```

### Comparing `pypomes_s3-0.3.1/PKG-INFO` & `pypomes_s3-0.3.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_s3
-Version: 0.3.1
+Version: 0.3.2
 Summary: A collection of Python pomes, pennyeach (S3 storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-S3
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-S3/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: boto3>=1.34.108
-Requires-Dist: minio>=7.2.5
+Requires-Dist: minio>=7.2.7
 Requires-Dist: pip>=24.0
 Requires-Dist: pypomes-core>=1.0.4
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.42.0
```

