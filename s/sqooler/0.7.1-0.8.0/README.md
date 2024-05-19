# Comparing `tmp/sqooler-0.7.1.tar.gz` & `tmp/sqooler-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqooler-0.7.1.tar", max compression
+gzip compressed data, was "sqooler-0.8.0.tar", max compression
```

## Comparing `sqooler-0.7.1.tar` & `sqooler-0.8.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1211 2024-04-18 18:44:41.208787 sqooler-0.7.1/LICENSE
--rw-r--r--   0        0        0     3928 2024-04-18 18:44:41.212121 sqooler-0.7.1/README.md
--rw-r--r--   0        0        0     1282 2024-05-11 21:00:58.760099 sqooler-0.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-18 18:44:41.212209 sqooler-0.7.1/src/sqooler/__init__.py
--rw-r--r--   0        0        0      810 2024-05-05 09:53:38.382220 sqooler-0.7.1/src/sqooler/cli.py
--rw-r--r--   0        0        0    14269 2024-05-09 13:07:12.492631 sqooler-0.7.1/src/sqooler/schemes.py
--rw-r--r--   0        0        0     8775 2024-04-18 18:44:42.470722 sqooler-0.7.1/src/sqooler/security.py
--rw-r--r--   0        0        0    27991 2024-04-19 14:40:24.524812 sqooler-0.7.1/src/sqooler/spoolers.py
--rw-r--r--   0        0        0        0 2024-04-18 18:44:42.471937 sqooler-0.7.1/src/sqooler/storage_providers/__init__.py
--rw-r--r--   0        0        0    30364 2024-05-11 20:32:01.563176 sqooler-0.7.1/src/sqooler/storage_providers/base.py
--rw-r--r--   0        0        0    30924 2024-05-11 21:01:09.976853 sqooler-0.7.1/src/sqooler/storage_providers/dropbox.py
--rw-r--r--   0        0        0    26238 2024-05-11 21:01:09.979534 sqooler-0.7.1/src/sqooler/storage_providers/local.py
--rw-r--r--   0        0        0    31587 2024-05-11 21:01:09.979964 sqooler-0.7.1/src/sqooler/storage_providers/mongodb.py
--rw-r--r--   0        0        0     6672 2024-05-11 20:06:14.172608 sqooler-0.7.1/src/sqooler/utils.py
--rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 sqooler-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-18 18:44:41.208787 sqooler-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3928 2024-04-18 18:44:41.212121 sqooler-0.8.0/README.md
+-rw-r--r--   0        0        0     1282 2024-05-19 09:58:10.012810 sqooler-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:41.212209 sqooler-0.8.0/src/sqooler/__init__.py
+-rw-r--r--   0        0        0      810 2024-05-05 09:53:38.382220 sqooler-0.8.0/src/sqooler/cli.py
+-rw-r--r--   0        0        0    14516 2024-05-18 06:49:27.763584 sqooler-0.8.0/src/sqooler/schemes.py
+-rw-r--r--   0        0        0     8775 2024-04-18 18:44:42.470722 sqooler-0.8.0/src/sqooler/security.py
+-rw-r--r--   0        0        0    27991 2024-04-19 14:40:24.524812 sqooler-0.8.0/src/sqooler/spoolers.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:44:42.471937 sqooler-0.8.0/src/sqooler/storage_providers/__init__.py
+-rw-r--r--   0        0        0    33316 2024-05-19 09:58:10.013582 sqooler-0.8.0/src/sqooler/storage_providers/base.py
+-rw-r--r--   0        0        0    31210 2024-05-18 14:26:53.804374 sqooler-0.8.0/src/sqooler/storage_providers/dropbox.py
+-rw-r--r--   0        0        0    26403 2024-05-18 14:26:53.806132 sqooler-0.8.0/src/sqooler/storage_providers/local.py
+-rw-r--r--   0        0        0    31810 2024-05-18 14:26:53.807488 sqooler-0.8.0/src/sqooler/storage_providers/mongodb.py
+-rw-r--r--   0        0        0     7715 2024-05-18 14:26:53.808507 sqooler-0.8.0/src/sqooler/utils.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 sqooler-0.8.0/PKG-INFO
```

### Comparing `sqooler-0.7.1/LICENSE` & `sqooler-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.1/README.md` & `sqooler-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.1/pyproject.toml` & `sqooler-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqooler"
-version = "0.7.1"
+version = "0.8.0"
 description = "Code that enables validated cloud access to quantum hardware (simulators)"
 authors = ["fretchen <fred.jendrzejewski@gmail.com>"]
 repository = "https://github.com/Alqor-UG/sqooler"
 documentation = "https://alqor-ug.github.io/sqooler"
 license = "Unlicense"
 readme = "README.md"
 packages = [{include = "sqooler", from = "src"}]
```

### Comparing `sqooler-0.7.1/src/sqooler/cli.py` & `sqooler-0.8.0/src/sqooler/cli.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.1/src/sqooler/schemes.py` & `sqooler-0.8.0/src/sqooler/schemes.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,23 @@
     Literal["sequential", "interleaved"],
     Field(
         description="The wire order of the backend. Either sequential or interleaved."
         " Non standard qiskit field."
     ),
 ]
 
+# a string that is allowed for paths without leading and trailing slashes
+PathStr = Annotated[
+    str,
+    Field(
+        description="The path to the file without leading and trailing slashes.",
+        pattern=r"^[a-zA-Z0-9_\-\.]+$",
+    ),
+]
+
 
 class StatusMsgDict(BaseModel):
     """
     A class that defines the structure of the status messages.
     """
 
     job_id: str = Field(description="unique execution id from the backend.")
```

### Comparing `sqooler-0.7.1/src/sqooler/security.py` & `sqooler-0.8.0/src/sqooler/security.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.1/src/sqooler/spoolers.py` & `sqooler-0.8.0/src/sqooler/spoolers.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.7.1/src/sqooler/storage_providers/base.py` & `sqooler-0.8.0/src/sqooler/storage_providers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 The module that contains all the necessary logic for communication with the external
 storage for the jobs. It creates an abstract API layer for the storage providers.
 """
 
 import functools
 import logging
 import re
+import warnings
 from abc import ABC, abstractmethod
 from datetime import datetime, timezone
 from typing import Any, Callable, Mapping, Optional
 
 from decouple import config
 
 from ..schemes import (
@@ -37,18 +38,17 @@
         if not self.is_active:
             raise ValueError("The storage provider is not active.")
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
-class StorageProvider(ABC):
-    """
-    The template for accessing any storage providers like dropbox, mongodb, amazon S3 etc.
+class StorageCore(ABC):
     """
+    A base class that is necessary to manipulate files in a consistent way."""
 
     def __init__(self, name: str, is_active: bool = True) -> None:
         """
         Any storage provide must have a name that is not empty.
 
         Args:
             name: The name of the storage provider
@@ -75,30 +75,127 @@
 
         Args:
             content_dict: The dictionary containing the content of the file
             storage_path: The path to the file
             job_id: The id of the job
         """
 
+    def upload_file(
+        self, content_dict: Mapping, storage_path: str, job_id: str
+    ) -> None:
+        """
+        Depreceated function. Use `upload` instead.
+        """
+        warnings.warn(
+            "`upload_file` is depreceated. Use `upload` instead.", DeprecationWarning
+        )
+        self.upload(content_dict, storage_path, job_id)
+
     @abstractmethod
-    def get_file_content(self, storage_path: str, job_id: str) -> dict:
+    def get(self, storage_path: str, job_id: str) -> dict:
         """
         Get the file content from the storage.
 
         Args:
             storage_path: The path to the file
             job_id: The id of the job
 
         Returns:
             The content of the file
 
         Raises:
             FileNotFoundError: If the file is not found
         """
 
+    def get_file_content(self, storage_path: str, job_id: str) -> dict:
+        """
+        Depreceated function. Use `get` instead.
+        """
+        warnings.warn(
+            "`get_file_content` is depreceated. Use `get` instead.", DeprecationWarning
+        )
+        return self.get(storage_path, job_id)
+
+    @abstractmethod
+    def update(self, content_dict: dict, storage_path: str, job_id: str) -> None:
+        """
+        Update the file content. It replaces the old content with the new content.
+
+        Args:
+            content_dict: The dictionary containing the new content of the file
+            storage_path: The path to the file
+            job_id: The id of the job
+
+        Returns:
+            None
+
+        Raises:
+            FileNotFoundError: If the file is not found
+        """
+
+    def update_file(self, content_dict: dict, storage_path: str, job_id: str) -> None:
+        """
+        Depreceated function. Use `update` instead.
+        """
+        warnings.warn(
+            "`update_file` is depreceated. Use `update` instead.", DeprecationWarning
+        )
+        self.update(content_dict, storage_path, job_id)
+
+    @abstractmethod
+    def move(self, start_path: str, final_path: str, job_id: str) -> None:
+        """
+        Move the file from `start_path` to `final_path`
+
+        Args:
+            start_path: The orginal path to the file
+            final_path: The targe path for the file
+            job_id: The id of the job
+        """
+
+    def move_file(self, start_path: str, final_path: str, job_id: str) -> None:
+        """
+        Depreceated function. Use `move` instead.
+        """
+        warnings.warn(
+            "`move_file` is depreceated. Use `move` instead.", DeprecationWarning
+        )
+        self.move(start_path, final_path, job_id)
+
+    @abstractmethod
+    def delete(self, storage_path: str, job_id: str) -> None:
+        """
+        Delete the file from the storage
+
+        Args:
+            storage_path: The path to the file
+            job_id: The id of the job
+
+        Raises:
+            FileNotFoundError: If the file is not found
+
+        Returns:
+            None
+        """
+
+    def delete_file(self, storage_path: str, job_id: str) -> None:
+        """
+        Depreceated function. Use `delete` instead.
+        """
+        warnings.warn(
+            "`delete_file` is depreceated. Use `delete` instead.", DeprecationWarning
+        )
+        self.delete(storage_path, job_id)
+
+
+class StorageProvider(StorageCore):
+    """
+    The template for accessing any storage providers like dropbox, mongodb, amazon S3 etc.
+    """
+
     @abstractmethod
     def get_backends(self) -> list[str]:
         """
         Get a list of all the backends that the provider offers.
         """
 
     @validate_active
@@ -156,26 +253,36 @@
             username: the name of the user that submitted the job
 
         Returns:
             The job id of the uploaded job.
         """
 
     @abstractmethod
-    def get_job_content(self, storage_path: str, job_id: str) -> dict:
+    def get_job(self, storage_path: str, job_id: str) -> dict:
         """
-        Get the content of the job from the storage. This is a wrapper around get_file_content
+        Get the content of the job from the storage. This is a wrapper around get
         and and handles the different ways of identifiying the job.
 
         storage_path: the path towards the file, excluding the filename / id
         job_id: the id of the file we are about to look up
 
         Returns:
             The content of the job
         """
 
+    def get_job_content(self, storage_path: str, job_id: str) -> dict:
+        """
+        Depreceated function. Use `get_job` instead.
+        """
+        warnings.warn(
+            "`get_job_content` is depreceated. Use `get_job` instead.",
+            DeprecationWarning,
+        )
+        return self.get_job(storage_path, job_id)
+
     @abstractmethod
     def upload_status(
         self,
         display_name: DisplayNameStr,
         username: str,
         job_id: str,
         private_jwk: Optional[JWK] = None,
@@ -294,53 +401,14 @@
             job_id: The job_id of the job that we want to upload the status for
 
         Returns:
             If it was possible to verify the result dict positively.
         """
 
     @abstractmethod
-    def update_file(self, content_dict: dict, storage_path: str, job_id: str) -> None:
-        """
-        Update the file content. It replaces the old content with the new content.
-
-        Args:
-            content_dict: The dictionary containing the new content of the file
-            storage_path: The path to the file
-            job_id: The id of the job
-
-        Returns:
-            None
-
-        Raises:
-            FileNotFoundError: If the file is not found
-        """
-
-    @abstractmethod
-    def move_file(self, start_path: str, final_path: str, job_id: str) -> None:
-        """
-        Move the file from `start_path` to `final_path`
-        """
-
-    @abstractmethod
-    def delete_file(self, storage_path: str, job_id: str) -> None:
-        """
-        Delete the file from the storage
-
-        Args:
-            storage_path: The path to the file
-            job_id: The id of the job
-
-        Raises:
-            FileNotFoundError: If the file is not found
-
-        Returns:
-            None
-        """
-
-    @abstractmethod
     def upload_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK],
     ) -> None:
         """
@@ -539,14 +607,36 @@
             # we should sign the result
             signed_result = sign_payload(result_dict.model_dump(), private_jwk)
             self.upload(signed_result.model_dump(), result_json_dir, result_json_name)
         else:
             self.upload(result_dict.model_dump(), result_json_dir, result_json_name)
         return True
 
+    def _verify_config(
+        self, config_dict: BackendConfigSchemaIn, display_name: DisplayNameStr
+    ) -> BackendConfigSchemaIn:
+        """
+        make sure that members of the config_dict are correct
+
+        Args:
+            config_dict: The dictionary containing the configuration
+            display_name: The name of the backend
+
+        Raises:
+            A warning if the display_name does not match the display_name of the config_dict
+
+        """
+        if not config_dict.display_name == display_name:
+            config_dict.display_name = display_name
+            warnings.warn(
+                f"The display_name of the config_dict had to be matched to {display_name}."
+            )
+
+        return config_dict
+
     def _format_config_dict(
         self, config_dict: BackendConfigSchemaIn, private_jwk: Optional[JWK] = None
     ) -> dict:
         """
         Format the config dict to a string that can be written to a file.
 
         Args:
```

### Comparing `sqooler-0.7.1/src/sqooler/storage_providers/dropbox.py` & `sqooler-0.8.0/src/sqooler/storage_providers/dropbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 from dropbox.files import WriteMode
 
 from ..schemes import (
     BackendConfigSchemaIn,
     DisplayNameStr,
     DropboxLoginInformation,
     NextJobSchema,
+    PathStr,
     ResultDict,
     StatusMsgDict,
 )
 from ..security import JWK, JWSDict
-from .base import StorageProvider, datetime_handler, validate_active
+from .base import StorageCore, StorageProvider, datetime_handler, validate_active
 
 
-class DropboxProviderExtended(StorageProvider):
+class DropboxCore(StorageCore):
     """
-    The class that implements the dropbox storage provider.
+    Base class that creates the most important functions for the local storage provider.
     """
 
     def __init__(
         self, login_dict: DropboxLoginInformation, name: str, is_active: bool = True
     ) -> None:
         """
         Args:
@@ -90,15 +91,15 @@
 
         # create the appropriate string for the dropbox API
         dump_str = json.dumps(content_dict, default=datetime_handler)
 
         self.upload_string(dump_str, storage_path, job_id)
 
     @validate_active
-    def get_file_content(self, storage_path: str, job_id: str) -> dict:
+    def get(self, storage_path: str, job_id: str) -> dict:
         """
         Get the file content from the dropbox
 
         storage_path: the path where the file should be stored, but excluding the file name
         job_id: the name of the file. Is a json file
         """
 
@@ -122,28 +123,16 @@
             except ApiError as err:
                 raise FileNotFoundError(
                     f"Could not find file under {full_path}"
                 ) from err
             data = res.content
         return json.loads(data.decode("utf-8"))
 
-    def get_job_content(self, storage_path: str, job_id: str) -> dict:
-        """
-        Get the content of the job from the storage. This is a wrapper around get_file_content
-        and and handles the different ways of identifiying the job.
-
-        storage_path: the path towards the file, excluding the filename / id
-        job_id: the id of the file we are about to look up
-
-        Returns:
-            The content of the job
-        """
-        return self.get_file_content(storage_path=storage_path, job_id=f"job-{job_id}")
-
-    def update_file(self, content_dict: dict, storage_path: str, job_id: str) -> None:
+    @validate_active
+    def update(self, content_dict: dict, storage_path: str, job_id: str) -> None:
         """
         Update the file content.
 
         Args:
             content_dict: The dictionary containing the new content of the file
             storage_path: The path to the file
             job_id: The id of the job
@@ -177,15 +166,15 @@
                 ) from err
 
             dbx.files_upload(
                 dump_str.encode("utf-8"), full_path, mode=WriteMode("overwrite")
             )
 
     @validate_active
-    def move_file(self, start_path: str, final_path: str, job_id: str) -> None:
+    def move(self, start_path: str, final_path: str, job_id: str) -> None:
         """
         Move the file from start_path to final_path
 
         start_path: the path where the file is currently stored, but excluding the file name
         final_path: the path where the file should be stored, but excluding the file name
         job_id: the name of the file. Is a json file
 
@@ -205,15 +194,15 @@
             dbx.users_get_current_account()
 
             full_start_path = "/" + start_path + "/" + job_id + ".json"
             full_final_path = "/" + final_path + "/" + job_id + ".json"
             dbx.files_move_v2(full_start_path, full_final_path)
 
     @validate_active
-    def delete_file(self, storage_path: str, job_id: str) -> None:
+    def delete(self, storage_path: str, job_id: str) -> None:
         """
         Remove the file from the dropbox
 
         Args:
             storage_path: the path where the file should be stored, but excluding the file name
             job_id: the name of the file. Is a json file
 
@@ -240,14 +229,70 @@
             try:
                 _ = dbx.files_delete_v2(path=full_path)
             except ApiError as err:
                 raise FileNotFoundError(
                     f"Could not delete file under {full_path}"
                 ) from err
 
+    def delete_folder(self, folder_path: str) -> None:
+        """
+        Remove the folder from the dropbox. Attention this will remove all the files in the folder.
+        It is not a standard function for storage providers, but allows us to better clean up the
+        tests.
+
+        Args:
+            folder_path: the path where the file should be stored, but excluding the file name
+
+        Returns:
+            None
+        """
+
+        # strip trailing and leading slashes from the storage_path
+        folder_path = folder_path.strip("/")
+
+        # Create an instance of a Dropbox class, which can make requests to the API.
+        with dropbox.Dropbox(
+            app_key=self.app_key,
+            app_secret=self.app_secret,
+            oauth2_refresh_token=self.refresh_token,
+        ) as dbx:
+            # Check that the access token is valid
+            try:
+                dbx.users_get_current_account()
+            except AuthError:
+                sys.exit("ERROR: Invalid access token.")
+
+            # to remove a folder there must be no trailing slash
+            full_path = "/" + folder_path
+            _ = dbx.files_delete_v2(path=full_path)
+
+
+class DropboxProviderExtended(StorageProvider, DropboxCore):
+    """
+    The class that implements the dropbox storage provider.
+
+    Attributes:
+        configs_path: The path to the folder where the configurations are stored
+    """
+
+    configs_path: PathStr = "Backend_files/Config"
+
+    def get_job(self, storage_path: str, job_id: str) -> dict:
+        """
+        Get the content of the job from the storage. This is a wrapper around get_file_content
+        and and handles the different ways of identifiying the job.
+
+        storage_path: the path towards the file, excluding the filename / id
+        job_id: the id of the file we are about to look up
+
+        Returns:
+            The content of the job
+        """
+        return self.get(storage_path=storage_path, job_id=f"job-{job_id}")
+
     def update_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
     ) -> None:
         """
@@ -261,17 +306,18 @@
             display_name : The name of the backend
             private_jwk: The private JWK to sign the configuration with
 
         Returns:
             None
         """
 
+        config_dict = self._verify_config(config_dict, display_name)
         # check that the file exists
-        config_path = "Backend_files/Config/" + display_name
-        old_config_jws = self.get_file_content(config_path, "config")
+        config_path = f"{self.configs_path}/{display_name}"
+        old_config_jws = self.get(config_path, "config")
 
         upload_dict = self._format_update_config(
             old_config_jws, config_dict, private_jwk
         )
         # maybe this should rather become the update_file function
         self.upload(upload_dict, config_path, "config")
 
@@ -291,19 +337,21 @@
             config_dict: The dictionary containing the configuration
             display_name : The name of the backend
             private_jwk: The private JWK to sign the configuration with
 
         Returns:
             None
         """
+        # make sure that the display_name is as it should be
+        config_dict = self._verify_config(config_dict, display_name)
 
-        config_path = "Backend_files/Config/" + display_name
+        config_path = f"{self.configs_path}/{display_name}"
         # check if the file already exists
         try:
-            self.get_file_content(storage_path=config_path, job_id="config")
+            self.get(storage_path=config_path, job_id="config")
             raise FileExistsError(
                 f"The configuration for {display_name} already exists and should not be overwritten."
             )
         except FileNotFoundError:
             pass
 
         upload_dict = self._format_config_dict(config_dict, private_jwk)
@@ -318,17 +366,18 @@
 
         Raises:
             FileNotFoundError: If the status does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
-        config_path = "Backend_files/Config/" + display_name
+        config_path = f"{self.configs_path}/{display_name}"
 
-        self.delete_file(storage_path=config_path, job_id="config")
+        self.delete(storage_path=config_path, job_id="config")
+        self.delete_folder(config_path)
         return True
 
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
         The function that uploads the spooler public JWK to the storage.
 
         Args:
@@ -368,17 +417,15 @@
         pk_paths = "Backend_files/public_keys"
 
         # now get the appropiate kid
         config_dict = self.get_config(display_name)
         if config_dict.kid is None:
             raise ValueError("The kid is not set in the backend configuration.")
 
-        public_jwk_dict = self.get_file_content(
-            storage_path=pk_paths, job_id=config_dict.kid
-        )
+        public_jwk_dict = self.get(storage_path=pk_paths, job_id=config_dict.kid)
         return JWK(**public_jwk_dict)
 
     def _delete_public_key(self, kid: str) -> bool:
         """
         Delete a public key from the storage. This is only intended for test purposes.
 
         Args:
@@ -387,15 +434,15 @@
         Raises:
             FileNotFoundError: If the status does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
         pk_paths = "Backend_files/public_keys"
-        self.delete_file(storage_path=pk_paths, job_id=kid)
+        self.delete(storage_path=pk_paths, job_id=kid)
         return True
 
     def update_in_database(
         self,
         result_dict: ResultDict,
         status_msg_dict: StatusMsgDict,
         job_id: str,
@@ -437,35 +484,31 @@
             job_finished_json_dir = (
                 "/Backend_files/Finished_Jobs/"
                 + display_name
                 + "/"
                 + extracted_username
                 + "/"
             )
-            self.move_file(job_json_start_dir, job_finished_json_dir, job_json_name)
+            self.move(job_json_start_dir, job_finished_json_dir, job_json_name)
 
         elif status_msg_dict.status == "ERROR":
             # because there was an error, we move the job to the deleted jobs
             deleted_json_dir = "Backend_files/Deleted_Jobs"
-            self.move_file(job_json_start_dir, deleted_json_dir, job_json_name)
+            self.move(job_json_start_dir, deleted_json_dir, job_json_name)
 
         try:
-            self.update_file(
-                status_msg_dict.model_dump(), status_json_dir, status_json_name
-            )
+            self.update(status_msg_dict.model_dump(), status_json_dir, status_json_name)
         except FileNotFoundError:
             logging.warning(
                 "The status file was missing for %s with job_id %s was missing.",
                 display_name,
                 job_id,
             )
             self.upload_status(display_name, username=extracted_username, job_id=job_id)
-            self.update_file(
-                status_msg_dict.model_dump(), status_json_dir, status_json_name
-            )
+            self.update(status_msg_dict.model_dump(), status_json_dir, status_json_name)
 
     def get_file_queue(self, storage_path: str) -> list[str]:
         """
         Get a list of files. Typically we are looking for the queued jobs of a backend here.
 
         Args:
             storage_path: Where are we looking for the files.
@@ -505,27 +548,32 @@
         return file_list
 
     @validate_active
     def get_backends(self) -> list[str]:
         """
         Get a list of all the backends that the provider offers.
         """
-        backend_config_path = "/Backend_files/Config/"
+
+        # strip possible trailing and leading slashes from the path
+        config_path = self.configs_path.strip("/")
+
+        # and now add them nicely
+        full_config_path = f"/{config_path}/"
         with dropbox.Dropbox(
             app_key=self.app_key,
             app_secret=self.app_secret,
             oauth2_refresh_token=self.refresh_token,
         ) as dbx:
             # Check that the access token is valid
             try:
                 dbx.users_get_current_account()
             except AuthError:
                 sys.exit("ERROR: Invalid access token.")
 
-            folders_results = dbx.files_list_folder(path=backend_config_path)
+            folders_results = dbx.files_list_folder(path=full_config_path)
             entries = folders_results.entries
             backend_names = []
             for entry in entries:
                 backend_names.append(entry.name)
         return backend_names
 
     def get_config(self, display_name: DisplayNameStr) -> BackendConfigSchemaIn:
@@ -537,18 +585,16 @@
 
         Raises:
             FileNotFoundError: If the backend does not exist
 
         Returns:
             The configuration of the backend in complete form.
         """
-        backend_json_path = f"Backend_files/Config/{display_name}"
-        backend_config_dict = self.get_file_content(
-            storage_path=backend_json_path, job_id="config"
-        )
+        backend_json_path = f"{self.configs_path}/{display_name}"
+        backend_config_dict = self.get(storage_path=backend_json_path, job_id="config")
         typed_config = self._adapt_get_config(backend_config_dict)
         return typed_config
 
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
         """
@@ -633,15 +679,15 @@
         Returns:
             The status dict of the job
         """
         status_json_dir = "Backend_files/Status/" + display_name + "/" + username
         status_json_name = "status-" + job_id
 
         try:
-            status_dict = self.get_file_content(
+            status_dict = self.get(
                 storage_path=status_json_dir, job_id=status_json_name
             )
         except FileNotFoundError:
             status_draft = {
                 "job_id": job_id,
                 "status": "ERROR",
                 "detail": "Could not find the status file.",
@@ -667,15 +713,16 @@
 
         Returns:
             Success if the file was deleted successfully
         """
         status_json_dir = "Backend_files/Status/" + display_name + "/" + username
         status_json_name = "status-" + job_id
 
-        self.delete_file(storage_path=status_json_dir, job_id=status_json_name)
+        self.delete(storage_path=status_json_dir, job_id=status_json_name)
+        self.delete_folder(status_json_dir)
         return True
 
     def upload_result(
         self,
         result_dict: ResultDict,
         display_name: DisplayNameStr,
         job_id: str,
@@ -722,15 +769,15 @@
         Returns:
             The result dict of the job. If the information is not available, the result dict
             has a status of "ERROR".
         """
         result_json_dir = "Backend_files/Result/" + display_name + "/" + username
         result_json_name = "result-" + job_id
         try:
-            result_dict = self.get_file_content(
+            result_dict = self.get(
                 storage_path=result_json_dir, job_id=result_json_name
             )
         except FileNotFoundError:
             return ResultDict(
                 display_name=display_name,
                 backend_version="",
                 job_id=job_id,
@@ -755,17 +802,15 @@
         Returns:
             If it was possible to verify the result dict positively.
         """
         username = job_id.split("-")[2]
         result_json_dir = "Backend_files/Result/" + display_name + "/" + username
         result_json_name = "result-" + job_id
 
-        result_dict = self.get_file_content(
-            storage_path=result_json_dir, job_id=result_json_name
-        )
+        result_dict = self.get(storage_path=result_json_dir, job_id=result_json_name)
         public_jwk = self.get_public_key(display_name)
 
         result_jws = JWSDict(**result_dict)
         return result_jws.verify_signature(public_jwk)
 
     def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
         """
@@ -778,21 +823,16 @@
 
         Raises:
             FileNotFoundError: If the result does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
-        extracted_username = job_id.split("-")[2]
-        result_json_dir = (
-            "Backend_files/Result/" + display_name + "/" + extracted_username
-        )
-        result_json_name = "result-" + job_id
-
-        self.delete_file(storage_path=result_json_dir, job_id=result_json_name)
+        result_device_dir = "/Backend_files/Result/" + display_name
+        self.delete_folder(result_device_dir)
         return True
 
     def get_next_job_in_queue(
         self, display_name: DisplayNameStr, private_jwk: Optional[JWK] = None
     ) -> NextJobSchema:
         """
         A function that obtains the next job in the queue.
@@ -816,50 +856,18 @@
         if job_list:
             job_json_name = job_list[0]
             job_dict["job_id"] = job_json_name[4:-5]
 
             # split the .json from the job_json_name
             job_json_name = job_json_name.split(".")[0]
             # and move the file into the right directory
-            self.move_file(job_json_dir, "Backend_files/Running_Jobs", job_json_name)
+            self.move(job_json_dir, "Backend_files/Running_Jobs", job_json_name)
             job_dict["job_json_path"] = "Backend_files/Running_Jobs"
         return NextJobSchema(**job_dict)
 
-    def delete_folder(self, folder_path: str) -> None:
-        """
-        Remove the folder from the dropbox. Attention this will remove all the files in the folder.
-        It is not a standard function for storage providers, but allows us to better clean up the
-        tests.
-
-        Args:
-            folder_path: the path where the file should be stored, but excluding the file name
-
-        Returns:
-            None
-        """
-
-        # strip trailing and leading slashes from the storage_path
-        folder_path = folder_path.strip("/")
-
-        # Create an instance of a Dropbox class, which can make requests to the API.
-        with dropbox.Dropbox(
-            app_key=self.app_key,
-            app_secret=self.app_secret,
-            oauth2_refresh_token=self.refresh_token,
-        ) as dbx:
-            # Check that the access token is valid
-            try:
-                dbx.users_get_current_account()
-            except AuthError:
-                sys.exit("ERROR: Invalid access token.")
-
-            # to remove a folder there must be no trailing slash
-            full_path = "/" + folder_path
-            _ = dbx.files_delete_v2(path=full_path)
-
 
 class DropboxProvider(DropboxProviderExtended):
     """
     The class that implements the dropbox storage provider.
     """
 
     def __init__(self, login_dict: DropboxLoginInformation) -> None:
```

### Comparing `sqooler-0.7.1/src/sqooler/storage_providers/local.py` & `sqooler-0.8.0/src/sqooler/storage_providers/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     DisplayNameStr,
     LocalLoginInformation,
     NextJobSchema,
     ResultDict,
     StatusMsgDict,
 )
 from ..security import JWK, JWSDict
-from .base import StorageProvider, datetime_handler, validate_active
+from .base import StorageCore, StorageProvider, datetime_handler, validate_active
 
 
-class LocalProviderExtended(StorageProvider):
+class LocalCore(StorageCore):
     """
-    Create a file storage that works on the local machine.
+    Base class that creates the most important functions for the local storage provider.
     """
 
     def __init__(
         self, login_dict: LocalLoginInformation, name: str, is_active: bool = True
     ) -> None:
         """
         Set up the neccessary keys and create the client through which all the connections will run.
@@ -69,15 +69,15 @@
         full_json_path = os.path.join(folder_path, file_name)
         secure_path = os.path.normpath(full_json_path)
 
         with open(secure_path, "w", encoding="utf-8") as json_file:
             json.dump(content_dict, json_file, default=datetime_handler)
 
     @validate_active
-    def get_file_content(self, storage_path: str, job_id: str) -> dict:
+    def get(self, storage_path: str, job_id: str) -> dict:
         """
         Get the file content from the storage
         """
         # strip trailing and leading slashes from the storage_path
         storage_path = storage_path.strip("/")
 
         # create the full path
@@ -90,29 +90,16 @@
             raise FileNotFoundError(
                 f"The file {secure_path} does not exist and cannot be loaded."
             )
         with open(secure_path, "r", encoding="utf-8") as json_file:
             loaded_data_dict = json.load(json_file)
         return loaded_data_dict
 
-    def get_job_content(self, storage_path: str, job_id: str) -> dict:
-        """
-        Get the content of the job from the storage. This is a wrapper around get_file_content
-        and and handles the different ways of identifiying the job.
-
-        storage_path: the path towards the file, excluding the filename / id
-        job_id: the id of the file we are about to look up
-
-        Returns:
-            The content of the job
-        """
-        job_dict = self.get_file_content(storage_path=storage_path, job_id=job_id)
-        return job_dict
-
-    def update_file(self, content_dict: dict, storage_path: str, job_id: str) -> None:
+    @validate_active
+    def update(self, content_dict: dict, storage_path: str, job_id: str) -> None:
         """
         Update the file content.
 
         Args:
             content_dict: The dictionary containing the new content of the file
             storage_path: The path to the file
             job_id: The id of the job
@@ -136,15 +123,15 @@
             raise FileNotFoundError(
                 f"The file {secure_path} does not exist and cannot be updated."
             )
         with open(secure_path, "w", encoding="utf-8") as json_file:
             json.dump(content_dict, json_file)
 
     @validate_active
-    def move_file(self, start_path: str, final_path: str, job_id: str) -> None:
+    def move(self, start_path: str, final_path: str, job_id: str) -> None:
         """
         Move the file from `start_path` to `final_path`
         """
         start_path = start_path.strip("/")
 
         source_file = self.base_path + "/" + start_path + "/" + job_id + ".json"
 
@@ -152,15 +139,15 @@
         if not os.path.exists(final_path):
             os.makedirs(final_path)
 
         # Move the file
         shutil.move(source_file, final_path)
 
     @validate_active
-    def delete_file(self, storage_path: str, job_id: str) -> None:
+    def delete(self, storage_path: str, job_id: str) -> None:
         """
         Delete the file from the storage
 
         Args:
             storage_path: the path where the file is currently stored, but excluding the file name
             job_id: the name of the file
 
@@ -170,21 +157,45 @@
         Returns:
             None
         """
         storage_path = storage_path.strip("/")
         source_file = self.base_path + "/" + storage_path + "/" + job_id + ".json"
         os.remove(source_file)
 
-    @validate_active
+
+class LocalProviderExtended(StorageProvider, LocalCore):
+    """
+    Create a file storage that works on the local machine.
+
+    Attributes:
+        configs_path: The path to the folder where the configurations are stored
+    """
+
+    configs_path: str = "backends/configs"
+
+    def get_job(self, storage_path: str, job_id: str) -> dict:
+        """
+        Get the content of the job from the storage. This is a wrapper around get_file_content
+        and and handles the different ways of identifiying the job.
+
+        storage_path: the path towards the file, excluding the filename / id
+        job_id: the id of the file we are about to look up
+
+        Returns:
+            The content of the job
+        """
+        job_dict = self.get(storage_path=storage_path, job_id=job_id)
+        return job_dict
+
     def get_backends(self) -> list[DisplayNameStr]:
         """
         Get a list of all the backends that the provider offers.
         """
         # path of the configs
-        config_path = self.base_path + "/backends/configs"
+        config_path = self.base_path + "/" + self.configs_path
         backend_names: list[DisplayNameStr] = []
 
         # If the folder does not exist, return an empty list
         if not os.path.exists(config_path):
             return backend_names
 
         # Get a list of all items in the folder
@@ -269,17 +280,15 @@
 
         Returns:
             The status dict of the job
         """
         status_json_dir = "status/" + display_name
 
         try:
-            status_dict = self.get_file_content(
-                storage_path=status_json_dir, job_id=job_id
-            )
+            status_dict = self.get(storage_path=status_json_dir, job_id=job_id)
             # return StatusMsgDict(**status_dict)
         except FileNotFoundError:
             # if the job_id is not valid, we return an error
             return StatusMsgDict(
                 job_id=job_id,
                 status="ERROR",
                 detail="Cannot get status",
@@ -303,15 +312,15 @@
             FileNotFoundError: If the status does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
         status_json_dir = "status/" + display_name
 
-        self.delete_file(storage_path=status_json_dir, job_id=job_id)
+        self.delete(storage_path=status_json_dir, job_id=job_id)
         return True
 
     def upload_result(
         self,
         result_dict: ResultDict,
         display_name: DisplayNameStr,
         job_id: str,
@@ -369,17 +378,15 @@
                 status="ERROR",
                 header={},
                 results=[],
             )
 
         result_json_dir = "results/" + display_name
         try:
-            result_dict = self.get_file_content(
-                storage_path=result_json_dir, job_id=job_id
-            )
+            result_dict = self.get(storage_path=result_json_dir, job_id=job_id)
         except FileNotFoundError:
             # if the job_id is not valid, we return an error
             return ResultDict(
                 display_name=display_name,
                 backend_version="",
                 job_id=job_id,
                 qobj_id=None,
@@ -399,15 +406,15 @@
             display_name: The name of the backend to which we want to upload the job
             job_id: The job_id of the job that we want to upload the status for
 
         Returns:
             If it was possible to verify the result dict positively.
         """
         result_json_dir = "results/" + display_name
-        result_dict = self.get_file_content(storage_path=result_json_dir, job_id=job_id)
+        result_dict = self.get(storage_path=result_json_dir, job_id=job_id)
         public_jwk = self.get_public_key(display_name)
 
         result_jws = JWSDict(**result_dict)
         return result_jws.verify_signature(public_jwk)
 
     def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
         """
@@ -423,15 +430,15 @@
 
         Returns:
             Success if the file was deleted successfully
         """
 
         result_json_dir = "results/" + display_name
 
-        self.delete_file(storage_path=result_json_dir, job_id=job_id)
+        self.delete(storage_path=result_json_dir, job_id=job_id)
         return True
 
     def update_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
@@ -443,16 +450,18 @@
             config_dict: The dictionary containing the configuration
             display_name : The name of the backend
             private_jwk: The private key of the backend
 
         Returns:
             None
         """
+
+        config_dict = self._verify_config(config_dict, display_name)
         # path of the configs
-        config_path = os.path.join(self.base_path, "backends/configs")
+        config_path = os.path.join(self.base_path, self.configs_path)
         config_path = os.path.normpath(config_path)
 
         file_name = display_name + ".json"
         full_json_path = os.path.join(config_path, file_name)
         secure_path = os.path.normpath(full_json_path)
 
         # check if the file already exists
@@ -470,15 +479,15 @@
 
         upload_dict = self._format_update_config(
             old_config_jws, config_dict, private_jwk
         )
         # maybe this should rather become the update method
         self.upload(
             content_dict=upload_dict,
-            storage_path="backends/configs",
+            storage_path=self.configs_path,
             job_id=display_name,
         )
 
     def upload_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
@@ -491,16 +500,18 @@
             config_dict: The dictionary containing the configuration
             display_name : The name of the backend
             private_jwk: The private key of the backend
 
         Returns:
             None
         """
+        config_dict = self._verify_config(config_dict, display_name)
+
         # path of the configs
-        config_path = os.path.join(self.base_path, "backends/configs")
+        config_path = os.path.join(self.base_path, self.configs_path)
         config_path = os.path.normpath(config_path)
         # test if the config path already exists. If it does not, create it
         if not os.path.exists(config_path):
             os.makedirs(config_path)
 
         file_name = display_name + ".json"
         full_json_path = os.path.join(config_path, file_name)
@@ -511,15 +522,15 @@
             raise FileExistsError(
                 f"The file {secure_path} already exists and should not be overwritten."
             )
 
         upload_dict = self._format_config_dict(config_dict, private_jwk)
         self.upload(
             content_dict=upload_dict,
-            storage_path="backends/configs",
+            storage_path=self.configs_path,
             job_id=display_name,
         )
 
     def get_config(self, display_name: DisplayNameStr) -> BackendConfigSchemaIn:
         """
         The function that downloads the spooler configuration to the storage.
 
@@ -529,16 +540,15 @@
         Raises:
             FileNotFoundError: If the backend does not exist
 
         Returns:
             The configuration of the backend in complete form.
         """
         # path of the configs
-        config_path = "/backends/configs"
-        backend_config_dict = self.get_file_content(config_path, job_id=display_name)
+        backend_config_dict = self.get(self.configs_path, job_id=display_name)
         typed_config = self._adapt_get_config(backend_config_dict)
         return typed_config
 
     def _delete_config(self, display_name: DisplayNameStr) -> bool:
         """
         Delete a config from the storage. This is only intended for test purposes.
 
@@ -547,17 +557,16 @@
 
         Raises:
             FileNotFoundError: If the status does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
-        config_path = "/backends/configs"
 
-        self.delete_file(storage_path=config_path, job_id=display_name)
+        self.delete(storage_path=self.configs_path, job_id=display_name)
         return True
 
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
         The function that uploads the spooler public JWK to the storage. It should
         only be used after `upload_config` as the kid is set there.
 
@@ -633,15 +642,15 @@
             FileNotFoundError: If the status does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
         key_path = "backends/public_keys"
 
-        self.delete_file(storage_path=key_path, job_id=kid)
+        self.delete(storage_path=key_path, job_id=kid)
         return True
 
     def update_in_database(
         self,
         result_dict: ResultDict,
         status_msg_dict: StatusMsgDict,
         job_id: str,
@@ -674,33 +683,33 @@
             )
             if not result_uploaded:
                 raise ValueError("The result was not uploaded successfully.")
 
             # now move the job out of the running jobs into the finished jobs
             job_finished_json_dir = "jobs/finished/" + display_name
 
-            self.move_file(job_json_start_dir, job_finished_json_dir, job_id)
+            self.move(job_json_start_dir, job_finished_json_dir, job_id)
 
         elif status_msg_dict.status == "ERROR":
             # because there was an error, we move the job to the deleted jobs
             deleted_json_dir = "jobs/deleted"
-            self.move_file(job_json_start_dir, deleted_json_dir, job_id)
+            self.move(job_json_start_dir, deleted_json_dir, job_id)
 
         # and create the status json file
         status_json_dir = "status/" + display_name
         try:
-            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+            self.update(status_msg_dict.model_dump(), status_json_dir, job_id)
         except FileNotFoundError:
             logging.warning(
                 "The status file was missing for %s with job_id %s was missing.",
                 display_name,
                 job_id,
             )
             self.upload_status(display_name, "", job_id)
-            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+            self.update(status_msg_dict.model_dump(), status_json_dir, job_id)
 
     def get_file_queue(self, storage_path: str) -> list[str]:
         """
         Get a list of files
 
         Args:
             storage_path: Where are we looking for the files.
@@ -738,15 +747,15 @@
         # if there is a job, we should move it
         if job_list:
             job_json_name = job_list[0]
             job_id = job_json_name[:-5]
             job_dict["job_id"] = job_id
 
             # and move the file into the right directory
-            self.move_file(queue_dir, "jobs/running", job_id)
+            self.move(queue_dir, "jobs/running", job_id)
             job_dict["job_json_path"] = "jobs/running"
         return NextJobSchema(**job_dict)
 
 
 class LocalProvider(LocalProviderExtended):
     """
     Create a file storage that works on the local machine.
```

### Comparing `sqooler-0.7.1/src/sqooler/storage_providers/mongodb.py` & `sqooler-0.8.0/src/sqooler/storage_providers/mongodb.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 import uuid
 from datetime import timezone
 from typing import Optional
 
 from bson.codec_options import CodecOptions
 from bson.errors import InvalidId
 from bson.objectid import ObjectId
+from pymongo.collection import Collection
+from pymongo.database import Database
 
 # necessary for the mongodb provider
 from pymongo.mongo_client import MongoClient
 
 from ..schemes import (
     BackendConfigSchemaIn,
     DisplayNameStr,
     MongodbLoginInformation,
     NextJobSchema,
+    PathStr,
     ResultDict,
     StatusMsgDict,
 )
 from ..security import JWK, JWSDict
-from .base import StorageProvider, validate_active
+from .base import StorageCore, StorageProvider, validate_active
 
 
-class MongodbProviderExtended(StorageProvider):
+class MongodbCore(StorageCore):
     """
-    The access to the mongodb
+    Base class that creates the most important functions for the mongodb storage provider.
     """
 
     def __init__(
         self, login_dict: MongodbLoginInformation, name: str, is_active: bool = True
     ) -> None:
         """
         Set up the neccessary keys and create the client through which all the connections will run.
@@ -65,31 +68,25 @@
         """
         Upload the file to the storage
 
         content_dict: the content that should be uploaded onto the mongodb base
         storage_path: the access path towards the mongodb collection
         job_id: the id of the file we are about to create
         """
-        storage_splitted = storage_path.split("/")
 
-        # get the database on which we work
-        database = self.client[storage_splitted[0]]
-
-        # get the collection on which we work
-        collection_name = ".".join(storage_splitted[1:])
-        collection = database[collection_name]
+        _, collection = self._get_database_and_collection(storage_path)
 
         content_dict["_id"] = ObjectId(job_id)
         collection.insert_one(content_dict)
 
         # remove the id from the content dict for further use
         content_dict.pop("_id", None)
 
     @validate_active
-    def get_file_content(self, storage_path: str, job_id: str) -> dict:
+    def get(self, storage_path: str, job_id: str) -> dict:
         """
         Get the file content from the storage
 
         Args:
             storage_path: the path towards the file, excluding the filename / id
             job_id: the id of the file we are about to look up
 
@@ -101,48 +98,29 @@
         except InvalidId as err:
             raise FileNotFoundError(
                 f"The job_id {job_id} is not valid. Please check the job_id."
             ) from err
 
         document_to_find = {"_id": ObjectId(job_id)}
 
-        # get the database on which we work
-        database = self.client[storage_path.split("/")[0]]
-
-        # get the collection on which we work
-        collection_name = ".".join(storage_path.split("/")[1:])
-        collection = database[collection_name]
+        _, collection = self._get_database_and_collection(storage_path)
 
         result_found = collection.find_one(document_to_find)
 
         if not result_found:
             raise FileNotFoundError(
                 f"Could not find a file under {storage_path} with the id {job_id}."
             )
 
         # remove the id from the result dict for further use
         result_found.pop("_id", None)
         return result_found
 
-    def get_job_content(self, storage_path: str, job_id: str) -> dict:
-        """
-        Get the content of the job from the storage. This is a wrapper around get_file_content
-        and and handles the different ways of identifiying the job.
-
-        storage_path: the path towards the file, excluding the filename / id
-        job_id: the id of the file we are about to look up
-
-        Returns:
-
-        """
-        job_dict = self.get_file_content(storage_path=storage_path, job_id=job_id)
-        job_dict.pop("_id", None)
-        return job_dict
-
-    def update_file(self, content_dict: dict, storage_path: str, job_id: str) -> None:
+    @validate_active
+    def update(self, content_dict: dict, storage_path: str, job_id: str) -> None:
         """
         Update the file content. It replaces the old content with the new content.
 
 
         Args:
             content_dict: The dictionary containing the new content of the file
             storage_path: The path to the file
@@ -150,97 +128,147 @@
 
         Returns:
             None
 
         Raises:
             FileNotFoundError: If the file is not found
         """
-        # get the database on which we work
-        database = self.client[storage_path.split("/")[0]]
 
-        # get the collection on which we work
-        collection_name = ".".join(storage_path.split("/")[1:])
-        collection = database[collection_name]
+        _, collection = self._get_database_and_collection(storage_path)
 
         filter_dict = {"_id": ObjectId(job_id)}
         result = collection.replace_one(filter_dict, content_dict)
 
         if result.matched_count == 0:
             raise FileNotFoundError(f"Could not update file under {storage_path}")
 
     @validate_active
-    def move_file(self, start_path: str, final_path: str, job_id: str) -> None:
+    def move(self, start_path: str, final_path: str, job_id: str) -> None:
         """
         Move the file from start_path to final_path
 
         start_path: the path where the file is currently stored, but excluding the file name
         final_path: the path where the file should be stored, but excluding the file name
         job_id: the name of the file. Is a json file
 
         Returns:
             None
         """
-        # get the database on which we work
-        database = self.client[start_path.split("/")[0]]
 
-        # get the collection on which we work
-        collection_name = ".".join(start_path.split("/")[1:])
-        collection = database[collection_name]
+        # delete the old file
+        _, collection = self._get_database_and_collection(start_path)
 
         document_to_find = {"_id": ObjectId(job_id)}
         result_found = collection.find_one(document_to_find)
 
-        # delete the old file
         collection.delete_one(document_to_find)
 
         # add the document to the new collection
-        database = self.client[final_path.split("/")[0]]
-        collection_name = ".".join(final_path.split("/")[1:])
-        collection = database[collection_name]
+        _, collection = self._get_database_and_collection(final_path)
+
         collection.insert_one(result_found)
 
     @validate_active
-    def delete_file(self, storage_path: str, job_id: str) -> None:
+    def delete(self, storage_path: str, job_id: str) -> None:
         """
         Remove the file from the mongodb database
 
         Args:
             storage_path: the path where the file is currently stored, but excluding the file name
             job_id: the name of the file
 
         Returns:
             None
         """
-        # get the database on which we work
-        database = self.client[storage_path.split("/")[0]]
+        _, collection = self._get_database_and_collection(storage_path)
 
-        # get the collection on which we work
-        collection_name = ".".join(storage_path.split("/")[1:])
-        collection = database[collection_name]
         try:
             document_to_find = {"_id": ObjectId(job_id)}
         except InvalidId as err:
             raise FileNotFoundError(
                 f"The job_id {job_id} is not valid. Please check the job_id."
             ) from err
         result = collection.delete_one(document_to_find)
         if result.deleted_count == 0:
             raise FileNotFoundError(
                 f"Could not find a file under {storage_path} with the id {job_id}."
             )
 
+    def _get_database_and_collection(
+        self, storage_path: str
+    ) -> tuple[Database, Collection]:
+        """
+        Get the database and the collection on which we work.
+
+        Args:
+            storage_path: the path where the file is currently stored, but excluding the file name
+
+        Returns:
+            The database and the collection on which we work
+        """
+        # strip the path from leading and trailing slashes
+        storage_path = storage_path.strip("/")
+
+        # get the database on which we work
+        database = self.client[storage_path.split("/")[0]]
+
+        # get the collection on which we work
+        collection_name = ".".join(storage_path.split("/")[1:])
+        collection = database[collection_name]
+        return database, collection
+
+
+class MongodbProviderExtended(StorageProvider, MongodbCore):
+    """
+    The access to the mongodb
+
+    Attributes:
+        configs_path: The path to the folder where the configurations are stored
+        queue_path: The path to the folder where the jobs are stored
+        running_path: The path to the folder where the running jobs are stored
+        finished_path: The path to the folder where the finished jobs are stored
+        deleted_path: The path to the folder where the deleted jobs are stored
+        status_path: The path to the folder where the status is stored
+        results_path: The path to the folder where the results are stored
+        pks_path: The path to the folder where the public keys are stored
+    """
+
+    configs_path: PathStr = "backends/configs"
+    queue_path: PathStr = "jobs/queued"
+    running_path: PathStr = "jobs/running"
+    finished_path: PathStr = "jobs/finished"
+    deleted_path: PathStr = "jobs/deleted"
+    status_path: PathStr = "status"
+    results_path: PathStr = "results"
+    pks_path: PathStr = "backends/public_keys"
+
+    def get_job(self, storage_path: str, job_id: str) -> dict:
+        """
+        Get the content of the job from the storage. This is a wrapper around get
+        and and handles the different ways of identifiying the job.
+
+        storage_path: the path towards the file, excluding the filename / id
+        job_id: the id of the file we are about to look up
+
+        Returns:
+            The content of the job
+        """
+        job_dict = self.get(storage_path=storage_path, job_id=job_id)
+        job_dict.pop("_id", None)
+        return job_dict
+
     @validate_active
     def get_backends(self) -> list[DisplayNameStr]:
         """
         Get a list of all the backends that the provider offers.
         """
 
-        # get the database on which we work
-        database = self.client["backends"]
-        config_collection = database["configs"]
+        # get the collection on which we work
+        _, config_collection = self._get_database_and_collection(self.configs_path)
+
         # get all the documents in the collection configs and save the disply_name in a list
         backend_names: list[DisplayNameStr] = []
         for config_dict in config_collection.find():
             config_dict.pop("_id")
             expected_keys_for_jws = {"header", "payload", "signature"}
             if set(config_dict.keys()) == expected_keys_for_jws:
                 backend_names.append(config_dict["payload"]["display_name"])
@@ -261,26 +289,22 @@
             config_dict: The dictionary containing the configuration
             display_name : The name of the backend
             private_jwk: The private JWK to sign the configuration with
 
         Returns:
             None
         """
-        config_path = "backends/configs"
-        config_dict.display_name = display_name
+        config_dict = self._verify_config(config_dict, display_name)
 
         # first we have to check if the device already exists in the database
 
         document_to_find = {"display_name": display_name}
 
-        # get the database on which we work
-        database = self.client["backends"]
-
         # get the collection on which we work
-        collection = database["configs"]
+        _, collection = self._get_database_and_collection(self.configs_path)
 
         document_to_find = {"display_name": display_name}
         result_found = collection.find_one(document_to_find)
         if result_found:
             raise FileExistsError(
                 f"The configuration for {display_name} already exists and should not be overwritten."
             )
@@ -291,15 +315,15 @@
         if result_found:
             raise FileExistsError(
                 f"The configuration for {display_name} already exists and should not be overwritten."
             )
 
         upload_dict = self._format_config_dict(config_dict, private_jwk)
         config_id = uuid.uuid4().hex[:24]
-        self.upload(upload_dict, config_path, config_id)
+        self.upload(upload_dict, self.configs_path, config_id)
 
     def update_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
     ) -> None:
@@ -310,23 +334,18 @@
             config_dict: The dictionary containing the configuration
             display_name : The name of the backend
             private_jwk: The private key of the backend
 
         Returns:
             None
         """
-        config_path = "backends/configs"
 
-        config_dict.display_name = display_name
+        config_dict = self._verify_config(config_dict, display_name)
 
-        # get the database on which we work
-        database = self.client["backends"]
-
-        # get the collection on which we work
-        collection = database["configs"]
+        _, collection = self._get_database_and_collection(self.configs_path)
 
         # now make sure that we add the timezone as we open the file
         collection_with_tz = collection.with_options(
             codec_options=CodecOptions(tz_aware=True, tzinfo=timezone.utc)
         )
         # first we have to check if the device already exists in the database
         document_to_find = {"display_name": display_name}
@@ -351,17 +370,17 @@
                     "Use the upload_config method instead."
                 )
             )
         upload_dict = self._format_update_config(
             old_config_jws, config_dict, private_jwk
         )
 
-        self.update_file(
+        self.update(
             content_dict=upload_dict,
-            storage_path=config_path,
+            storage_path=self.configs_path,
             job_id=job_id,
         )
 
     @validate_active
     def get_config(self, display_name: DisplayNameStr) -> BackendConfigSchemaIn:
         """
         The function that downloads the spooler configuration to the storage.
@@ -371,17 +390,16 @@
 
         Raises:
             FileNotFoundError: If the backend does not exist
 
         Returns:
             The configuration of the backend in complete form.
         """
-        # get the database on which we work
-        database = self.client["backends"]
-        config_collection = database["configs"]
+        # get the collection on which we work
+        _, config_collection = self._get_database_and_collection(self.configs_path)
 
         # create the filter for the document with display_name that is equal to display_name
         document_to_find = {"display_name": display_name}
         backend_config_dict = config_collection.find_one(document_to_find)
 
         signed_document_to_find = {"payload.display_name": display_name}
         signed_backend_config_dict = config_collection.find_one(signed_document_to_find)
@@ -410,27 +428,25 @@
             FileNotFoundError: If the config does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
 
         config_dict = self.get_config(display_name)
-        config_path = "backends/configs"
-        database = self.client["backends"]
-        collection = database["configs"]
+        _, collection = self._get_database_and_collection(self.configs_path)
 
         if not config_dict.sign:
             document_to_find = {"display_name": display_name}
         else:
             document_to_find = {"payload.display_name": display_name}
 
         result_found = collection.find_one(document_to_find)
         if result_found is None:
             raise FileNotFoundError(f"the config for {display_name} does not exist.")
-        self.delete_file(config_path, str(result_found["_id"]))
+        self.delete(self.configs_path, str(result_found["_id"]))
 
         return True
 
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
         """
@@ -441,15 +457,15 @@
             display_name: the name of the backend
             username: the name of the user that submitted the job
 
         Returns:
             The job id of the uploaded job.
         """
 
-        storage_path = "jobs/queued/" + display_name
+        storage_path = f"{self.queue_path}/{display_name}"
         job_id = (uuid.uuid4().hex)[:24]
 
         self.upload(content_dict=job_dict, storage_path=storage_path, job_id=job_id)
         return job_id
 
     def upload_status(
         self,
@@ -466,15 +482,15 @@
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
             private_jwk: The private key of the backend
 
         Returns:
             The status dict of the job
         """
-        storage_path = "status/" + display_name
+        storage_path = f"{self.status_path}/{display_name}"
         status_draft = {
             "job_id": job_id,
             "status": "INITIALIZING",
             "detail": "Got your json.",
             "error_message": "None",
         }
 
@@ -500,20 +516,18 @@
             display_name: The name of the backend to which we want to upload the job
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
 
         Returns:
             The status dict of the job
         """
-        status_json_dir = "status/" + display_name
+        status_json_dir = f"{self.status_path}/{display_name}"
 
         try:
-            status_dict = self.get_file_content(
-                storage_path=status_json_dir, job_id=job_id
-            )
+            status_dict = self.get(storage_path=status_json_dir, job_id=job_id)
         except FileNotFoundError as err:
             # if the job_id is not valid, we return an error
             return StatusMsgDict(
                 job_id=job_id,
                 status="ERROR",
                 detail="The job_id is not valid.",
                 error_message=str(err),
@@ -534,17 +548,17 @@
 
         Raises:
             FileNotFoundError: If the status does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
-        status_json_dir = "status/" + display_name
+        status_json_dir = f"{self.status_path}/{display_name}"
 
-        self.delete_file(storage_path=status_json_dir, job_id=job_id)
+        self.delete(storage_path=status_json_dir, job_id=job_id)
         return True
 
     def upload_result(
         self,
         result_dict: ResultDict,
         display_name: DisplayNameStr,
         job_id: str,
@@ -558,15 +572,15 @@
             display_name: The name of the backend to which we want to upload the job
             job_id: The job_id of the job that we want to upload the status for
             private_jwk: The private key of the backend
 
         Returns:
             The success of the upload process
         """
-        result_json_dir = "results/" + display_name
+        result_json_dir = f"{self.results_path}/{display_name}"
 
         return self._common_upload_result(
             result_dict,
             display_name,
             job_id,
             result_json_dir,
             result_json_name=job_id,
@@ -584,19 +598,17 @@
             username: The username of the user that is uploading the job
             job_id: The job_id of the job that we want to upload the status for
 
         Returns:
             The result dict of the job. If the information is not available, the result dict
             has a status of "ERROR".
         """
-        result_json_dir = "results/" + display_name
+        result_json_dir = f"{self.results_path}/{display_name}"
         try:
-            result_dict = self.get_file_content(
-                storage_path=result_json_dir, job_id=job_id
-            )
+            result_dict = self.get(storage_path=result_json_dir, job_id=job_id)
         except FileNotFoundError:
             # if the job_id is not valid, we return an error
             return ResultDict(
                 display_name=display_name,
                 backend_version="",
                 job_id=job_id,
                 qobj_id=None,
@@ -616,16 +628,16 @@
         Args:
             display_name: The name of the backend to which we want to upload the job
             job_id: The job_id of the job that we want to upload the status for
 
         Returns:
             If it was possible to verify the result dict positively.
         """
-        result_json_dir = "results/" + display_name
-        result_dict = self.get_file_content(storage_path=result_json_dir, job_id=job_id)
+        result_json_dir = f"{self.results_path}/{display_name}"
+        result_dict = self.get(storage_path=result_json_dir, job_id=job_id)
         public_jwk = self.get_public_key(display_name)
 
         result_jws = JWSDict(**result_dict)
         return result_jws.verify_signature(public_jwk)
 
     def _delete_result(self, display_name: DisplayNameStr, job_id: str) -> bool:
         """
@@ -638,18 +650,17 @@
 
         Raises:
             FileNotFoundError: If the result does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
+        result_json_dir = f"{self.results_path}/{display_name}"
 
-        result_json_dir = "results/" + display_name
-
-        self.delete_file(storage_path=result_json_dir, job_id=job_id)
+        self.delete(storage_path=result_json_dir, job_id=job_id)
         return True
 
     def upload_public_key(self, public_jwk: JWK, display_name: DisplayNameStr) -> None:
         """
         The function that uploads the spooler public JWK to the storage.
 
         Args:
@@ -663,58 +674,51 @@
         if not public_jwk.key_ops == "verify":
             raise ValueError("The key is not intended for verification")
 
         # make sure that the key does not contain a private key
         if public_jwk.d is not None:
             raise ValueError("The key contains a private key")
 
-        pk_paths = "backends/public_keys"
-
         # make sure that the key has the correct kid
         config_dict = self.get_config(display_name)
         if public_jwk.kid != config_dict.kid:
             raise ValueError("The key does not have the correct kid.")
 
-        # first we have to check if the device already exists in the database
+        _, collection = self._get_database_and_collection(self.pks_path)
 
+        # first we have to check if the device already exists in the database
         document_to_find = {"kid": config_dict.kid}
 
-        # get the database on which we work
-        database = self.client["backends"]
-
-        # get the collection on which we work
-        collection = database["public_keys"]
-
         result_found = collection.find_one(document_to_find)
         if result_found:
             # update the file
-            self.update_file(
+            self.update(
                 content_dict=public_jwk.model_dump(),
-                storage_path=pk_paths,
+                storage_path=self.pks_path,
                 job_id=result_found["_id"],
             )
             return
 
         # if the device does not exist, we have to create it
         config_id = uuid.uuid4().hex[:24]
-        self.upload(public_jwk.model_dump(), pk_paths, config_id)
+        self.upload(public_jwk.model_dump(), self.pks_path, config_id)
 
     def get_public_key(self, display_name: DisplayNameStr) -> JWK:
         """
         The function that gets the spooler public JWK for the device.
 
         Args:
             display_name : The name of the backend
 
         Returns:
             JWk : The public JWK object
         """
+
         # get the database on which we work
-        database = self.client["backends"]
-        collection = database["public_keys"]
+        _, collection = self._get_database_and_collection(self.pks_path)
 
         # now get the appropiate kid
         config_dict = self.get_config(display_name)
         if config_dict.kid is None:
             raise ValueError("The kid is not set in the backend configuration.")
 
         # create the filter for the document with display_name that is equal to display_name
@@ -736,23 +740,22 @@
 
         Raises:
             FileNotFoundError: If the public key does not exist.
 
         Returns:
             Success if the file was deleted successfully
         """
-        key_path = "backends/public_keys"
         document_to_find = {"kid": kid}
+        # get the database on which we work
+        _, collection = self._get_database_and_collection(self.pks_path)
 
-        database = self.client["backends"]
-        collection = database["public_keys"]
         result_found = collection.find_one(document_to_find)
         if result_found is None:
             raise FileNotFoundError(f"The public key with kid {kid} does not exist")
-        self.delete_file(key_path, str(result_found["_id"]))
+        self.delete(self.pks_path, str(result_found["_id"]))
         return True
 
     def update_in_database(
         self,
         result_dict: ResultDict | None,
         status_msg_dict: StatusMsgDict,
         job_id: str,
@@ -776,71 +779,64 @@
         Returns:
             None
 
         Raises:
 
         """
 
-        job_json_start_dir = "jobs/running"
+        job_json_start_dir = self.running_path
         # check if the job is done or had an error
         if status_msg_dict.status == "DONE":
             # test if the result dict is None
             if result_dict is None:
                 raise ValueError(
                     "The 'result_dict' argument cannot be None if the job is done."
                 )
             result_uploaded = self.upload_result(
                 result_dict, display_name, job_id, private_jwk
             )
             if not result_uploaded:
                 raise ValueError("The result was not uploaded successfully.")
 
             # now move the job out of the running jobs into the finished jobs
-            job_finished_json_dir = "jobs/finished/" + display_name
-            self.move_file(job_json_start_dir, job_finished_json_dir, job_id)
+            job_finished_json_dir = f"{self.finished_path}/{display_name}"
+            self.move(job_json_start_dir, job_finished_json_dir, job_id)
 
         elif status_msg_dict.status == "ERROR":
             # because there was an error, we move the job to the deleted jobs
-            deleted_json_dir = "jobs/deleted"
-            self.move_file(job_json_start_dir, deleted_json_dir, job_id)
+            deleted_json_dir = self.deleted_path
+            self.move(job_json_start_dir, deleted_json_dir, job_id)
 
         # TODO: most likely we should raise an error if the status of the job is not DONE or ERROR
 
         # and create the status json file
-        status_json_dir = "status/" + display_name
+        status_json_dir = f"{self.status_path}/{display_name}"
         try:
-            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+            self.update(status_msg_dict.model_dump(), status_json_dir, job_id)
         except FileNotFoundError:
             logging.warning(
                 "The status file was missing for %s with job_id %s was missing.",
                 display_name,
                 job_id,
             )
             self.upload_status(display_name, "", job_id)
-            self.update_file(status_msg_dict.model_dump(), status_json_dir, job_id)
+            self.update(status_msg_dict.model_dump(), status_json_dir, job_id)
 
     def get_file_queue(self, storage_path: str) -> list[str]:
         """
         Get a list of documents in the collection of all the queued jobs.
 
         Args:
             storage_path: Where are we looking for the files.
 
         Returns:
             A list of files that was found.
         """
-        # strip trailing and leading slashes from the paths
-        storage_path = storage_path.strip("/")
 
-        # get the database on which we work
-        database = self.client[storage_path.split("/")[0]]
-
-        # get the collection on which we work
-        collection_name = ".".join(storage_path.split("/")[1:])
-        collection = database[collection_name]
+        _, collection = self._get_database_and_collection(storage_path)
 
         # now get the id of all the documents in the collection
         results = collection.find({}, {"_id": 1})
         file_list = []
         for result in results:
             file_list.append(str(result["_id"]))
         return file_list
@@ -857,30 +853,30 @@
             display_name: The name of the backend
             private_jwk: The private JWK to sign the result with
 
         Returns:
             the job dict
         """
 
-        queue_dir = "jobs/queued/" + display_name
+        queue_dir = f"{self.queue_path}/{display_name}"
 
         job_dict = self._get_default_next_schema_dict()
         job_list = self.get_file_queue(queue_dir)
 
         # update the time stamp of the last job
         self.timestamp_queue(display_name, private_jwk)
 
         # if there is a job, we should move it
         if job_list:
             job_id = job_list[0]
             job_dict["job_id"] = job_id
 
             # and move the file into the right directory
-            self.move_file(queue_dir, "jobs/running", job_id)
-            job_dict["job_json_path"] = "jobs/running"
+            self.move(queue_dir, self.running_path, job_id)
+            job_dict["job_json_path"] = self.running_path
         return NextJobSchema(**job_dict)
 
 
 class MongodbProvider(MongodbProviderExtended):
     """
     The access to the mongodb. This is the simplified version for people that are running devices.
     """
```

### Comparing `sqooler-0.7.1/src/sqooler/utils.py` & `sqooler-0.8.0/src/sqooler/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,27 @@
 This module contains some functions that are especially helpful for deployment of the 
 sqooler package.
 """
 
 import logging
 import time
 import traceback
+import uuid
+from typing import Tuple
 
 import regex as re
 from decouple import config
 from pydantic import ValidationError
 
-from .schemes import NextJobSchema, get_init_results, get_init_status
+from .schemes import (
+    BackendConfigSchemaIn,
+    NextJobSchema,
+    get_init_results,
+    get_init_status,
+)
 from .security import public_from_private_jwk
 from .spoolers import Spooler
 from .storage_providers.base import StorageProvider
 
 
 def update_backends(
     storage_provider: StorageProvider, backends: dict[str, Spooler]
@@ -117,15 +124,15 @@
             )
             job_dict = NextJobSchema(job_id="None", job_json_path="None")
 
         if job_dict.job_json_path == "None":
             counter += 1
             continue
         logging.debug("Got a job in %s", requested_backend)
-        job_json_dict = storage_provider.get_job_content(
+        job_json_dict = storage_provider.get_job(
             storage_path=job_dict.job_json_path, job_id=job_dict.job_id
         )
 
         result_dict = get_init_results()
         # Fix this pylint issue whenever you have time, but be careful !
         # pylint: disable=W0703
         try:
@@ -179,7 +186,39 @@
     """
 
     result_dict, status_msg_dict = spooler.add_job(json_dict, job_id)
     if not status_msg_dict.status == "DONE":
         logging.error(status_msg_dict.error_message)
         raise AssertionError("Job failed")
     return result_dict.model_dump()
+
+
+def get_dummy_config(sign: bool = True) -> Tuple[str, BackendConfigSchemaIn]:
+    """
+    Generate the dummy config of the fermion type.
+
+    Args:
+        sign: Whether to sign the files.
+    Returns:
+        The backend name and the backend config input.
+    """
+
+    dummy_id = uuid.uuid4().hex[:5]
+    backend_name = f"dummy{dummy_id}"
+
+    dummy_dict: dict = {}
+    dummy_dict["gates"] = []
+    dummy_dict["display_name"] = backend_name
+    dummy_dict["num_wires"] = 3
+    dummy_dict["version"] = "0.0.1"
+    dummy_dict["description"] = "This is a dummy backend."
+    dummy_dict["cold_atom_type"] = "fermion"
+    dummy_dict["max_experiments"] = 1
+    dummy_dict["max_shots"] = 1
+    dummy_dict["simulator"] = True
+    dummy_dict["supported_instructions"] = []
+    dummy_dict["wire_order"] = "interleaved"
+    dummy_dict["num_species"] = 1
+    dummy_dict["sign"] = sign
+
+    backend_info = BackendConfigSchemaIn(**dummy_dict)
+    return backend_name, backend_info
```

### Comparing `sqooler-0.7.1/PKG-INFO` & `sqooler-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqooler
-Version: 0.7.1
+Version: 0.8.0
 Summary: Code that enables validated cloud access to quantum hardware (simulators)
 Home-page: https://github.com/Alqor-UG/sqooler
 License: Unlicense
 Keywords: pydantic,quantum-hardware,sdk-python
 Author: fretchen
 Author-email: fred.jendrzejewski@gmail.com
 Requires-Python: >=3.10,<4.0
```

