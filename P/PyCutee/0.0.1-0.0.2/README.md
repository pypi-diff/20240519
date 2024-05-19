# Comparing `tmp/pycutee-0.0.1.tar.gz` & `tmp/pycutee-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutee-0.0.1.tar", last modified: Sun May 19 10:53:27 2024, max compression
+gzip compressed data, was "pycutee-0.0.2.tar", last modified: Sun May 19 11:03:17 2024, max compression
```

## Comparing `pycutee-0.0.1.tar` & `pycutee-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:53:27.391472 pycutee-0.0.1/
--rw-rw-rw-   0        0        0     1282 2024-05-19 10:53:27.391472 pycutee-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 10:53:27.374642 pycutee-0.0.1/PyCutee/
--rw-rw-rw-   0        0        0      135 2024-04-16 16:28:03.000000 pycutee-0.0.1/PyCutee/__init__.py
--rw-rw-rw-   0        0        0     1003 2024-04-16 16:41:36.000000 pycutee-0.0.1/PyCutee/button_rounded.py
--rw-rw-rw-   0        0        0      792 2024-04-16 16:38:54.000000 pycutee-0.0.1/PyCutee/button_simple.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:53:27.390472 pycutee-0.0.1/PyCutee.egg-info/
--rw-rw-rw-   0        0        0     1282 2024-05-19 10:53:27.000000 pycutee-0.0.1/PyCutee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-05-19 10:53:27.000000 pycutee-0.0.1/PyCutee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:53:27.000000 pycutee-0.0.1/PyCutee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-19 10:53:27.000000 pycutee-0.0.1/PyCutee.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 10:53:27.000000 pycutee-0.0.1/PyCutee.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      674 2024-05-19 10:52:05.000000 pycutee-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 10:53:27.391472 pycutee-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1139 2024-05-19 10:50:32.000000 pycutee-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:03:17.713917 pycutee-0.0.2/
+-rw-rw-rw-   0        0        0     2441 2024-05-19 11:03:17.713917 pycutee-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 11:03:17.696025 pycutee-0.0.2/PyCutee/
+-rw-rw-rw-   0        0        0      135 2024-04-16 16:28:03.000000 pycutee-0.0.2/PyCutee/__init__.py
+-rw-rw-rw-   0        0        0     1003 2024-04-16 16:41:36.000000 pycutee-0.0.2/PyCutee/button_rounded.py
+-rw-rw-rw-   0        0        0      792 2024-04-16 16:38:54.000000 pycutee-0.0.2/PyCutee/button_simple.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:03:17.712411 pycutee-0.0.2/PyCutee.egg-info/
+-rw-rw-rw-   0        0        0     2441 2024-05-19 11:03:17.000000 pycutee-0.0.2/PyCutee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2024-05-19 11:03:17.000000 pycutee-0.0.2/PyCutee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:03:17.000000 pycutee-0.0.2/PyCutee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-19 11:03:17.000000 pycutee-0.0.2/PyCutee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 11:03:17.000000 pycutee-0.0.2/PyCutee.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1793 2024-05-19 11:02:19.000000 pycutee-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:03:17.713917 pycutee-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2024-05-19 11:03:05.000000 pycutee-0.0.2/setup.py
```

### Comparing `pycutee-0.0.1/PyCutee/button_rounded.py` & `pycutee-0.0.2/PyCutee/button_rounded.py`

 * *Files identical despite different names*

### Comparing `pycutee-0.0.1/PyCutee/button_simple.py` & `pycutee-0.0.2/PyCutee/button_simple.py`

 * *Files identical despite different names*

### Comparing `pycutee-0.0.1/setup.py` & `pycutee-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'This app is a lil framework for PyQt5 like bootstrap for HTML5'
 LONG_DESCRIPTION = 'A package that allows to build simple PyQt5 apps faster and cooler.'
 
 # Setting up
 setup(
     name="PyCutee",
     version=VERSION,
```

