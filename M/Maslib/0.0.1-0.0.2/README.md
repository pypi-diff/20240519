# Comparing `tmp/Maslib-0.0.1.tar.gz` & `tmp/Maslib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Maslib-0.0.1.tar", last modified: Sat May 18 17:27:26 2024, max compression
+gzip compressed data, was "Maslib-0.0.2.tar", last modified: Sat May 18 17:40:11 2024, max compression
```

## Comparing `Maslib-0.0.1.tar` & `Maslib-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 17:27:26.048780 Maslib-0.0.1/
--rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2024-05-18 17:27:26.029762 Maslib-0.0.1/MasLib/
--rw-rw-rw-   0        0        0      344 2024-05-18 17:23:43.000000 Maslib-0.0.1/MasLib/__init__.py
--rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.1/MasLib/correlation.py
--rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.1/MasLib/encoding.py
--rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.1/MasLib/grid_search_optimization.py
--rw-rw-rw-   0        0        0     5238 2024-05-18 16:32:58.000000 Maslib-0.0.1/MasLib/regression.py
-drwxrwxrwx   0        0        0        0 2024-05-18 17:27:26.046779 Maslib-0.0.1/Maslib.egg-info/
--rw-rw-rw-   0        0        0      879 2024-05-18 17:27:25.000000 Maslib-0.0.1/Maslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-05-18 17:27:25.000000 Maslib-0.0.1/Maslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 17:27:25.000000 Maslib-0.0.1/Maslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-18 17:27:25.000000 Maslib-0.0.1/Maslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-18 17:27:25.000000 Maslib-0.0.1/Maslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      879 2024-05-18 17:27:26.047780 Maslib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-18 17:27:26.048780 Maslib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      844 2024-05-18 17:06:05.000000 Maslib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 17:27:26.045778 Maslib-0.0.1/tests/
--rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.1/tests/test_correlation.py
--rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.1/tests/test_encoding.py
--rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.1/tests/test_grid_search.py
--rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.1/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-05-18 17:40:11.673195 Maslib-0.0.2/
+-rw-rw-rw-   0        0        0       19 2024-05-18 17:23:43.000000 Maslib-0.0.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2024-05-18 17:40:11.658182 Maslib-0.0.2/MasLib/
+-rw-rw-rw-   0        0        0      344 2024-05-18 17:23:43.000000 Maslib-0.0.2/MasLib/__init__.py
+-rw-rw-rw-   0        0        0     1598 2024-05-18 17:23:43.000000 Maslib-0.0.2/MasLib/correlation.py
+-rw-rw-rw-   0        0        0      937 2024-05-18 16:33:03.000000 Maslib-0.0.2/MasLib/encoding.py
+-rw-rw-rw-   0        0        0     2383 2024-05-18 16:56:08.000000 Maslib-0.0.2/MasLib/grid_search_optimization.py
+-rw-rw-rw-   0        0        0     5238 2024-05-18 16:32:58.000000 Maslib-0.0.2/MasLib/regression.py
+drwxrwxrwx   0        0        0        0 2024-05-18 17:40:11.671194 Maslib-0.0.2/Maslib.egg-info/
+-rw-rw-rw-   0        0        0      884 2024-05-18 17:40:11.000000 Maslib-0.0.2/Maslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-18 17:40:11.000000 Maslib-0.0.2/Maslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 17:40:11.000000 Maslib-0.0.2/Maslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-18 17:40:11.000000 Maslib-0.0.2/Maslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 17:40:11.000000 Maslib-0.0.2/Maslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      884 2024-05-18 17:40:11.672194 Maslib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-18 17:06:26.000000 Maslib-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-18 17:40:11.673195 Maslib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      849 2024-05-18 17:39:16.000000 Maslib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 17:40:11.669192 Maslib-0.0.2/tests/
+-rw-rw-rw-   0        0        0     1419 2024-05-18 17:23:43.000000 Maslib-0.0.2/tests/test_correlation.py
+-rw-rw-rw-   0        0        0     1477 2024-05-18 17:23:43.000000 Maslib-0.0.2/tests/test_encoding.py
+-rw-rw-rw-   0        0        0     2625 2024-05-18 17:23:43.000000 Maslib-0.0.2/tests/test_grid_search.py
+-rw-rw-rw-   0        0        0     2328 2024-05-18 17:00:25.000000 Maslib-0.0.2/tests/test_regression.py
```

### Comparing `Maslib-0.0.1/MasLib/correlation.py` & `Maslib-0.0.2/MasLib/correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/MasLib/encoding.py` & `Maslib-0.0.2/MasLib/encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/MasLib/grid_search_optimization.py` & `Maslib-0.0.2/MasLib/grid_search_optimization.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/MasLib/regression.py` & `Maslib-0.0.2/MasLib/regression.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/Maslib.egg-info/PKG-INFO` & `Maslib-0.0.2/Maslib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Это моя библиотека для оптимизации кода для python
 Home-page: https://github.com/yourusername/MasLib
 Author: Александр В.В
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: phik
 Requires-Dist: matplotlib
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: unittest
 
 # mylib
 
 mylib - СЌС‚Рѕ Р±РёР±Р»РёРѕС‚РµРєР° Python РґР»СЏ СѓРјРµРЅСЊС€РµРЅРёСЏ РєРѕРґР°
 ## РЈСЃС‚Р°РЅРѕРІРєР°
```

### Comparing `Maslib-0.0.1/PKG-INFO` & `Maslib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Maslib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Это моя библиотека для оптимизации кода для python
 Home-page: https://github.com/yourusername/MasLib
 Author: Александр В.В
 Author-email: dxomko@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: phik
 Requires-Dist: matplotlib
-Requires-Dist: sklearn
+Requires-Dist: scikit-learn
 Requires-Dist: catboost
 Requires-Dist: unittest
 
 # mylib
 
 mylib - СЌС‚Рѕ Р±РёР±Р»РёРѕС‚РµРєР° Python РґР»СЏ СѓРјРµРЅСЊС€РµРЅРёСЏ РєРѕРґР°
 ## РЈСЃС‚Р°РЅРѕРІРєР°
```

### Comparing `Maslib-0.0.1/setup.py` & `Maslib-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Maslib',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'phik',
         'matplotlib',
-        'sklearn',
+        'scikit-learn',
         'catboost',
         'unittest',
 
     ],
     author='Александр В.В',
     author_email='dxomko@gmail.com',
     description='Это моя библиотека для оптимизации кода для python',
```

### Comparing `Maslib-0.0.1/tests/test_correlation.py` & `Maslib-0.0.2/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/tests/test_encoding.py` & `Maslib-0.0.2/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/tests/test_grid_search.py` & `Maslib-0.0.2/tests/test_grid_search.py`

 * *Files identical despite different names*

### Comparing `Maslib-0.0.1/tests/test_regression.py` & `Maslib-0.0.2/tests/test_regression.py`

 * *Files identical despite different names*

