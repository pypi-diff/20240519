# Comparing `tmp/TaGra-0.1.5.tar.gz` & `tmp/TaGra-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TaGra-0.1.5.tar", last modified: Sun May 19 00:35:09 2024, max compression
+gzip compressed data, was "TaGra-0.1.6.tar", last modified: Sun May 19 13:48:09 2024, max compression
```

## Comparing `TaGra-0.1.5.tar` & `TaGra-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:35:09.402901 TaGra-0.1.5/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.5/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 00:35:09.402901 TaGra-0.1.5/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)     3116 2024-05-19 00:21:18.000000 TaGra-0.1.5/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:35:09.402901 TaGra-0.1.5/TaGra.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 00:35:09.000000 TaGra-0.1.5/TaGra.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-19 00:35:09.000000 TaGra-0.1.5/TaGra.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-19 00:35:09.000000 TaGra-0.1.5/TaGra.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-19 00:35:09.000000 TaGra-0.1.5/TaGra.egg-info/entry_points.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-19 00:35:09.000000 TaGra-0.1.5/TaGra.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-19 00:35:09.000000 TaGra-0.1.5/TaGra.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-19 00:35:09.402901 TaGra-0.1.5/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-19 00:34:48.000000 TaGra-0.1.5/setup.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:35:09.402901 TaGra-0.1.5/tagra/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.5/tagra/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.5/tagra/analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.5/tagra/config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.5/tagra/graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.5/tagra/preprocessing.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     7340 2024-05-19 00:32:06.000000 TaGra-0.1.5/tagra/utils.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 00:35:09.402901 TaGra-0.1.5/tests/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.5/tests/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.5/tests/test_analysis.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.5/tests/test_config.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.5/tests/test_graph.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.5/tests/test_preprocessing.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:48:09.146184 TaGra-0.1.6/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1084 2024-05-18 14:14:07.000000 TaGra-0.1.6/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 13:48:09.146184 TaGra-0.1.6/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3116 2024-05-19 00:21:18.000000 TaGra-0.1.6/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:48:09.146184 TaGra-0.1.6/TaGra.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3627 2024-05-19 13:48:09.000000 TaGra-0.1.6/TaGra.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      417 2024-05-19 13:48:09.000000 TaGra-0.1.6/TaGra.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-19 13:48:09.000000 TaGra-0.1.6/TaGra.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       39 2024-05-19 13:48:09.000000 TaGra-0.1.6/TaGra.egg-info/entry_points.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       53 2024-05-19 13:48:09.000000 TaGra-0.1.6/TaGra.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       12 2024-05-19 13:48:09.000000 TaGra-0.1.6/TaGra.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       38 2024-05-19 13:48:09.146184 TaGra-0.1.6/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)      881 2024-05-19 13:43:39.000000 TaGra-0.1.6/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:48:09.146184 TaGra-0.1.6/tagra/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:06.000000 TaGra-0.1.6/tagra/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2829 2024-05-19 00:09:22.000000 TaGra-0.1.6/tagra/analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1062 2024-05-18 15:46:39.000000 TaGra-0.1.6/tagra/config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3892 2024-05-18 16:04:47.000000 TaGra-0.1.6/tagra/graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7803 2024-05-18 16:00:39.000000 TaGra-0.1.6/tagra/preprocessing.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     7315 2024-05-19 13:36:33.000000 TaGra-0.1.6/tagra/utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-19 13:48:09.146184 TaGra-0.1.6/tests/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2024-05-18 11:59:49.000000 TaGra-0.1.6/tests/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2447 2024-05-19 00:12:28.000000 TaGra-0.1.6/tests/test_analysis.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1444 2024-05-18 13:20:47.000000 TaGra-0.1.6/tests/test_config.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      977 2024-05-18 14:06:00.000000 TaGra-0.1.6/tests/test_graph.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2803 2024-05-18 13:52:06.000000 TaGra-0.1.6/tests/test_preprocessing.py
```

### Comparing `TaGra-0.1.5/LICENSE` & `TaGra-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/PKG-INFO` & `TaGra-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.5
+Version: 0.1.6
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TaGra-0.1.5/README.md` & `TaGra-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/TaGra.egg-info/PKG-INFO` & `TaGra-0.1.6/TaGra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TaGra
-Version: 0.1.5
+Version: 0.1.6
 Summary: TaGra: TAbular data preprocessing to GRAph representation.
 Home-page: https://github.com/davidetorre92/TaGra
 Author: Davide Torre, Davide Chicco
 Author-email: davidetorre92@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TaGra-0.1.5/setup.py` & `TaGra-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='TaGra',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'pandas',
         'scikit-learn',
         'matplotlib',
         'networkx',
```

### Comparing `TaGra-0.1.5/tagra/analysis.py` & `TaGra-0.1.6/tagra/analysis.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tagra/config.py` & `TaGra-0.1.6/tagra/config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tagra/graph.py` & `TaGra-0.1.6/tagra/graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tagra/preprocessing.py` & `TaGra-0.1.6/tagra/preprocessing.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tagra/utils.py` & `TaGra-0.1.6/tagra/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import networkx as nx
 import matplotlib.pyplot as plt
-from matplotlib import cm
 import pandas as pd
 import numpy as np
 
 def analyze_neighborhood_attributes(graph, attribute_name, return_probs=False):
     """
     Analyzes attributes in the neighborhoods of each node in a graph, optionally returning probabilities.
 
@@ -162,15 +161,15 @@
     node_color = []
     if attribute is not None:
         classification_attribute_name = attribute
         y = np.array([G.nodes[node][classification_attribute_name] for node in G.nodes()])
         unique = np.unique(y)
         unique_dict = {key: index for index, key in enumerate(unique)}
         colors = np.linspace(0, 1, len(unique))
-        cmap = cm.get_cmap(palette, len(unique))
+        cmap = plt.get_cmap(palette, len(unique))
         color_array = cmap(colors)
         node_color = [color_array[unique_dict[key]] for key in y]
     nx.draw(G, pos, with_labels=True, node_size=50, font_size=8, node_color = node_color)
     plt.title("Graph of Relations Based on Manifold Learning Transformed Data")
     if outpath:
         plt.savefig(outpath)
         print(f'{datetime.datetime.now()}: Graph saved in {outpath}')
```

### Comparing `TaGra-0.1.5/tests/test_analysis.py` & `TaGra-0.1.6/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tests/test_config.py` & `TaGra-0.1.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tests/test_graph.py` & `TaGra-0.1.6/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `TaGra-0.1.5/tests/test_preprocessing.py` & `TaGra-0.1.6/tests/test_preprocessing.py`

 * *Files identical despite different names*

