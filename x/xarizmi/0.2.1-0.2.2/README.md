# Comparing `tmp/xarizmi-0.2.1.tar.gz` & `tmp/xarizmi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarizmi-0.2.1.tar", last modified: Sun May 19 07:20:44 2024, max compression
+gzip compressed data, was "xarizmi-0.2.2.tar", last modified: Sun May 19 07:31:48 2024, max compression
```

## Comparing `xarizmi-0.2.1.tar` & `xarizmi-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:20:44.419379 xarizmi-0.2.1/
--rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.2.1/LICENSE
--rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-19 07:20:44.419303 xarizmi-0.2.1/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      377 2024-05-19 06:54:11.000000 xarizmi-0.2.1/README.md
--rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.2.1/pyproject.toml
--rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-19 07:20:44.419640 xarizmi-0.2.1/setup.cfg
--rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 07:14:04.000000 xarizmi-0.2.1/setup.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:20:44.417955 xarizmi-0.2.1/tests/
--rw-r--r--   0 javad      (501) staff       (20)      608 2024-05-19 07:00:40.000000 xarizmi-0.2.1/tests/test_candlestick.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:20:44.418375 xarizmi-0.2.1/xarizmi/
--rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-19 07:19:06.000000 xarizmi-0.2.1/xarizmi/__init__.py
--rw-r--r--   0 javad      (501) staff       (20)      127 2024-05-19 05:19:14.000000 xarizmi-0.2.1/xarizmi/candlestick.py
--rw-r--r--   0 javad      (501) staff       (20)       86 2024-05-19 06:57:33.000000 xarizmi-0.2.1/xarizmi/enums.py
-drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:20:44.419092 xarizmi-0.2.1/xarizmi.egg-info/
--rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-19 07:20:44.000000 xarizmi-0.2.1/xarizmi.egg-info/PKG-INFO
--rw-r--r--   0 javad      (501) staff       (20)      261 2024-05-19 07:20:44.000000 xarizmi-0.2.1/xarizmi.egg-info/SOURCES.txt
--rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-19 07:20:44.000000 xarizmi-0.2.1/xarizmi.egg-info/dependency_links.txt
--rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-19 07:20:44.000000 xarizmi-0.2.1/xarizmi.egg-info/top_level.txt
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:31:48.094215 xarizmi-0.2.2/
+-rw-r--r--   0 javad      (501) staff       (20)    11345 2024-05-19 03:25:40.000000 xarizmi-0.2.2/LICENSE
+-rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-19 07:31:48.094138 xarizmi-0.2.2/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      377 2024-05-19 06:54:11.000000 xarizmi-0.2.2/README.md
+-rw-r--r--   0 javad      (501) staff       (20)       30 2024-05-19 03:25:40.000000 xarizmi-0.2.2/pyproject.toml
+-rw-r--r--   0 javad      (501) staff       (20)      280 2024-05-19 07:31:48.094498 xarizmi-0.2.2/setup.cfg
+-rw-r--r--   0 javad      (501) staff       (20)      849 2024-05-19 07:14:04.000000 xarizmi-0.2.2/setup.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:31:48.092839 xarizmi-0.2.2/tests/
+-rw-r--r--   0 javad      (501) staff       (20)     1026 2024-05-19 07:29:48.000000 xarizmi-0.2.2/tests/test_candlestick.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:31:48.093242 xarizmi-0.2.2/xarizmi/
+-rw-r--r--   0 javad      (501) staff       (20)       22 2024-05-19 07:30:26.000000 xarizmi-0.2.2/xarizmi/__init__.py
+-rw-r--r--   0 javad      (501) staff       (20)      209 2024-05-19 07:27:21.000000 xarizmi-0.2.2/xarizmi/candlestick.py
+-rw-r--r--   0 javad      (501) staff       (20)       86 2024-05-19 06:57:33.000000 xarizmi-0.2.2/xarizmi/enums.py
+drwxr-xr-x   0 javad      (501) staff       (20)        0 2024-05-19 07:31:48.093912 xarizmi-0.2.2/xarizmi.egg-info/
+-rw-r--r--   0 javad      (501) staff       (20)      760 2024-05-19 07:31:48.000000 xarizmi-0.2.2/xarizmi.egg-info/PKG-INFO
+-rw-r--r--   0 javad      (501) staff       (20)      261 2024-05-19 07:31:48.000000 xarizmi-0.2.2/xarizmi.egg-info/SOURCES.txt
+-rw-r--r--   0 javad      (501) staff       (20)        1 2024-05-19 07:31:48.000000 xarizmi-0.2.2/xarizmi.egg-info/dependency_links.txt
+-rw-r--r--   0 javad      (501) staff       (20)        8 2024-05-19 07:31:48.000000 xarizmi-0.2.2/xarizmi.egg-info/top_level.txt
```

### Comparing `xarizmi-0.2.1/LICENSE` & `xarizmi-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarizmi-0.2.1/PKG-INFO` & `xarizmi-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarizmi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Xarizmi (read Khwarizmi) project is an educational project thatcontains tools for technical analysis in Python.
 Home-page: https://github.com/javadebadi/xarizmi
 Author: Javad Ebadi
 Author-email: javad@javadebadi.com
 License: Apache 2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `xarizmi-0.2.1/setup.py` & `xarizmi-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `xarizmi-0.2.1/xarizmi.egg-info/PKG-INFO` & `xarizmi-0.2.2/xarizmi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xarizmi
-Version: 0.2.1
+Version: 0.2.2
 Summary: Xarizmi (read Khwarizmi) project is an educational project thatcontains tools for technical analysis in Python.
 Home-page: https://github.com/javadebadi/xarizmi
 Author: Javad Ebadi
 Author-email: javad@javadebadi.com
 License: Apache 2.0
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

