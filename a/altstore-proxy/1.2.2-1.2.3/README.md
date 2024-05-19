# Comparing `tmp/altstore_proxy-1.2.2.tar.gz` & `tmp/altstore_proxy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.2.2.tar", last modified: Sun May 19 11:04:36 2024, max compression
+gzip compressed data, was "altstore_proxy-1.2.3.tar", last modified: Sun May 19 18:42:51 2024, max compression
```

## Comparing `altstore_proxy-1.2.2.tar` & `altstore_proxy-1.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:04:36.049917 altstore_proxy-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 11:04:36.049917 altstore_proxy-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:04:36.049917 altstore_proxy-1.2.2/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:04:36.049917 altstore_proxy-1.2.2/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/altstore_proxy/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/altstore_proxy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:04:36.049917 altstore_proxy-1.2.2/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 11:04:35.000000 altstore_proxy-1.2.2/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:04:36.049917 altstore_proxy-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-19 11:04:30.000000 altstore_proxy-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 18:42:51.000000 altstore_proxy-1.2.3/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:42:51.238589 altstore_proxy-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-19 18:42:46.000000 altstore_proxy-1.2.3/setup.py
```

### Comparing `altstore_proxy-1.2.2/LICENSE.md` & `altstore_proxy-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.2/PKG-INFO` & `altstore_proxy-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.2.2/README.md` & `altstore_proxy-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.2/altstore_proxy/run.py` & `altstore_proxy-1.2.3/altstore_proxy/run.py`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.2/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.2.3/altstore_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `altstore_proxy-1.2.2/setup.py` & `altstore_proxy-1.2.3/setup.py`

 * *Files identical despite different names*

