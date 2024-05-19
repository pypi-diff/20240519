# Comparing `tmp/TestGeneratorPluginLib-1.2.2.tar.gz` & `tmp/TestGeneratorPluginLib-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TestGeneratorPluginLib-1.2.2.tar", last modified: Fri May 17 16:48:08 2024, max compression
+gzip compressed data, was "TestGeneratorPluginLib-1.2.3.tar", last modified: Sat May 18 18:46:19 2024, max compression
```

## Comparing `TestGeneratorPluginLib-1.2.2.tar` & `TestGeneratorPluginLib-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 16:48:08.342444 TestGeneratorPluginLib-1.2.2/
--rw-rw-rw-   0        0        0     1090 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     1569 2024-05-17 16:48:08.342444 TestGeneratorPluginLib-1.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-17 16:48:08.326825 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/
--rw-rw-rw-   0        0        0      425 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/__init__.py
--rw-rw-rw-   0        0        0     2419 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_built_plugin.py
--rw-rw-rw-   0        0        0       19 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_config.py
--rw-rw-rw-   0        0        0     1839 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_language.py
--rw-rw-rw-   0        0        0     1219 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_managers.py
--rw-rw-rw-   0        0        0      645 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_plugin.py
--rw-rw-rw-   0        0        0     2854 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_plugin_setup.py
--rw-rw-rw-   0        0        0     3344 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-17 16:48:08.326825 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/
--rw-rw-rw-   0        0        0     1569 2024-05-17 16:48:08.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-05-17 16:48:08.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 16:48:08.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-17 16:48:08.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-17 16:48:08.000000 TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 16:48:08.342444 TestGeneratorPluginLib-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1288 2024-05-17 16:47:26.000000 TestGeneratorPluginLib-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:46:19.899820 TestGeneratorPluginLib-1.2.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1569 2024-05-18 18:46:19.899820 TestGeneratorPluginLib-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 18:46:19.884205 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/
+-rw-rw-rw-   0        0        0      425 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/__init__.py
+-rw-rw-rw-   0        0        0     2419 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_built_plugin.py
+-rw-rw-rw-   0        0        0       19 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_config.py
+-rw-rw-rw-   0        0        0     1839 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_language.py
+-rw-rw-rw-   0        0        0     1219 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_managers.py
+-rw-rw-rw-   0        0        0      645 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_plugin.py
+-rw-rw-rw-   0        0        0     2854 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_plugin_setup.py
+-rw-rw-rw-   0        0        0     3344 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-18 18:46:19.899820 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/
+-rw-rw-rw-   0        0        0     1569 2024-05-18 18:46:19.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2024-05-18 18:46:19.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 18:46:19.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-18 18:46:19.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-18 18:46:19.000000 TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 18:46:19.899820 TestGeneratorPluginLib-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2024-05-18 18:45:22.000000 TestGeneratorPluginLib-1.2.3/setup.py
```

### Comparing `TestGeneratorPluginLib-1.2.2/LICENSE` & `TestGeneratorPluginLib-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/PKG-INFO` & `TestGeneratorPluginLib-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.2.2
+Version: 1.2.3
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_built_plugin.py` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_built_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_language.py` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_language.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_managers.py` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_managers.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_plugin.py` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_plugin.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_plugin_setup.py` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_plugin_setup.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib/_widgets.py` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib/_widgets.py`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/PKG-INFO` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TestGeneratorPluginLib
-Version: 1.2.2
+Version: 1.2.3
 Summary: A TestGeneratorPluginLib package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) [year] [fullname]
```

### Comparing `TestGeneratorPluginLib-1.2.2/TestGeneratorPluginLib.egg-info/SOURCES.txt` & `TestGeneratorPluginLib-1.2.3/TestGeneratorPluginLib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TestGeneratorPluginLib-1.2.2/setup.py` & `TestGeneratorPluginLib-1.2.3/setup.py`

 * *Files identical despite different names*

