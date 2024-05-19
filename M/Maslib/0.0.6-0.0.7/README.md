# Comparing `tmp/Maslib-0.0.6.tar.gz` & `tmp/Maslib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.0.6.tar", last modified: Sun May 19 11:13:43 2024, max compression
+gzip compressed data, was "Maslib-0.0.7.tar", last modified: Sun May 19 11:15:51 2024, max compression
```

## Comparing `Maslib-0.0.6.tar` & `Maslib-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.590384 Maslib-0.0.6/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.558355 Maslib-0.0.6/MasLib/
--rw-rw-rw-   0        0        0      350 2024-05-19 10:55:47.000000 Maslib-0.0.6/MasLib/__init__.py
--rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.6/MasLib/correlation.py
--rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.6/MasLib/encoding.py
--rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.6/MasLib/grid_search_optimization.py
--rw-rw-rw-   0        0        0     5232 2024-05-19 11:12:32.000000 Maslib-0.0.6/MasLib/regression.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.586380 Maslib-0.0.6/Maslib.egg-info/
--rw-rw-rw-   0        0        0      799 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2024-05-19 11:13:43.588382 Maslib-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 11:13:43.590384 Maslib-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-05-19 11:13:12.000000 Maslib-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.584379 Maslib-0.0.6/tests/
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.6/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.6/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.6/tests/test_grid_search.py
--rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.6/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:15:51.115300 Maslib-0.0.7/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.7/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-19 11:15:51.096283 Maslib-0.0.7/MasLib/
+-rw-rw-rw-   0        0        0      344 2024-05-19 11:15:25.000000 Maslib-0.0.7/MasLib/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.7/MasLib/correlation.py
+-rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.7/MasLib/encoding.py
+-rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.7/MasLib/grid_search_optimization.py
+-rw-rw-rw-   0        0        0     5232 2024-05-19 11:12:32.000000 Maslib-0.0.7/MasLib/regression.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:15:51.111297 Maslib-0.0.7/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-05-19 11:15:50.000000 Maslib-0.0.7/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-19 11:15:51.000000 Maslib-0.0.7/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:15:50.000000 Maslib-0.0.7/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-19 11:15:50.000000 Maslib-0.0.7/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 11:15:50.000000 Maslib-0.0.7/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      799 2024-05-19 11:15:51.113298 Maslib-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:15:51.116301 Maslib-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-19 11:15:41.000000 Maslib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:15:51.108294 Maslib-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.7/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.7/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.7/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.7/tests/test_regression.py
```

### Comparing `Maslib-0.0.6/MasLib/correlation.py` & `Maslib-0.0.7/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/MasLib/encoding.py` & `Maslib-0.0.7/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/MasLib/grid_search_optimization.py` & `Maslib-0.0.7/MasLib/grid_search_optimization.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/MasLib/regression.py` & `Maslib-0.0.7/MasLib/regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/Maslib.egg-info/PKG-INFO` & `Maslib-0.0.7/Maslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.0.6/PKG-INFO` & `Maslib-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.6
+Version: 0.0.7
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.0.6/setup.py` & `Maslib-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.0.6',
+    version='0.0.7',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
```

### Comparing `Maslib-0.0.6/tests/test_correlation.py` & `Maslib-0.0.7/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/tests/test_encoding.py` & `Maslib-0.0.7/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/tests/test_grid_search.py` & `Maslib-0.0.7/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.6/tests/test_regression.py` & `Maslib-0.0.7/tests/test_regression.py`

 * *Files identical despite different names*

