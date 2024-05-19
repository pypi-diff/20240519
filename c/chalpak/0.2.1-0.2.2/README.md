# Comparing `tmp/chalpak-0.2.1.tar.gz` & `tmp/chalpak-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chalpak-0.2.1.tar", last modified: Sun May 19 16:57:38 2024, max compression
+gzip compressed data, was "chalpak-0.2.2.tar", last modified: Sun May 19 17:06:16 2024, max compression
```

## Comparing `chalpak-0.2.1.tar` & `chalpak-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:57:38.458103 chalpak-0.2.1/
--rw-rw-rw-   0        0        0     1826 2024-05-19 16:57:38.457091 chalpak-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2024-05-19 16:51:22.000000 chalpak-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 16:57:38.424417 chalpak-0.2.1/chalpak/
--rw-rw-rw-   0        0        0       63 2024-05-19 16:04:44.000000 chalpak-0.2.1/chalpak/__init__.py
--rw-rw-rw-   0        0        0     3464 2024-05-19 16:06:18.000000 chalpak-0.2.1/chalpak/app.py
--rw-rw-rw-   0        0        0     1419 2024-05-16 14:53:39.000000 chalpak-0.2.1/chalpak/exceptions.py
--rw-rw-rw-   0        0        0     1534 2024-05-19 16:01:52.000000 chalpak-0.2.1/chalpak/response.py
--rw-rw-rw-   0        0        0     1745 2024-05-19 16:02:54.000000 chalpak-0.2.1/chalpak/routes.py
--rw-rw-rw-   0        0        0      996 2024-05-16 14:56:23.000000 chalpak-0.2.1/chalpak/schema.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:57:38.454092 chalpak-0.2.1/chalpak.egg-info/
--rw-rw-rw-   0        0        0     1826 2024-05-19 16:57:38.000000 chalpak-0.2.1/chalpak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-19 16:57:38.000000 chalpak-0.2.1/chalpak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:57:38.000000 chalpak-0.2.1/chalpak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-05-19 16:57:38.000000 chalpak-0.2.1/chalpak.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 16:57:38.000000 chalpak-0.2.1/chalpak.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 16:57:38.458103 chalpak-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     4023 2024-05-19 16:57:23.000000 chalpak-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:06:16.715931 chalpak-0.2.2/
+-rw-rw-rw-   0        0        0     1758 2024-05-19 17:06:16.714948 chalpak-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2024-05-19 17:02:15.000000 chalpak-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:06:16.665125 chalpak-0.2.2/chalpak/
+-rw-rw-rw-   0        0        0       63 2024-05-19 16:04:44.000000 chalpak-0.2.2/chalpak/__init__.py
+-rw-rw-rw-   0        0        0     3466 2024-05-19 17:05:55.000000 chalpak-0.2.2/chalpak/app.py
+-rw-rw-rw-   0        0        0     1419 2024-05-16 14:53:39.000000 chalpak-0.2.2/chalpak/exceptions.py
+-rw-rw-rw-   0        0        0     1534 2024-05-19 16:01:52.000000 chalpak-0.2.2/chalpak/response.py
+-rw-rw-rw-   0        0        0     1747 2024-05-19 17:06:08.000000 chalpak-0.2.2/chalpak/routes.py
+-rw-rw-rw-   0        0        0      996 2024-05-16 14:56:23.000000 chalpak-0.2.2/chalpak/schema.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:06:16.679931 chalpak-0.2.2/chalpak.egg-info/
+-rw-rw-rw-   0        0        0     1758 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 17:06:16.000000 chalpak-0.2.2/chalpak.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:06:16.717281 chalpak-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     4023 2024-05-19 17:02:03.000000 chalpak-0.2.2/setup.py
```

### Comparing `chalpak-0.2.1/PKG-INFO` & `chalpak-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalpak
-Version: 0.2.1
+Version: 0.2.2
 Summary: Chalpak - mini web framework like fastAPi, flask
 Home-page: https://github.com/me/myproject
 Author: Mehmonov Husniddin
 Author-email: mehmonov.husniddin1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -18,15 +18,14 @@
 
 # Chalpak Web Framework
 
 Chalpak is a simple and easy-to-use web framework that helps you create fast and efficient web applications.
 [![Chalpak version](https://img.shields.io/pypi/v/chalpak.svg)](https://pypi.org/project/chalpak)
 [![PyPI version](https://badge.fury.io/py/chalpak.svg)](https://badge.fury.io/py/chalpak)
 [![Documentation Status](https://readthedocs.org/projects/chalpak/badge/?version=latest)](https://chalpak.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.com/username/chalpak.svg?branch=master)](https://travis-ci.com/username/chalpak)
 
 
 
 **Install Chalpak**
 
 ```bash
 pip install chalpak
@@ -63,7 +62,13 @@
 @app.get("/html/{name}")
 async def html(request, name):
     return render("index.html", request, {"name": name})
 
 app.run()
 ```
 
+## Run
+
+```bash
+jurigged -v script.py
+```
+
```

### Comparing `chalpak-0.2.1/README.md` & `chalpak-0.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Chalpak Web Framework
 
 Chalpak is a simple and easy-to-use web framework that helps you create fast and efficient web applications.
 [![Chalpak version](https://img.shields.io/pypi/v/chalpak.svg)](https://pypi.org/project/chalpak)
 [![PyPI version](https://badge.fury.io/py/chalpak.svg)](https://badge.fury.io/py/chalpak)
 [![Documentation Status](https://readthedocs.org/projects/chalpak/badge/?version=latest)](https://chalpak.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.com/username/chalpak.svg?branch=master)](https://travis-ci.com/username/chalpak)
 
 
 
 **Install Chalpak**
 
 ```bash
 pip install chalpak
@@ -45,7 +44,13 @@
 @app.get("/html/{name}")
 async def html(request, name):
     return render("index.html", request, {"name": name})
 
 app.run()
 ```
 
+## Run
+
+```bash
+jurigged -v script.py
+```
+
```

### Comparing `chalpak-0.2.1/chalpak/app.py` & `chalpak-0.2.2/chalpak/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from aiohttp import web
 from aiohttp.web import Request
 from typing import Callable, List, Optional
 import logging
 import jinja2
 import aiohttp_jinja2
-from routes import Route
-from response import HTMLResponse, Response
+from .routes import Route
+from .response import HTMLResponse, Response
 
 logging.basicConfig(level=logging.INFO)
 
 class ChalpakApp:
     def __init__(self, host: str = "127.0.0.1", port: int = 6767, templates: Optional[str] = None, static_folder: Optional[str] = None) -> None:
         self.host = host
         self.port = port
```

### Comparing `chalpak-0.2.1/chalpak/exceptions.py` & `chalpak-0.2.2/chalpak/exceptions.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.1/chalpak/response.py` & `chalpak-0.2.2/chalpak/response.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.1/chalpak/routes.py` & `chalpak-0.2.2/chalpak/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import logging
 from json import JSONDecodeError as JSONDecodeException
 from typing import Callable
 
 from aiohttp.web_request import Request
 
-from schema import SchemaModel  
-from exceptions import APIError, ClassBaseError 
+from .schema import SchemaModel  
+from .exceptions import APIError, ClassBaseError 
 
 logging.basicConfig(level=logging.DEBUG,format='%(asctime)s - %(levelname)s - %(message)s - %(pathname)s:%(lineno)d')
 
 
 class Route:
     
     def __init__(self, path: str, handler: Callable, method: str, name: str, **kwargs):
```

### Comparing `chalpak-0.2.1/chalpak/schema.py` & `chalpak-0.2.2/chalpak/schema.py`

 * *Files identical despite different names*

### Comparing `chalpak-0.2.1/chalpak.egg-info/PKG-INFO` & `chalpak-0.2.2/chalpak.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chalpak
-Version: 0.2.1
+Version: 0.2.2
 Summary: Chalpak - mini web framework like fastAPi, flask
 Home-page: https://github.com/me/myproject
 Author: Mehmonov Husniddin
 Author-email: mehmonov.husniddin1@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -18,15 +18,14 @@
 
 # Chalpak Web Framework
 
 Chalpak is a simple and easy-to-use web framework that helps you create fast and efficient web applications.
 [![Chalpak version](https://img.shields.io/pypi/v/chalpak.svg)](https://pypi.org/project/chalpak)
 [![PyPI version](https://badge.fury.io/py/chalpak.svg)](https://badge.fury.io/py/chalpak)
 [![Documentation Status](https://readthedocs.org/projects/chalpak/badge/?version=latest)](https://chalpak.readthedocs.io/en/latest/?badge=latest)
-[![Build Status](https://travis-ci.com/username/chalpak.svg?branch=master)](https://travis-ci.com/username/chalpak)
 
 
 
 **Install Chalpak**
 
 ```bash
 pip install chalpak
@@ -63,7 +62,13 @@
 @app.get("/html/{name}")
 async def html(request, name):
     return render("index.html", request, {"name": name})
 
 app.run()
 ```
 
+## Run
+
+```bash
+jurigged -v script.py
+```
+
```

### Comparing `chalpak-0.2.1/setup.py` & `chalpak-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'chalpak'
 DESCRIPTION = 'Chalpak - mini web framework like fastAPi, flask'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'mehmonov.husniddin1@gmail.com'
 AUTHOR = 'Mehmonov Husniddin'
 REQUIRES_PYTHON = '>=3.11.9'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'aiohttp==3.9.5',
     'aiohttp-jinja2==1.6',
     'watchdog==4.0.0',
     'jurigged==0.5.7',
```

