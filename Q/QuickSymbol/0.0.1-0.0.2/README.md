# Comparing `tmp/QuickSymbol-0.0.1.tar.gz` & `tmp/QuickSymbol-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickSymbol-0.0.1.tar", last modified: Sun May 19 12:10:43 2024, max compression
+gzip compressed data, was "QuickSymbol-0.0.2.tar", last modified: Sun May 19 12:53:57 2024, max compression
```

## Comparing `QuickSymbol-0.0.1.tar` & `QuickSymbol-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 12:10:43.732546 QuickSymbol-0.0.1/
--rw-rw-rw-   0        0        0       79 2024-05-19 11:50:24.000000 QuickSymbol-0.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0       25 2024-05-19 11:51:16.000000 QuickSymbol-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      623 2024-05-19 12:10:43.731147 QuickSymbol-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 12:10:43.713460 QuickSymbol-0.0.1/QuickSymbol.egg-info/
--rw-rw-rw-   0        0        0      623 2024-05-19 12:10:43.000000 QuickSymbol-0.0.1/QuickSymbol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-05-19 12:10:43.000000 QuickSymbol-0.0.1/QuickSymbol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 12:10:43.000000 QuickSymbol-0.0.1/QuickSymbol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-19 12:10:43.000000 QuickSymbol-0.0.1/QuickSymbol.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-19 12:10:43.728637 QuickSymbol-0.0.1/QuickSymbols/
--rw-rw-rw-   0        0        0     1038 2024-05-19 11:46:24.000000 QuickSymbol-0.0.1/QuickSymbols/__init__.py
--rw-rw-rw-   0        0        0       50 2024-05-19 11:47:32.000000 QuickSymbol-0.0.1/README.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 12:10:43.732546 QuickSymbol-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      711 2024-05-19 12:00:31.000000 QuickSymbol-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:53:57.116092 QuickSymbol-0.0.2/
+-rw-rw-rw-   0        0        0       79 2024-05-19 12:44:23.000000 QuickSymbol-0.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0       25 2024-05-19 11:51:16.000000 QuickSymbol-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      623 2024-05-19 12:53:57.115093 QuickSymbol-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 12:53:57.114098 QuickSymbol-0.0.2/QuickSymbol.egg-info/
+-rw-rw-rw-   0        0        0      623 2024-05-19 12:53:57.000000 QuickSymbol-0.0.2/QuickSymbol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-19 12:53:57.000000 QuickSymbol-0.0.2/QuickSymbol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:53:57.000000 QuickSymbol-0.0.2/QuickSymbol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:53:57.000000 QuickSymbol-0.0.2/QuickSymbol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       50 2024-05-19 11:47:32.000000 QuickSymbol-0.0.2/README.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:53:57.116092 QuickSymbol-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      711 2024-05-19 12:48:27.000000 QuickSymbol-0.0.2/setup.py
```

### Comparing `QuickSymbol-0.0.1/PKG-INFO` & `QuickSymbol-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickSymbol
-Version: 0.0.1
+Version: 0.0.2
 Summary: A symbol library for simple use
 Home-page: 
 Author: Ibrahim Abushawish
 Author-email: ibrahim.hamed2701@gmail.com
 License: MIT
 Keywords: symbol
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,10 +14,10 @@
 Classifier: Programming Language :: Python :: 3
 
 this is a symbol library for fast use by utf8 code
 
 CHANGE LOG
 ==========
 
-0.0.1 (19/05/2024)
+0.0.2 (19/05/2024)
 ------------------
-First Release
+Fixed Errors
```

### Comparing `QuickSymbol-0.0.1/QuickSymbol.egg-info/PKG-INFO` & `QuickSymbol-0.0.2/QuickSymbol.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuickSymbol
-Version: 0.0.1
+Version: 0.0.2
 Summary: A symbol library for simple use
 Home-page: 
 Author: Ibrahim Abushawish
 Author-email: ibrahim.hamed2701@gmail.com
 License: MIT
 Keywords: symbol
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,10 +14,10 @@
 Classifier: Programming Language :: Python :: 3
 
 this is a symbol library for fast use by utf8 code
 
 CHANGE LOG
 ==========
 
-0.0.1 (19/05/2024)
+0.0.2 (19/05/2024)
 ------------------
-First Release
+Fixed Errors
```

### Comparing `QuickSymbol-0.0.1/setup.py` & `QuickSymbol-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='QuickSymbol',
-  version='0.0.1',
+  version='0.0.2',
   description='A symbol library for simple use',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='Ibrahim Abushawish',
   author_email='ibrahim.hamed2701@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

