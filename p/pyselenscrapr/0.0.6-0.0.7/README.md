# Comparing `tmp/pyselenscrapr-0.0.6.tar.gz` & `tmp/pyselenscrapr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyselenscrapr-0.0.6.tar", last modified: Sat May 18 22:57:29 2024, max compression
+gzip compressed data, was "pyselenscrapr-0.0.7.tar", last modified: Sun May 19 08:31:01 2024, max compression
```

## Comparing `pyselenscrapr-0.0.6.tar` & `pyselenscrapr-0.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.151703 pyselenscrapr-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.143703 pyselenscrapr-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.147703 pyselenscrapr-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-18 22:57:29.151703 pyselenscrapr-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.147703 pyselenscrapr-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.147703 pyselenscrapr-0.0.6/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/source/pyselenscrapr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.151703 pyselenscrapr-0.0.6/pyselenscrapr/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingBackend.py
--rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingBot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingLogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStep.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStepGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStepLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStepPagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/ValidationError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/pyselenscrapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:57:29.151703 pyselenscrapr-0.0.6/pyselenscrapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-18 22:57:29.000000 pyselenscrapr-0.0.6/pyselenscrapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-18 22:57:29.000000 pyselenscrapr-0.0.6/pyselenscrapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:57:29.000000 pyselenscrapr-0.0.6/pyselenscrapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 22:57:29.000000 pyselenscrapr-0.0.6/pyselenscrapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-18 22:57:29.000000 pyselenscrapr-0.0.6/pyselenscrapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-18 22:57:16.000000 pyselenscrapr-0.0.6/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:57:29.151703 pyselenscrapr-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.059172 pyselenscrapr-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.055171 pyselenscrapr-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.055171 pyselenscrapr-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-19 08:31:01.059172 pyselenscrapr-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.055171 pyselenscrapr-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.055171 pyselenscrapr-0.0.7/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/source/pyselenscrapr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.059172 pyselenscrapr-0.0.7/pyselenscrapr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingBackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13161 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingBot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12269 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingLogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStepGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStepLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStepPagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/ValidationError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/pyselenscrapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:01.059172 pyselenscrapr-0.0.7/pyselenscrapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-19 08:31:01.000000 pyselenscrapr-0.0.7/pyselenscrapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-19 08:31:01.000000 pyselenscrapr-0.0.7/pyselenscrapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:31:01.000000 pyselenscrapr-0.0.7/pyselenscrapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 08:31:01.000000 pyselenscrapr-0.0.7/pyselenscrapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 08:31:01.000000 pyselenscrapr-0.0.7/pyselenscrapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-19 08:30:49.000000 pyselenscrapr-0.0.7/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:31:01.059172 pyselenscrapr-0.0.7/setup.cfg
```

### Comparing `pyselenscrapr-0.0.6/.github/workflows/pypi.yml` & `pyselenscrapr-0.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/LICENSE` & `pyselenscrapr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/PKG-INFO` & `pyselenscrapr-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.6
+Version: 0.0.7
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.6/README.rst` & `pyselenscrapr-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/docs/Makefile` & `pyselenscrapr-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/docs/make.bat` & `pyselenscrapr-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/docs/source/conf.py` & `pyselenscrapr-0.0.7/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 
 project = 'PySelenScrapr'
 copyright = '2024, Thoren Lederer'
 author = 'donnercody'
 
-release = '0.0.6'
-version = '0.0.6'
+release = '0.0.7'
+version = '0.0.7'
 
 # -- General configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
```

### Comparing `pyselenscrapr-0.0.6/docs/source/index.rst` & `pyselenscrapr-0.0.7/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/docs/source/pyselenscrapr.rst` & `pyselenscrapr-0.0.7/docs/source/pyselenscrapr.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/docs/source/usage.rst` & `pyselenscrapr-0.0.7/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr/ScrapingBackend.py` & `pyselenscrapr-0.0.7/pyselenscrapr/ScrapingBackend.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 from abc import ABC
 import requests
 
 # interface IScrapingBackend with the method "saveData" and "errorHandling" and "notify"
 class IScrapingBackend(ABC):
     """
     This is a interface that represents a backend for the scraping process.
@@ -27,27 +28,36 @@
         self._error_route = url + error_route
         self._notify_route = url + notify_route
         self._data_route = url + data_route
 
     def saveData(self, data: dict, key: str = None):
         try:
             d = json.dumps(data)
-            requests.post(self._data_route, data=d, headers={"Content-Type": "application/json", "Accept": "application/json"})
+            ret = requests.post(self._data_route, data=d, headers={"Content-Type": "application/json", "Accept": "application/json"})
+            logging.debug("data return")
+            logging.debug(ret.status_code)
+            logging.debug(ret)
         except Exception as e:
             print(e)
             raise e
 
     def errorHandling(self, error: Exception):
         try:
             d = json.dumps({"error": str(error)})
-            requests.post(self._error_route, data=d, headers={"Content-Type": "application/json", "Accept": "application/json"})
+            ret = requests.post(self._error_route, data=d, headers={"Content-Type": "application/json", "Accept": "application/json"})
+            logging.debug("data return")
+            logging.debug(ret.status_code)
+            logging.debug(ret)
         except Exception as e:
             print(e)
             raise e
 
     def notify(self, message: str):
         try:
             d = json.dumps({"message": str(message)})
-            requests.post(self._notify_route, data=d, headers={"Content-Type": "application/json", "Accept": "application/json"})
+            ret = requests.post(self._notify_route, data=d, headers={"Content-Type": "application/json", "Accept": "application/json"})
+            logging.debug("data return")
+            logging.debug(ret.status_code)
+            logging.debug(ret)
         except Exception as e:
             print(e)
             raise e
```

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr/ScrapingBot.py` & `pyselenscrapr-0.0.7/pyselenscrapr/ScrapingBot.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr/ScrapingLogic.py` & `pyselenscrapr-0.0.7/pyselenscrapr/ScrapingLogic.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStep.py` & `pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStep.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStepLoop.py` & `pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStepLoop.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr/ScrapingStepPagination.py` & `pyselenscrapr-0.0.7/pyselenscrapr/ScrapingStepPagination.py`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr.egg-info/PKG-INFO` & `pyselenscrapr-0.0.7/pyselenscrapr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyselenscrapr
-Version: 0.0.6
+Version: 0.0.7
 Summary: A web scraping library for selenium and beautifulsoup
 Author-email: donnercody <donnercody86@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
```

### Comparing `pyselenscrapr-0.0.6/pyselenscrapr.egg-info/SOURCES.txt` & `pyselenscrapr-0.0.7/pyselenscrapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyselenscrapr-0.0.6/sample.py` & `pyselenscrapr-0.0.7/sample.py`

 * *Files identical despite different names*

