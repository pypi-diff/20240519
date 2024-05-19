# Comparing `tmp/debug_utility-0.3.tar.gz` & `tmp/debug_utility-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debug_utility-0.3.tar", last modified: Thu May  9 00:21:50 2024, max compression
+gzip compressed data, was "debug_utility-0.4.tar", last modified: Sun May 19 03:03:45 2024, max compression
```

## Comparing `debug_utility-0.3.tar` & `debug_utility-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 00:21:50.535000 debug_utility-0.3/
--rw-rw-rw-   0        0        0      427 2024-05-09 00:21:50.522000 debug_utility-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-08 23:10:50.000000 debug_utility-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 00:21:50.453000 debug_utility-0.3/debug_utility/
--rw-rw-rw-   0        0        0       95 2024-05-09 00:18:25.000000 debug_utility-0.3/debug_utility/__init__.py
--rw-rw-rw-   0        0        0     2744 2024-05-08 23:10:50.000000 debug_utility-0.3/debug_utility/debug_file.py
--rw-rw-rw-   0        0        0     7820 2024-05-08 23:10:50.000000 debug_utility-0.3/debug_utility/utility_file.py
-drwxrwxrwx   0        0        0        0 2024-05-09 00:21:50.512000 debug_utility-0.3/debug_utility.egg-info/
--rw-rw-rw-   0        0        0      427 2024-05-09 00:21:50.000000 debug_utility-0.3/debug_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2024-05-09 00:21:50.000000 debug_utility-0.3/debug_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 00:21:50.000000 debug_utility-0.3/debug_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-09 00:21:50.000000 debug_utility-0.3/debug_utility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 00:21:50.533000 debug_utility-0.3/setup.cfg
--rw-rw-rw-   0        0        0      688 2024-05-09 00:21:16.000000 debug_utility-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:03:45.684000 debug_utility-0.4/
+-rw-rw-rw-   0        0        0      966 2024-05-19 03:03:45.672000 debug_utility-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-05-19 03:03:36.000000 debug_utility-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 03:03:45.602000 debug_utility-0.4/debug_utility/
+-rw-rw-rw-   0        0        0       95 2024-05-09 00:18:25.000000 debug_utility-0.4/debug_utility/__init__.py
+-rw-rw-rw-   0        0        0     2860 2024-05-19 03:02:14.000000 debug_utility-0.4/debug_utility/debug_file.py
+-rw-rw-rw-   0        0        0     7724 2024-05-15 22:47:59.000000 debug_utility-0.4/debug_utility/utility_file.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:03:45.665000 debug_utility-0.4/debug_utility.egg-info/
+-rw-rw-rw-   0        0        0      966 2024-05-19 03:03:45.000000 debug_utility-0.4/debug_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-19 03:03:45.000000 debug_utility-0.4/debug_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 03:03:45.000000 debug_utility-0.4/debug_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-19 03:03:45.000000 debug_utility-0.4/debug_utility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 03:03:45.682000 debug_utility-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      688 2024-05-19 03:02:14.000000 debug_utility-0.4/setup.py
```

### Comparing `debug_utility-0.3/debug_utility/debug_file.py` & `debug_utility-0.4/debug_utility/debug_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import datetime
 import os
 class debug_class():
     debug_activated = True
     def __init__(self, custom_variables={"No variables provided": True}, debug_activated=False, file_name='debug.txt', pretty=False):
+
         self.debug_activated = debug_activated
+        if isinstance(self.debug_activated, str):
+            self.debug_activated = bool(self.debug_activated)
         self.pretty = pretty
         self.file_name = file_name
         self.indent_number = 0
         self.tab = self.get_number_of_tabs_as_string()
         self.debug_variable_dictionary = custom_variables
         if self.debug_activated is True:
             self.print_dictionary()
```

### Comparing `debug_utility-0.3/debug_utility/utility_file.py` & `debug_utility-0.4/debug_utility/utility_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,19 +149,17 @@
     # save_config(config_dict, file_path)
 
     @classmethod
     def load_configuration_file(cls, inputs):
         # required inputs for load_configuration_file
         # ri = {
         #     "configuration_full_path_file_name": None,
-        #     "configuration_dictionary": None,
         # }
         ri = {
             "configuration_full_path_file_name": None,
-            "configuration_dictionary": None,
         }
         ri.update(inputs)
         file_path = ri['configuration_full_path_file_name']
         config = configparser.ConfigParser()
         config.read(file_path)
         config_dict = {section: dict(config.items(section)) for section in config.sections()}
         return config_dict
```

### Comparing `debug_utility-0.3/setup.py` & `debug_utility-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='debug_utility',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     description='common functions used while programming in python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Hien Quoc',
     author_email='',
     url='',
```

