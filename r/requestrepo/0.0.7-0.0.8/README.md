# Comparing `tmp/requestrepo-0.0.7.tar.gz` & `tmp/requestrepo-0.0.8.tar.gz`

## Comparing `requestrepo-0.0.7.tar` & `requestrepo-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 requestrepo-0.0.7/requirements.txt
--rw-r--r--   0        0        0    10322 2020-02-02 00:00:00.000000 requestrepo-0.0.7/src/requestrepo/__init__.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 requestrepo-0.0.7/src/requestrepo/models/__init__.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 requestrepo-0.0.7/tests/dns.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 requestrepo-0.0.7/tests/request.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 requestrepo-0.0.7/tests/response.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 requestrepo-0.0.7/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.7/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 requestrepo-0.0.8/requirements.txt
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 requestrepo-0.0.8/src/requestrepo/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 requestrepo-0.0.8/src/requestrepo/models/__init__.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 requestrepo-0.0.8/tests/dns.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 requestrepo-0.0.8/tests/request.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 requestrepo-0.0.8/tests/response.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 requestrepo-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.8/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.8/PKG-INFO
```

### Comparing `requestrepo-0.0.7/src/requestrepo/__init__.py` & `requestrepo-0.0.8/src/requestrepo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import jwt
-import sys
 import json
 import base64
 import asyncio
+import logging
 import requests
-import warnings
 from websockets.client import connect
 from typing import Union, Dict, List, Callable, Optional
 from jwt.exceptions import DecodeError
 from .models import HttpRequest, DnsRequest, HttpResponse, DnsRecord
 
 class Requestrepo:
   """
@@ -57,15 +56,16 @@
 
     try:
       subdomain: str = jwt.decode(token, options={"verify_signature": False})["subdomain"]
     except DecodeError:
       subdomain: str = jwt.decode(token, verify=False)["subdomain"]
 
     if info:
-      warnings.warn(f"[+] Running on {subdomain}.{host} with token: {token}")
+      logger = logging.getLogger(__name__)
+      logger.info(f"Running on {subdomain}.{host} with token: {token}")
 
     self.__token = token
     self.subdomain = subdomain
     self.domain = subdomain + "." + host
 
     if "https" == protocol.lower():
       wsp = "wss"
```

### Comparing `requestrepo-0.0.7/src/requestrepo/models/__init__.py` & `requestrepo-0.0.8/src/requestrepo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.7/tests/request.py` & `requestrepo-0.0.8/tests/request.py`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.7/tests/response.py` & `requestrepo-0.0.8/tests/response.py`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.7/.gitignore` & `requestrepo-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.7/LICENSE` & `requestrepo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.7/README.md` & `requestrepo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.7/pyproject.toml` & `requestrepo-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "requestrepo"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{ name = "Dragos Albastroiu", email = "adragos@protonmail.com" }]
 description = "Python bindings to automate requestrepo.com"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `requestrepo-0.0.7/PKG-INFO` & `requestrepo-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: requestrepo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bindings to automate requestrepo.com
 Project-URL: Homepage, https://github.com/adrgs/requestrepo-lib
 Project-URL: Issues, https://github.com/adrgs/requestrepo-lib/issues
 Author-email: Dragos Albastroiu <adragos@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

