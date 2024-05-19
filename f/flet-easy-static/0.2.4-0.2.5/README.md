# Comparing `tmp/flet_easy_static-0.2.4.tar.gz` & `tmp/flet_easy_static-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_easy_static-0.2.4.tar", last modified: Sat May 18 17:43:11 2024, max compression
+gzip compressed data, was "flet_easy_static-0.2.5.tar", last modified: Sat May 18 18:00:06 2024, max compression
```

## Comparing `flet_easy_static-0.2.4.tar` & `flet_easy_static-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 17:43:11.607164 flet_easy_static-0.2.4/
--rw-rw-rw-   0        0        0     6959 2024-05-18 17:43:11.607164 flet_easy_static-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     6795 2024-05-18 17:42:05.000000 flet_easy_static-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 17:43:11.598187 flet_easy_static-0.2.4/flet_easy_static/
--rw-rw-rw-   0        0        0      481 2024-05-18 13:38:21.000000 flet_easy_static-0.2.4/flet_easy_static/__init__.py
--rw-rw-rw-   0        0        0     1289 2024-05-18 13:38:21.000000 flet_easy_static-0.2.4/flet_easy_static/auto_route.py
--rw-rw-rw-   0        0        0    12267 2024-05-18 13:36:12.000000 flet_easy_static-0.2.4/flet_easy_static/datasy.py
--rw-rw-rw-   0        0        0      187 2024-05-05 15:12:55.000000 flet_easy_static-0.2.4/flet_easy_static/extra.py
--rw-rw-rw-   0        0        0     2483 2024-05-05 15:12:55.000000 flet_easy_static-0.2.4/flet_easy_static/extrasJwt.py
--rw-rw-rw-   0        0        0    18475 2024-05-18 17:04:32.000000 flet_easy_static-0.2.4/flet_easy_static/fletEasy.py
--rw-rw-rw-   0        0        0     9856 2024-05-05 15:12:55.000000 flet_easy_static-0.2.4/flet_easy_static/inheritance.py
--rw-rw-rw-   0        0        0     1191 2024-05-05 15:12:55.000000 flet_easy_static-0.2.4/flet_easy_static/job.py
--rw-rw-rw-   0        0        0     4045 2024-05-18 13:36:12.000000 flet_easy_static-0.2.4/flet_easy_static/jwt.py
--rw-rw-rw-   0        0        0     7526 2024-05-18 13:36:12.000000 flet_easy_static-0.2.4/flet_easy_static/pagesy.py
--rw-rw-rw-   0        0        0    11213 2024-05-18 13:36:12.000000 flet_easy_static-0.2.4/flet_easy_static/route.py
--rw-rw-rw-   0        0        0     1540 2024-05-05 15:12:55.000000 flet_easy_static-0.2.4/flet_easy_static/view_404.py
-drwxrwxrwx   0        0        0        0 2024-05-18 17:43:11.606166 flet_easy_static-0.2.4/flet_easy_static.egg-info/
--rw-rw-rw-   0        0        0     6959 2024-05-18 17:43:11.000000 flet_easy_static-0.2.4/flet_easy_static.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2024-05-18 17:43:11.000000 flet_easy_static-0.2.4/flet_easy_static.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 17:43:11.000000 flet_easy_static-0.2.4/flet_easy_static.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-18 17:43:11.000000 flet_easy_static-0.2.4/flet_easy_static.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-18 17:43:11.000000 flet_easy_static-0.2.4/flet_easy_static.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 17:43:11.607164 flet_easy_static-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      364 2024-05-18 17:42:39.000000 flet_easy_static-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:00:06.420402 flet_easy_static-0.2.5/
+-rw-rw-rw-   0        0        0     6979 2024-05-18 18:00:06.420402 flet_easy_static-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6815 2024-05-18 17:59:56.000000 flet_easy_static-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 18:00:06.389974 flet_easy_static-0.2.5/flet_easy_static/
+-rw-rw-rw-   0        0        0      481 2024-05-18 13:38:21.000000 flet_easy_static-0.2.5/flet_easy_static/__init__.py
+-rw-rw-rw-   0        0        0     1289 2024-05-18 13:38:21.000000 flet_easy_static-0.2.5/flet_easy_static/auto_route.py
+-rw-rw-rw-   0        0        0    12267 2024-05-18 13:36:12.000000 flet_easy_static-0.2.5/flet_easy_static/datasy.py
+-rw-rw-rw-   0        0        0      187 2024-05-05 15:12:55.000000 flet_easy_static-0.2.5/flet_easy_static/extra.py
+-rw-rw-rw-   0        0        0     2483 2024-05-05 15:12:55.000000 flet_easy_static-0.2.5/flet_easy_static/extrasJwt.py
+-rw-rw-rw-   0        0        0    18475 2024-05-18 17:04:32.000000 flet_easy_static-0.2.5/flet_easy_static/fletEasy.py
+-rw-rw-rw-   0        0        0     9856 2024-05-05 15:12:55.000000 flet_easy_static-0.2.5/flet_easy_static/inheritance.py
+-rw-rw-rw-   0        0        0     1191 2024-05-05 15:12:55.000000 flet_easy_static-0.2.5/flet_easy_static/job.py
+-rw-rw-rw-   0        0        0     4045 2024-05-18 13:36:12.000000 flet_easy_static-0.2.5/flet_easy_static/jwt.py
+-rw-rw-rw-   0        0        0     7526 2024-05-18 13:36:12.000000 flet_easy_static-0.2.5/flet_easy_static/pagesy.py
+-rw-rw-rw-   0        0        0    11213 2024-05-18 13:36:12.000000 flet_easy_static-0.2.5/flet_easy_static/route.py
+-rw-rw-rw-   0        0        0     1540 2024-05-05 15:12:55.000000 flet_easy_static-0.2.5/flet_easy_static/view_404.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:00:06.419405 flet_easy_static-0.2.5/flet_easy_static.egg-info/
+-rw-rw-rw-   0        0        0     6979 2024-05-18 18:00:06.000000 flet_easy_static-0.2.5/flet_easy_static.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2024-05-18 18:00:06.000000 flet_easy_static-0.2.5/flet_easy_static.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:00:06.000000 flet_easy_static-0.2.5/flet_easy_static.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-18 18:00:06.000000 flet_easy_static-0.2.5/flet_easy_static.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-18 18:00:06.000000 flet_easy_static-0.2.5/flet_easy_static.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 18:00:06.421402 flet_easy_static-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      398 2024-05-18 17:59:56.000000 flet_easy_static-0.2.5/setup.py
```

### Comparing `flet_easy_static-0.2.4/PKG-INFO` & `flet_easy_static-0.2.5/flet_easy_static.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flet_easy_static
-Version: 0.2.4
+Name: flet-easy-static
+Version: 0.2.5
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://github.com/Daxexs/flet-easy/blob/main/media/logo.png?raw=true" alt="logo" width="250">
 </div>
 
 
@@ -13,15 +13,15 @@
 
 # Modification 
 `Flet-Easy-Static` is a modification of `Flet-Easy` that allows you to create and publish your `Flet-Easy` project as a static pyodide website
 ### As a result, the following features are not available:
 - Export As AGSI Application is removed (This was the limiting factor for creating a static website since it is not available in the flet-pyodide package)
 - FastAPI Integration is removed (This was the limiting factor for creating a static website since it is not available in the flet-pyodide package)
 - Removed `flet` as a required dependency since `flet-pyodide` is used in the web not the `flet` package
-- Added `PyJWT` as a requirement since it not included in pyodide environment
+- Added `PyJWT` `rsa` `ssl` `parse` as a requirement since it not included in pyodide environment
 ### How To Use:
 - Add `flet-easy-static` to your project `requirements.txt`
 - How To Import Package:
 ```python
 # Method 1: Importing the package as fs in your project (Disadvantage: You will have to import this in you whole project, and also install the package)
 import flet_easy_static as fs
 # Method 2: Check if the platform is emscripten and import the package accordingly (Disadvantage: You will have to import this in you whole project)
```

### Comparing `flet_easy_static-0.2.4/README.md` & `flet_easy_static-0.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Modification 
 `Flet-Easy-Static` is a modification of `Flet-Easy` that allows you to create and publish your `Flet-Easy` project as a static pyodide website
 ### As a result, the following features are not available:
 - Export As AGSI Application is removed (This was the limiting factor for creating a static website since it is not available in the flet-pyodide package)
 - FastAPI Integration is removed (This was the limiting factor for creating a static website since it is not available in the flet-pyodide package)
 - Removed `flet` as a required dependency since `flet-pyodide` is used in the web not the `flet` package
-- Added `PyJWT` as a requirement since it not included in pyodide environment
+- Added `PyJWT` `rsa` `ssl` `parse` as a requirement since it not included in pyodide environment
 ### How To Use:
 - Add `flet-easy-static` to your project `requirements.txt`
 - How To Import Package:
 ```python
 # Method 1: Importing the package as fs in your project (Disadvantage: You will have to import this in you whole project, and also install the package)
 import flet_easy_static as fs
 # Method 2: Check if the platform is emscripten and import the package accordingly (Disadvantage: You will have to import this in you whole project)
```

### Comparing `flet_easy_static-0.2.4/flet_easy_static/auto_route.py` & `flet_easy_static-0.2.5/flet_easy_static/auto_route.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/datasy.py` & `flet_easy_static-0.2.5/flet_easy_static/datasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/extrasJwt.py` & `flet_easy_static-0.2.5/flet_easy_static/extrasJwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/fletEasy.py` & `flet_easy_static-0.2.5/flet_easy_static/fletEasy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/inheritance.py` & `flet_easy_static-0.2.5/flet_easy_static/inheritance.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/job.py` & `flet_easy_static-0.2.5/flet_easy_static/job.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/jwt.py` & `flet_easy_static-0.2.5/flet_easy_static/jwt.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/pagesy.py` & `flet_easy_static-0.2.5/flet_easy_static/pagesy.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/route.py` & `flet_easy_static-0.2.5/flet_easy_static/route.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static/view_404.py` & `flet_easy_static-0.2.5/flet_easy_static/view_404.py`

 * *Files identical despite different names*

### Comparing `flet_easy_static-0.2.4/flet_easy_static.egg-info/PKG-INFO` & `flet_easy_static-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flet-easy-static
-Version: 0.2.4
+Name: flet_easy_static
+Version: 0.2.5
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="https://github.com/Daxexs/flet-easy/blob/main/media/logo.png?raw=true" alt="logo" width="250">
 </div>
 
 
@@ -13,15 +13,15 @@
 
 # Modification 
 `Flet-Easy-Static` is a modification of `Flet-Easy` that allows you to create and publish your `Flet-Easy` project as a static pyodide website
 ### As a result, the following features are not available:
 - Export As AGSI Application is removed (This was the limiting factor for creating a static website since it is not available in the flet-pyodide package)
 - FastAPI Integration is removed (This was the limiting factor for creating a static website since it is not available in the flet-pyodide package)
 - Removed `flet` as a required dependency since `flet-pyodide` is used in the web not the `flet` package
-- Added `PyJWT` as a requirement since it not included in pyodide environment
+- Added `PyJWT` `rsa` `ssl` `parse` as a requirement since it not included in pyodide environment
 ### How To Use:
 - Add `flet-easy-static` to your project `requirements.txt`
 - How To Import Package:
 ```python
 # Method 1: Importing the package as fs in your project (Disadvantage: You will have to import this in you whole project, and also install the package)
 import flet_easy_static as fs
 # Method 2: Check if the platform is emscripten and import the package accordingly (Disadvantage: You will have to import this in you whole project)
```

### Comparing `flet_easy_static-0.2.4/flet_easy_static.egg-info/SOURCES.txt` & `flet_easy_static-0.2.5/flet_easy_static.egg-info/SOURCES.txt`

 * *Files identical despite different names*

