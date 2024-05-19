# Comparing `tmp/eras-0.1.1.tar.gz` & `tmp/eras-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.1.1.tar", last modified: Sun May 19 19:27:33 2024, max compression
+gzip compressed data, was "eras-0.1.2.tar", last modified: Sun May 19 19:39:54 2024, max compression
```

## Comparing `eras-0.1.1.tar` & `eras-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:27:33.698104 eras-0.1.1/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.1/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.1/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 19:27:33.697785 eras-0.1.1/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.1/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 19:27:33.698172 eras-0.1.1/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)      905 2024-05-19 19:26:59.000000 eras-0.1.1/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:27:33.695405 eras-0.1.1/src/
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:27:33.697420 eras-0.1.1/src/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:39:54.823439 eras-0.1.2/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.2/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.2/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 19:39:54.823111 eras-0.1.2/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.2/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 19:39:54.823499 eras-0.1.2/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)      905 2024-05-19 19:39:46.000000 eras-0.1.2/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:39:54.820618 eras-0.1.2/src/
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:39:54.822739 eras-0.1.2/src/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 19:39:54.000000 eras-0.1.2/src/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 19:39:54.000000 eras-0.1.2/src/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:39:54.000000 eras-0.1.2/src/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 19:39:54.000000 eras-0.1.2/src/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 19:39:54.000000 eras-0.1.2/src/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:39:54.000000 eras-0.1.2/src/eras.egg-info/top_level.txt
```

### Comparing `eras-0.1.1/PKG-INFO` & `eras-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.1
+Version: 0.1.2
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.1.1/setup.py` & `eras-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.1.1',
+    version='0.1.2',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     install_requires=[
         'openai==1.26.0',
         'keyboard==0.13.5',
         'python-dotenv==1.0.0',
     ],
```

### Comparing `eras-0.1.1/src/eras.egg-info/PKG-INFO` & `eras-0.1.2/src/eras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.1
+Version: 0.1.2
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

