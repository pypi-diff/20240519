# Comparing `tmp/TaGra-0.1.3.tar.gz` & `tmp/TaGra-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TaGra-0.1.3.tar", last modified: Sun May 19 00:14:46 2024, max compression
+gzip compressed data, was "TaGra-0.1.4.tar", last modified: Sun May 19 00:26:48 2024, max compression
```

## Comparing `TaGra-0.1.3.tar` & `TaGra-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.596997 TaGra-0.1.3/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.3/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)     3336 2024-05-19 00:14:46.596997 TaGra-0.1.3/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)     2825 2024-05-18 16:28:01.000000 TaGra-0.1.3/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.592997 TaGra-0.1.3/TaGra.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)     3336 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/entry_points.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-19 00:14:46.000000 TaGra-0.1.3/TaGra.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-19 00:14:46.596997 TaGra-0.1.3/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-19 00:14:10.000000 TaGra-0.1.3/setup.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.592997 TaGra-0.1.3/tagra/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.3/tagra/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.3/tagra/analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.3/tagra/config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.3/tagra/graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.3/tagra/preprocessing.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7373 2024-05-19 00:03:59.000000 TaGra-0.1.3/tagra/utils.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:14:46.596997 TaGra-0.1.3/tests/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.3/tests/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.3/tests/test_analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.3/tests/test_config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.3/tests/test_graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.3/tests/test_preprocessing.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:26:48.365706 TaGra-0.1.4/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.4/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 00:26:48.365706 TaGra-0.1.4/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3116 2024-05-19 00:21:18.000000 TaGra-0.1.4/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:26:48.365706 TaGra-0.1.4/TaGra.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 00:26:48.000000 TaGra-0.1.4/TaGra.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-19 00:26:48.000000 TaGra-0.1.4/TaGra.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-19 00:26:48.000000 TaGra-0.1.4/TaGra.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-19 00:26:48.000000 TaGra-0.1.4/TaGra.egg-info/entry_points.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-19 00:26:48.000000 TaGra-0.1.4/TaGra.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-19 00:26:48.000000 TaGra-0.1.4/TaGra.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-19 00:26:48.365706 TaGra-0.1.4/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-19 00:26:45.000000 TaGra-0.1.4/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:26:48.365706 TaGra-0.1.4/tagra/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.4/tagra/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.4/tagra/analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.4/tagra/config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.4/tagra/graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.4/tagra/preprocessing.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7372 2024-05-19 00:24:42.000000 TaGra-0.1.4/tagra/utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:26:48.365706 TaGra-0.1.4/tests/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.4/tests/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.4/tests/test_analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.4/tests/test_config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.4/tests/test_graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.4/tests/test_preprocessing.py
```

### Comparing `TaGra-0.1.3/LICENSE` & `TaGra-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/PKG-INFO` & `TaGra-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.3
+Version: 0.1.4
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,20 @@
 ## Installation
 
 To install TaGra, simply use pip:
 
 ```sh
 pip install tagra
 ```
+## Quickstart
+```sh
+python3 examples/examples_usage.py -c examples/example_config.json
+```
+You can edit the option in ```examples/example_config.json``` and adapt them as you wish.
+The default option will produce a prepreocessing and a graph based on the ```moons``` dataset (SciKit Learn).
 
 # Usage
 ## Data Preprocessing
 
 ```python
 from tagra.preprocessing import preprocess_dataframe
```

### Comparing `TaGra-0.1.3/README.md` & `TaGra-0.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 ## Installation
 
 To install TaGra, simply use pip:
 
 ```sh
 pip install tagra
 ```
+## Quickstart
+```sh
+python3 examples/examples_usage.py -c examples/example_config.json
+```
+You can edit the option in ```examples/example_config.json``` and adapt them as you wish.
+The default option will produce a prepreocessing and a graph based on the ```moons``` dataset (SciKit Learn).
 
 # Usage
 ## Data Preprocessing
 
 ```python
 from tagra.preprocessing import preprocess_dataframe
```

### Comparing `TaGra-0.1.3/TaGra.egg-info/PKG-INFO` & `TaGra-0.1.4/TaGra.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.3
+Version: 0.1.4
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,14 +28,20 @@
 ## Installation
 
 To install TaGra, simply use pip:
 
 ```sh
 pip install tagra
 ```
+## Quickstart
+```sh
+python3 examples/examples_usage.py -c examples/example_config.json
+```
+You can edit the option in ```examples/example_config.json``` and adapt them as you wish.
+The default option will produce a prepreocessing and a graph based on the ```moons``` dataset (SciKit Learn).
 
 # Usage
 ## Data Preprocessing
 
 ```python
 from tagra.preprocessing import preprocess_dataframe
```

### Comparing `TaGra-0.1.3/setup.py` & `TaGra-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TaGra',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'scikit-learn',
         'matplotlib',
         'networkx',
```

### Comparing `TaGra-0.1.3/tagra/analysis.py` & `TaGra-0.1.4/tagra/analysis.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tagra/config.py` & `TaGra-0.1.4/tagra/config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tagra/graph.py` & `TaGra-0.1.4/tagra/graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tagra/preprocessing.py` & `TaGra-0.1.4/tagra/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tagra/utils.py` & `TaGra-0.1.4/tagra/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import networkx as nx
 import matplotlib.pyplot as plt
-import matplotlib.cm as cm
+from matplotlib import cm
 import pandas as pd
 import numpy as np
 
 def analyze_neighborhood_attributes(graph, attribute_name, return_probs=False):
     """
     Analyzes attributes in the neighborhoods of each node in a graph, optionally returning probabilities.
```

### Comparing `TaGra-0.1.3/tests/test_analysis.py` & `TaGra-0.1.4/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tests/test_config.py` & `TaGra-0.1.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tests/test_graph.py` & `TaGra-0.1.4/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.3/tests/test_preprocessing.py` & `TaGra-0.1.4/tests/test_preprocessing.py`

 * *Files identical despite different names*

