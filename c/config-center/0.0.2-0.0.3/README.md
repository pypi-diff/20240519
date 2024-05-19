# Comparing `tmp/config_center-0.0.2.tar.gz` & `tmp/config_center-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_center-0.0.2.tar", last modified: Fri May 17 16:15:56 2024, max compression
+gzip compressed data, was "config_center-0.0.3.tar", last modified: Fri May 17 16:43:45 2024, max compression
```

## Comparing `config_center-0.0.2.tar` & `config_center-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 16:15:56.446528 config_center-0.0.2/
--rw-rw-rw-   0        0        0     1093 2024-05-17 15:58:59.000000 config_center-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1777 2024-05-17 16:15:56.446528 config_center-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 16:15:56.442470 config_center-0.0.2/cfgc/
--rw-rw-rw-   0        0        0      498 2024-05-17 14:26:52.000000 config_center-0.0.2/cfgc/__init__.py
--rw-rw-rw-   0        0        0     3680 2024-05-17 15:12:56.000000 config_center-0.0.2/cfgc/center.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:15:56.445244 config_center-0.0.2/config_center.egg-info/
--rw-rw-rw-   0        0        0     1777 2024-05-17 16:15:56.000000 config_center-0.0.2/config_center.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-05-17 16:15:56.000000 config_center-0.0.2/config_center.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 16:15:56.000000 config_center-0.0.2/config_center.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-17 16:15:56.000000 config_center-0.0.2/config_center.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 16:15:56.447534 config_center-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1416 2024-05-17 16:15:52.000000 config_center-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:43:45.444336 config_center-0.0.3/
+-rw-rw-rw-   0        0        0     1093 2024-05-17 15:58:59.000000 config_center-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1777 2024-05-17 16:43:45.443371 config_center-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-17 16:43:45.439011 config_center-0.0.3/cfgc/
+-rw-rw-rw-   0        0        0      498 2024-05-17 14:26:52.000000 config_center-0.0.3/cfgc/__init__.py
+-rw-rw-rw-   0        0        0     3836 2024-05-17 16:42:09.000000 config_center-0.0.3/cfgc/center.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:43:45.443371 config_center-0.0.3/config_center.egg-info/
+-rw-rw-rw-   0        0        0     1777 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-17 16:43:45.000000 config_center-0.0.3/config_center.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 16:43:45.444336 config_center-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1416 2024-05-17 16:43:32.000000 config_center-0.0.3/setup.py
```

### Comparing `config_center-0.0.2/LICENSE.txt` & `config_center-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_center-0.0.2/PKG-INFO` & `config_center-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-center
-Version: 0.0.2
+Version: 0.0.3
 Summary: A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!
 Home-page: https://github.com/WhatMelonGua/config-center
 Author: VaterFus
 Author-email: 1107818699@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `config_center-0.0.2/cfgc/center.py` & `config_center-0.0.3/cfgc/center.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,8 +97,15 @@
         :param name: 环境名称
         :return:
         """
         with open(PATH_ENV / f'{name}.pkl', "rb") as cfg:
             cfg = pickle.load(cfg)
         self.define(**cfg)
     def rename(self, name):
-        self.name = name
+        self.name = name
+
+
+# Check Envs
+def envList():
+    envs = os.listdir(PATH_ENV)
+    for i, e in enumerate(envs):
+        print(f"{i} -\t{e.split('.',maxsplit=1)[0]}")
```

### Comparing `config_center-0.0.2/config_center.egg-info/PKG-INFO` & `config_center-0.0.3/config_center.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-center
-Version: 0.0.2
+Version: 0.0.3
 Summary: A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!
 Home-page: https://github.com/WhatMelonGua/config-center
 Author: VaterFus
 Author-email: 1107818699@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `config_center-0.0.2/setup.py` & `config_center-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     SetUp for config-center [site-package]
 """  # [By: HuYw]
 
 # region |- Import -|
 import setuptools
 # endregion
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="config-center",
     version=VERSION,
```

