# Comparing `tmp/func2stream-0.0.1.dev2405190653.tar.gz` & `tmp/func2stream-0.0.1.dev2405191627.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2stream-0.0.1.dev2405190653.tar", last modified: Sun May 19 06:53:02 2024, max compression
+gzip compressed data, was "func2stream-0.0.1.dev2405191627.tar", last modified: Sun May 19 16:27:06 2024, max compression
```

## Comparing `func2stream-0.0.1.dev2405190653.tar` & `func2stream-0.0.1.dev2405191627.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:53:02.776051 func2stream-0.0.1.dev2405190653/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-19 06:52:58.000000 func2stream-0.0.1.dev2405190653/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 06:53:02.776051 func2stream-0.0.1.dev2405190653/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-19 06:52:58.000000 func2stream-0.0.1.dev2405190653/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:53:02.776051 func2stream-0.0.1.dev2405190653/func2stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 06:53:02.000000 func2stream-0.0.1.dev2405190653/func2stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-19 06:53:02.000000 func2stream-0.0.1.dev2405190653/func2stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:53:02.000000 func2stream-0.0.1.dev2405190653/func2stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 06:53:02.000000 func2stream-0.0.1.dev2405190653/func2stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:53:02.000000 func2stream-0.0.1.dev2405190653/func2stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 06:52:58.000000 func2stream-0.0.1.dev2405190653/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 06:53:02.776051 func2stream-0.0.1.dev2405190653/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-19 06:52:58.000000 func2stream-0.0.1.dev2405190653/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:27:06.315423 func2stream-0.0.1.dev2405191627/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 16:27:06.315423 func2stream-0.0.1.dev2405191627/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:27:06.311423 func2stream-0.0.1.dev2405191627/func2stream/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/func2stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/func2stream/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/func2stream/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/func2stream/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:27:06.315423 func2stream-0.0.1.dev2405191627/func2stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-19 16:27:06.000000 func2stream-0.0.1.dev2405191627/func2stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-19 16:27:06.000000 func2stream-0.0.1.dev2405191627/func2stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:27:06.000000 func2stream-0.0.1.dev2405191627/func2stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 16:27:06.000000 func2stream-0.0.1.dev2405191627/func2stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 16:27:06.000000 func2stream-0.0.1.dev2405191627/func2stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 16:27:06.315423 func2stream-0.0.1.dev2405191627/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-19 16:26:56.000000 func2stream-0.0.1.dev2405191627/setup.py
```

### Comparing `func2stream-0.0.1.dev2405190653/LICENSE` & `func2stream-0.0.1.dev2405191627/LICENSE`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.1.dev2405190653/PKG-INFO` & `func2stream-0.0.1.dev2405191627/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2stream
-Version: 0.0.1.dev2405190653
+Version: 0.0.1.dev2405191627
 Summary: Effortlessly transform functions into asynchronous elements for building high-performance pipelines
 Home-page: https://github.com/BICHENG/func2stream
 Author: BI CHENG
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `func2stream-0.0.1.dev2405190653/README.md` & `func2stream-0.0.1.dev2405191627/README.md`

 * *Files identical despite different names*

### Comparing `func2stream-0.0.1.dev2405190653/func2stream.egg-info/PKG-INFO` & `func2stream-0.0.1.dev2405191627/func2stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2stream
-Version: 0.0.1.dev2405190653
+Version: 0.0.1.dev2405191627
 Summary: Effortlessly transform functions into asynchronous elements for building high-performance pipelines
 Home-page: https://github.com/BICHENG/func2stream
 Author: BI CHENG
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `func2stream-0.0.1.dev2405190653/setup.py` & `func2stream-0.0.1.dev2405191627/setup.py`

 * *Files identical despite different names*

