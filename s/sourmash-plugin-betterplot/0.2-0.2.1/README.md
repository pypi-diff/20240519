# Comparing `tmp/sourmash_plugin_betterplot-0.2.tar.gz` & `tmp/sourmash_plugin_betterplot-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_betterplot-0.2.tar", last modified: Sat May 18 14:55:00 2024, max compression
+gzip compressed data, was "sourmash_plugin_betterplot-0.2.1.tar", last modified: Sat May 18 15:06:17 2024, max compression
```

## Comparing `sourmash_plugin_betterplot-0.2.tar` & `sourmash_plugin_betterplot-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.242818 sourmash_plugin_betterplot-0.2/
--rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     4636 2024-05-18 14:55:00.242616 sourmash_plugin_betterplot-0.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     4275 2024-05-18 14:49:39.000000 sourmash_plugin_betterplot-0.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      512 2024-05-18 14:43:24.000000 sourmash_plugin_betterplot-0.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2024-05-18 14:55:00.242855 sourmash_plugin_betterplot-0.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.241049 sourmash_plugin_betterplot-0.2/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.242409 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     4636 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)      132 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       55 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2024-05-18 14:55:00.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)    13099 2024-05-18 14:41:09.000000 sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 14:55:00.242117 sourmash_plugin_betterplot-0.2/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.812973 sourmash_plugin_betterplot-0.2.1/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2.1/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     4638 2024-05-18 15:06:17.812783 sourmash_plugin_betterplot-0.2.1/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     4275 2024-05-18 14:55:28.000000 sourmash_plugin_betterplot-0.2.1/README.md
+-rw-r--r--   0 t          (502) staff       (20)      514 2024-05-18 15:06:08.000000 sourmash_plugin_betterplot-0.2.1/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2024-05-18 15:06:17.813007 sourmash_plugin_betterplot-0.2.1/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.811006 sourmash_plugin_betterplot-0.2.1/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.812575 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     4638 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      422 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)      132 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       55 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2024-05-18 15:06:17.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)    13099 2024-05-18 14:41:09.000000 sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2024-05-18 15:06:17.812269 sourmash_plugin_betterplot-0.2.1/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2024-05-17 15:38:24.000000 sourmash_plugin_betterplot-0.2.1/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_betterplot-0.2/LICENSE` & `sourmash_plugin_betterplot-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_betterplot-0.2/PKG-INFO` & `sourmash_plugin_betterplot-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.2
+Version: 0.2.1
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `sourmash_plugin_betterplot-0.2/README.md` & `sourmash_plugin_betterplot-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_betterplot-0.2/pyproject.toml` & `sourmash_plugin_betterplot-0.2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "sourmash_plugin_betterplot"
 description = "sourmash plugin for improved plotting/viz and cluster examination."
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.2"
+version = "0.2.1"
 
 dependencies = ["sourmash>=4.8.8,<5",
                 "matplotlib", "numpy", "scipy", "scikit-learn"]
 
 [metadata]
 license = { text = "BSD 3-Clause License" }
```

### Comparing `sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.egg-info/PKG-INFO` & `sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_betterplot
-Version: 0.2
+Version: 0.2.1
 Summary: sourmash plugin for improved plotting/viz and cluster examination.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sourmash<5,>=4.8.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
```

### Comparing `sourmash_plugin_betterplot-0.2/src/sourmash_plugin_betterplot.py` & `sourmash_plugin_betterplot-0.2.1/src/sourmash_plugin_betterplot.py`

 * *Files identical despite different names*

