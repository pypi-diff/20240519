# Comparing `tmp/testit_adapter_nose-3.1.1.tar.gz` & `tmp/testit_adapter_nose-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_adapter_nose-3.1.1.tar", last modified: Mon May 13 12:53:41 2024, max compression
+gzip compressed data, was "testit_adapter_nose-3.2.0.tar", last modified: Sun May 19 21:52:40 2024, max compression
```

## Comparing `testit_adapter_nose-3.1.1.tar` & `testit_adapter_nose-3.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:41.396862 testit_adapter_nose-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-05-13 12:53:41.396862 testit_adapter_nose-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-05-13 12:53:37.000000 testit_adapter_nose-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:53:41.396862 testit_adapter_nose-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-13 12:53:37.000000 testit_adapter_nose-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:41.396862 testit_adapter_nose-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:41.396862 testit_adapter_nose-3.1.1/src/testit_adapter_nose/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:37.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-13 12:53:37.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-13 12:53:37.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-05-13 12:53:37.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:41.396862 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-05-13 12:53:41.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-13 12:53:41.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:53:41.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 12:53:41.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 12:53:41.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 12:53:41.000000 testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:40.959464 testit_adapter_nose-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-05-19 21:52:40.959464 testit_adapter_nose-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10869 2024-05-19 21:52:36.000000 testit_adapter_nose-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:52:40.959464 testit_adapter_nose-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-19 21:52:36.000000 testit_adapter_nose-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:40.955464 testit_adapter_nose-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:40.955464 testit_adapter_nose-3.2.0/src/testit_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:36.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-19 21:52:36.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-19 21:52:36.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11966 2024-05-19 21:52:36.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:40.959464 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-05-19 21:52:40.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 21:52:40.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:52:40.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-19 21:52:40.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 21:52:40.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 21:52:40.000000 testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/top_level.txt
```

### Comparing `testit_adapter_nose-3.1.1/PKG-INFO` & `testit_adapter_nose-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 3.1.1
+Version: 3.2.0
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: nose2
-Requires-Dist: testit-python-commons==3.1.1
+Requires-Dist: testit-python-commons==3.2.0
 
 # Test IT TMS adapter for Nose
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-nose?style=plastic)](https://pypi.python.org/pypi/testit-adapter-nose)
```

### Comparing `testit_adapter_nose-3.1.1/README.md` & `testit_adapter_nose-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `testit_adapter_nose-3.1.1/setup.py` & `testit_adapter_nose-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testit-adapter-nose',
-    version='3.1.1',
+    version='3.2.0',
     description='Nose adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -19,14 +19,14 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testit-python-commons==3.1.1'],
+    install_requires=['attrs', 'nose2', 'testit-python-commons==3.2.0'],
     entry_points={
             'nose.plugins.0.10': [
                 'testit_adapter_nose = testit_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testit_adapter_nose-3.1.1/src/testit_adapter_nose/listener.py` & `testit_adapter_nose-3.2.0/src/testit_adapter_nose/listener.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_nose-3.1.1/src/testit_adapter_nose/plugin.py` & `testit_adapter_nose-3.2.0/src/testit_adapter_nose/plugin.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_nose-3.1.1/src/testit_adapter_nose/utils.py` & `testit_adapter_nose-3.2.0/src/testit_adapter_nose/utils.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_nose-3.1.1/src/testit_adapter_nose.egg-info/PKG-INFO` & `testit_adapter_nose-3.2.0/src/testit_adapter_nose.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 3.1.1
+Version: 3.2.0
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: nose2
-Requires-Dist: testit-python-commons==3.1.1
+Requires-Dist: testit-python-commons==3.2.0
 
 # Test IT TMS adapter for Nose
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-nose?style=plastic)](https://pypi.python.org/pypi/testit-adapter-nose)
```

