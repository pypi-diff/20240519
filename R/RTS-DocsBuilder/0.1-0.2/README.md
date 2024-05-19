# Comparing `tmp/RTS_DocsBuilder-0.1.tar.gz` & `tmp/RTS_DocsBuilder-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RTS_DocsBuilder-0.1.tar", last modified: Mon Apr 29 17:38:45 2024, max compression
+gzip compressed data, was "RTS_DocsBuilder-0.2.tar", last modified: Sun May 19 10:20:42 2024, max compression
```

## Comparing `RTS_DocsBuilder-0.1.tar` & `RTS_DocsBuilder-0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:38:45.248887 RTS_DocsBuilder-0.1/
--rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_DocsBuilder-0.1/LICENCE
--rw-rw-rw-   0        0        0      869 2024-04-29 17:38:45.248382 RTS_DocsBuilder-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      118 2024-04-29 16:53:23.000000 RTS_DocsBuilder-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:38:45.235326 RTS_DocsBuilder-0.1/RTS_DocsBuilder/
--rw-rw-rw-   0        0        0     5795 2024-04-29 15:39:29.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder/RInitiate.py
--rw-rw-rw-   0        0        0        0 2024-04-28 07:42:27.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder/__init__.py
--rw-rw-rw-   0        0        0    10655 2024-04-29 16:06:45.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder/doclayout.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:38:45.247378 RTS_DocsBuilder-0.1/RTS_DocsBuilder.egg-info/
--rw-rw-rw-   0        0        0      869 2024-04-29 17:38:45.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-29 17:38:45.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:38:45.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 17:38:45.000000 RTS_DocsBuilder-0.1/RTS_DocsBuilder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 17:38:45.248887 RTS_DocsBuilder-0.1/setup.cfg
--rw-rw-rw-   0        0        0      920 2024-04-29 17:37:59.000000 RTS_DocsBuilder-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:20:42.615400 RTS_DocsBuilder-0.2/
+-rw-rw-rw-   0        0        0     1349 2024-04-01 09:09:39.000000 RTS_DocsBuilder-0.2/LICENCE
+-rw-rw-rw-   0        0        0      869 2024-05-19 10:20:42.614893 RTS_DocsBuilder-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      118 2024-04-29 16:53:23.000000 RTS_DocsBuilder-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 10:20:42.598597 RTS_DocsBuilder-0.2/RTS_DocsBuilder/
+-rw-rw-rw-   0        0        0     5757 2024-05-19 10:20:36.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder/RInitiate.py
+-rw-rw-rw-   0        0        0        0 2024-04-28 07:42:27.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder/__init__.py
+-rw-rw-rw-   0        0        0    10655 2024-04-29 16:06:45.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder/doclayout.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:20:42.613889 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/
+-rw-rw-rw-   0        0        0      869 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-19 10:20:42.000000 RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:20:42.615400 RTS_DocsBuilder-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      938 2024-04-29 17:41:43.000000 RTS_DocsBuilder-0.2/setup.py
```

### Comparing `RTS_DocsBuilder-0.1/LICENCE` & `RTS_DocsBuilder-0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `RTS_DocsBuilder-0.1/PKG-INFO` & `RTS_DocsBuilder-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS_DocsBuilder
-Version: 0.1
+Version: 0.2
 Summary: Create local documentations for your modules. Requires RTS_WebUIBuilder.
 Home-page: https://github.com/RandomTimeLP/RTS_Documentations
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Work in Progress,Documentations
 Platform: UNKNOWN
```

### Comparing `RTS_DocsBuilder-0.1/RTS_DocsBuilder/RInitiate.py` & `RTS_DocsBuilder-0.2/RTS_DocsBuilder/RInitiate.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     def __init__(self):
         try:
             from RTS_WebUIBuilder import rtswuib_cache
             ws = None
             while ws is None:
                 ws = rtswuib_cache.MAIN_WEBSERVER
                 if ws is None:
-                    print("⚠️  Webserver is not running yet. Waiting...")
                     time.sleep(1)  # Wait for 1 second before checking again
                 else:
-                    print("✅  Webserver is running.")
-                    ws.enableSourceRoute(os.path.normpath(os.path.join(os.getcwd(),"RTS_Documentations", "srcFolder")))
+                    modul_pfad = os.path.dirname(os.path.abspath(__file__))
+                    ziel_pfad = os.path.normpath(os.path.join(modul_pfad, "srcFolder"))
+                    ws.enableSourceRoute(ziel_pfad)
         except ImportError:
             print("⚠️  You may not remove the dependency module 'RTS_WebUIBuilder'.")
             return
     
         self.topics:list = []
         self.subtopics:list = []
         self.initiator:list = []
```

### Comparing `RTS_DocsBuilder-0.1/RTS_DocsBuilder/doclayout.py` & `RTS_DocsBuilder-0.2/RTS_DocsBuilder/doclayout.py`

 * *Files identical despite different names*

### Comparing `RTS_DocsBuilder-0.1/RTS_DocsBuilder.egg-info/PKG-INFO` & `RTS_DocsBuilder-0.2/RTS_DocsBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RTS-DocsBuilder
-Version: 0.1
+Version: 0.2
 Summary: Create local documentations for your modules. Requires RTS_WebUIBuilder.
 Home-page: https://github.com/RandomTimeLP/RTS_Documentations
 Author: RandomTimeTV
 Author-email: dergepanzerte1@gmail.com
 License: MIT with required credit to the author.
 Keywords: Work in Progress,Documentations
 Platform: UNKNOWN
```

### Comparing `RTS_DocsBuilder-0.1/setup.py` & `RTS_DocsBuilder-0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RTS_DocsBuilder',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='Create local documentations for your modules. Requires RTS_WebUIBuilder.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='RandomTimeTV',
     author_email='dergepanzerte1@gmail.com',
     license='MIT with required credit to the author.',
@@ -16,9 +16,9 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords='Work in Progress, Documentations',
-    install_requires=[],
+    install_requires=["RTS-WebUIBuilder"],
 )
```

