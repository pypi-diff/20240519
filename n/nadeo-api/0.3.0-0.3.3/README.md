# Comparing `tmp/nadeo_api-0.3.0.tar.gz` & `tmp/nadeo_api-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadeo_api-0.3.0.tar", last modified: Fri May 17 19:36:51 2024, max compression
+gzip compressed data, was "nadeo_api-0.3.3.tar", last modified: Sun May 19 19:35:42 2024, max compression
```

## Comparing `nadeo_api-0.3.0.tar` & `nadeo_api-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:51.416930 nadeo_api-0.3.0/
--rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3506 2024-05-17 19:36:51.415929 nadeo_api-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1633 2024-05-17 18:39:02.000000 nadeo_api-0.3.0/README.md
--rw-rw-rw-   0        0        0      671 2024-05-17 19:36:19.000000 nadeo_api-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 19:36:51.416930 nadeo_api-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:51.371624 nadeo_api-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:51.400965 nadeo_api-0.3.0/src/nadeo_api/
--rw-rw-rw-   0        0        0     1374 2024-05-17 19:36:22.000000 nadeo_api-0.3.0/src/nadeo_api/__init__.py
--rw-rw-rw-   0        0        0    10109 2024-05-16 23:12:13.000000 nadeo_api-0.3.0/src/nadeo_api/auth.py
--rw-rw-rw-   0        0        0     2046 2024-05-16 23:18:12.000000 nadeo_api-0.3.0/src/nadeo_api/core.py
--rw-rw-rw-   0        0        0     2848 2024-05-16 23:18:18.000000 nadeo_api-0.3.0/src/nadeo_api/live.py
--rw-rw-rw-   0        0        0     1327 2024-05-17 19:36:32.000000 nadeo_api-0.3.0/src/nadeo_api/meet.py
--rw-rw-rw-   0        0        0     2881 2024-05-17 19:15:57.000000 nadeo_api-0.3.0/src/nadeo_api/oauth.py
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:51.415929 nadeo_api-0.3.0/src/nadeo_api.egg-info/
--rw-rw-rw-   0        0        0     3506 2024-05-17 19:36:51.000000 nadeo_api-0.3.0/src/nadeo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-17 19:36:51.000000 nadeo_api-0.3.0/src/nadeo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:36:51.000000 nadeo_api-0.3.0/src/nadeo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 19:36:51.000000 nadeo_api-0.3.0/src/nadeo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 19:36:51.000000 nadeo_api-0.3.0/src/nadeo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 19:36:51.414478 nadeo_api-0.3.0/tests/
--rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.3.0/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:35:42.107756 nadeo_api-0.3.3/
+-rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     3606 2024-05-19 19:35:42.106755 nadeo_api-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1628 2024-05-18 06:39:15.000000 nadeo_api-0.3.3/README.md
+-rw-rw-rw-   0        0        0      777 2024-05-19 19:33:23.000000 nadeo_api-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 19:35:42.107756 nadeo_api-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 19:35:42.025749 nadeo_api-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 19:35:42.083547 nadeo_api-0.3.3/src/nadeo_api/
+-rw-rw-rw-   0        0        0     1442 2024-05-19 19:34:06.000000 nadeo_api-0.3.3/src/nadeo_api/__init__.py
+-rw-rw-rw-   0        0        0    10109 2024-05-16 23:12:13.000000 nadeo_api-0.3.3/src/nadeo_api/auth.py
+-rw-rw-rw-   0        0        0     2053 2024-05-19 19:33:14.000000 nadeo_api-0.3.3/src/nadeo_api/core.py
+-rw-rw-rw-   0        0        0     2855 2024-05-18 07:08:54.000000 nadeo_api-0.3.3/src/nadeo_api/live.py
+-rw-rw-rw-   0        0        0     1334 2024-05-18 07:08:43.000000 nadeo_api-0.3.3/src/nadeo_api/meet.py
+-rw-rw-rw-   0        0        0     2902 2024-05-18 07:08:29.000000 nadeo_api-0.3.3/src/nadeo_api/oauth.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:35:42.105754 nadeo_api-0.3.3/src/nadeo_api.egg-info/
+-rw-rw-rw-   0        0        0     3606 2024-05-19 19:35:42.000000 nadeo_api-0.3.3/src/nadeo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-19 19:35:42.000000 nadeo_api-0.3.3/src/nadeo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 19:35:42.000000 nadeo_api-0.3.3/src/nadeo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 19:35:42.000000 nadeo_api-0.3.3/src/nadeo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 19:35:42.000000 nadeo_api-0.3.3/src/nadeo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 19:35:42.104749 nadeo_api-0.3.3/tests/
+-rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.3.3/tests/test_auth.py
```

### Comparing `nadeo_api-0.3.0/LICENSE.txt` & `nadeo_api-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.0/PKG-INFO` & `nadeo_api-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.3.0
+Version: 0.3.3
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,26 +23,28 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/ezio416/py-nadeo-api
 Project-URL: Bug Tracker, https://github.com/ezio416/py-nadeo-api/issues
+Project-URL: Documentation, https://nadeo-api.readthedocs.io/en/latest/
+Keywords: nadeo,api,trackmania
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
 
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
-<!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
+[![docs](https://readthedocs.org/projects/nadeo-api/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/)
 [![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
 
 The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
 The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
```

### Comparing `nadeo_api-0.3.0/README.md` & `nadeo_api-0.3.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
-<!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
+[![docs](https://readthedocs.org/projects/nadeo-api/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/)
 [![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
 
 The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
 The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
```

### Comparing `nadeo_api-0.3.0/pyproject.toml` & `nadeo_api-0.3.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nadeo-api"
-version = "0.3.0"
+version = "0.3.3"
 authors = [
   { name="Ezio416", email="e@e416.dev" },
 ]
 description = "Access Nadeo's web services API and the public Trackmania API"
+keywords = ["nadeo", "api", "trackmania"]
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.12"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
@@ -20,7 +21,8 @@
 dependencies = [
   "requests >= 2.31.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ezio416/py-nadeo-api"
 "Bug Tracker" = "https://github.com/ezio416/py-nadeo-api/issues"
+"Documentation" = "https://nadeo-api.readthedocs.io/en/latest/"
```

### Comparing `nadeo_api-0.3.0/src/nadeo_api/__init__.py` & `nadeo_api-0.3.3/src/nadeo_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-07
-| Modified: 2024-05-17
+| Modified: 2024-05-19
 
 - A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
+- This is the main module - most of what you need is in sub-modules.
 '''
 
 import base64
 import re
 
 
-__version__: tuple = 0, 3, 0
+__version__: tuple = 0, 3, 3
 
 
 def account_id_from_login(account_login: str) -> str:
     '''
-    - converts an base64-encoded login to an Ubisoft account ID (UUID)
+    - converts a base64-encoded login to an Ubisoft account ID (UUID)
 
     Parameters
     ----------
     account_login: str
         - base64-encoded login
 
     Returns
```

### Comparing `nadeo_api-0.3.0/src/nadeo_api/auth.py` & `nadeo_api-0.3.3/src/nadeo_api/auth.py`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.3.0/src/nadeo_api/core.py` & `nadeo_api-0.3.3/src/nadeo_api/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-14
-| Modified: 2024-05-16
+| Modified: 2024-05-18
 
 - Functions for interacting with the web services Core API
 '''
 
-import auth
+from . import auth
 
 
 def get(token: auth.Token, endpoint: str, params: dict = {}) -> dict:
     '''
     - sends a GET request to the Core API
 
     Parameters
```

### Comparing `nadeo_api-0.3.0/src/nadeo_api/live.py` & `nadeo_api-0.3.3/src/nadeo_api/live.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-15
-| Modified: 2024-05-16
+| Modified: 2024-05-18
 
 - Functions for interacting with the web services Live API
 '''
 
-import auth
+from . import auth
 
 
 def get(token: auth.Token, endpoint: str, params: dict = {}) -> dict:
     '''
     - sends a GET request to the Live API
 
     Parameters
```

### Comparing `nadeo_api-0.3.0/src/nadeo_api/meet.py` & `nadeo_api-0.3.3/src/nadeo_api/meet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-15
-| Modified: 2024-05-16
+| Modified: 2024-05-18
 
 - Functions for interacting with the web services Meet API
 '''
 
-import auth
+from . import auth
 
 
 def get(token: auth.Token, endpoint: str, params: dict = {}) -> dict:
     '''
     - sends a GET request to the Meet API
 
     Parameters
```

### Comparing `nadeo_api-0.3.0/src/nadeo_api/oauth.py` & `nadeo_api-0.3.3/src/nadeo_api/oauth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-15
-| Modified: 2024-05-17
+| Modified: 2024-05-18
 
 - Functions for interacting with the public Trackmania API
 '''
 
 from typing import Iterable
 
-import auth
+from . import auth
 
 
 def get(token: auth.Token, endpoint: str, params: dict = {}) -> dict:
     '''
     - sends a GET request to the OAuth2 API
 
     Parameters
@@ -42,15 +42,15 @@
 def account_names_from_ids(token: auth.Token, account_ids: str | Iterable[str]) -> dict:
     '''
     - gets Ubisoft account names given account IDs (UUID)
     - https://webservices.openplanet.dev/oauth/reference/accounts/id-to-name
 
     Parameters
     ----------
-    token: str
+    token: auth.Token
         - authentication token gotten from `auth.get_token`
 
     account_ids: str | Iterable[str]
         - account ID
         - may be an iterable of account IDs (max 50)
         - raises a `ValueError` if you try to request more than 50 names
         - if an ID is not found, it will be omitted from the results
@@ -74,15 +74,15 @@
 def account_ids_from_names(token: auth.Token, account_names: str | Iterable[str]) -> dict:
     '''
     - gets Ubisoft account IDs (UUID) given account names
     - https://webservices.openplanet.dev/oauth/reference/accounts/name-to-id
 
     Parameters
     ----------
-    token: str
+    token: auth.Token
         - authentication token gotten from `auth.get_token`
 
     account_name: str | Iterable[str]
         - account name
         - may be an iterable of account names
         - if a name is not found, it will be omitted from the results
```

### Comparing `nadeo_api-0.3.0/src/nadeo_api.egg-info/PKG-INFO` & `nadeo_api-0.3.3/src/nadeo_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.3.0
+Version: 0.3.3
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,26 +23,28 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/ezio416/py-nadeo-api
 Project-URL: Bug Tracker, https://github.com/ezio416/py-nadeo-api/issues
+Project-URL: Documentation, https://nadeo-api.readthedocs.io/en/latest/
+Keywords: nadeo,api,trackmania
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests>=2.31.0
 
 # nadeo-api
 
 <!-- [![tests](https://github.com/ezio416/py416/actions/workflows/tests.yml/badge.svg)](https://github.com/ezio416/py-nadeo-api/actions) -->
-<!-- [![docs](https://readthedocs.org/projects/py416/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/) -->
+[![docs](https://readthedocs.org/projects/nadeo-api/badge/?version=latest)](https://nadeo-api.readthedocs.io/en/latest/)
 [![PyPI](https://badge.fury.io/py/nadeo-api.svg)](https://pypi.org/project/nadeo-api/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
 
 The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
 The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
```

