# Comparing `tmp/apiframe-0.0.2.tar.gz` & `tmp/apiframe-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiframe-0.0.2.tar", last modified: Sun May 12 07:37:48 2024, max compression
+gzip compressed data, was "apiframe-1.0.0.tar", last modified: Sun May 19 10:27:35 2024, max compression
```

## Comparing `apiframe-0.0.2.tar` & `apiframe-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 07:37:48.146909 apiframe-0.0.2/
--rw-rw-rw-   0        0        0      869 2024-05-12 07:37:48.145387 apiframe-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      423 2024-05-12 07:21:53.000000 apiframe-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 07:37:48.140423 apiframe-0.0.2/apiframe.egg-info/
--rw-rw-rw-   0        0        0      869 2024-05-12 07:37:48.000000 apiframe-0.0.2/apiframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-05-12 07:37:48.000000 apiframe-0.0.2/apiframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 07:37:48.000000 apiframe-0.0.2/apiframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 07:37:48.000000 apiframe-0.0.2/apiframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-12 07:37:48.000000 apiframe-0.0.2/apiframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 07:37:48.144387 apiframe-0.0.2/apiframe_python/
--rw-rw-rw-   0        0        0       32 2024-05-12 06:41:34.000000 apiframe-0.0.2/apiframe_python/__init__.py
--rw-rw-rw-   0        0        0     1150 2024-05-12 07:03:11.000000 apiframe-0.0.2/apiframe_python/main.py
--rw-rw-rw-   0        0        0       42 2024-05-12 07:37:48.146909 apiframe-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      684 2024-05-12 07:37:44.000000 apiframe-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:27:35.800708 apiframe-1.0.0/
+-rw-rw-rw-   0        0        0      883 2024-05-19 10:27:35.799709 apiframe-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2024-05-12 07:21:53.000000 apiframe-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 10:27:35.794204 apiframe-1.0.0/apiframe.egg-info/
+-rw-rw-rw-   0        0        0      883 2024-05-19 10:27:35.000000 apiframe-1.0.0/apiframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-05-19 10:27:35.000000 apiframe-1.0.0/apiframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:27:35.000000 apiframe-1.0.0/apiframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 10:27:35.000000 apiframe-1.0.0/apiframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-19 10:27:35.000000 apiframe-1.0.0/apiframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 10:27:35.797748 apiframe-1.0.0/apiframe_python/
+-rw-rw-rw-   0        0        0       32 2024-05-12 06:41:34.000000 apiframe-1.0.0/apiframe_python/__init__.py
+-rw-rw-rw-   0        0        0    25658 2024-05-19 10:23:03.000000 apiframe-1.0.0/apiframe_python/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:27:35.801958 apiframe-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      703 2024-05-19 10:23:27.000000 apiframe-1.0.0/setup.py
```

### Comparing `apiframe-0.0.2/PKG-INFO` & `apiframe-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: apiframe
-Version: 0.0.2
+Version: 1.0.0
 Summary: A Python client for the Apiframe API
 Home-page: https://github.com/APIFRAME-PRO/apiframe-python
 Author: APIFRAME.PRO
 Author-email: hello@apiframe.pro
+License: MIT
 Keywords: apiframe,midjourney client,midjourney api,api midjourney,midjourney ai api,midjourney bot api,api midjourney api,api midjourney bot,midjourney api access
 Description-Content-Type: text/markdown
 
 # apiframe_python
 Python library for [APIFRAME.PRO](https://apiframe.pro) (Midjourney API)
 
 API Documentation is available at https://docs.apiframe.pro
```

### Comparing `apiframe-0.0.2/apiframe.egg-info/PKG-INFO` & `apiframe-1.0.0/apiframe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: apiframe
-Version: 0.0.2
+Version: 1.0.0
 Summary: A Python client for the Apiframe API
 Home-page: https://github.com/APIFRAME-PRO/apiframe-python
 Author: APIFRAME.PRO
 Author-email: hello@apiframe.pro
+License: MIT
 Keywords: apiframe,midjourney client,midjourney api,api midjourney,midjourney ai api,midjourney bot api,api midjourney api,api midjourney bot,midjourney api access
 Description-Content-Type: text/markdown
 
 # apiframe_python
 Python library for [APIFRAME.PRO](https://apiframe.pro) (Midjourney API)
 
 API Documentation is available at https://docs.apiframe.pro
```

### Comparing `apiframe-0.0.2/setup.py` & `apiframe-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='apiframe',
     url='https://github.com/APIFRAME-PRO/apiframe-python',
-    version='0.0.2',
+    version='1.0.0',
     packages=find_packages(),
     install_requires=['requests'],
     description='A Python client for the Apiframe API',
     author='APIFRAME.PRO',
     author_email='hello@apiframe.pro',
     keywords=['apiframe', 'midjourney client', 'midjourney api', 'api midjourney', 'midjourney ai api', 'midjourney bot api', 'api midjourney api', 'api midjourney bot', 'midjourney api access'],
     long_description=description,
-    long_description_content_type="text/markdown"
+    long_description_content_type="text/markdown",
+    license='MIT'
 )
```

