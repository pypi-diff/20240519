# Comparing `tmp/cortexannotate-0.1.2.tar.gz` & `tmp/cortexannotate-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortexannotate-0.1.2.tar", last modified: Sun May 19 14:16:32 2024, max compression
+gzip compressed data, was "cortexannotate-0.1.3.tar", last modified: Sun May 19 14:24:22 2024, max compression
```

## Comparing `cortexannotate-0.1.2.tar` & `cortexannotate-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.040271 cortexannotate-0.1.2/
--rw-r--r--   0 nben       (503) staff       (20)     1076 2023-09-18 16:31:33.000000 cortexannotate-0.1.2/LICENSE
--rw-r--r--   0 nben       (503) staff       (20)     1385 2024-05-19 14:16:32.040104 cortexannotate-0.1.2/PKG-INFO
--rw-r--r--   0 nben       (503) staff       (20)     3113 2023-09-18 16:31:33.000000 cortexannotate-0.1.2/README.md
--rw-r--r--   0 nben       (503) staff       (20)       89 2024-05-19 13:34:04.000000 cortexannotate-0.1.2/pyproject.toml
--rw-r--r--   0 nben       (503) staff       (20)       38 2024-05-19 14:16:32.040307 cortexannotate-0.1.2/setup.cfg
--rw-r--r--   0 nben       (503) staff       (20)     1574 2024-05-19 14:15:57.000000 cortexannotate-0.1.2/setup.py
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.037896 cortexannotate-0.1.2/src/
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.039339 cortexannotate-0.1.2/src/cortexannotate/
--rw-r--r--   0 nben       (503) staff       (20)     1039 2024-05-19 14:16:03.000000 cortexannotate-0.1.2/src/cortexannotate/__init__.py
--rw-r--r--   0 nben       (503) staff       (20)    26754 2024-05-16 13:47:10.000000 cortexannotate-0.1.2/src/cortexannotate/_config.py
--rw-r--r--   0 nben       (503) staff       (20)    21486 2024-05-17 20:14:42.000000 cortexannotate-0.1.2/src/cortexannotate/_control.py
--rw-r--r--   0 nben       (503) staff       (20)    34583 2024-05-18 02:43:06.000000 cortexannotate-0.1.2/src/cortexannotate/_core.py
--rw-r--r--   0 nben       (503) staff       (20)    23823 2024-05-17 20:15:30.000000 cortexannotate-0.1.2/src/cortexannotate/_figure.py
--rw-r--r--   0 nben       (503) staff       (20)    10154 2024-05-17 20:14:17.000000 cortexannotate-0.1.2/src/cortexannotate/_util.py
--rw-r--r--   0 nben       (503) staff       (20)    14943 2024-05-19 13:29:41.000000 cortexannotate-0.1.2/src/cortexannotate/prfs.py
-drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:16:32.039935 cortexannotate-0.1.2/src/cortexannotate.egg-info/
--rw-r--r--   0 nben       (503) staff       (20)     1385 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/PKG-INFO
--rw-r--r--   0 nben       (503) staff       (20)      414 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/SOURCES.txt
--rw-r--r--   0 nben       (503) staff       (20)        1 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/dependency_links.txt
--rw-r--r--   0 nben       (503) staff       (20)       15 2024-05-19 14:16:32.000000 cortexannotate-0.1.2/src/cortexannotate.egg-info/top_level.txt
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:24:22.940307 cortexannotate-0.1.3/
+-rw-r--r--   0 nben       (503) staff       (20)     1076 2023-09-18 16:31:33.000000 cortexannotate-0.1.3/LICENSE
+-rw-r--r--   0 nben       (503) staff       (20)     1604 2024-05-19 14:24:22.940137 cortexannotate-0.1.3/PKG-INFO
+-rw-r--r--   0 nben       (503) staff       (20)     3113 2023-09-18 16:31:33.000000 cortexannotate-0.1.3/README.md
+-rw-r--r--   0 nben       (503) staff       (20)       89 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/pyproject.toml
+-rw-r--r--   0 nben       (503) staff       (20)       38 2024-05-19 14:24:22.940365 cortexannotate-0.1.3/setup.cfg
+-rw-r--r--   0 nben       (503) staff       (20)     1803 2024-05-19 14:24:00.000000 cortexannotate-0.1.3/setup.py
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:24:22.937574 cortexannotate-0.1.3/src/
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:24:22.939122 cortexannotate-0.1.3/src/cortexannotate/
+-rw-r--r--   0 nben       (503) staff       (20)     1039 2024-05-19 14:24:07.000000 cortexannotate-0.1.3/src/cortexannotate/__init__.py
+-rw-r--r--   0 nben       (503) staff       (20)    26754 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/src/cortexannotate/_config.py
+-rw-r--r--   0 nben       (503) staff       (20)    21486 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/src/cortexannotate/_control.py
+-rw-r--r--   0 nben       (503) staff       (20)    34583 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/src/cortexannotate/_core.py
+-rw-r--r--   0 nben       (503) staff       (20)    23823 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/src/cortexannotate/_figure.py
+-rw-r--r--   0 nben       (503) staff       (20)    10154 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/src/cortexannotate/_util.py
+-rw-r--r--   0 nben       (503) staff       (20)    14943 2024-05-19 14:18:39.000000 cortexannotate-0.1.3/src/cortexannotate/prfs.py
+drwxr-xr-x   0 nben       (503) staff       (20)        0 2024-05-19 14:24:22.939922 cortexannotate-0.1.3/src/cortexannotate.egg-info/
+-rw-r--r--   0 nben       (503) staff       (20)     1604 2024-05-19 14:24:22.000000 cortexannotate-0.1.3/src/cortexannotate.egg-info/PKG-INFO
+-rw-r--r--   0 nben       (503) staff       (20)      455 2024-05-19 14:24:22.000000 cortexannotate-0.1.3/src/cortexannotate.egg-info/SOURCES.txt
+-rw-r--r--   0 nben       (503) staff       (20)        1 2024-05-19 14:24:22.000000 cortexannotate-0.1.3/src/cortexannotate.egg-info/dependency_links.txt
+-rw-r--r--   0 nben       (503) staff       (20)      114 2024-05-19 14:24:22.000000 cortexannotate-0.1.3/src/cortexannotate.egg-info/requires.txt
+-rw-r--r--   0 nben       (503) staff       (20)       15 2024-05-19 14:24:22.000000 cortexannotate-0.1.3/src/cortexannotate.egg-info/top_level.txt
```

### Comparing `cortexannotate-0.1.2/LICENSE` & `cortexannotate-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/PKG-INFO` & `cortexannotate-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortexannotate
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolbox for flexible annotation of the cortical surface by many raters
 Home-page: https://github.com/noahbenson/cortex-annotate
 Download-URL: https://github.com/noahbenson/cortex-annotate
 Author: Noah C. Benson
 Author-email: nben@uw.edu
 Maintainer-email: nben@uw.edu
 License: MIT
@@ -23,12 +23,19 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
+Requires-Dist: neuropythy>=0.12.13
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: ipywidgets>=8.1.2
+Requires-Dist: ipycanvas>=0.13.2
+Requires-Dist: imageio>=2.26.0
+Requires-Dist: pandas>=1.4.1
 
 
         See the README.md file at the github repository for this package:
         https://github.com/noahbenson/cortex-annotate
```

### Comparing `cortexannotate-0.1.2/README.md` & `cortexannotate-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/setup.py` & `cortexannotate-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 
 import os
 from setuptools import (setup, Extension)
 
 setup(
     name='cortexannotate',
-    version='0.1.2',
+    version='0.1.3',
     description='Toolbox for flexible annotation of the cortical surface by many raters',
     keywords='neuroscience cortex annotation',
     author='Noah C. Benson',
     author_email='nben@uw.edu',
     maintainer_email='nben@uw.edu',
     long_description='''
         See the README.md file at the github repository for this package:
@@ -33,8 +33,16 @@
         'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
         'Operating System :: POSIX',
         'Operating System :: Unix',
         'Operating System :: MacOS'],
+    install_requires=[
+        'neuropythy >= 0.12.13',
+        'pandas >= 2.2.2',
+        'pyyaml >= 6.0.1',
+        'ipywidgets >= 8.1.2',
+        'ipycanvas >= 0.13.2',
+        'imageio >= 2.26.0',
+        'pandas >= 1.4.1'],
     packages=['cortexannotate'])
```

### Comparing `cortexannotate-0.1.2/src/cortexannotate/__init__.py` & `cortexannotate-0.1.3/src/cortexannotate/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 from ._util import (delay, ldict, watershed_contours)
 from ._core import AnnotationTool
 from .prfs  import annotate_prfs
 
 
 # Meta-Data ####################################################################
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 #__all__ = ("AnnotationTool",)
```

### Comparing `cortexannotate-0.1.2/src/cortexannotate/_config.py` & `cortexannotate-0.1.3/src/cortexannotate/_config.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/src/cortexannotate/_control.py` & `cortexannotate-0.1.3/src/cortexannotate/_control.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/src/cortexannotate/_core.py` & `cortexannotate-0.1.3/src/cortexannotate/_core.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/src/cortexannotate/_figure.py` & `cortexannotate-0.1.3/src/cortexannotate/_figure.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/src/cortexannotate/_util.py` & `cortexannotate-0.1.3/src/cortexannotate/_util.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/src/cortexannotate/prfs.py` & `cortexannotate-0.1.3/src/cortexannotate/prfs.py`

 * *Files identical despite different names*

### Comparing `cortexannotate-0.1.2/src/cortexannotate.egg-info/PKG-INFO` & `cortexannotate-0.1.3/src/cortexannotate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cortexannotate
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolbox for flexible annotation of the cortical surface by many raters
 Home-page: https://github.com/noahbenson/cortex-annotate
 Download-URL: https://github.com/noahbenson/cortex-annotate
 Author: Noah C. Benson
 Author-email: nben@uw.edu
 Maintainer-email: nben@uw.edu
 License: MIT
@@ -23,12 +23,19 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
+Requires-Dist: neuropythy>=0.12.13
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: ipywidgets>=8.1.2
+Requires-Dist: ipycanvas>=0.13.2
+Requires-Dist: imageio>=2.26.0
+Requires-Dist: pandas>=1.4.1
 
 
         See the README.md file at the github repository for this package:
         https://github.com/noahbenson/cortex-annotate
```

