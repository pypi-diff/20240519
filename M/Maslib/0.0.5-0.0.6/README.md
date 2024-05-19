# Comparing `tmp/Maslib-0.0.5.tar.gz` & `tmp/Maslib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.0.5.tar", last modified: Sun May 19 11:11:30 2024, max compression
+gzip compressed data, was "Maslib-0.0.6.tar", last modified: Sun May 19 11:13:43 2024, max compression
```

## Comparing `Maslib-0.0.5.tar` & `Maslib-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 11:11:30.737958 Maslib-0.0.5/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-19 11:11:30.721941 Maslib-0.0.5/MasLib/
--rw-rw-rw-   0        0        0      350 2024-05-19 10:55:47.000000 Maslib-0.0.5/MasLib/__init__.py
--rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.5/MasLib/correlation.py
--rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.5/MasLib/encoding.py
--rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.5/MasLib/grid_search_optimization.py
--rw-rw-rw-   0        0        0     5238 2024-05-18 16:32:58.000000 Maslib-0.0.5/MasLib/regression.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:11:30.735957 Maslib-0.0.5/Maslib.egg-info/
--rw-rw-rw-   0        0        0      799 2024-05-19 11:11:30.000000 Maslib-0.0.5/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-05-19 11:11:30.000000 Maslib-0.0.5/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 11:11:30.000000 Maslib-0.0.5/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-19 11:11:30.000000 Maslib-0.0.5/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 11:11:30.000000 Maslib-0.0.5/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2024-05-19 11:11:30.736957 Maslib-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 11:11:30.737958 Maslib-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      766 2024-05-19 11:10:46.000000 Maslib-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:11:30.733955 Maslib-0.0.5/tests/
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.5/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.5/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.5/tests/test_grid_search.py
--rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.5/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.590384 Maslib-0.0.6/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.558355 Maslib-0.0.6/MasLib/
+-rw-rw-rw-   0        0        0      350 2024-05-19 10:55:47.000000 Maslib-0.0.6/MasLib/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.6/MasLib/correlation.py
+-rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.6/MasLib/encoding.py
+-rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.6/MasLib/grid_search_optimization.py
+-rw-rw-rw-   0        0        0     5232 2024-05-19 11:12:32.000000 Maslib-0.0.6/MasLib/regression.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.586380 Maslib-0.0.6/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      799 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 11:13:43.000000 Maslib-0.0.6/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      799 2024-05-19 11:13:43.588382 Maslib-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:13:43.590384 Maslib-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      766 2024-05-19 11:13:12.000000 Maslib-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:13:43.584379 Maslib-0.0.6/tests/
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.6/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.6/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.6/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.6/tests/test_regression.py
```

### Comparing `Maslib-0.0.5/MasLib/correlation.py` & `Maslib-0.0.6/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.5/MasLib/encoding.py` & `Maslib-0.0.6/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.5/MasLib/grid_search_optimization.py` & `Maslib-0.0.6/MasLib/grid_search_optimization.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.5/MasLib/regression.py` & `Maslib-0.0.6/MasLib/regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sklearn.ensemble import GradientBoostingRegressor, RandomForestRegressor
 from sklearn.linear_model import LinearRegression
 from catboost import CatBoostRegressor
 from sklearn.metrics import mean_absolute_error, mean_squared_error
 from sklearn.model_selection import cross_val_score
 import numpy as np
 
-def gb_boost_regression(X_train, X_test, y_train, y_test):
+def gb_regression(X_train, X_test, y_train, y_test):
     """
     Функция для тренировки и оценки модели CatBoostRegression.
 
     Parameters:
     X_train: обучающая выборка признаков
     X_test: тестовая выборка признаков
     y_train: обучающая выборка целевой переменной
```

### Comparing `Maslib-0.0.5/Maslib.egg-info/PKG-INFO` & `Maslib-0.0.6/Maslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.0.5/PKG-INFO` & `Maslib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.5
+Version: 0.0.6
 Summary: Это моя библиотека для оптимизации кода для python
 Author: Alecsandr_C.V.V
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `Maslib-0.0.5/setup.py` & `Maslib-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
         'scikit-learn',
```

### Comparing `Maslib-0.0.5/tests/test_correlation.py` & `Maslib-0.0.6/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.5/tests/test_encoding.py` & `Maslib-0.0.6/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.5/tests/test_grid_search.py` & `Maslib-0.0.6/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.5/tests/test_regression.py` & `Maslib-0.0.6/tests/test_regression.py`

 * *Files identical despite different names*
