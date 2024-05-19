# Comparing `tmp/testit_adapter_pytest-3.1.1.tar.gz` & `tmp/testit_adapter_pytest-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_adapter_pytest-3.1.1.tar", last modified: Mon May 13 12:53:49 2024, max compression
+gzip compressed data, was "testit_adapter_pytest-3.2.0.tar", last modified: Sun May 19 21:52:47 2024, max compression
```

## Comparing `testit_adapter_pytest-3.1.1.tar` & `testit_adapter_pytest-3.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:49.922701 testit_adapter_pytest-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-05-13 12:53:49.922701 testit_adapter_pytest-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:53:49.922701 testit_adapter_pytest-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:49.918701 testit_adapter_pytest-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:49.918701 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/fixture_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/fixture_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/fixture_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:49.922701 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/models/executable_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/models/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-13 12:53:36.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:49.922701 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-05-13 12:53:49.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-13 12:53:49.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:53:49.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 12:53:49.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 12:53:49.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 12:53:49.000000 testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:47.943079 testit_adapter_pytest-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-05-19 21:52:47.943079 testit_adapter_pytest-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:52:47.943079 testit_adapter_pytest-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:47.939079 testit_adapter_pytest-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:47.943079 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/fixture_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/fixture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/fixture_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:47.943079 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/models/executable_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/models/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-05-19 21:52:41.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:47.943079 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15238 2024-05-19 21:52:47.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-19 21:52:47.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:52:47.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 21:52:47.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 21:52:47.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 21:52:47.000000 testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit_adapter_pytest-3.1.1/PKG-INFO` & `testit_adapter_pytest-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 3.1.1
+Version: 3.2.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: attrs
-Requires-Dist: testit-python-commons==3.1.1
+Requires-Dist: testit-python-commons==3.2.0
 
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-pytest?style=plastic)](https://pypi.python.org/pypi/testit-adapter-pytest)
```

### Comparing `testit_adapter_pytest-3.1.1/README.md` & `testit_adapter_pytest-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/setup.py` & `testit_adapter_pytest-3.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='3.1.1',
+    version='3.2.0',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -17,10 +17,10 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'attrs', 'testit-python-commons==3.1.1'],
+    install_requires=['pytest', 'pytest-xdist', 'attrs', 'testit-python-commons==3.2.0'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/fixture_context.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/fixture_context.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/fixture_manager.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/fixture_manager.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/fixture_storage.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/fixture_storage.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/listener.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/listener.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/models/executable_test.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/models/executable_test.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/models/fixture.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/models/fixture.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/plugin.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest/utils.py` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest/utils.py`

 * *Files identical despite different names*

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 3.1.1
+Version: 3.2.0
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: attrs
-Requires-Dist: testit-python-commons==3.1.1
+Requires-Dist: testit-python-commons==3.2.0
 
 # Test IT TMS adapter for Pytest
 
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-pytest?style=plastic)](https://pypi.python.org/pypi/testit-adapter-pytest)
```

### Comparing `testit_adapter_pytest-3.1.1/src/testit_adapter_pytest.egg-info/SOURCES.txt` & `testit_adapter_pytest-3.2.0/src/testit_adapter_pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

