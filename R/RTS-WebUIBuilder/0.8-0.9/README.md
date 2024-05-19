# Comparing `tmp/RTS-WebUIBuilder-0.8.tar.gz` & `tmp/RTS-WebUIBuilder-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS-WebUIBuilder-0.8.tar", last modified: Sun May 19 11:19:32 2024, max compression
+gzip compressed data, was "RTS-WebUIBuilder-0.9.tar", last modified: Sun May 19 11:25:25 2024, max compression
```

## Comparing `RTS-WebUIBuilder-0.8.tar` & `RTS-WebUIBuilder-0.9.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 11:19:32.880777 RTS-WebUIBuilder-0.8/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS-WebUIBuilder-0.8/LICENCE
--rw-rw-rw-   0        0        0      823 2024-05-19 11:19:32.880150 RTS-WebUIBuilder-0.8/PKG-INFO
--rw-rw-rw-   0        0        0       92 2024-04-29 16:57:15.000000 RTS-WebUIBuilder-0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 11:19:32.865366 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/
--rw-rw-rw-   0        0        0     1055 2024-04-15 18:28:33.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RAdditions.py
--rw-rw-rw-   0        0        0     2282 2024-04-29 16:01:41.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RBody.py
--rw-rw-rw-   0        0        0     2718 2024-04-28 15:20:36.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RBox.py
--rw-rw-rw-   0        0        0     3233 2024-04-29 15:07:44.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RDocument.py
--rw-rw-rw-   0        0        0     2320 2024-04-13 14:53:29.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RFrame.py
--rw-rw-rw-   0        0        0    10637 2024-04-24 17:48:28.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RGroupStyle.py
--rw-rw-rw-   0        0        0     1261 2024-04-13 14:44:52.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RHead.py
--rw-rw-rw-   0        0        0       92 2024-04-13 18:50:09.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RImage.py
--rw-rw-rw-   0        0        0     2754 2024-04-21 08:51:23.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RInput.py
--rw-rw-rw-   0        0        0      839 2024-04-26 21:26:34.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RLabel.py
--rw-rw-rw-   0        0        0      326 2024-04-27 16:51:27.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RQuickScripts.py
--rw-rw-rw-   0        0        0    10454 2024-04-24 17:44:53.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RStyle.py
--rw-rw-rw-   0        0        0      796 2024-04-28 18:56:26.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RTitle.py
--rw-rw-rw-   0        0        0     6142 2024-05-05 15:26:16.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RWebserver.py
--rw-rw-rw-   0        0        0     3523 2024-04-29 16:16:05.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RpyColorizer.py
--rw-rw-rw-   0        0        0      538 2024-05-19 11:18:34.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/__init__.py
--rw-rw-rw-   0        0        0      370 2024-04-13 17:25:24.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/cache.py
--rw-rw-rw-   0        0        0      888 2024-04-29 15:07:12.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/exeptional.py
--rw-rw-rw-   0        0        0     1015 2024-04-21 15:08:22.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/privatizehead.py
-drwxrwxrwx   0        0        0        0 2024-05-19 11:19:32.878644 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-19 11:19:32.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2024-05-19 11:19:32.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 11:19:32.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 11:19:32.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-19 11:19:32.000000 RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 11:19:32.880777 RTS-WebUIBuilder-0.8/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-05-19 11:19:15.000000 RTS-WebUIBuilder-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:25:25.303711 RTS-WebUIBuilder-0.9/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS-WebUIBuilder-0.9/LICENCE
+-rw-rw-rw-   0        0        0      823 2024-05-19 11:25:25.303711 RTS-WebUIBuilder-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2024-04-29 16:57:15.000000 RTS-WebUIBuilder-0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 11:25:25.288556 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/
+-rw-rw-rw-   0        0        0     1055 2024-04-15 18:28:33.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RAdditions.py
+-rw-rw-rw-   0        0        0     2282 2024-04-29 16:01:41.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RBody.py
+-rw-rw-rw-   0        0        0     2718 2024-04-28 15:20:36.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RBox.py
+-rw-rw-rw-   0        0        0     3233 2024-04-29 15:07:44.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RDocument.py
+-rw-rw-rw-   0        0        0     2320 2024-04-13 14:53:29.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RFrame.py
+-rw-rw-rw-   0        0        0    10637 2024-04-24 17:48:28.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RGroupStyle.py
+-rw-rw-rw-   0        0        0     1261 2024-04-13 14:44:52.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RHead.py
+-rw-rw-rw-   0        0        0       92 2024-04-13 18:50:09.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RImage.py
+-rw-rw-rw-   0        0        0     2754 2024-04-21 08:51:23.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RInput.py
+-rw-rw-rw-   0        0        0      839 2024-04-26 21:26:34.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RLabel.py
+-rw-rw-rw-   0        0        0      326 2024-04-27 16:51:27.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RQuickScripts.py
+-rw-rw-rw-   0        0        0    10454 2024-04-24 17:44:53.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RStyle.py
+-rw-rw-rw-   0        0        0      796 2024-04-28 18:56:26.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RTitle.py
+-rw-rw-rw-   0        0        0     6142 2024-05-05 15:26:16.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RWebserver.py
+-rw-rw-rw-   0        0        0     3523 2024-04-29 16:16:05.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RpyColorizer.py
+-rw-rw-rw-   0        0        0      538 2024-05-19 11:18:34.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/__init__.py
+-rw-rw-rw-   0        0        0      370 2024-04-13 17:25:24.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/cache.py
+-rw-rw-rw-   0        0        0      888 2024-04-29 15:07:12.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/exeptional.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:25:25.302404 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/presets/
+-rw-rw-rw-   0        0        0     1336 2024-04-26 21:27:46.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/presets/Button1.py
+-rw-rw-rw-   0        0        0        0 2024-05-19 11:25:15.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/presets/__init__.py
+-rw-rw-rw-   0        0        0     1015 2024-04-21 15:08:22.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/privatizehead.py
+drwxrwxrwx   0        0        0        0 2024-05-19 11:25:25.299891 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-19 11:25:25.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2024-05-19 11:25:25.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 11:25:25.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 11:25:25.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 11:25:25.000000 RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 11:25:25.303711 RTS-WebUIBuilder-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-05-19 11:25:23.000000 RTS-WebUIBuilder-0.9/setup.py
```

### Comparing `RTS-WebUIBuilder-0.8/LICENCE` & `RTS-WebUIBuilder-0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/PKG-INFO` & `RTS-WebUIBuilder-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-WebUIBuilder
-Version: 0.8
+Version: 0.9
 Summary: A simple webserver with a simple webui builder.
 Home-page: https://github.com/RandomTimeLP/RTS_Webbuilder
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: WebUIBuilder,Webserver,Work In Progress
 Platform: UNKNOWN
```

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RAdditions.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RAdditions.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RBody.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RBody.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RBox.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RBox.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RDocument.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RDocument.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RFrame.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RFrame.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RGroupStyle.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RGroupStyle.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RHead.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RHead.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RInput.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RInput.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RLabel.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RLabel.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RStyle.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RStyle.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RTitle.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RTitle.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RWebserver.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RWebserver.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/RpyColorizer.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/RpyColorizer.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/__init__.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/exeptional.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/exeptional.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder/privatizehead.py` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder/privatizehead.py`

 * *Files identical despite different names*

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/PKG-INFO` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-WebUIBuilder
-Version: 0.8
+Version: 0.9
 Summary: A simple webserver with a simple webui builder.
 Home-page: https://github.com/RandomTimeLP/RTS_Webbuilder
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: WebUIBuilder,Webserver,Work In Progress
 Platform: UNKNOWN
```

### Comparing `RTS-WebUIBuilder-0.8/RTS_WebUIBuilder.egg-info/SOURCES.txt` & `RTS-WebUIBuilder-0.9/RTS_WebUIBuilder.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 RTS_WebUIBuilder/cache.py
 RTS_WebUIBuilder/exeptional.py
 RTS_WebUIBuilder/privatizehead.py
 RTS_WebUIBuilder.egg-info/PKG-INFO
 RTS_WebUIBuilder.egg-info/SOURCES.txt
 RTS_WebUIBuilder.egg-info/dependency_links.txt
 RTS_WebUIBuilder.egg-info/requires.txt
-RTS_WebUIBuilder.egg-info/top_level.txt
+RTS_WebUIBuilder.egg-info/top_level.txt
+RTS_WebUIBuilder/presets/Button1.py
+RTS_WebUIBuilder/presets/__init__.py
```

### Comparing `RTS-WebUIBuilder-0.8/setup.py` & `RTS-WebUIBuilder-0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS-WebUIBuilder',
-    version='0.8',
+    version='0.9',
     packages=find_packages(),
     description='A simple webserver with a simple webui builder.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
```

