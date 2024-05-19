# Comparing `tmp/nice_gui_utils-0.3.1.dev8.tar.gz` & `tmp/nice_gui_utils-0.3.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice_gui_utils-0.3.1.dev8.tar", last modified: Mon Mar 18 20:49:14 2024, max compression
+gzip compressed data, was "nice_gui_utils-0.3.1.dev9.tar", last modified: Sun Mar 31 20:29:27 2024, max compression
```

## Comparing `nice_gui_utils-0.3.1.dev8.tar` & `nice_gui_utils-0.3.1.dev9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      903 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      364 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      852 2024-03-17 21:14:33.000000 nice_gui_utils-0.3.1.dev8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.170026 nice_gui_utils-0.3.1.dev8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.170026 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/keycloak_js/
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/keycloak_js/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/keycloak_js/keycloak.js
--rw-rw-rw-   0 root         (0) root         (0)     2742 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/keycloak_js/keycloak.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/router/
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/router/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2361 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/router/router.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/router/router_frame.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)      903 2024-03-18 20:49:14.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2024-03-18 20:49:14.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 20:49:14.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-18 20:49:14.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-18 20:49:14.000000 nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:49:14.174026 nice_gui_utils-0.3.1.dev8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1883 2024-02-04 19:17:28.000000 nice_gui_utils-0.3.1.dev8/tests/test_login.py
--rw-rw-rw-   0 root         (0) root         (0)     2070 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev8/tests/test_single_page.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.941980 nice_gui_utils-0.3.1.dev9/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      903 2024-03-31 20:29:27.937980 nice_gui_utils-0.3.1.dev9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      364 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-03-31 20:12:25.000000 nice_gui_utils-0.3.1.dev9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 20:29:27.941980 nice_gui_utils-0.3.1.dev9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.933980 nice_gui_utils-0.3.1.dev9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.937980 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.937980 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/keycloak_js/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/keycloak_js/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/keycloak_js/keycloak.js
+-rw-rw-rw-   0 root         (0) root         (0)     2742 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/keycloak_js/keycloak.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.937980 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/router/
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/router/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2361 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/router/router.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/router/router_frame.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.937980 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      903 2024-03-31 20:29:27.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2024-03-31 20:29:27.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 20:29:27.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-03-31 20:29:27.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-03-31 20:29:27.000000 nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:29:27.937980 nice_gui_utils-0.3.1.dev9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2024-02-04 19:17:28.000000 nice_gui_utils-0.3.1.dev9/tests/test_login.py
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2024-01-23 14:06:44.000000 nice_gui_utils-0.3.1.dev9/tests/test_single_page.py
```

### Comparing `nice_gui_utils-0.3.1.dev8/LICENSE` & `nice_gui_utils-0.3.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/PKG-INFO` & `nice_gui_utils-0.3.1.dev9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice_gui_utils
-Version: 0.3.1.dev8
+Version: 0.3.1.dev9
 Summary: Utils to use with NiceGUI.
 Author: Harter Kern
 Project-URL: Homepage, https://gitlab.com/harter-kern-public/nice-gui-utils
 Project-URL: Bug Tracker, https://gitlab.com/harter-kern-public/nice-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nice_gui_utils-0.3.1.dev8/pyproject.toml` & `nice_gui_utils-0.3.1.dev9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nice_gui_utils"
-version = "0.3.1dev8"
+version = "0.3.1dev9"
 dynamic = ["dependencies"]
 authors = [
     { name = "Harter Kern" },
 ]
 description = "Utils to use with NiceGUI."
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/keycloak_js/keycloak.js` & `nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/keycloak_js/keycloak.js`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/keycloak_js/keycloak.py` & `nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/keycloak_js/keycloak.py`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/router/router.py` & `nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/router/router.py`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/src/nice_gui_utils/router/router_frame.js` & `nice_gui_utils-0.3.1.dev9/src/nice_gui_utils/router/router_frame.js`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/PKG-INFO` & `nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice_gui_utils
-Version: 0.3.1.dev8
+Version: 0.3.1.dev9
 Summary: Utils to use with NiceGUI.
 Author: Harter Kern
 Project-URL: Homepage, https://gitlab.com/harter-kern-public/nice-gui-utils
 Project-URL: Bug Tracker, https://gitlab.com/harter-kern-public/nice-gui-utils/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nice_gui_utils-0.3.1.dev8/src/nice_gui_utils.egg-info/SOURCES.txt` & `nice_gui_utils-0.3.1.dev9/src/nice_gui_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/tests/test_login.py` & `nice_gui_utils-0.3.1.dev9/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `nice_gui_utils-0.3.1.dev8/tests/test_single_page.py` & `nice_gui_utils-0.3.1.dev9/tests/test_single_page.py`

 * *Files identical despite different names*

