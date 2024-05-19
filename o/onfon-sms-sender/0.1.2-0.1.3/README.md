# Comparing `tmp/onfon_sms_sender-0.1.2.tar.gz` & `tmp/onfon_sms_sender-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onfon_sms_sender-0.1.2.tar", last modified: Sun May 19 00:51:54 2024, max compression
+gzip compressed data, was "onfon_sms_sender-0.1.3.tar", last modified: Sun May 19 06:44:15 2024, max compression
```

## Comparing `onfon_sms_sender-0.1.2.tar` & `onfon_sms_sender-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.234413 onfon_sms_sender-0.1.2/
--rw-r--r--   0 la         (501) staff       (20)     1072 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1.2/LICENSE
--rw-r--r--   0 la         (501) staff       (20)     2051 2024-05-19 00:51:54.234174 onfon_sms_sender-0.1.2/PKG-INFO
--rw-r--r--   0 la         (501) staff       (20)     1288 2024-05-19 00:36:24.000000 onfon_sms_sender-0.1.2/README.md
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.233923 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/
--rw-r--r--   0 la         (501) staff       (20)     2051 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/PKG-INFO
--rw-r--r--   0 la         (501) staff       (20)      311 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/SOURCES.txt
--rw-r--r--   0 la         (501) staff       (20)        1 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/dependency_links.txt
--rw-r--r--   0 la         (501) staff       (20)       23 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/requires.txt
--rw-r--r--   0 la         (501) staff       (20)       17 2024-05-19 00:51:54.000000 onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/top_level.txt
--rw-r--r--   0 la         (501) staff       (20)       38 2024-05-19 00:51:54.234459 onfon_sms_sender-0.1.2/setup.cfg
--rw-r--r--   0 la         (501) staff       (20)     1084 2024-05-19 00:51:16.000000 onfon_sms_sender-0.1.2/setup.py
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.233168 onfon_sms_sender-0.1.2/sms_sender/
--rw-r--r--   0 la         (501) staff       (20)       28 2024-05-18 11:35:18.000000 onfon_sms_sender-0.1.2/sms_sender/__init__.py
--rw-r--r--   0 la         (501) staff       (20)     3000 2024-05-19 00:08:52.000000 onfon_sms_sender-0.1.2/sms_sender/utils.py
-drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 00:51:54.233591 onfon_sms_sender-0.1.2/tests/
--rw-r--r--   0 la         (501) staff       (20)        0 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1.2/tests/__init__.py
--rw-r--r--   0 la         (501) staff       (20)     4580 2024-05-19 00:29:16.000000 onfon_sms_sender-0.1.2/tests/test_sms_sender.py
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 06:44:15.151391 onfon_sms_sender-0.1.3/
+-rw-r--r--   0 la         (501) staff       (20)     1072 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1.3/LICENSE
+-rw-r--r--   0 la         (501) staff       (20)     2051 2024-05-19 06:44:15.151121 onfon_sms_sender-0.1.3/PKG-INFO
+-rw-r--r--   0 la         (501) staff       (20)     1288 2024-05-19 00:36:24.000000 onfon_sms_sender-0.1.3/README.md
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 06:44:15.150837 onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/
+-rw-r--r--   0 la         (501) staff       (20)     2051 2024-05-19 06:44:15.000000 onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/PKG-INFO
+-rw-r--r--   0 la         (501) staff       (20)      311 2024-05-19 06:44:15.000000 onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/SOURCES.txt
+-rw-r--r--   0 la         (501) staff       (20)        1 2024-05-19 06:44:15.000000 onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/dependency_links.txt
+-rw-r--r--   0 la         (501) staff       (20)       23 2024-05-19 06:44:15.000000 onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/requires.txt
+-rw-r--r--   0 la         (501) staff       (20)       11 2024-05-19 06:44:15.000000 onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/top_level.txt
+-rw-r--r--   0 la         (501) staff       (20)       38 2024-05-19 06:44:15.151449 onfon_sms_sender-0.1.3/setup.cfg
+-rw-r--r--   0 la         (501) staff       (20)     1122 2024-05-19 06:30:21.000000 onfon_sms_sender-0.1.3/setup.py
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 06:44:15.149747 onfon_sms_sender-0.1.3/sms_sender/
+-rw-r--r--   0 la         (501) staff       (20)       28 2024-05-18 11:35:18.000000 onfon_sms_sender-0.1.3/sms_sender/__init__.py
+-rw-r--r--   0 la         (501) staff       (20)     3000 2024-05-19 00:08:52.000000 onfon_sms_sender-0.1.3/sms_sender/utils.py
+drwxr-xr-x   0 la         (501) staff       (20)        0 2024-05-19 06:44:15.150254 onfon_sms_sender-0.1.3/tests/
+-rw-r--r--   0 la         (501) staff       (20)        0 2024-05-18 11:32:13.000000 onfon_sms_sender-0.1.3/tests/__init__.py
+-rw-r--r--   0 la         (501) staff       (20)     4580 2024-05-19 00:29:16.000000 onfon_sms_sender-0.1.3/tests/test_sms_sender.py
```

### Comparing `onfon_sms_sender-0.1.2/LICENSE` & `onfon_sms_sender-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `onfon_sms_sender-0.1.2/PKG-INFO` & `onfon_sms_sender-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onfon-sms-sender
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to send SMS using Onfon Media API
 Home-page: https://github.com/antonnifo/Onfon-SMS-Sender
 Author: Antonnifo
 Author-email: antonnifo@live.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `onfon_sms_sender-0.1.2/README.md` & `onfon_sms_sender-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `onfon_sms_sender-0.1.2/onfon_sms_sender.egg-info/PKG-INFO` & `onfon_sms_sender-0.1.3/onfon_sms_sender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onfon-sms-sender
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to send SMS using Onfon Media API
 Home-page: https://github.com/antonnifo/Onfon-SMS-Sender
 Author: Antonnifo
 Author-email: antonnifo@live.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `onfon_sms_sender-0.1.2/setup.py` & `onfon_sms_sender-0.1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='onfon-sms-sender',
-    version='0.1.2',
-    packages=find_packages(),
+    version='0.1.3',
+    packages=find_packages(include=['sms_sender', 'sms_sender.*']),
     install_requires=[
         'requests',
         'python-dotenv',],
     entry_points={
         'console_scripts': [
             # Add command-line scripts here if needed
         ],
```

### Comparing `onfon_sms_sender-0.1.2/sms_sender/utils.py` & `onfon_sms_sender-0.1.3/sms_sender/utils.py`

 * *Files identical despite different names*

### Comparing `onfon_sms_sender-0.1.2/tests/test_sms_sender.py` & `onfon_sms_sender-0.1.3/tests/test_sms_sender.py`

 * *Files identical despite different names*

