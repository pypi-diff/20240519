# Comparing `tmp/wol_api-1.0.0.tar.gz` & `tmp/wol_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wol_api-1.0.0.tar", last modified: Sun May 19 12:43:52 2024, max compression
+gzip compressed data, was "wol_api-1.0.1.tar", last modified: Sun May 19 18:39:34 2024, max compression
```

## Comparing `wol_api-1.0.0.tar` & `wol_api-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 12:43:45.000000 wol_api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 12:43:45.000000 wol_api-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 12:43:52.323850 wol_api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 12:43:45.000000 wol_api-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:43:52.323850 wol_api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-19 12:43:45.000000 wol_api-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/wol_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/wol_api/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/wol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:39:34.500320 wol_api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 18:39:29.000000 wol_api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 18:39:29.000000 wol_api-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 18:39:34.500320 wol_api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 18:39:29.000000 wol_api-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:39:34.500320 wol_api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-19 18:39:29.000000 wol_api-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:39:34.496320 wol_api-1.0.1/wol_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:39:29.000000 wol_api-1.0.1/wol_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:39:34.500320 wol_api-1.0.1/wol_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:39:29.000000 wol_api-1.0.1/wol_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 18:39:29.000000 wol_api-1.0.1/wol_api/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-19 18:39:29.000000 wol_api-1.0.1/wol_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-19 18:39:29.000000 wol_api-1.0.1/wol_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:39:34.500320 wol_api-1.0.1/wol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 18:39:34.000000 wol_api-1.0.1/wol_api.egg-info/top_level.txt
```

### Comparing `wol_api-1.0.0/LICENSE` & `wol_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.0/LICENSE.md` & `wol_api-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.0/PKG-INFO` & `wol_api-1.0.1/wol_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wol_api
-Version: 1.0.0
+Name: wol-api
+Version: 1.0.1
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wol_api-1.0.0/README.md` & `wol_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.0/setup.py` & `wol_api-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.0/wol_api/run.py` & `wol_api-1.0.1/wol_api/run.py`

 * *Files identical despite different names*

### Comparing `wol_api-1.0.0/wol_api.egg-info/PKG-INFO` & `wol_api-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wol-api
-Version: 1.0.0
+Name: wol_api
+Version: 1.0.1
 Summary: Full template for python web projects with Docker, Github Actions, PyPI, and more.
 Home-page: https://github.com/rix1337/WakeOnLAN-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

