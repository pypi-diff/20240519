# Comparing `tmp/onfon_sms_sender-0.1.tar.gz` & `tmp/onfon_sms_sender-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onfon_sms_sender-0.1.tar", last modified: Sat May 18 11:59:21 2024, max compression
+gzip compressed data, was "onfon_sms_sender-0.1.2.tar", last modified: Sun May 19 00:51:54 2024, max compression
```

## Comparing `onfon_sms_sender-0.1.tar` & `onfon_sms_sender-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-18 11:59:21.285590 onfon_sms_sender-0.1/
--rw-r--r--   0 la         (501) staff       (20)     1072 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1/LICENSE
--rw-r--r--   0 la         (501) staff       (20)     1128 2024-05-18 11:59:21.285404 onfon_sms_sender-0.1/PKG-INFO
--rw-r--r--   0 la         (501) staff       (20)      374 2024-05-18 11:42:01.000000 onfon_sms_sender-0.1/README.md
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-18 11:59:21.285215 onfon_sms_sender-0.1/onfon_sms_sender.egg-info/
--rw-r--r--   0 la         (501) staff       (20)     1128 2024-05-18 11:59:21.000000 onfon_sms_sender-0.1/onfon_sms_sender.egg-info/PKG-INFO
--rw-r--r--   0 la         (501) staff       (20)      311 2024-05-18 11:59:21.000000 onfon_sms_sender-0.1/onfon_sms_sender.egg-info/SOURCES.txt
--rw-r--r--   0 la         (501) staff       (20)        1 2024-05-18 11:59:21.000000 onfon_sms_sender-0.1/onfon_sms_sender.egg-info/dependency_links.txt
--rw-r--r--   0 la         (501) staff       (20)       16 2024-05-18 11:59:21.000000 onfon_sms_sender-0.1/onfon_sms_sender.egg-info/requires.txt
--rw-r--r--   0 la         (501) staff       (20)       17 2024-05-18 11:59:21.000000 onfon_sms_sender-0.1/onfon_sms_sender.egg-info/top_level.txt
--rw-r--r--   0 la         (501) staff       (20)       38 2024-05-18 11:59:21.285637 onfon_sms_sender-0.1/setup.cfg
--rw-r--r--   0 la         (501) staff       (20)     1079 2024-05-18 11:40:05.000000 onfon_sms_sender-0.1/setup.py
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-18 11:59:21.284579 onfon_sms_sender-0.1/sms_sender/
--rw-r--r--   0 la         (501) staff       (20)       28 2024-05-18 11:35:18.000000 onfon_sms_sender-0.1/sms_sender/__init__.py
--rw-r--r--   0 la         (501) staff       (20)     1309 2024-05-18 11:35:31.000000 onfon_sms_sender-0.1/sms_sender/utils.py
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-18 11:59:21.285046 onfon_sms_sender-0.1/tests/
--rw-r--r--   0 la         (501) staff       (20)        0 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1/tests/__init__.py
--rw-r--r--   0 la         (501) staff       (20)        0 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1/tests/test_sms_sender.py
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.234413 onfon_sms_sender-0.1.2/
+-rw-r--r--   0 la         (501) staff       (20)     1072 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1.2/LICENSE
+-rw-r--r--   0 la         (501) staff       (20)     2051 2024-05-19 00:51:54.234174 onfon_sms_sender-0.1.2/PKG-INFO
+-rw-r--r--   0 la         (501) staff       (20)     1288 2024-05-19 00:36:24.000000 onfon_sms_sender-0.1.2/README.md
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.233923 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/
+-rw-r--r--   0 la         (501) staff       (20)     2051 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/PKG-INFO
+-rw-r--r--   0 la         (501) staff       (20)      311 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/SOURCES.txt
+-rw-r--r--   0 la         (501) staff       (20)        1 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/dependency_links.txt
+-rw-r--r--   0 la         (501) staff       (20)       23 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/requires.txt
+-rw-r--r--   0 la         (501) staff       (20)       17 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/top_level.txt
+-rw-r--r--   0 la         (501) staff       (20)       38 2024-05-19 00:51:54.234459 onfon_sms_sender-0.1.2/setup.cfg
+-rw-r--r--   0 la         (501) staff       (20)     1084 2024-05-19 00:51:16.000000 onfon_sms_sender-0.1.2/setup.py
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.233168 onfon_sms_sender-0.1.2/sms_sender/
+-rw-r--r--   0 la         (501) staff       (20)       28 2024-05-18 11:35:18.000000 onfon_sms_sender-0.1.2/sms_sender/__init__.py
+-rw-r--r--   0 la         (501) staff       (20)     3000 2024-05-19 00:08:52.000000 onfon_sms_sender-0.1.2/sms_sender/utils.py
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.233591 onfon_sms_sender-0.1.2/tests/
+-rw-r--r--   0 la         (501) staff       (20)        0 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1.2/tests/__init__.py
+-rw-r--r--   0 la         (501) staff       (20)     4580 2024-05-19 00:29:16.000000 onfon_sms_sender-0.1.2/tests/test_sms_sender.py
```

### Comparing `onfon_sms_sender-0.1/LICENSE` & `onfon_sms_sender-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onfon_sms_sender-0.1/setup.py` & `onfon_sms_sender-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='onfon-sms-sender',
-    version='0.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'requests',
-        'Django'
-    ],
+        'python-dotenv',],
     entry_points={
         'console_scripts': [
             # Add command-line scripts here if needed
         ],
     },
     include_package_data=True,
     description='A package to send SMS using Onfon Media API',
```

