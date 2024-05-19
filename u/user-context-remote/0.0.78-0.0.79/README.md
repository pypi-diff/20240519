# Comparing `tmp/user_context_remote-0.0.78.tar.gz` & `tmp/user_context_remote-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user_context_remote-0.0.78.tar", last modified: Sun May 19 17:49:33 2024, max compression
+gzip compressed data, was "user_context_remote-0.0.79.tar", last modified: Sun May 19 18:38:25 2024, max compression
```

## Comparing `user_context_remote-0.0.78.tar` & `user_context_remote-0.0.79.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.213081 user_context_remote-0.0.78/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.213081 user_context_remote-0.0.78/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-19 17:49:11.000000 user_context_remote-0.0.78/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:49:33.217081 user_context_remote-0.0.78/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 17:49:33.000000 user_context_remote-0.0.78/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:38:25.097244 user_context_remote-0.0.79/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 18:38:25.097244 user_context_remote-0.0.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-19 18:38:08.000000 user_context_remote-0.0.79/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-19 18:38:08.000000 user_context_remote-0.0.79/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:38:25.097244 user_context_remote-0.0.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-19 18:38:08.000000 user_context_remote-0.0.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:38:25.093244 user_context_remote-0.0.79/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:38:25.097244 user_context_remote-0.0.79/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:38:08.000000 user_context_remote-0.0.79/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18991 2024-05-19 18:38:08.000000 user_context_remote-0.0.79/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:38:25.097244 user_context_remote-0.0.79/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-19 18:38:25.000000 user_context_remote-0.0.79/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-19 18:38:25.000000 user_context_remote-0.0.79/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:38:25.000000 user_context_remote-0.0.79/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 18:38:25.000000 user_context_remote-0.0.79/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 18:38:25.000000 user_context_remote-0.0.79/user_context_remote.egg-info/top_level.txt
```

### Comparing `user_context_remote-0.0.78/PKG-INFO` & `user_context_remote-0.0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.78
+Version: 0.0.79
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user_context_remote-0.0.78/README.md` & `user_context_remote-0.0.79/README.md`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.78/pyproject.toml` & `user_context_remote-0.0.79/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.78/setup.py` & `user_context_remote-0.0.79/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.78',  # https://pypi.org/project/user-context-remote/
+    version='0.0.79',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user_context_remote-0.0.78/user_context_remote/src/user_context.py` & `user_context_remote-0.0.79/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user_context_remote-0.0.78/user_context_remote.egg-info/PKG-INFO` & `user_context_remote-0.0.79/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.78
+Version: 0.0.79
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

