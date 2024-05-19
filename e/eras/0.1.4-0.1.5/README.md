# Comparing `tmp/eras-0.1.4.tar.gz` & `tmp/eras-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eras-0.1.4.tar", last modified: Sun May 19 20:02:56 2024, max compression
+gzip compressed data, was "eras-0.1.5.tar", last modified: Sun May 19 20:06:50 2024, max compression
```

## Comparing `eras-0.1.4.tar` & `eras-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:02:56.263123 eras-0.1.4/
--rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.4/LICENSE
--rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.4/MANIFEST.in
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:02:56.262813 eras-0.1.4/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.4/README.md
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 20:02:56.263186 eras-0.1.4/setup.cfg
--rw-r--r--   0 jason      (501) staff       (20)     1223 2024-05-19 20:01:58.000000 eras-0.1.4/setup.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:02:56.260081 eras-0.1.4/src/
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:02:56.262432 eras-0.1.4/src/eras.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:02:56.000000 eras-0.1.4/src/eras.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 20:02:56.000000 eras-0.1.4/src/eras.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:02:56.000000 eras-0.1.4/src/eras.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 20:02:56.000000 eras-0.1.4/src/eras.egg-info/entry_points.txt
--rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 20:02:56.000000 eras-0.1.4/src/eras.egg-info/requires.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:02:56.000000 eras-0.1.4/src/eras.egg-info/top_level.txt
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:06:50.824754 eras-0.1.5/
+-rw-r--r--   0 jason      (501) staff       (20)        3 2024-05-19 19:06:16.000000 eras-0.1.5/LICENSE
+-rw-r--r--   0 jason      (501) staff       (20)       33 2024-05-19 19:06:10.000000 eras-0.1.5/MANIFEST.in
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:06:50.824437 eras-0.1.5/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)       82 2024-05-19 18:38:38.000000 eras-0.1.5/README.md
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-05-19 20:06:50.824818 eras-0.1.5/setup.cfg
+-rw-r--r--   0 jason      (501) staff       (20)     1302 2024-05-19 20:06:20.000000 eras-0.1.5/setup.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:06:50.821947 eras-0.1.5/src/
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-05-19 20:06:50.824049 eras-0.1.5/src/eras.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)      676 2024-05-19 20:06:50.000000 eras-0.1.5/src/eras.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)      232 2024-05-19 20:06:50.000000 eras-0.1.5/src/eras.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:06:50.000000 eras-0.1.5/src/eras.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)       35 2024-05-19 20:06:50.000000 eras-0.1.5/src/eras.egg-info/entry_points.txt
+-rw-r--r--   0 jason      (501) staff       (20)       53 2024-05-19 20:06:50.000000 eras-0.1.5/src/eras.egg-info/requires.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-05-19 20:06:50.000000 eras-0.1.5/src/eras.egg-info/top_level.txt
```

### Comparing `eras-0.1.4/PKG-INFO` & `eras-0.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.4
+Version: 0.1.5
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eras-0.1.4/setup.py` & `eras-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
-import os
+import subprocess
 import sys
 
 
 class PostInstallCommand(install):
     """Post-installation for installation mode."""
     def run(self):
         install.run(self)
-        os.system(f"{sys.executable} -m post_install")
+        # Run the post_install.py script after installation
+        subprocess.call([sys.executable, 'src/post_install.py'])
 
 
 setup(
     name='eras',
-    version='0.1.4',
+    version='0.1.5',
     package_dir={'': 'src'},
     packages=find_packages(where='src'),
     install_requires=[
         'openai==1.26.0',
         'keyboard==0.13.5',
         'python-dotenv==1.0.0',
     ],
@@ -37,8 +38,8 @@
     url='https://github.com/jasonmcaffee/eras',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-)
+)
```

### Comparing `eras-0.1.4/src/eras.egg-info/PKG-INFO` & `eras-0.1.5/src/eras.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eras
-Version: 0.1.4
+Version: 0.1.5
 Summary: A terminal command library that provides a Natural Language Interface for running shell commands.
 Home-page: https://github.com/jasonmcaffee/eras
 Author: Jason McAffee
 Author-email: jasonlmcaffee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

