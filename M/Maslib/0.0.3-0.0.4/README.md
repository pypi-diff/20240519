# Comparing `tmp/Maslib-0.0.3.tar.gz` & `tmp/Maslib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.0.3.tar", last modified: Sun May 19 10:50:42 2024, max compression
+gzip compressed data, was "Maslib-0.0.4.tar", last modified: Sun May 19 11:08:06 2024, max compression
```

## Comparing `Maslib-0.0.3.tar` & `Maslib-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:50:42.228313 Maslib-0.0.3/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.3/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-19 10:50:42.212302 Maslib-0.0.3/MasLib/
--rw-rw-rw-   0        0        0      344 2024-05-18 17:23:43.000000 Maslib-0.0.3/MasLib/__init__.py
--rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.3/MasLib/correlation.py
--rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.3/MasLib/encoding.py
--rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.3/MasLib/grid_search_optimization.py
--rw-rw-rw-   0        0        0     5238 2024-05-18 16:32:58.000000 Maslib-0.0.3/MasLib/regression.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:50:42.225310 Maslib-0.0.3/Maslib.egg-info/
--rw-rw-rw-   0        0        0      799 2024-05-19 10:50:42.000000 Maslib-0.0.3/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-05-19 10:50:42.000000 Maslib-0.0.3/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:50:42.000000 Maslib-0.0.3/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-19 10:50:42.000000 Maslib-0.0.3/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 10:50:42.000000 Maslib-0.0.3/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2024-05-19 10:50:42.226310 Maslib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 10:50:42.228313 Maslib-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-05-19 10:50:32.000000 Maslib-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:50:42.223307 Maslib-0.0.3/tests/
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.3/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.3/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.3/tests/test_grid_search.py
--rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.3/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:08:06.745801 Maslib-0.0.4/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.4/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-19 11:08:06.727784 Maslib-0.0.4/MasLib/
+-rw-rw-rw-   0        0        0      350 2024-05-19 10:55:47.000000 Maslib-0.0.4/MasLib/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.4/MasLib/correlation.py
+-rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.4/MasLib/encoding.py
+-rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.4/MasLib/grid_search_optimization.py
+-rw-rw-rw-   0        0        0     5238 2024-05-18 16:32:58.000000 Maslib-0.0.4/MasLib/regression.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:08:06.742797 Maslib-0.0.4/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-05-19 11:08:06.000000 Maslib-0.0.4/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-19 11:08:06.000000 Maslib-0.0.4/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:08:06.000000 Maslib-0.0.4/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-19 11:08:06.000000 Maslib-0.0.4/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 11:08:06.000000 Maslib-0.0.4/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      799 2024-05-19 11:08:06.744799 Maslib-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:08:06.746801 Maslib-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-19 11:07:47.000000 Maslib-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:08:06.740796 Maslib-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.4/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.4/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.4/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.4/tests/test_regression.py
```

### Comparing `Maslib-0.0.3/MasLib/correlation.py` & `Maslib-0.0.4/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/MasLib/encoding.py` & `Maslib-0.0.4/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/MasLib/grid_search_optimization.py` & `Maslib-0.0.4/MasLib/grid_search_optimization.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/MasLib/regression.py` & `Maslib-0.0.4/MasLib/regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/Maslib.egg-info/PKG-INFO` & `Maslib-0.0.4/Maslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.0.3/PKG-INFO` & `Maslib-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.0.3/setup.py` & `Maslib-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
```

### Comparing `Maslib-0.0.3/tests/test_correlation.py` & `Maslib-0.0.4/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/tests/test_encoding.py` & `Maslib-0.0.4/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/tests/test_grid_search.py` & `Maslib-0.0.4/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.3/tests/test_regression.py` & `Maslib-0.0.4/tests/test_regression.py`

 * *Files identical despite different names*

