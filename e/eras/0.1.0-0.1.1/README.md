# Comparing `tmp/eras-0.1.0.tar.gz` & `tmp/eras-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.1.0.tar", last modified: Sun May 19 19:11:45 2024, max compression
+gzip compressed data, was "eras-0.1.1.tar", last modified: Sun May 19 19:27:33 2024, max compression
```

## Comparing `eras-0.1.0.tar` & `eras-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:11:45.962859 eras-0.1.0/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.0/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.0/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)      640 2024-05-19 19:11:45.962552 eras-0.1.0/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.0/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 19:11:45.962922 eras-0.1.0/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)      987 2024-05-19 19:04:30.000000 eras-0.1.0/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:11:45.960082 eras-0.1.0/src/
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:11:45.962211 eras-0.1.0/src/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)      640 2024-05-19 19:11:45.000000 eras-0.1.0/src/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 19:11:45.000000 eras-0.1.0/src/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:11:45.000000 eras-0.1.0/src/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 19:11:45.000000 eras-0.1.0/src/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       32 2024-05-19 19:11:45.000000 eras-0.1.0/src/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:11:45.000000 eras-0.1.0/src/eras.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:27:33.698104 eras-0.1.1/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.1/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.1/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 19:27:33.697785 eras-0.1.1/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.1/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 19:27:33.698172 eras-0.1.1/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)      905 2024-05-19 19:26:59.000000 eras-0.1.1/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:27:33.695405 eras-0.1.1/src/
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 19:27:33.697420 eras-0.1.1/src/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 19:27:33.000000 eras-0.1.1/src/eras.egg-info/top_level.txt
```

### Comparing `eras-0.1.0/PKG-INFO` & `eras-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.0
+Version: 0.1.1
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
+Requires-Dist: python-dotenv==1.0.0
 
 # ERAS
 Easily Run AI Shell
 Marcus AI is an AI agent capable of performing actions.
```

### Comparing `eras-0.1.0/setup.py` & `eras-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eras',
-    version='0.1.0',
+    version='0.1.1',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     install_requires=[
-        'openai==1.26.0',  # Specify the version here
-        'keyboard==0.13.5',  # Specify the version here
-        # Add other dependencies with their versions here
+        'openai==1.26.0',
+        'keyboard==0.13.5',
+        'python-dotenv==1.0.0',
     ],
     entry_points={
         'console_scripts': [
             'eras=main:main',
         ],
     },
     author='Jason McAffee',
```

### Comparing `eras-0.1.0/src/eras.egg-info/PKG-INFO` & `eras-0.1.1/src/eras.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.0
+Version: 0.1.1
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai==1.26.0
 Requires-Dist: keyboard==0.13.5
+Requires-Dist: python-dotenv==1.0.0
 
 # ERAS
 Easily Run AI Shell
 Marcus AI is an AI agent capable of performing actions.
```

