# Comparing `tmp/approval_utilities-8.4.1.tar.gz` & `tmp/approval_utilities-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approval_utilities-8.4.1.tar", last modified: Sun Jul 16 18:37:43 2023, max compression
+gzip compressed data, was "approval_utilities-9.0.0.tar", last modified: Sun Aug 27 19:49:44 2023, max compression
```

## Comparing `approval_utilities-8.4.1.tar` & `approval_utilities-9.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.366535 approval_utilities-8.4.1/approval_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.366535 approval_utilities-8.4.1/approval_utilities/approvaltests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/approvaltests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.366535 approval_utilities-8.4.1/approval_utilities/approvaltests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/approvaltests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/approvaltests/core/executable_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/approvaltests/core/verifiable.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/approvaltests/core/verify_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/list_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/approval_utilities/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/clipboard_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/approval_utilities/utilities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/exceptions/exception_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/exceptions/exception_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/exceptions/multiple_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/approval_utilities/utilities/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/logger/logging_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/logger/simple_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/map_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/markdown_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/multiline_string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/os_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/approval_utilities/utilities/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/persistence/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/persistence/saver.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/stack_frame_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/string_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/time_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utilities/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/approval_utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:37:43.366535 approval_utilities-8.4.1/approval_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-16 18:37:43.000000 approval_utilities-8.4.1/approval_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-16 18:37:43.000000 approval_utilities-8.4.1/approval_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:37:43.000000 approval_utilities-8.4.1/approval_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 18:37:43.000000 approval_utilities-8.4.1/approval_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/requirements.prod.extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/requirements.prod.required.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/requirements.prod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-16 18:37:43.370535 approval_utilities-8.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-16 18:37:42.000000 approval_utilities-8.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-16 18:37:30.000000 approval_utilities-8.4.1/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-16 18:37:41.000000 approval_utilities-8.4.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/
+-rw-r--r--   0 runner    (1001) docker     (999)    10273 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)      117 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     1003 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)    12745 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.278067 approval_utilities-9.0.0/approval_utilities/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities/approvaltests/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/approvaltests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities/approvaltests/core/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/approvaltests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      428 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/approvaltests/core/executable_command.py
+-rw-r--r--   0 runner    (1001) docker     (999)      257 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/approvaltests/core/verifiable.py
+-rw-r--r--   0 runner    (1001) docker     (999)       99 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/approvaltests/core/verify_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/list_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities/utilities/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      188 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/clipboard_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (999)      822 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities/utilities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1080 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/exceptions/exception_collector.py
+-rw-r--r--   0 runner    (1001) docker     (999)      103 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/exceptions/exception_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)      296 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/exceptions/multiple_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities/utilities/logger/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7505 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/logger/logging_instance.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2765 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/logger/simple_logger.py
+-rw-r--r--   0 runner    (1001) docker     (999)      191 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1602 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/markdown_table.py
+-rw-r--r--   0 runner    (1001) docker     (999)      183 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/multiline_string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)      150 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/os_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities/utilities/persistence/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      218 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/persistence/loader.py
+-rw-r--r--   0 runner    (1001) docker     (999)      223 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/persistence/saver.py
+-rw-r--r--   0 runner    (1001) docker     (999)      311 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/stack_frame_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (999)      230 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/string_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (999)      524 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/time_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (999)      563 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utilities/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1917 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/approval_utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/approval_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     1003 2023-08-27 19:49:44.000000 approval_utilities-9.0.0/approval_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1744 2023-08-27 19:49:44.000000 approval_utilities-9.0.0/approval_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-27 19:49:44.000000 approval_utilities-9.0.0/approval_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-27 19:49:44.000000 approval_utilities-9.0.0/approval_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      255 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/requirements.prod.extras.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       60 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/requirements.prod.required.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       66 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/requirements.prod.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       79 2023-08-27 19:49:44.282067 approval_utilities-9.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1372 2023-08-27 19:49:43.000000 approval_utilities-9.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2069 2023-08-27 19:49:31.000000 approval_utilities-9.0.0/setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)       26 2023-08-27 19:49:42.000000 approval_utilities-9.0.0/version.py
```

### Comparing `approval_utilities-8.4.1/LICENSE` & `approval_utilities-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/PKG-INFO` & `approval_utilities-9.0.0/approval_utilities.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: approval_utilities
-Version: 8.4.1
+Name: approval-utilities
+Version: 9.0.0
 Summary: Utilities for your production code that work well with approvaltests
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `approval_utilities-8.4.1/README.md` & `approval_utilities-9.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,15 @@
 
 ### Missing Documentation?
 
 If there is documentation you wish existed, please add a `page request` to [this issue](https://github.com/approvals/ApprovalTests.Python/issues/135).
 
 ### Dependencies
 
-ApprovalTests require Python 3.7 or greater and the following dependencies:
+ApprovalTests require Python 3.8 or greater and the following dependencies:
 
 #### Required dependencies
 
 These dependencies are always required for approvaltests
 
 <!-- snippet: requirements.prod.required.txt -->
 <a id='snippet-requirements.prod.required.txt'></a>
@@ -313,11 +313,11 @@
 
 Pull requests are welcomed, particularly those accompanied by automated tests.
 
 To run the self-tests, install pytest and tox, then execute
 
     python -m tox
 
-This will run the self-tests on several python versions. We support python 3.7 and above.
+This will run the self-tests on several python versions. We support python 3.8 and above.
 
 All pull requests will be pre-checked using GitHub actions to execute all these tests. You can see the [results of test
 runs here](https://github.com/approvals/ApprovalTests.Python/actions).
```

### Comparing `approval_utilities-8.4.1/approval_utilities/list_utils.py` & `approval_utilities-9.0.0/approval_utilities/list_utils.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/deprecated.py` & `approval_utilities-9.0.0/approval_utilities/utilities/deprecated.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/exceptions/exception_collector.py` & `approval_utilities-9.0.0/approval_utilities/utilities/exceptions/exception_collector.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/logger/logging_instance.py` & `approval_utilities-9.0.0/approval_utilities/utilities/logger/logging_instance.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/logger/simple_logger.py` & `approval_utilities-9.0.0/approval_utilities/utilities/logger/simple_logger.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/markdown_table.py` & `approval_utilities-9.0.0/approval_utilities/utilities/markdown_table.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/time_utilities.py` & `approval_utilities-9.0.0/approval_utilities/utilities/time_utilities.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utilities/wrapper.py` & `approval_utilities-9.0.0/approval_utilities/utilities/wrapper.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities/utils.py` & `approval_utilities-9.0.0/approval_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/approval_utilities.egg-info/PKG-INFO` & `approval_utilities-9.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: approval-utilities
-Version: 8.4.1
+Name: approval_utilities
+Version: 9.0.0
 Summary: Utilities for your production code that work well with approvaltests
 Home-page: https://github.com/approvals/ApprovalTests.Python
 Author: ApprovalTests Contributors
 Author-email: llewellyn.falco@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 License-File: LICENSE
```

### Comparing `approval_utilities-8.4.1/approval_utilities.egg-info/SOURCES.txt` & `approval_utilities-9.0.0/approval_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `approval_utilities-8.4.1/setup.py` & `approval_utilities-9.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 setup(
     name="approval_utilities",
     version=get_version(),
     description="Utilities for your production code that work well with approvaltests",
     author="ApprovalTests Contributors",
     author_email="llewellyn.falco@gmail.com",
     url="https://github.com/approvals/ApprovalTests.Python",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     packages=find_packages(include=["approval_utilities*"]),
     package_data={},
     install_requires=[],
     # long_description=(get_parent_directory() / "README.md").read_text(),
     # long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
         "Topic :: Utilities",
     ],
 )
```

### Comparing `approval_utilities-8.4.1/setup_utils.py` & `approval_utilities-9.0.0/setup_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     setup(
         name=package_name,
         version=get_version(),
         description=package_description,
         author="ApprovalTests Contributors",
         author_email="llewellyn.falco@gmail.com",
         url="https://github.com/approvals/ApprovalTests.Python",
-        python_requires=">=3.7",
+        python_requires=">=3.8",
         packages=find_packages(include=["approvaltests*"]),
         package_data={"approvaltests": ["reporters/reporters.json"]},
         install_requires=required,
         extras_require=extra_requires,
         long_description=(get_parent_directory() / "README.md").read_text(),
         long_description_content_type="text/markdown",
         classifiers=[
@@ -40,16 +40,16 @@
             "Intended Audience :: Developers",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: POSIX",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: MacOS :: MacOS X",
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3 :: Only",
-            "Programming Language :: Python :: 3.6",
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Topic :: Software Development :: Libraries",
             "Topic :: Software Development :: Testing",
             "Topic :: Utilities",
         ],
     )
```

