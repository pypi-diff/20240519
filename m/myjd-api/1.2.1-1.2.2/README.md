# Comparing `tmp/myjd_api-1.2.1.tar.gz` & `tmp/myjd_api-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myjd_api-1.2.1.tar", last modified: Sun May 19 12:58:36 2024, max compression
+gzip compressed data, was "myjd_api-1.2.2.tar", last modified: Sun May 19 18:37:40 2024, max compression
```

## Comparing `myjd_api-1.2.1.tar` & `myjd_api-1.2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:58:36.352004 myjd_api-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 12:58:28.000000 myjd_api-1.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-19 12:58:36.352004 myjd_api-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-19 12:58:28.000000 myjd_api-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:58:36.348004 myjd_api-1.2.1/myjd_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:58:36.352004 myjd_api-1.2.1/myjd_api/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/myjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/myjdapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-05-19 12:58:28.000000 myjd_api-1.2.1/myjd_api/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:58:36.348004 myjd_api-1.2.1/myjd_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 12:58:36.000000 myjd_api-1.2.1/myjd_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:58:36.352004 myjd_api-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-19 12:58:28.000000 myjd_api-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:37:40.419215 myjd_api-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 18:37:30.000000 myjd_api-1.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-19 18:37:40.419215 myjd_api-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-19 18:37:30.000000 myjd_api-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:37:40.419215 myjd_api-1.2.2/myjd_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:37:40.419215 myjd_api-1.2.2/myjd_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/myjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/myjdapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-05-19 18:37:30.000000 myjd_api-1.2.2/myjd_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:37:40.419215 myjd_api-1.2.2/myjd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 18:37:40.000000 myjd_api-1.2.2/myjd_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:37:40.419215 myjd_api-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-19 18:37:30.000000 myjd_api-1.2.2/setup.py
```

### Comparing `myjd_api-1.2.1/LICENSE.md` & `myjd_api-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/PKG-INFO` & `myjd_api-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myjd_api
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple json interface for the MyJDownloader API to be used with Organizr
 Home-page: https://github.com/rix1337/MyJD-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myjd_api-1.2.1/README.md` & `myjd_api-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/providers/common.py` & `myjd_api-1.2.2/myjd_api/providers/common.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/providers/config.py` & `myjd_api-1.2.2/myjd_api/providers/config.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/providers/files.py` & `myjd_api-1.2.2/myjd_api/providers/files.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/providers/myjd.py` & `myjd_api-1.2.2/myjd_api/providers/myjd.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/providers/myjdapi.py` & `myjd_api-1.2.2/myjd_api/providers/myjdapi.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/providers/requests.py` & `myjd_api-1.2.2/myjd_api/providers/requests.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api/run.py` & `myjd_api-1.2.2/myjd_api/run.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/myjd_api.egg-info/PKG-INFO` & `myjd_api-1.2.2/myjd_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myjd-api
-Version: 1.2.1
+Version: 1.2.2
 Summary: A simple json interface for the MyJDownloader API to be used with Organizr
 Home-page: https://github.com/rix1337/MyJD-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myjd_api-1.2.1/myjd_api.egg-info/SOURCES.txt` & `myjd_api-1.2.2/myjd_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myjd_api-1.2.1/setup.py` & `myjd_api-1.2.2/setup.py`

 * *Files identical despite different names*

