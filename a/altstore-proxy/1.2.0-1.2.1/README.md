# Comparing `tmp/altstore_proxy-1.2.0.tar.gz` & `tmp/altstore_proxy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.2.0.tar", last modified: Sun May 19 09:37:38 2024, max compression
+gzip compressed data, was "altstore_proxy-1.2.1.tar", last modified: Sun May 19 09:48:21 2024, max compression
```

## Comparing `altstore_proxy-1.2.0.tar` & `altstore_proxy-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/providers/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:48:21.108807 altstore_proxy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 09:48:21.108807 altstore_proxy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:48:21.104807 altstore_proxy-1.2.1/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:48:21.104807 altstore_proxy-1.2.1/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:48:21.104807 altstore_proxy-1.2.1/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 09:48:21.000000 altstore_proxy-1.2.1/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:48:21.108807 altstore_proxy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-19 09:48:14.000000 altstore_proxy-1.2.1/setup.py
```

### Comparing `altstore_proxy-1.2.0/LICENSE.md` & `altstore_proxy-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.0/PKG-INFO` & `altstore_proxy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore_proxy
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 License-File: LICENSE.md
 
 #  AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
-A simple proxy for slow AltStore servers.
+A simple proxy for slow AltStore servers
 
 # Setup
 
 `pip install altstore_proxy`
 
 # Run
```

### Comparing `altstore_proxy-1.2.0/README.md` & `altstore_proxy-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
-A simple proxy for slow AltStore servers.
+A simple proxy for slow AltStore servers
 
 # Setup
 
 `pip install altstore_proxy`
 
 # Run
```

### Comparing `altstore_proxy-1.2.0/altstore_proxy/run.py` & `altstore_proxy-1.2.1/altstore_proxy/run.py`

 * *Files identical despite different names*

### Comparing `altstore_proxy-1.2.0/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.2.1/altstore_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altstore-proxy
-Version: 1.2.0
+Version: 1.2.1
 Summary: A simple proxy for slow AltStore servers
 Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 License-File: LICENSE.md
 
 #  AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
-A simple proxy for slow AltStore servers.
+A simple proxy for slow AltStore servers
 
 # Setup
 
 `pip install altstore_proxy`
 
 # Run
```

### Comparing `altstore_proxy-1.2.0/setup.py` & `altstore_proxy-1.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
     long_description = io.open('README.md', encoding='utf-8').read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
-    name="altstore_proxy",
+    name="altstore_proxy",  # case-sensitive replace this string, and this string with a dash in entire repo
     version=get_version(),
     author="rix1337",
     author_email="",
-    description="A simple proxy for slow AltStore servers",
+    description="A simple proxy for slow AltStore servers",  # case-sensitive replace here and in README.md
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/rix1337/AltStore-Proxy",
+    url="https://github.com/rix1337/AltStore-Proxy",  # case-sensitive replace the repo name in entire repo
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=required,
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

