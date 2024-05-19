# Comparing `tmp/testit_importer_allure-1.6.3.tar.gz` & `tmp/testit_importer_allure-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit_importer_allure-1.6.3.tar", last modified: Tue May 14 10:08:17 2024, max compression
+gzip compressed data, was "testit_importer_allure-1.7.0.tar", last modified: Sun May 19 21:49:54 2024, max compression
```

## Comparing `testit_importer_allure-1.6.3.tar` & `testit_importer_allure-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/connection_config.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/apiclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    13509 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/filedto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/filereader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/minioreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-14 10:08:13.000000 testit_importer_allure-1.6.3/src/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.349547 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 10:08:17.000000 testit_importer_allure-1.6.3/testit_importer_allure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:49:54.957768 testit_importer_allure-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 21:49:54.957768 testit_importer_allure-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/connection_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:49:54.957768 testit_importer_allure-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:49:54.953768 testit_importer_allure-1.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/apiclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13509 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/filedto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/filereader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/minioreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-19 21:49:50.000000 testit_importer_allure-1.7.0/src/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:49:54.957768 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 21:49:54.000000 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-19 21:49:54.000000 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:49:54.000000 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-19 21:49:54.000000 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 21:49:54.000000 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 21:49:54.000000 testit_importer_allure-1.7.0/testit_importer_allure.egg-info/top_level.txt
```

### Comparing `testit_importer_allure-1.6.3/PKG-INFO` & `testit_importer_allure-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.6.3
+Version: 1.7.0
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Requires-Dist: testit-api-client==3.5.0
+Requires-Dist: testit-api-client==4.0.0
 Requires-Dist: xmltodict
 Requires-Dist: python-interface
 Requires-Dist: minio
 Requires-Dist: pika
 
 # Test IT TMS importers
 ![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
```

### Comparing `testit_importer_allure-1.6.3/README.md` & `testit_importer_allure-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/setup.py` & `testit_importer_allure-1.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='testit-importer-allure',
-    version='1.6.3',
+    version='1.7.0',
     description='Allure report importer for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://pypi.org/project/testit-importer-allure/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -20,15 +20,15 @@
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     packages=['testit_importer_allure'],
     package_data={'testit_importer_allure': ['../connection_config.ini']},
     package_dir={'testit_importer_allure': 'src'},
     install_requires=[
-        'testit-api-client==3.5.0',
+        'testit-api-client==4.0.0',
         'xmltodict',
         'python-interface',
         'minio',
         'pika'
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `testit_importer_allure-1.6.3/src/__main__.py` & `testit_importer_allure-1.7.0/src/__main__.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/apiclient.py` & `testit_importer_allure-1.7.0/src/apiclient.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/configurator.py` & `testit_importer_allure-1.7.0/src/configurator.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/converter.py` & `testit_importer_allure-1.7.0/src/converter.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/filereader.py` & `testit_importer_allure-1.7.0/src/filereader.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/importer.py` & `testit_importer_allure-1.7.0/src/importer.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/minioreader.py` & `testit_importer_allure-1.7.0/src/minioreader.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/parser.py` & `testit_importer_allure-1.7.0/src/parser.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/src/rabbitmq.py` & `testit_importer_allure-1.7.0/src/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `testit_importer_allure-1.6.3/testit_importer_allure.egg-info/PKG-INFO` & `testit_importer_allure-1.7.0/testit_importer_allure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: testit-importer-allure
-Version: 1.6.3
+Version: 1.7.0
 Summary: Allure report importer for Test IT
 Home-page: https://pypi.org/project/testit-importer-allure/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Requires-Dist: testit-api-client==3.5.0
+Requires-Dist: testit-api-client==4.0.0
 Requires-Dist: xmltodict
 Requires-Dist: python-interface
 Requires-Dist: minio
 Requires-Dist: pika
 
 # Test IT TMS importers
 ![Test IT](https://raw.githubusercontent.com/testit-tms/importers/main/images/banner.png)
```

### Comparing `testit_importer_allure-1.6.3/testit_importer_allure.egg-info/SOURCES.txt` & `testit_importer_allure-1.7.0/testit_importer_allure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

