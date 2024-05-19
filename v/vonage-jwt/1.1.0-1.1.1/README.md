# Comparing `tmp/vonage_jwt-1.1.0.tar.gz` & `tmp/vonage_jwt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_jwt-1.1.0.tar", last modified: Wed Oct 18 14:13:53 2023, max compression
+gzip compressed data, was "vonage_jwt-1.1.1.tar", last modified: Sun May 19 02:49:24 2024, max compression
```

## Comparing `vonage_jwt-1.1.0.tar` & `vonage_jwt-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-10-18 14:13:53.758169 vonage_jwt-1.1.0/
--rw-r--r--   0 mkahan     (503) staff       (20)    11357 2023-06-02 02:36:35.000000 vonage_jwt-1.1.0/LICENSE
--rw-r--r--   0 mkahan     (503) staff       (20)     2764 2023-10-18 14:13:53.757504 vonage_jwt-1.1.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     1897 2023-10-18 14:13:27.000000 vonage_jwt-1.1.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      927 2023-10-18 14:13:27.000000 vonage_jwt-1.1.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2023-10-18 14:13:53.758216 vonage_jwt-1.1.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-10-18 14:13:53.749653 vonage_jwt-1.1.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-10-18 14:13:53.753563 vonage_jwt-1.1.0/src/vonage_jwt/
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2023-06-02 11:52:51.000000 vonage_jwt-1.1.0/src/vonage_jwt/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2006 2023-10-18 14:13:27.000000 vonage_jwt-1.1.0/src/vonage_jwt/jwt.py
--rw-r--r--   0 mkahan     (503) staff       (20)      502 2023-10-18 14:13:27.000000 vonage_jwt-1.1.0/src/vonage_jwt/verify_jwt.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-10-18 14:13:53.755823 vonage_jwt-1.1.0/src/vonage_jwt.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     2764 2023-10-18 14:13:53.000000 vonage_jwt-1.1.0/src/vonage_jwt.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      352 2023-10-18 14:13:53.000000 vonage_jwt-1.1.0/src/vonage_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-10-18 14:13:53.000000 vonage_jwt-1.1.0/src/vonage_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       21 2023-10-18 14:13:53.000000 vonage_jwt-1.1.0/src/vonage_jwt.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       11 2023-10-18 14:13:53.000000 vonage_jwt-1.1.0/src/vonage_jwt.egg-info/top_level.txt
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-10-18 14:13:53.756853 vonage_jwt-1.1.0/tests/
--rw-r--r--   0 mkahan     (503) staff       (20)     2254 2023-10-18 14:13:27.000000 vonage_jwt-1.1.0/tests/test_jwt_generator.py
--rw-r--r--   0 mkahan     (503) staff       (20)      746 2023-10-18 14:13:27.000000 vonage_jwt-1.1.0/tests/test_verify_jwt.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:49:24.351307 vonage_jwt-1.1.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2504 2024-05-19 02:49:24.350369 vonage_jwt-1.1.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     1734 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      831 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-05-19 02:49:24.351379 vonage_jwt-1.1.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:49:24.341584 vonage_jwt-1.1.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:49:24.345345 vonage_jwt-1.1.1/src/vonage_jwt/
+-rw-r--r--   0 mkahan     (503) staff       (20)      212 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/src/vonage_jwt/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      221 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/src/vonage_jwt/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1943 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/src/vonage_jwt/jwt.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      446 2024-05-19 02:49:23.000000 vonage_jwt-1.1.1/src/vonage_jwt/verify_jwt.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-19 02:49:24.349095 vonage_jwt-1.1.1/src/vonage_jwt.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2504 2024-05-19 02:49:24.000000 vonage_jwt-1.1.1/src/vonage_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      332 2024-05-19 02:49:24.000000 vonage_jwt-1.1.1/src/vonage_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-19 02:49:24.000000 vonage_jwt-1.1.1/src/vonage_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       41 2024-05-19 02:49:24.000000 vonage_jwt-1.1.1/src/vonage_jwt.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       11 2024-05-19 02:49:24.000000 vonage_jwt-1.1.1/src/vonage_jwt.egg-info/top_level.txt
```

### Comparing `vonage_jwt-1.1.0/PKG-INFO` & `vonage_jwt-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
-Name: vonage_jwt
-Version: 1.1.0
-Summary: A JWT Generator for Python. Creates JWTs for use with Vonage APIs.
-Author-email: Vonage Developer Relations <devrel@vonage.com>
-Project-URL: Homepage, https://github.com/Vonage/vonage-python-jwt
-Project-URL: Bug Tracker, https://github.com/Vonage/vonage-python-jwt/issues
+Name: vonage-jwt
+Version: 1.1.1
+Summary: Tooling for working with JWTs for Vonage APIs in Python.
+Author-email: Vonage <devrel@vonage.com>
+Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: vonage-utils>=1.1.2
 Requires-Dist: pyjwt[crypto]>=1.6.4
 
 # Vonage JWT Generator for Python
 
-[![PyPI version](https://badge.fury.io/py/vonage-jwt.svg)](https://badge.fury.io/py/vonage-jwt)
-[![Build Status](https://github.com/Vonage/vonage-python-jwt/workflows/Build/badge.svg)](https://github.com/Vonage/vonage-python-jwt/actions)
-[![Python versions supported](https://img.shields.io/pypi/pyversions/vonage-jwt)](https://pypi.python.org/pypi/vonage-jwt)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+This package (`vonage-jwt`) provides functionality to generate a JWT in Python code.
 
-This package provides functionality to generate a JWT in Python code.
+It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk), specifically by the `vonage-http-client` package, to generate JWTs for authentication. Thus, it doesn't require manual installation or configuration unless you're using this package independently of an SDK.
 
-It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk).
+For full API documentation, refer to the [Vonage developer documentation](https://developer.vonage.com).
 
 - [Installation](#installation)
 - [Generating JWTs](#generating-jwts)
 - [Verifying a JWT signature](#verifying-a-jwt-signature)
 
 ## Installation
 
@@ -46,15 +42,15 @@
 This JWT Generator can be used implicitly, just by using the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk) to make JWT-authenticated API calls.
 
 It can also be used as a standalone JWT generator for use with Vonage APIs, like so:
 
 ### Import the `JwtClient` object
 
 ```python
-from vonage_jwt.jwt import JwtClient
+from vonage_jwt import JwtClient
 ```
 
 ### Create a `JwtClient` object
 
 ```python
 jwt_client = JwtClient(application_id, private_key)
 ```
@@ -73,11 +69,11 @@
 ```
 
 ## Verifying a JWT signature
 
 You can use the `verify_jwt.verify_signature` method to verify a JWT signature is valid.
 
 ```python
-from vonage_jwt.verify_jwt import verify_signature
+from vonage_jwt import verify_signature
 
 verify_signature(TOKEN, SIGNATURE_SECRET) # Returns a boolean
 ```
```

### Comparing `vonage_jwt-1.1.0/src/vonage_jwt/jwt.py` & `vonage_jwt-1.1.1/src/vonage_jwt/jwt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import re
 from time import time
-from jwt import encode
-from uuid import uuid4
 from typing import Union
+from uuid import uuid4
+
+from jwt import encode
+
+from .errors import VonageJwtError
 
 
 class JwtClient:
     """Object used to pass in an application ID and private key to generate JWT methods."""
 
     def __init__(self, application_id: str, private_key: str):
         self._application_id = application_id
@@ -18,16 +21,16 @@
 
         if self._application_id is None or self._private_key is None:
             raise VonageJwtError(
                 'Both of "application_id" and "private_key" are required.'
             )
 
     def generate_application_jwt(self, jwt_options: dict = {}):
-        """
-        Generates a JWT for the specified Vonage application.
+        """Generates a JWT for the specified Vonage application.
+
         You can override values for application_id and private_key on the JWTClient object by
         specifying them in the `jwt_options` dict if required.
         """
 
         iat = int(time())
 
         payload = jwt_options
@@ -47,11 +50,7 @@
                 self._private_key = key_file.read()
         elif isinstance(key, str) and '-----BEGIN PRIVATE KEY-----' not in key:
             raise VonageJwtError(
                 "If passing the private key directly as a string, it must be formatted correctly with newlines."
             )
         else:
             self._private_key = key
-
-
-class VonageJwtError(Exception):
-    """An error relating to the Vonage JWT Generator."""
```

### Comparing `vonage_jwt-1.1.0/src/vonage_jwt.egg-info/PKG-INFO` & `vonage_jwt-1.1.1/src/vonage_jwt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: vonage-jwt
-Version: 1.1.0
-Summary: A JWT Generator for Python. Creates JWTs for use with Vonage APIs.
-Author-email: Vonage Developer Relations <devrel@vonage.com>
-Project-URL: Homepage, https://github.com/Vonage/vonage-python-jwt
-Project-URL: Bug Tracker, https://github.com/Vonage/vonage-python-jwt/issues
+Version: 1.1.1
+Summary: Tooling for working with JWTs for Vonage APIs in Python.
+Author-email: Vonage <devrel@vonage.com>
+Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: vonage-utils>=1.1.2
 Requires-Dist: pyjwt[crypto]>=1.6.4
 
 # Vonage JWT Generator for Python
 
-[![PyPI version](https://badge.fury.io/py/vonage-jwt.svg)](https://badge.fury.io/py/vonage-jwt)
-[![Build Status](https://github.com/Vonage/vonage-python-jwt/workflows/Build/badge.svg)](https://github.com/Vonage/vonage-python-jwt/actions)
-[![Python versions supported](https://img.shields.io/pypi/pyversions/vonage-jwt)](https://pypi.python.org/pypi/vonage-jwt)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+This package (`vonage-jwt`) provides functionality to generate a JWT in Python code.
 
-This package provides functionality to generate a JWT in Python code.
+It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk), specifically by the `vonage-http-client` package, to generate JWTs for authentication. Thus, it doesn't require manual installation or configuration unless you're using this package independently of an SDK.
 
-It is used by the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk).
+For full API documentation, refer to the [Vonage developer documentation](https://developer.vonage.com).
 
 - [Installation](#installation)
 - [Generating JWTs](#generating-jwts)
 - [Verifying a JWT signature](#verifying-a-jwt-signature)
 
 ## Installation
 
@@ -46,15 +42,15 @@
 This JWT Generator can be used implicitly, just by using the [Vonage Python SDK](https://github.com/Vonage/vonage-python-sdk) to make JWT-authenticated API calls.
 
 It can also be used as a standalone JWT generator for use with Vonage APIs, like so:
 
 ### Import the `JwtClient` object
 
 ```python
-from vonage_jwt.jwt import JwtClient
+from vonage_jwt import JwtClient
 ```
 
 ### Create a `JwtClient` object
 
 ```python
 jwt_client = JwtClient(application_id, private_key)
 ```
@@ -73,11 +69,11 @@
 ```
 
 ## Verifying a JWT signature
 
 You can use the `verify_jwt.verify_signature` method to verify a JWT signature is valid.
 
 ```python
-from vonage_jwt.verify_jwt import verify_signature
+from vonage_jwt import verify_signature
 
 verify_signature(TOKEN, SIGNATURE_SECRET) # Returns a boolean
 ```
```

