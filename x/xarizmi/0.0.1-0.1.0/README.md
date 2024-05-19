# Comparing `tmp/xarizmi-0.0.1.tar.gz` & `tmp/xarizmi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarizmi-0.0.1.tar", last modified: Sun May 19 04:07:46 2024, max compression
+gzip compressed data, was "xarizmi-0.1.0.tar", last modified: Sun May 19 04:37:20 2024, max compression
```

## Comparing `xarizmi-0.0.1.tar` & `xarizmi-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:07:46.826279 xarizmi-0.0.1/
--rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.0.1/LICENSE
--rw-r--r--   0 javad      (501) staff       (20)      558 2024-05-19 04:07:46.826216 xarizmi-0.0.1/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      175 2024-05-19 03:29:04.000000 xarizmi-0.0.1/README.md
--rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.0.1/pyproject.toml
--rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-19 04:07:46.826529 xarizmi-0.0.1/setup.cfg
--rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 03:47:51.000000 xarizmi-0.0.1/setup.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:07:46.825232 xarizmi-0.0.1/xarizmi/
--rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-19 04:07:13.000000 xarizmi-0.0.1/xarizmi/__init__.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:07:46.826002 xarizmi-0.0.1/xarizmi.egg-info/
--rw-r--r--   0 javad      (501) staff       (20)      558 2024-05-19 04:07:46.000000 xarizmi-0.0.1/xarizmi.egg-info/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      195 2024-05-19 04:07:46.000000 xarizmi-0.0.1/xarizmi.egg-info/SOURCES.txt
--rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-19 04:07:46.000000 xarizmi-0.0.1/xarizmi.egg-info/dependency_links.txt
--rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-19 04:07:46.000000 xarizmi-0.0.1/xarizmi.egg-info/top_level.txt
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.537333 xarizmi-0.1.0/
+-rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.1.0/LICENSE
+-rw-r--r--   0 javad      (501) staff       (20)      558 2024-05-19 04:37:20.537224 xarizmi-0.1.0/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      175 2024-05-19 03:29:04.000000 xarizmi-0.1.0/README.md
+-rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.1.0/pyproject.toml
+-rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-19 04:37:20.537629 xarizmi-0.1.0/setup.cfg
+-rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 03:47:51.000000 xarizmi-0.1.0/setup.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.535945 xarizmi-0.1.0/tests/
+-rw-r--r--   0 javad      (501) staff       (20)      158 2024-05-19 04:34:21.000000 xarizmi-0.1.0/tests/test_candlestick.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.536207 xarizmi-0.1.0/xarizmi/
+-rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-19 04:36:44.000000 xarizmi-0.1.0/xarizmi/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)       28 2024-05-19 04:33:16.000000 xarizmi-0.1.0/xarizmi/candlestick.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 04:37:20.536939 xarizmi-0.1.0/xarizmi.egg-info/
+-rw-r--r--   0 javad      (501) staff       (20)      558 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      244 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/SOURCES.txt
+-rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/dependency_links.txt
+-rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-19 04:37:20.000000 xarizmi-0.1.0/xarizmi.egg-info/top_level.txt
```

### Comparing `xarizmi-0.0.1/LICENSE` & `xarizmi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarizmi-0.0.1/PKG-INFO` & `xarizmi-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarizmi
-Version: 0.0.1
+Version: 0.1.0
 Summary: Xarizmi (read Khwarizmi) project is an educational project thatcontains tools for technical analysis in Python.
 Home-page: https://github.com/javadebadi/xarizmi
 Author: Javad Ebadi
 Author-email: javad@javadebadi.com
 License: Apache 2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `xarizmi-0.0.1/setup.py` & `xarizmi-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `xarizmi-0.0.1/xarizmi.egg-info/PKG-INFO` & `xarizmi-0.1.0/xarizmi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarizmi
-Version: 0.0.1
+Version: 0.1.0
 Summary: Xarizmi (read Khwarizmi) project is an educational project thatcontains tools for technical analysis in Python.
 Home-page: https://github.com/javadebadi/xarizmi
 Author: Javad Ebadi
 Author-email: javad@javadebadi.com
 License: Apache 2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

