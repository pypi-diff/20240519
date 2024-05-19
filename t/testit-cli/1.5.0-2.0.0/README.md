# Comparing `tmp/testit-cli-1.5.0.tar.gz` & `tmp/testit_cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-cli-1.5.0.tar", last modified: Wed Mar 13 06:21:52 2024, max compression
+gzip compressed data, was "testit_cli-2.0.0.tar", last modified: Sun May 19 21:48:05 2024, max compression
```

## Comparing `testit-cli-1.5.0.tar` & `testit_cli-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:52.383364 testit-cli-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-13 06:21:45.000000 testit-cli-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-13 06:21:52.383364 testit-cli-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-13 06:21:45.000000 testit-cli-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 06:21:52.383364 testit-cli-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-13 06:21:45.000000 testit-cli-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:52.379364 testit-cli-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:52.383364 testit-cli-1.5.0/src/testit_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/click_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/dir_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/file_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:52.383364 testit-cli-1.5.0/src/testit_cli/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/models/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/models/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/models/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/models/testrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/service_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-13 06:21:45.000000 testit-cli-1.5.0/src/testit_cli/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:52.383364 testit-cli-1.5.0/src/testit_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-13 06:21:52.000000 testit-cli-1.5.0/src/testit_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-13 06:21:52.000000 testit-cli-1.5.0/src/testit_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 06:21:52.000000 testit-cli-1.5.0/src/testit_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-13 06:21:52.000000 testit-cli-1.5.0/src/testit_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-13 06:21:52.000000 testit-cli-1.5.0/src/testit_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 06:21:52.000000 testit-cli-1.5.0/src/testit_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 06:21:52.383364 testit-cli-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-03-13 06:21:45.000000 testit-cli-1.5.0/tests/test_click.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:48:05.192262 testit_cli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 21:47:57.000000 testit_cli-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-19 21:48:05.192262 testit_cli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-19 21:47:57.000000 testit_cli-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:48:05.192262 testit_cli-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-19 21:47:57.000000 testit_cli-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:48:05.184262 testit_cli-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:48:05.188262 testit_cli-2.0.0/src/testit_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/click_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/dir_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/file_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:48:05.188262 testit_cli-2.0.0/src/testit_cli/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/models/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/models/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/models/testrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/service_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-19 21:47:57.000000 testit_cli-2.0.0/src/testit_cli/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:48:05.192262 testit_cli-2.0.0/src/testit_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-19 21:48:05.000000 testit_cli-2.0.0/src/testit_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-19 21:48:05.000000 testit_cli-2.0.0/src/testit_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:48:05.000000 testit_cli-2.0.0/src/testit_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 21:48:05.000000 testit_cli-2.0.0/src/testit_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 21:48:05.000000 testit_cli-2.0.0/src/testit_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 21:48:05.000000 testit_cli-2.0.0/src/testit_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:48:05.188262 testit_cli-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2024-05-19 21:47:57.000000 testit_cli-2.0.0/tests/test_click.py
```

### Comparing `testit-cli-1.5.0/LICENSE` & `testit_cli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/PKG-INFO` & `testit_cli-2.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 1.5.0
+Version: 2.0.0
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit-cli/
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
 License-File: LICENSE
-Requires-Dist: testit-api-client==3.5.0
+Requires-Dist: testit-api-client==4.0.0
 Requires-Dist: validators
 Requires-Dist: tqdm
 Requires-Dist: click~=8.0.4
 
 # Test IT CLI
 
 [![Release
@@ -34,7 +34,8 @@
 
 | Test IT | Test IT CLI |
 |---------|-------------|
 | 3.5+    | 0.1         |
 | 4.4     | 1.0         |
 | 4.5     | 1.2         |
 | 4.6     | 1.5         |
+| 5.0     | 2.0         |
```

### Comparing `testit-cli-1.5.0/setup.py` & `testit_cli-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-cli',
-    version='1.5.0',
+    version='2.0.0',
     description='This tool is the command line wrapper of Test IT allowing you to upload the test results in real time '
                 'to Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit-cli/',
     author='Integration team',
     author_email='integrations@testit.software',
@@ -20,14 +20,14 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_cli'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['testit-api-client==3.5.0', 'validators', 'tqdm', 'click~=8.0.4'],
+    install_requires=['testit-api-client==4.0.0', 'validators', 'tqdm', 'click~=8.0.4'],
     entry_points={
         'console_scripts': [
             'testit = testit_cli.__main__:console_main'
         ]
     }
 )
```

### Comparing `testit-cli-1.5.0/src/testit_cli/apiclient.py` & `testit_cli-2.0.0/src/testit_cli/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/click_commands.py` & `testit_cli-2.0.0/src/testit_cli/click_commands.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/converter.py` & `testit_cli-2.0.0/src/testit_cli/converter.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/dir_worker.py` & `testit_cli-2.0.0/src/testit_cli/dir_worker.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/file_worker.py` & `testit_cli-2.0.0/src/testit_cli/file_worker.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/importer.py` & `testit_cli-2.0.0/src/testit_cli/importer.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/models/testcase.py` & `testit_cli-2.0.0/src/testit_cli/models/testcase.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/parser.py` & `testit_cli-2.0.0/src/testit_cli/parser.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/service.py` & `testit_cli-2.0.0/src/testit_cli/service.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/service_factory.py` & `testit_cli-2.0.0/src/testit_cli/service_factory.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli/validation.py` & `testit_cli-2.0.0/src/testit_cli/validation.py`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/src/testit_cli.egg-info/PKG-INFO` & `testit_cli-2.0.0/src/testit_cli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-cli
-Version: 1.5.0
+Version: 2.0.0
 Summary: This tool is the command line wrapper of Test IT allowing you to upload the test results in real time to Test IT
 Home-page: https://pypi.org/project/testit-cli/
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
 License-File: LICENSE
-Requires-Dist: testit-api-client==3.5.0
+Requires-Dist: testit-api-client==4.0.0
 Requires-Dist: validators
 Requires-Dist: tqdm
 Requires-Dist: click~=8.0.4
 
 # Test IT CLI
 
 [![Release
@@ -34,7 +34,8 @@
 
 | Test IT | Test IT CLI |
 |---------|-------------|
 | 3.5+    | 0.1         |
 | 4.4     | 1.0         |
 | 4.5     | 1.2         |
 | 4.6     | 1.5         |
+| 5.0     | 2.0         |
```

### Comparing `testit-cli-1.5.0/src/testit_cli.egg-info/SOURCES.txt` & `testit_cli-2.0.0/src/testit_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testit-cli-1.5.0/tests/test_click.py` & `testit_cli-2.0.0/tests/test_click.py`

 * *Files identical despite different names*

