# Comparing `tmp/trengine-1.3.tar.gz` & `tmp/trengine-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trengine-1.3.tar", last modified: Sat May 18 17:18:51 2024, max compression
+gzip compressed data, was "trengine-1.4.tar", last modified: Sun May 19 16:01:10 2024, max compression
```

## Comparing `trengine-1.3.tar` & `trengine-1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-18 17:18:51.870627 trengine-1.3/
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1060 2024-05-18 16:59:11.000000 trengine-1.3/LICENSE
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1865 2024-05-18 17:18:51.869627 trengine-1.3/PKG-INFO
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1283 2024-05-18 16:59:11.000000 trengine-1.3/README.md
--rw-r--r--   0 zaid      (1000) zaid      (1000)      551 2024-05-18 17:15:32.000000 trengine-1.3/pyproject.toml
--rw-r--r--   0 zaid      (1000) zaid      (1000)       38 2024-05-18 17:18:51.870627 trengine-1.3/setup.cfg
-drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-18 17:18:51.865627 trengine-1.3/trengine/
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1231 2024-05-18 16:59:11.000000 trengine-1.3/trengine/__init__.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)     3092 2024-05-18 16:59:11.000000 trengine-1.3/trengine/ajax.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)       40 2024-05-18 16:59:11.000000 trengine-1.3/trengine/exceptions.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1375 2024-05-18 16:59:11.000000 trengine-1.3/trengine/google.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1722 2024-05-18 16:59:11.000000 trengine-1.3/trengine/hozory.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)     2862 2024-05-18 17:15:12.000000 trengine-1.3/trengine/ocr.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)      930 2024-05-18 16:59:11.000000 trengine-1.3/trengine/tdict.py
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1712 2024-05-18 16:59:11.000000 trengine-1.3/trengine/types.py
-drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-18 17:18:51.868627 trengine-1.3/trengine.egg-info/
--rw-r--r--   0 zaid      (1000) zaid      (1000)     1865 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/PKG-INFO
--rw-r--r--   0 zaid      (1000) zaid      (1000)      342 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/SOURCES.txt
--rw-r--r--   0 zaid      (1000) zaid      (1000)        1 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/dependency_links.txt
--rw-r--r--   0 zaid      (1000) zaid      (1000)       25 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/requires.txt
--rw-r--r--   0 zaid      (1000) zaid      (1000)        9 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/top_level.txt
+drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-19 16:01:10.635479 trengine-1.4/
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1060 2024-05-19 15:52:32.000000 trengine-1.4/LICENSE
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1865 2024-05-19 16:01:10.634479 trengine-1.4/PKG-INFO
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1283 2024-05-19 15:52:32.000000 trengine-1.4/README.md
+-rw-r--r--   0 zaid      (1000) zaid      (1000)      551 2024-05-19 15:59:52.000000 trengine-1.4/pyproject.toml
+-rw-r--r--   0 zaid      (1000) zaid      (1000)       38 2024-05-19 16:01:10.635479 trengine-1.4/setup.cfg
+drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-19 16:01:10.627479 trengine-1.4/trengine/
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1231 2024-05-19 15:52:32.000000 trengine-1.4/trengine/__init__.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     3092 2024-05-19 15:52:32.000000 trengine-1.4/trengine/ajax.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)       40 2024-05-19 15:52:32.000000 trengine-1.4/trengine/exceptions.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1375 2024-05-19 15:52:32.000000 trengine-1.4/trengine/google.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1722 2024-05-19 15:52:32.000000 trengine-1.4/trengine/hozory.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     2841 2024-05-19 15:53:33.000000 trengine-1.4/trengine/ocr.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)      930 2024-05-19 15:52:32.000000 trengine-1.4/trengine/tdict.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1712 2024-05-19 15:52:32.000000 trengine-1.4/trengine/types.py
+drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-19 16:01:10.633478 trengine-1.4/trengine.egg-info/
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1865 2024-05-19 16:01:10.000000 trengine-1.4/trengine.egg-info/PKG-INFO
+-rw-r--r--   0 zaid      (1000) zaid      (1000)      342 2024-05-19 16:01:10.000000 trengine-1.4/trengine.egg-info/SOURCES.txt
+-rw-r--r--   0 zaid      (1000) zaid      (1000)        1 2024-05-19 16:01:10.000000 trengine-1.4/trengine.egg-info/dependency_links.txt
+-rw-r--r--   0 zaid      (1000) zaid      (1000)       25 2024-05-19 16:01:10.000000 trengine-1.4/trengine.egg-info/requires.txt
+-rw-r--r--   0 zaid      (1000) zaid      (1000)        9 2024-05-19 16:01:10.000000 trengine-1.4/trengine.egg-info/top_level.txt
```

### Comparing `trengine-1.3/LICENSE` & `trengine-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trengine-1.3/PKG-INFO` & `trengine-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trengine
-Version: 1.3
+Version: 1.4
 Summary: TREngine is python library based on 4 translators engines
 Author-email: ZAID <y8838@hotmail.com>
 Project-URL: Homepage, https://github.com/zaid5o5/trengine
 Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trengine-1.3/README.md` & `trengine-1.4/README.md`

 * *Files identical despite different names*

### Comparing `trengine-1.3/pyproject.toml` & `trengine-1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "trengine"
-version = "1.3"
+version = "1.4"
 authors = [
   { name="ZAID", email="y8838@hotmail.com" },
 ]
 description = "TREngine is python library based on 4 translators engines"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `trengine-1.3/trengine/__init__.py` & `trengine-1.4/trengine/__init__.py`

 * *Files identical despite different names*

### Comparing `trengine-1.3/trengine/ajax.py` & `trengine-1.4/trengine/ajax.py`

 * *Files identical despite different names*

### Comparing `trengine-1.3/trengine/google.py` & `trengine-1.4/trengine/google.py`

 * *Files identical despite different names*

### Comparing `trengine-1.3/trengine/hozory.py` & `trengine-1.4/trengine/hozory.py`

 * *Files identical despite different names*

### Comparing `trengine-1.3/trengine/ocr.py` & `trengine-1.4/trengine/ocr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 import aiohttp
 import json
-import os
 
 
 from .exceptions import ApiException
 from typing import Union
 
 
 class OCR:
@@ -68,15 +67,15 @@
                 "IsCreateSearchablePDF": False,
                 "isSearchablePdfHideTextLayer": True,
                 "FileType": ".AUTO",
             }
             data = aiohttp.formdata.FormData(quote_fields=False)
             for k, v in payload.items():
                 data.add_field(k, str(v))
-            data.add_field("file", b, filename=os.path.basename(path))
+            data.add_field("file", b, filename="photo.png")
             async with session.post(
                 "https://api8.ocr.space/parse/image", data=data
             ) as response:
                 try:
                     result = await response.json()
                 except Exception as e:
                     raise BaseException(str(e))
```

### Comparing `trengine-1.3/trengine/tdict.py` & `trengine-1.4/trengine/tdict.py`

 * *Files identical despite different names*

### Comparing `trengine-1.3/trengine/types.py` & `trengine-1.4/trengine/types.py`

 * *Files identical despite different names*

### Comparing `trengine-1.3/trengine.egg-info/PKG-INFO` & `trengine-1.4/trengine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trengine
-Version: 1.3
+Version: 1.4
 Summary: TREngine is python library based on 4 translators engines
 Author-email: ZAID <y8838@hotmail.com>
 Project-URL: Homepage, https://github.com/zaid5o5/trengine
 Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

