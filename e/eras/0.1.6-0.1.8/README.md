# Comparing `tmp/eras-0.1.6.tar.gz` & `tmp/eras-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.1.6.tar", last modified: Sun May 19 20:09:50 2024, max compression
+gzip compressed data, was "eras-0.1.8.tar", last modified: Sun May 19 20:24:55 2024, max compression
```

## Comparing `eras-0.1.6.tar` & `eras-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:09:50.818836 eras-0.1.6/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.6/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.6/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:09:50.818322 eras-0.1.6/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.6/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 20:09:50.818909 eras-0.1.6/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1302 2024-05-19 20:09:41.000000 eras-0.1.6/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:09:50.815453 eras-0.1.6/src/
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:09:50.817804 eras-0.1.6/src/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:09:50.000000 eras-0.1.6/src/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 20:09:50.000000 eras-0.1.6/src/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:09:50.000000 eras-0.1.6/src/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 20:09:50.000000 eras-0.1.6/src/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 20:09:50.000000 eras-0.1.6/src/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:09:50.000000 eras-0.1.6/src/eras.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:24:55.405360 eras-0.1.8/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.8/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.8/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:24:55.405051 eras-0.1.8/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.8/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 20:24:55.405422 eras-0.1.8/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1300 2024-05-19 20:19:53.000000 eras-0.1.8/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:24:55.402541 eras-0.1.8/src/
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:24:55.404681 eras-0.1.8/src/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/top_level.txt
```

### Comparing `eras-0.1.6/PKG-INFO` & `eras-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.6
+Version: 0.1.8
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.1.6/setup.py` & `eras-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
 import sys
 
-
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
         # Run the post_install.py script after installation
         subprocess.call([sys.executable, 'src/post_install.py'])
 
-
 setup(
     name='eras',
-    version='0.1.6',
+    version='0.1.8',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     install_requires=[
         'openai==1.26.0',
         'keyboard==0.13.5',
         'python-dotenv==1.0.0',
     ],
```

### Comparing `eras-0.1.6/src/eras.egg-info/PKG-INFO` & `eras-0.1.8/src/eras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.6
+Version: 0.1.8
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

