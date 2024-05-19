# Comparing `tmp/extrautilities-1.0.tar.gz` & `tmp/extrautilities-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrautilities-1.0.tar", last modified: Sat May 18 11:20:09 2024, max compression
+gzip compressed data, was "extrautilities-1.1.tar", last modified: Sun May 19 10:11:31 2024, max compression
```

## Comparing `extrautilities-1.0.tar` & `extrautilities-1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 11:20:09.617848 extrautilities-1.0/
-drwxrwxrwx   0        0        0        0 2024-05-18 11:20:09.598828 extrautilities-1.0/ExtraUtils/
--rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.0/ExtraUtils/RateLimit.py
--rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.0/ExtraUtils/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-1.0/ExtraUtils/asyncTokens.py
--rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.0/ExtraUtils/getFileContent.py
--rw-rw-rw-   0        0        0     4453 2024-05-16 16:25:09.000000 extrautilities-1.0/ExtraUtils/timeBasedToken.py
--rw-rw-rw-   0        0        0     3322 2024-05-18 11:20:09.617348 extrautilities-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 11:20:09.616844 extrautilities-1.0/extrautilities.egg-info/
--rw-rw-rw-   0        0        0     3322 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 11:20:09.000000 extrautilities-1.0/extrautilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 11:20:09.617848 extrautilities-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1103 2024-05-18 11:20:01.000000 extrautilities-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:11:31.951259 extrautilities-1.1/
+drwxrwxrwx   0        0        0        0 2024-05-19 10:11:31.934270 extrautilities-1.1/ExtraUtils/
+-rw-rw-rw-   0        0        0     2498 2024-05-12 11:47:12.000000 extrautilities-1.1/ExtraUtils/RateLimit.py
+-rw-rw-rw-   0        0        0       34 2024-05-12 10:56:58.000000 extrautilities-1.1/ExtraUtils/__init__.py
+-rw-rw-rw-   0        0        0     1766 2024-05-13 18:01:30.000000 extrautilities-1.1/ExtraUtils/asyncTokens.py
+-rw-rw-rw-   0        0        0       46 2024-05-19 10:08:26.000000 extrautilities-1.1/ExtraUtils/callbackVoid.py
+-rw-rw-rw-   0        0        0     2851 2024-05-18 11:19:25.000000 extrautilities-1.1/ExtraUtils/getFileContent.py
+-rw-rw-rw-   0        0        0     4453 2024-05-16 16:25:09.000000 extrautilities-1.1/ExtraUtils/timeBasedToken.py
+-rw-rw-rw-   0        0        0     3335 2024-05-19 10:11:31.950254 extrautilities-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2457 2024-05-16 14:51:40.000000 extrautilities-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 10:11:31.950254 extrautilities-1.1/extrautilities.egg-info/
+-rw-rw-rw-   0        0        0     3335 2024-05-19 10:11:31.000000 extrautilities-1.1/extrautilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2024-05-19 10:11:31.000000 extrautilities-1.1/extrautilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:11:31.000000 extrautilities-1.1/extrautilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:11:31.000000 extrautilities-1.1/extrautilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 10:11:31.000000 extrautilities-1.1/extrautilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:11:31.951259 extrautilities-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-19 10:08:50.000000 extrautilities-1.1/setup.py
```

### Comparing `extrautilities-1.0/ExtraUtils/RateLimit.py` & `extrautilities-1.1/ExtraUtils/RateLimit.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.0/ExtraUtils/asyncTokens.py` & `extrautilities-1.1/ExtraUtils/asyncTokens.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.0/ExtraUtils/getFileContent.py` & `extrautilities-1.1/ExtraUtils/getFileContent.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.0/ExtraUtils/timeBasedToken.py` & `extrautilities-1.1/ExtraUtils/timeBasedToken.py`

 * *Files identical despite different names*

### Comparing `extrautilities-1.0/PKG-INFO` & `extrautilities-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.0
+Version: 1.1
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit,timeBasedToken,getFileContent
+Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `extrautilities-1.0/README.md` & `extrautilities-1.1/README.md`

 * *Files identical despite different names*

### Comparing `extrautilities-1.0/extrautilities.egg-info/PKG-INFO` & `extrautilities-1.1/extrautilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: extrautilities
-Version: 1.0
+Version: 1.1
 Summary: This package provides a few extra utilities for Python, like a "RateLimiter" class.
 Home-page: https://github.com/RandomTimeLP/ExtraUtils
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: Unlicensed
-Keywords: RateLimit,timeBasedToken,getFileContent
+Keywords: RateLimit,timeBasedToken,getFileContent,callbackVoid
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `extrautilities-1.0/setup.py` & `extrautilities-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='extrautilities',
-    version='1.0',
+    version='1.1',
     packages=find_packages(),
     description='This package provides a few extra utilities for Python, like a "RateLimiter" class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='Unlicensed',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    keywords='RateLimit, timeBasedToken, getFileContent',
+    keywords='RateLimit, timeBasedToken, getFileContent, callbackVoid',
     install_requires=["extradecorators", "cryptography","pycryptodome"],
 )
```

