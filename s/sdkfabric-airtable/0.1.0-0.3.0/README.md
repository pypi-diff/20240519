# Comparing `tmp/sdkfabric_airtable-0.1.0.tar.gz` & `tmp/sdkfabric_airtable-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_airtable-0.1.0.tar", last modified: Sat May 18 10:31:10 2024, max compression
+gzip compressed data, was "sdkfabric_airtable-0.3.0.tar", last modified: Sun May 19 21:53:21 2024, max compression
```

## Comparing `sdkfabric_airtable-0.1.0.tar` & `sdkfabric_airtable-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:10.483329 sdkfabric_airtable-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-18 10:31:10.483329 sdkfabric_airtable-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:31:10.483329 sdkfabric_airtable-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:10.479329 sdkfabric_airtable-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:10.479329 sdkfabric_airtable-0.1.0/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/bulk_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/bulk_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/meta_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/record_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/records_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-18 10:31:02.000000 sdkfabric_airtable-0.1.0/src/sdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:31:10.479329 sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-18 10:31:10.000000 sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 10:31:10.000000 sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:31:10.000000 sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 10:31:10.000000 sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 10:31:10.000000 sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.170533 sdkfabric_airtable-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/bulk_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/bulk_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/field_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/fields_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/meta_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/record_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/records_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 21:53:17.000000 sdkfabric_airtable-0.3.0/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:53:21.174533 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 21:53:21.000000 sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/top_level.txt
```

### Comparing `sdkfabric_airtable-0.1.0/LICENSE` & `sdkfabric_airtable-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.1.0/PKG-INFO` & `sdkfabric_airtable-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-airtable
-Version: 0.1.0
+Version: 0.3.0
 Summary: Airtable Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/airtable-python
 Project-URL: Issues, https://github.com/sdk-fabric/airtable-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Airtable](https://app.typehub.cloud/d/sdkfabric/airtable)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/airtable
```

### Comparing `sdkfabric_airtable-0.1.0/README.md` & `sdkfabric_airtable-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Airtable](https://app.typehub.cloud/d/sdkfabric/airtable)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/airtable
```

### Comparing `sdkfabric_airtable-0.1.0/pyproject.toml` & `sdkfabric_airtable-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-airtable"
-version = "0.1.0"
+version = "0.3.0"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Airtable Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_airtable-0.1.0/src/sdk/bulk_update_request.py` & `sdkfabric_airtable-0.3.0/src/sdk/bulk_update_request.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.1.0/src/sdk/bulk_update_response.py` & `sdkfabric_airtable-0.3.0/src/sdk/bulk_update_response.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.1.0/src/sdk/client.py` & `sdkfabric_airtable-0.3.0/src/sdk/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .meta_tag import MetaTag
 from .records_tag import RecordsTag
+from .fields_tag import FieldsTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     def meta(self) -> MetaTag:
         return MetaTag(
@@ -23,13 +24,19 @@
 
     def records(self) -> RecordsTag:
         return RecordsTag(
             self.http_client,
             self.parser
         )
 
+    def fields(self) -> FieldsTag:
+        return FieldsTag(
+            self.http_client,
+            self.parser
+        )
+
 
 
     @staticmethod
     def build(token: str):
         return Client("https://api.airtable.com/", sdkgen.HttpBearer(token))
```

### Comparing `sdkfabric_airtable-0.1.0/src/sdk/meta_tag.py` & `sdkfabric_airtable-0.3.0/src/sdk/meta_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.1.0/src/sdk/record.py` & `sdkfabric_airtable-0.3.0/src/sdk/record.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.1.0/src/sdk/records_tag.py` & `sdkfabric_airtable-0.3.0/src/sdk/records_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_airtable-0.1.0/src/sdkfabric_airtable.egg-info/PKG-INFO` & `sdkfabric_airtable-0.3.0/src/sdkfabric_airtable.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-airtable
-Version: 0.1.0
+Version: 0.3.0
 Summary: Airtable Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/airtable-python
 Project-URL: Issues, https://github.com/sdk-fabric/airtable-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -29,15 +29,19 @@
 please register at the [TypeHub](https://typehub.cloud/) platform and create
 a pull request at the [Airtable](https://app.typehub.cloud/d/sdkfabric/airtable)
 specification. The system will then automatically create a GIT commit and update
 the code.
 
 ## Usage
 
-The following example shows how you can use the client:
+The following example shows how you initialize the client:
 
 ```python
-const credentials = new HttpBearer('[access_token]');
-const client = Client::build(credentials);
+from sdk.client import Client
+
+client = Client.build("[access_token]")
 
 // @TODO use the client
 ```
+
+You can find all available operations and types at:
+https://app.typehub.cloud/d/sdkfabric/airtable
```

