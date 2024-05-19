# Comparing `tmp/testit_adapter_behave-3.1.1.tar.gz` & `tmp/testit_adapter_behave-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_adapter_behave-3.1.1.tar", last modified: Mon May 13 12:53:42 2024, max compression
+gzip compressed data, was "testit_adapter_behave-3.2.0.tar", last modified: Sun May 19 21:52:41 2024, max compression
```

## Comparing `testit_adapter_behave-3.1.1.tar` & `testit_adapter_behave-3.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.646762 testit_adapter_behave-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-13 12:53:42.646762 testit_adapter_behave-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:53:42.646762 testit_adapter_behave-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.642762 testit_adapter_behave-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.642762 testit_adapter_behave-3.1.1/src/testit_adapter_behave/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.646762 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/label.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/option.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/test_result_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/models/url_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/scenario_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/tags_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-13 12:53:36.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.646762 testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-13 12:53:42.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-13 12:53:42.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:53:42.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 12:53:42.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 12:53:42.000000 testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.695427 testit_adapter_behave-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-19 21:52:41.695427 testit_adapter_behave-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:52:41.695427 testit_adapter_behave-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.691427 testit_adapter_behave-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.691427 testit_adapter_behave-3.2.0/src/testit_adapter_behave/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.695427 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/models/url_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/scenario_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/tags_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-19 21:52:37.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.695427 testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-19 21:52:41.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-19 21:52:41.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:52:41.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 21:52:41.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 21:52:41.000000 testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/top_level.txt
```

### Comparing `testit_adapter_behave-3.1.1/PKG-INFO` & `testit_adapter_behave-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 3.1.1
+Version: 3.2.0
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: behave
-Requires-Dist: testit-python-commons==3.1.1
+Requires-Dist: testit-python-commons==3.2.0
 Requires-Dist: attrs
 
 # Test IT TMS adapter for Behave
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
```

### Comparing `testit_adapter_behave-3.1.1/README.md` & `testit_adapter_behave-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `testit_adapter_behave-3.1.1/setup.py` & `testit_adapter_behave-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-behave',
-    version='3.1.1',
+    version='3.2.0',
     description='Behave adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -21,10 +21,10 @@
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_behave'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'behave',
-        'testit-python-commons==3.1.1',
+        'testit-python-commons==3.2.0',
         'attrs'],
 )
```

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave/formatter.py` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave/formatter.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave/listener.py` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave/listener.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave/scenario_parser.py` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave/scenario_parser.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave/tags_parser.py` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave/tags_parser.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave/utils.py` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave/utils.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/PKG-INFO` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 3.1.1
+Version: 3.2.0
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: behave
-Requires-Dist: testit-python-commons==3.1.1
+Requires-Dist: testit-python-commons==3.2.0
 Requires-Dist: attrs
 
 # Test IT TMS adapter for Behave
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
```

### Comparing `testit_adapter_behave-3.1.1/src/testit_adapter_behave.egg-info/SOURCES.txt` & `testit_adapter_behave-3.2.0/src/testit_adapter_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

