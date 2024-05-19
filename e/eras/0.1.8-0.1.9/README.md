# Comparing `tmp/eras-0.1.8.tar.gz` & `tmp/eras-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.1.8.tar", last modified: Sun May 19 20:24:55 2024, max compression
+gzip compressed data, was "eras-0.1.9.tar", last modified: Sun May 19 20:35:43 2024, max compression
```

## Comparing `eras-0.1.8.tar` & `eras-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:24:55.405360 eras-0.1.8/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.8/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.8/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:24:55.405051 eras-0.1.8/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.8/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 20:24:55.405422 eras-0.1.8/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1300 2024-05-19 20:19:53.000000 eras-0.1.8/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:24:55.402541 eras-0.1.8/src/
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:24:55.404681 eras-0.1.8/src/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:24:55.000000 eras-0.1.8/src/eras.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:35:43.697155 eras-0.1.9/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.9/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.9/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:35:43.696841 eras-0.1.9/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.9/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:35:43.694390 eras-0.1.9/eras/
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:35:43.696467 eras-0.1.9/eras/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:35:43.000000 eras-0.1.9/eras/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      238 2024-05-19 20:35:43.000000 eras-0.1.9/eras/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:35:43.000000 eras-0.1.9/eras/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 20:35:43.000000 eras-0.1.9/eras/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 20:35:43.000000 eras-0.1.9/eras/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:35:43.000000 eras-0.1.9/eras/eras.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 20:35:43.697223 eras-0.1.9/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1302 2024-05-19 20:35:32.000000 eras-0.1.9/setup.py
```

### Comparing `eras-0.1.8/PKG-INFO` & `eras-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.8
+Version: 0.1.9
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.1.8/setup.py` & `eras-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     def run(self):
         install.run(self)
         # Run the post_install.py script after installation
         subprocess.call([sys.executable, 'src/post_install.py'])
 
 setup(
     name='eras',
-    version='0.1.8',
-    package_dir={'': 'src'},
-    packages=find_packages(where='src'),
+    version='0.1.9',
+    package_dir={'': 'eras'},
+    packages=find_packages(where='eras'),
     install_requires=[
         'openai==1.26.0',
         'keyboard==0.13.5',
         'python-dotenv==1.0.0',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `eras-0.1.8/src/eras.egg-info/PKG-INFO` & `eras-0.1.9/eras/eras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.8
+Version: 0.1.9
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

