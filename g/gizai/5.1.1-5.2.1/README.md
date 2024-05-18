# Comparing `tmp/gizai-5.1.1.tar.gz` & `tmp/gizai-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gizai-5.1.1.tar", last modified: Sat May 18 23:41:39 2024, max compression
+gzip compressed data, was "gizai-5.2.1.tar", last modified: Sat May 18 23:45:54 2024, max compression
```

## Comparing `gizai-5.1.1.tar` & `gizai-5.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:41:39.973909 gizai-5.1.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-23 00:28:51.000000 gizai-5.1.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)      139 2024-05-18 23:41:39.972798 gizai-5.1.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      446 2024-05-12 21:46:09.000000 gizai-5.1.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:41:39.968774 gizai-5.1.1/gizai/
--rw-r--r--   0 kamangir   (502) staff       (20)      101 2024-05-18 23:39:32.000000 gizai-5.1.1/gizai/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1253 2024-05-18 23:39:40.000000 gizai-5.1.1/gizai/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      273 2024-05-18 23:39:55.000000 gizai-5.1.1/gizai/build.py
--rw-r--r--   0 kamangir   (502) staff       (20)     3155 2024-05-18 23:39:59.000000 gizai-5.1.1/gizai/digest.py
--rw-r--r--   0 kamangir   (502) staff       (20)       86 2024-05-18 23:40:07.000000 gizai-5.1.1/gizai/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-23 00:28:51.000000 gizai-5.1.1/gizai/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:41:39.971923 gizai-5.1.1/gizai.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)      139 2024-05-18 23:41:39.000000 gizai-5.1.1/gizai.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-18 23:41:39.000000 gizai-5.1.1/gizai.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-18 23:41:39.000000 gizai-5.1.1/gizai.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-18 23:41:39.000000 gizai-5.1.1/gizai.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-18 23:41:39.974061 gizai-5.1.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-18 23:40:15.000000 gizai-5.1.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:45:54.674404 gizai-5.2.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-01-23 00:28:51.000000 gizai-5.2.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)      139 2024-05-18 23:45:54.673693 gizai-5.2.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      454 2024-05-18 23:45:26.000000 gizai-5.2.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:45:54.669687 gizai-5.2.1/gizai/
+-rw-r--r--   0 kamangir   (502) staff       (20)      101 2024-05-18 23:44:32.000000 gizai-5.2.1/gizai/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1253 2024-05-18 23:39:40.000000 gizai-5.2.1/gizai/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      273 2024-05-18 23:39:55.000000 gizai-5.2.1/gizai/build.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     3155 2024-05-18 23:39:59.000000 gizai-5.2.1/gizai/digest.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       86 2024-05-18 23:40:07.000000 gizai-5.2.1/gizai/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-01-23 00:28:51.000000 gizai-5.2.1/gizai/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-18 23:45:54.673163 gizai-5.2.1/gizai.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)      139 2024-05-18 23:45:54.000000 gizai-5.2.1/gizai.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-18 23:45:54.000000 gizai-5.2.1/gizai.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-18 23:45:54.000000 gizai-5.2.1/gizai.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        6 2024-05-18 23:45:54.000000 gizai-5.2.1/gizai.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-18 23:45:54.674535 gizai-5.2.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-18 23:40:15.000000 gizai-5.2.1/setup.py
```

### Comparing `gizai-5.1.1/LICENSE` & `gizai-5.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gizai-5.1.1/gizai/__main__.py` & `gizai-5.2.1/gizai/__main__.py`

 * *Files identical despite different names*

### Comparing `gizai-5.1.1/gizai/digest.py` & `gizai-5.2.1/gizai/digest.py`

 * *Files identical despite different names*

