# Comparing `tmp/cortexannotate-0.1.1.tar.gz` & `tmp/cortexannotate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortexannotate-0.1.1.tar", last modified: Sun May 19 14:10:25 2024, max compression
+gzip compressed data, was "cortexannotate-0.1.2.tar", last modified: Sun May 19 14:16:32 2024, max compression
```

## Comparing `cortexannotate-0.1.1.tar` & `cortexannotate-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:10:25.638119 cortexannotate-0.1.1/
--rw-r--r--   0 nben       (503) staff       (20)     1076 2023-09-18 16:31:33.000000 cortexannotate-0.1.1/LICENSE
--rw-r--r--   0 nben       (503) staff       (20)     1385 2024-05-19 14:10:25.637950 cortexannotate-0.1.1/PKG-INFO
--rw-r--r--   0 nben       (503) staff       (20)     3113 2023-09-18 16:31:33.000000 cortexannotate-0.1.1/README.md
--rw-r--r--   0 nben       (503) staff       (20)       89 2024-05-19 13:34:04.000000 cortexannotate-0.1.1/pyproject.toml
--rw-r--r--   0 nben       (503) staff       (20)       38 2024-05-19 14:10:25.638158 cortexannotate-0.1.1/setup.cfg
--rw-r--r--   0 nben       (503) staff       (20)     1574 2024-05-19 14:10:20.000000 cortexannotate-0.1.1/setup.py
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:10:25.635688 cortexannotate-0.1.1/src/
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:10:25.637135 cortexannotate-0.1.1/src/cortexannotate/
--rw-r--r--   0 nben       (503) staff       (20)     1039 2024-05-19 13:53:58.000000 cortexannotate-0.1.1/src/cortexannotate/__init__.py
--rw-r--r--   0 nben       (503) staff       (20)    26754 2024-05-16 13:47:10.000000 cortexannotate-0.1.1/src/cortexannotate/_config.py
--rw-r--r--   0 nben       (503) staff       (20)    21486 2024-05-17 20:14:42.000000 cortexannotate-0.1.1/src/cortexannotate/_control.py
--rw-r--r--   0 nben       (503) staff       (20)    34583 2024-05-18 02:43:06.000000 cortexannotate-0.1.1/src/cortexannotate/_core.py
--rw-r--r--   0 nben       (503) staff       (20)    23823 2024-05-17 20:15:30.000000 cortexannotate-0.1.1/src/cortexannotate/_figure.py
--rw-r--r--   0 nben       (503) staff       (20)    10154 2024-05-17 20:14:17.000000 cortexannotate-0.1.1/src/cortexannotate/_util.py
--rw-r--r--   0 nben       (503) staff       (20)    14943 2024-05-19 13:29:41.000000 cortexannotate-0.1.1/src/cortexannotate/prfs.py
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:10:25.637779 cortexannotate-0.1.1/src/cortexannotate.egg-info/
--rw-r--r--   0 nben       (503) staff       (20)     1385 2024-05-19 14:10:25.000000 cortexannotate-0.1.1/src/cortexannotate.egg-info/PKG-INFO
--rw-r--r--   0 nben       (503) staff       (20)      414 2024-05-19 14:10:25.000000 cortexannotate-0.1.1/src/cortexannotate.egg-info/SOURCES.txt
--rw-r--r--   0 nben       (503) staff       (20)        1 2024-05-19 14:10:25.000000 cortexannotate-0.1.1/src/cortexannotate.egg-info/dependency_links.txt
--rw-r--r--   0 nben       (503) staff       (20)       15 2024-05-19 14:10:25.000000 cortexannotate-0.1.1/src/cortexannotate.egg-info/top_level.txt
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.040271 cortexannotate-0.1.2/
+-rw-r--r--   0 nben       (503) staff       (20)     1076 2023-09-18 16:31:33.000000 cortexannotate-0.1.2/LICENSE
+-rw-r--r--   0 nben       (503) staff       (20)     1385 2024-05-19 14:16:32.040104 cortexannotate-0.1.2/PKG-INFO
+-rw-r--r--   0 nben       (503) staff       (20)     3113 2023-09-18 16:31:33.000000 cortexannotate-0.1.2/README.md
+-rw-r--r--   0 nben       (503) staff       (20)       89 2024-05-19 13:34:04.000000 cortexannotate-0.1.2/pyproject.toml
+-rw-r--r--   0 nben       (503) staff       (20)       38 2024-05-19 14:16:32.040307 cortexannotate-0.1.2/setup.cfg
+-rw-r--r--   0 nben       (503) staff       (20)     1574 2024-05-19 14:15:57.000000 cortexannotate-0.1.2/setup.py
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.037896 cortexannotate-0.1.2/src/
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.039339 cortexannotate-0.1.2/src/cortexannotate/
+-rw-r--r--   0 nben       (503) staff       (20)     1039 2024-05-19 14:16:03.000000 cortexannotate-0.1.2/src/cortexannotate/__init__.py
+-rw-r--r--   0 nben       (503) staff       (20)    26754 2024-05-16 13:47:10.000000 cortexannotate-0.1.2/src/cortexannotate/_config.py
+-rw-r--r--   0 nben       (503) staff       (20)    21486 2024-05-17 20:14:42.000000 cortexannotate-0.1.2/src/cortexannotate/_control.py
+-rw-r--r--   0 nben       (503) staff       (20)    34583 2024-05-18 02:43:06.000000 cortexannotate-0.1.2/src/cortexannotate/_core.py
+-rw-r--r--   0 nben       (503) staff       (20)    23823 2024-05-17 20:15:30.000000 cortexannotate-0.1.2/src/cortexannotate/_figure.py
+-rw-r--r--   0 nben       (503) staff       (20)    10154 2024-05-17 20:14:17.000000 cortexannotate-0.1.2/src/cortexannotate/_util.py
+-rw-r--r--   0 nben       (503) staff       (20)    14943 2024-05-19 13:29:41.000000 cortexannotate-0.1.2/src/cortexannotate/prfs.py
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.039935 cortexannotate-0.1.2/src/cortexannotate.egg-info/
+-rw-r--r--   0 nben       (503) staff       (20)     1385 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/PKG-INFO
+-rw-r--r--   0 nben       (503) staff       (20)      414 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/SOURCES.txt
+-rw-r--r--   0 nben       (503) staff       (20)        1 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/dependency_links.txt
+-rw-r--r--   0 nben       (503) staff       (20)       15 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/top_level.txt
```

### Comparing `cortexannotate-0.1.1/LICENSE` & `cortexannotate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/PKG-INFO` & `cortexannotate-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortexannotate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolbox for flexible annotation of the cortical surface by many raters
 Home-page: https://github.com/noahbenson/cortex-annotate
 Download-URL: https://github.com/noahbenson/cortex-annotate
 Author: Noah C. Benson
 Author-email: nben@uw.edu
 Maintainer-email: nben@uw.edu
 License: MIT
```

### Comparing `cortexannotate-0.1.1/README.md` & `cortexannotate-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/setup.py` & `cortexannotate-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 
 import os
 from setuptools import (setup, Extension)
 
 setup(
     name='cortexannotate',
-    version='0.1.1',
+    version='0.1.2',
     description='Toolbox for flexible annotation of the cortical surface by many raters',
     keywords='neuroscience cortex annotation',
     author='Noah C. Benson',
     author_email='nben@uw.edu',
     maintainer_email='nben@uw.edu',
     long_description='''
         See the README.md file at the github repository for this package:
```

### Comparing `cortexannotate-0.1.1/src/cortexannotate/__init__.py` & `cortexannotate-0.1.2/src/cortexannotate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 from ._util import (delay, ldict, watershed_contours)
 from ._core import AnnotationTool
 from .prfs  import annotate_prfs
 
 
 # Meta-Data ####################################################################
 
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 #__all__ = ("AnnotationTool",)
```

### Comparing `cortexannotate-0.1.1/src/cortexannotate/_config.py` & `cortexannotate-0.1.2/src/cortexannotate/_config.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/src/cortexannotate/_control.py` & `cortexannotate-0.1.2/src/cortexannotate/_control.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/src/cortexannotate/_core.py` & `cortexannotate-0.1.2/src/cortexannotate/_core.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/src/cortexannotate/_figure.py` & `cortexannotate-0.1.2/src/cortexannotate/_figure.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/src/cortexannotate/_util.py` & `cortexannotate-0.1.2/src/cortexannotate/_util.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/src/cortexannotate/prfs.py` & `cortexannotate-0.1.2/src/cortexannotate/prfs.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.1/src/cortexannotate.egg-info/PKG-INFO` & `cortexannotate-0.1.2/src/cortexannotate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortexannotate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolbox for flexible annotation of the cortical surface by many raters
 Home-page: https://github.com/noahbenson/cortex-annotate
 Download-URL: https://github.com/noahbenson/cortex-annotate
 Author: Noah C. Benson
 Author-email: nben@uw.edu
 Maintainer-email: nben@uw.edu
 License: MIT
```

