# Comparing `tmp/sms-message-inforu-local-0.0.2.tar.gz` & `tmp/sms_message_inforu_local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sms-message-inforu-local-0.0.2.tar", last modified: Fri Nov 17 14:44:24 2023, max compression
+gzip compressed data, was "sms_message_inforu_local-0.0.3.tar", last modified: Sat May 18 21:31:41 2024, max compression
```

## Comparing `sms-message-inforu-local-0.0.2.tar` & `sms_message_inforu_local-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:44:24.523552 sms-message-inforu-local-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2023-11-17 14:44:24.523552 sms-message-inforu-local-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-11-17 14:43:51.000000 sms-message-inforu-local-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-17 14:43:51.000000 sms-message-inforu-local-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 14:44:24.523552 sms-message-inforu-local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-17 14:43:51.000000 sms-message-inforu-local-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:44:24.519552 sms-message-inforu-local-0.0.2/sms-message-inforu-local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:44:24.519552 sms-message-inforu-local-0.0.2/sms-message-inforu-local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 14:43:51.000000 sms-message-inforu-local-0.0.2/sms-message-inforu-local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-11-17 14:43:51.000000 sms-message-inforu-local-0.0.2/sms-message-inforu-local/src/sendsms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 14:44:24.523552 sms-message-inforu-local-0.0.2/sms_message_inforu_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2023-11-17 14:44:24.000000 sms-message-inforu-local-0.0.2/sms_message_inforu_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-17 14:44:24.000000 sms-message-inforu-local-0.0.2/sms_message_inforu_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 14:44:24.000000 sms-message-inforu-local-0.0.2/sms_message_inforu_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-17 14:44:24.000000 sms-message-inforu-local-0.0.2/sms_message_inforu_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-17 14:44:24.000000 sms-message-inforu-local-0.0.2/sms_message_inforu_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:31:41.679104 sms_message_inforu_local-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 21:31:41.679104 sms_message_inforu_local-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-18 21:31:09.000000 sms_message_inforu_local-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-18 21:31:09.000000 sms_message_inforu_local-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 21:31:41.679104 sms_message_inforu_local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-18 21:31:09.000000 sms_message_inforu_local-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:31:41.675104 sms_message_inforu_local-0.0.3/sms_message_inforu_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:31:41.679104 sms_message_inforu_local-0.0.3/sms_message_inforu_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 21:31:09.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-18 21:31:09.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local/src/sms_message_inforu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 21:31:41.679104 sms_message_inforu_local-0.0.3/sms_message_inforu_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 21:31:41.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-18 21:31:41.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 21:31:41.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-18 21:31:41.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 21:31:41.000000 sms_message_inforu_local-0.0.3/sms_message_inforu_local.egg-info/top_level.txt
```

### Comparing `sms-message-inforu-local-0.0.2/PKG-INFO` & `sms_message_inforu_local-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sms-message-inforu-local
-Version: 0.0.2
-Summary: PyPI Package for Circles Project SMS
-Home-page: https://github.com/circ-zone/sms-message-inforu-local-python-package.git
-Author: Circles
-Author-email: info@circles.life
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: message-local>=0.0.5
-Requires-Dist: sms-message-local>=0.0.1
-
 # python-package-template
 This repository is designed to help you create local and remote package layers in Python.  
 It focuses on building package layers and does not include GraphQL and REST-API layers.
 
 ## Download Environment
 To set up the environment, follow these steps in your terminal:
 ```shell
```

### Comparing `sms-message-inforu-local-0.0.2/pyproject.toml` & `sms_message_inforu_local-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sms-message-inforu-local-0.0.2/setup.py` & `sms_message_inforu_local-0.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 PACKAGE_NAME = "sms-message-inforu-local"
-package_dir = PACKAGE_NAME #.replace("-", "_")
+package_dir = PACKAGE_NAME.replace("-", "_")
 
-with open('README.md') as f:
-    readme = f.read()
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.2', 
+    version='0.0.3',  # https://pypi.org/project/sms-message-inforu-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Project SMS",
-    long_description=open('README.md').read(),
+    long_description="PyPI Package for Circles Project SMS",
     long_description_content_type='text/markdown',
-    url="https://github.com/circ-zone/sms-message-inforu-local-python-package.git",  
+    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},  
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[
-        'message-local>=0.0.5',
-        'sms-message-local>=0.0.1'
-    ],
+    install_requires=[# "api-management-local>=0.0.61",
+                      'logger-local>=0.0.135',
+                      "message-local>=0.0.123",
+                      "database-mysql-local>=0.0.290",
+                      "python-sdk-remote>=0.0.93"],
 )
```

