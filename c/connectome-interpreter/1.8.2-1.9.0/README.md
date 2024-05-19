# Comparing `tmp/connectome_interpreter-1.8.2.tar.gz` & `tmp/connectome_interpreter-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectome_interpreter-1.8.2.tar", last modified: Wed May 15 14:28:27 2024, max compression
+gzip compressed data, was "connectome_interpreter-1.9.0.tar", last modified: Sun May 19 12:30:35 2024, max compression
```

## Comparing `connectome_interpreter-1.8.2.tar` & `connectome_interpreter-1.9.0.tar`

### file list

```diff
@@ -1,22 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 14:28:27.169427 connectome_interpreter-1.8.2/
--rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.2/LICENSE
--rw-rw-rw-   0        0        0     1066 2024-05-15 14:28:27.168437 connectome_interpreter-1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 14:28:27.129202 connectome_interpreter-1.8.2/connectome_interpreter/
--rw-rw-rw-   0        0        0      136 2024-03-07 21:35:51.000000 connectome_interpreter-1.8.2/connectome_interpreter/__init__.py
--rw-rw-rw-   0        0        0    36418 2024-05-11 20:34:13.000000 connectome_interpreter-1.8.2/connectome_interpreter/activation_maximisation.py
--rw-rw-rw-   0        0        0    22758 2024-05-15 13:20:48.000000 connectome_interpreter-1.8.2/connectome_interpreter/compress_paths.py
--rw-rw-rw-   0        0        0    16221 2024-05-07 10:46:28.000000 connectome_interpreter-1.8.2/connectome_interpreter/path_finding.py
--rw-rw-rw-   0        0        0    35768 2024-05-15 14:26:16.000000 connectome_interpreter-1.8.2/connectome_interpreter/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:28:27.163763 connectome_interpreter-1.8.2/connectome_interpreter.egg-info/
--rw-rw-rw-   0        0        0     1066 2024-05-15 14:28:27.000000 connectome_interpreter-1.8.2/connectome_interpreter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-05-15 14:28:27.000000 connectome_interpreter-1.8.2/connectome_interpreter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 14:28:27.000000 connectome_interpreter-1.8.2/connectome_interpreter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2024-05-15 14:28:27.000000 connectome_interpreter-1.8.2/connectome_interpreter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-15 14:28:27.000000 connectome_interpreter-1.8.2/connectome_interpreter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 14:28:27.169427 connectome_interpreter-1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2068 2024-05-15 14:27:00.000000 connectome_interpreter-1.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 14:28:27.167327 connectome_interpreter-1.8.2/tests/
--rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.8.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.8.2/tests/test_compress_paths.py
--rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.8.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.988152 connectome_interpreter-1.9.0/
+-rw-rw-rw-   0        0        0     1086 2024-02-16 09:04:27.000000 connectome_interpreter-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0     1160 2024-05-19 12:30:35.988152 connectome_interpreter-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-04-14 17:28:06.000000 connectome_interpreter-1.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.847746 connectome_interpreter-1.9.0/connectome_interpreter/
+-rw-rw-rw-   0        0        0      150 2024-05-19 11:49:28.000000 connectome_interpreter-1.9.0/connectome_interpreter/__init__.py
+-rw-rw-rw-   0        0        0    36418 2024-05-11 20:34:13.000000 connectome_interpreter-1.9.0/connectome_interpreter/activation_maximisation.py
+-rw-rw-rw-   0        0        0    22758 2024-05-15 13:20:48.000000 connectome_interpreter-1.9.0/connectome_interpreter/compress_paths.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.826262 connectome_interpreter-1.9.0/connectome_interpreter/data/
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.920777 connectome_interpreter-1.9.0/connectome_interpreter/data/DoOR/
+-rw-rw-rw-   0        0        0    70570 2024-05-16 14:59:43.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/DoOR/door_chemical_meta.csv
+-rw-rw-rw-   0        0        0    12925 2024-05-16 14:21:59.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/DoOR/door_receptor_mappings.csv
+-rw-rw-rw-   0        0        0   297106 2024-05-16 14:21:59.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/DoOR/door_response_matrix.csv
+-rw-rw-rw-   0        0        0   265329 2024-05-18 21:16:55.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/DoOR/processed_door_adult.csv
+-rw-rw-rw-   0        0        0   671356 2024-05-18 21:16:55.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/DoOR/processed_door_adult_sfr_subtracted.csv
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.984165 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/
+-rw-rw-rw-   0        0        0    35430 2024-05-16 16:32:36.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/1-s2.0-S2211124718306636-mmc2.xlsx
+-rw-rw-rw-   0        0        0    41406 2024-05-16 16:38:31.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/1-s2.0-S2211124718306636-mmc3.xlsx
+-rw-rw-rw-   0        0        0    46704 2024-05-16 16:45:49.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/1-s2.0-S2211124718306636-mmc4.xlsx
+-rw-rw-rw-   0        0        0    21649 2024-05-19 12:00:41.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/adult_chem2glom.csv
+-rw-rw-rw-   0        0        0    10527 2024-05-19 12:00:41.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/adult_fruit2glom.csv
+-rw-rw-rw-   0        0        0    12036 2024-05-19 12:00:41.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/larva_chem2or.csv
+-rw-rw-rw-   0        0        0     5777 2024-05-19 12:00:41.000000 connectome_interpreter-1.9.0/connectome_interpreter/data/Dweck2018/larva_fruit2or.csv
+-rw-rw-rw-   0        0        0     6505 2024-05-19 12:08:48.000000 connectome_interpreter-1.9.0/connectome_interpreter/external_map.py
+-rw-rw-rw-   0        0        0    16221 2024-05-07 10:46:28.000000 connectome_interpreter-1.9.0/connectome_interpreter/path_finding.py
+-rw-rw-rw-   0        0        0    35768 2024-05-15 14:26:16.000000 connectome_interpreter-1.9.0/connectome_interpreter/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.874791 connectome_interpreter-1.9.0/connectome_interpreter.egg-info/
+-rw-rw-rw-   0        0        0     1160 2024-05-19 12:30:35.000000 connectome_interpreter-1.9.0/connectome_interpreter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2024-05-19 12:30:35.000000 connectome_interpreter-1.9.0/connectome_interpreter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 12:30:35.000000 connectome_interpreter-1.9.0/connectome_interpreter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      153 2024-05-19 12:30:35.000000 connectome_interpreter-1.9.0/connectome_interpreter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-19 12:30:35.000000 connectome_interpreter-1.9.0/connectome_interpreter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 12:30:35.989149 connectome_interpreter-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2225 2024-05-19 12:29:35.000000 connectome_interpreter-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 12:30:35.986159 connectome_interpreter-1.9.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-02-16 09:04:27.000000 connectome_interpreter-1.9.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-04-20 17:48:24.000000 connectome_interpreter-1.9.0/tests/test_compress_paths.py
+-rw-rw-rw-   0        0        0     2534 2024-04-20 14:38:13.000000 connectome_interpreter-1.9.0/tests/test_utils.py
```

### Comparing `connectome_interpreter-1.8.2/LICENSE` & `connectome_interpreter-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/PKG-INFO` & `connectome_interpreter-1.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome_interpreter
-Version: 1.8.2
+Version: 1.9.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
@@ -18,9 +18,11 @@
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
+Provides-Extra: map-to-experiment
+Requires-Dist: scikit-learn; extra == "map-to-experiment"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.8.2/README.md` & `connectome_interpreter-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/connectome_interpreter/activation_maximisation.py` & `connectome_interpreter-1.9.0/connectome_interpreter/activation_maximisation.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/connectome_interpreter/compress_paths.py` & `connectome_interpreter-1.9.0/connectome_interpreter/compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/connectome_interpreter/path_finding.py` & `connectome_interpreter-1.9.0/connectome_interpreter/path_finding.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/connectome_interpreter/utils.py` & `connectome_interpreter-1.9.0/connectome_interpreter/utils.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/connectome_interpreter.egg-info/PKG-INFO` & `connectome_interpreter-1.9.0/connectome_interpreter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectome-interpreter
-Version: 1.8.2
+Version: 1.9.0
 Summary: A tool for connectomics data interpretation
 Author: Yijie Yin
 Author-email: yy432@cam.ac.uk
 Project-URL: Source, https: // github.com/YijieYin/connectome_interpreter
 Project-URL: Documentation, https://connectome-interpreter.readthedocs.io/en/latest/
 Project-URL: Larva connectome example, https://colab.research.google.com/drive/1VIMNFBp7dCgN5XOQ9vvzPaqb80BGPZx4?usp=sharing
 Project-URL: Adult connectome example (FAFB), https://colab.research.google.com/drive/1ECUagwN-r2rnKyfcYgtR1oG8Lox8m8BW?usp=sharing
@@ -18,9 +18,11 @@
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: seaborn
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
 Provides-Extra: get-ngl-link
 Requires-Dist: nglscenes; extra == "get-ngl-link"
+Provides-Extra: map-to-experiment
+Requires-Dist: scikit-learn; extra == "map-to-experiment"
 Provides-Extra: wandb
 Requires-Dist: wandb; extra == "wandb"
```

### Comparing `connectome_interpreter-1.8.2/setup.py` & `connectome_interpreter-1.9.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,21 +31,26 @@
 
 
 setup(
     name='connectome_interpreter',
     # If you're making a patch or a minor bug fix, increment the patch version, e.g., from 0.1.0 to 0.1.1.
     # If you're adding functionality in a backwards-compatible manner, increment the minor version, e.g., from 0.1.0 to 0.2.0.
     # If you're making incompatible API changes, increment the major version, e.g., from 0.1.0 to 1.0.0.
-    version='1.8.2',
+    version='1.9.0',
     packages=find_packages(),
     install_requires=install_requires_list,
     extras_require={
         'get_ngl_link': ['nglscenes'],
+        'map_to_experiment': ['scikit-learn'],
         'wandb': ['wandb'],
     },
+    include_package_data=True,
+    package_data={
+        'connectome_interpreter': ['data/*/*'],
+    },
     # Optional metadata
     author='Yijie Yin',
     author_email='yy432@cam.ac.uk',
     description='A tool for connectomics data interpretation',
     keywords=['connectomics', 'neural network',
               'mechanistic interpretability'],
     project_urls={
```

### Comparing `connectome_interpreter-1.8.2/tests/test_compress_paths.py` & `connectome_interpreter-1.9.0/tests/test_compress_paths.py`

 * *Files identical despite different names*

### Comparing `connectome_interpreter-1.8.2/tests/test_utils.py` & `connectome_interpreter-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

