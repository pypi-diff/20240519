# Comparing `tmp/uploadthing_py-0.1.0.tar.gz` & `tmp/uploadthing_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.1.0.tar", max compression
+gzip compressed data, was "uploadthing_py-0.1.1.tar", max compression
```

## Comparing `uploadthing_py-0.1.0.tar` & `uploadthing_py-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-19 15:22:38.340742 uploadthing_py-0.1.0/README.md
--rw-r--r--   0        0        0      575 2024-05-19 21:29:30.267723 uploadthing_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      278 2024-05-19 21:12:17.803152 uploadthing_py-0.1.0/utpy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.1.0/utpy/py.typed
--rw-r--r--   0        0        0     2507 2024-05-19 21:12:18.711453 uploadthing_py-0.1.0/utpy/types.py
--rw-r--r--   0        0        0     5333 2024-05-19 21:12:28.329384 uploadthing_py-0.1.0/utpy/utapi.py
--rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.1.0/utpy/utils.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 uploadthing_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-19 15:22:38.340742 uploadthing_py-0.1.1/README.md
+-rw-r--r--   0        0        0      555 2024-05-19 21:39:23.893185 uploadthing_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-05-19 21:37:22.451857 uploadthing_py-0.1.1/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.1.1/uploadthing_py/py.typed
+-rw-r--r--   0        0        0     2507 2024-05-19 21:12:18.711453 uploadthing_py-0.1.1/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5393 2024-05-19 21:37:39.542526 uploadthing_py-0.1.1/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0      717 2024-05-19 21:11:35.769126 uploadthing_py-0.1.1/uploadthing_py/utils.py
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 uploadthing_py-0.1.1/PKG-INFO
```

### Comparing `uploadthing_py-0.1.0/pyproject.toml` & `uploadthing_py-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "uploadthing.py"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python SDK for UploadThing"
 authors = ["juliusmarminge <julius0216@outlook.com>"]
 readme = "README.md"
-packages = [{ include = "utpy" }, { include = "utpy/py.typed" }]
+packages = [{ include = "uploadthing_py" }]
 license = "MIT"
 
+
 [tool.poetry.dependencies]
 python = "^3.12"
 httpx = "^0.27.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
```

### Comparing `uploadthing_py-0.1.0/utpy/types.py` & `uploadthing_py-0.1.1/uploadthing_py/types.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.1.0/utpy/utapi.py` & `uploadthing_py-0.1.1/uploadthing_py/utapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import typing as t, logging
 from httpx import AsyncClient, Response
 
-import utpy
-from utpy.types import (
+import uploadthing_py
+from uploadthing_py.types import (
     ACL,
     MaybeList,
     File,
     ListFiles,
     DeleteFiles,
     RenameFile,
     GetUsageInfo,
     GetSignedUrl,
     UpdateACL,
 )
-from utpy.utils import json_stringify, del_none
+from uploadthing_py.utils import json_stringify, del_none
 
 
 class HttpError(Exception):
     def __init__(self, response: Response):
         self.status_code = response.status_code
         self.message = response.text
 
@@ -41,21 +41,21 @@
         base_url: str = "https://api.uploadthing.com",
     ):
         self._api_key = api_key
         self._client = AsyncClient(
             base_url=base_url,
             headers={
                 "x-uploadthing-api-key": self._api_key,
-                "x-uploadthing-be-adapter": f"utpy@{utpy.__version__}",
+                "x-uploadthing-be-adapter": f"uploadthing_py@{uploadthing_py.__version__}",
                 "x-uploadthing-version": "6.10.0",
             },
         )
         self._baseUrl = base_url
         self._default_key_type = key_type
-        self._logger = logging.getLogger("UTPY")
+        self._logger = logging.getLogger("uploadthing_py")
 
     async def _request_ut_api(self, path: str, payload: t.Dict = None) -> t.Dict:
         stringified = json_stringify(del_none(payload or {}))
         self._logger.debug(f"Requesting UploadThing API with: {path} {stringified}")
         response = await self._client.post(
             path,
             content=stringified,
```

### Comparing `uploadthing_py-0.1.0/utpy/utils.py` & `uploadthing_py-0.1.1/uploadthing_py/utils.py`

 * *Files identical despite different names*

