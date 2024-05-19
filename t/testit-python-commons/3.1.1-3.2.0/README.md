# Comparing `tmp/testit_python_commons-3.1.1.tar.gz` & `tmp/testit_python_commons-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_python_commons-3.1.1.tar", last modified: Mon May 13 12:53:42 2024, max compression
+gzip compressed data, was "testit_python_commons-3.2.0.tar", last modified: Sun May 19 21:52:41 2024, max compression
```

## Comparing `testit_python_commons-3.1.1.tar` & `testit_python_commons-3.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.189807 testit_python_commons-3.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.189807 testit_python_commons-3.1.1/src/testit_python_commons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/app_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.189807 testit_python_commons-3.1.1/src/testit_python_commons/client/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/client/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/dynamic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/src/testit_python_commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/adapter_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/link_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/outcome_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/step_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/src/testit_python_commons/services/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/step_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/step_result_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-13 12:53:37.000000 testit_python_commons-3.1.1/src/testit_python_commons/step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:42.193807 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 12:53:42.000000 testit_python_commons-3.1.1/src/testit_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.096119 testit_python_commons-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 21:52:41.096119 testit_python_commons-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:52:41.096119 testit_python_commons-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.088118 testit_python_commons-3.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.092118 testit_python_commons-3.2.0/src/testit_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.092118 testit_python_commons-3.2.0/src/testit_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.092118 testit_python_commons-3.2.0/src/testit_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/outcome_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/step_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.096119 testit_python_commons-3.2.0/src/testit_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/step_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/step_result_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-19 21:52:37.000000 testit_python_commons-3.2.0/src/testit_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:52:41.096119 testit_python_commons-3.2.0/src/testit_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 21:52:41.000000 testit_python_commons-3.2.0/src/testit_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-19 21:52:41.000000 testit_python_commons-3.2.0/src/testit_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:52:41.000000 testit_python_commons-3.2.0/src/testit_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 21:52:41.000000 testit_python_commons-3.2.0/src/testit_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-19 21:52:41.000000 testit_python_commons-3.2.0/src/testit_python_commons.egg-info/top_level.txt
```

### Comparing `testit_python_commons-3.1.1/PKG-INFO` & `testit_python_commons-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python commons for Test IT
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
 Requires-Dist: pluggy
-Requires-Dist: testit-api-client==3.5.0
+Requires-Dist: testit-api-client==4.0.0
 
 # How to enable debug logging?
 1. Add in **connection_config.ini** file from the root directory of the project:
 ```
 [debug]
 __DEV = true
 ```
```

### Comparing `testit_python_commons-3.1.1/setup.py` & `testit_python_commons-3.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-python-commons',
-    version='3.1.1',
+    version='3.2.0',
     description='Python commons for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -19,9 +19,9 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit', 'testit_python_commons'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pluggy', 'testit-api-client==3.5.0']
+    install_requires=['pluggy', 'testit-api-client==4.0.0']
 )
```

### Comparing `testit_python_commons-3.1.1/src/testit.py` & `testit_python_commons-3.2.0/src/testit.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/app_properties.py` & `testit_python_commons-3.2.0/src/testit_python_commons/app_properties.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/client/api_client.py` & `testit_python_commons-3.2.0/src/testit_python_commons/client/api_client.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/client/client_configuration.py` & `testit_python_commons-3.2.0/src/testit_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/client/converter.py` & `testit_python_commons-3.2.0/src/testit_python_commons/client/converter.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/decorators.py` & `testit_python_commons-3.2.0/src/testit_python_commons/decorators.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/dynamic_methods.py` & `testit_python_commons-3.2.0/src/testit_python_commons/dynamic_methods.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/models/link.py` & `testit_python_commons-3.2.0/src/testit_python_commons/models/link.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/models/step_result.py` & `testit_python_commons-3.2.0/src/testit_python_commons/models/step_result.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/models/test_result.py` & `testit_python_commons-3.2.0/src/testit_python_commons/models/test_result.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py` & `testit_python_commons-3.2.0/src/testit_python_commons/models/test_result_with_all_fixture_step_results_model.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/adapter_manager.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/adapter_manager_configuration.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/logger.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/logger.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/plugin_manager.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/step_manager.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/step_manager.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/step_result_storage.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/step_result_storage.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/services/utils.py` & `testit_python_commons-3.2.0/src/testit_python_commons/services/utils.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons/step.py` & `testit_python_commons-3.2.0/src/testit_python_commons/step.py`

 * *Files identical despite different names*

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons.egg-info/PKG-INFO` & `testit_python_commons-3.2.0/src/testit_python_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python commons for Test IT
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
 Requires-Dist: pluggy
-Requires-Dist: testit-api-client==3.5.0
+Requires-Dist: testit-api-client==4.0.0
 
 # How to enable debug logging?
 1. Add in **connection_config.ini** file from the root directory of the project:
 ```
 [debug]
 __DEV = true
 ```
```

### Comparing `testit_python_commons-3.1.1/src/testit_python_commons.egg-info/SOURCES.txt` & `testit_python_commons-3.2.0/src/testit_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

