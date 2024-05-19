# Comparing `tmp/GSG-0.5.7.tar.gz` & `tmp/GSG-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GSG-0.5.7.tar", last modified: Tue May 14 02:56:09 2024, max compression
+gzip compressed data, was "dist/GSG-0.5.8.tar", last modified: Sun May 19 02:21:25 2024, max compression
```

## Comparing `GSG-0.5.7.tar` & `GSG-0.5.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-14 02:56:09.000000 GSG-0.5.7/
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-14 02:56:09.000000 GSG-0.5.7/GSG.egg-info/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-14 02:56:09.000000 GSG-0.5.7/GSG.egg-info/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-05-14 02:56:09.000000 GSG-0.5.7/GSG.egg-info/SOURCES.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-05-14 02:56:09.000000 GSG-0.5.7/GSG.egg-info/dependency_links.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      224 2024-05-14 02:56:09.000000 GSG-0.5.7/GSG.egg-info/requires.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-05-14 02:56:09.000000 GSG-0.5.7/GSG.egg-info/top_level.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    40714 2024-05-13 12:37:54.000000 GSG-0.5.7/GSG.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-14 02:56:09.000000 GSG-0.5.7/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2764 2024-05-01 01:59:10.000000 GSG-0.5.7/README.md
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-14 02:56:09.000000 GSG-0.5.7/datasets/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.7/datasets/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.7/datasets/data_util.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-14 02:56:09.000000 GSG-0.5.7/models/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.7/models/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.7/models/dot_gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.7/models/edcoder.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.7/models/gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.7/models/gcn.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.7/models/gin.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.7/models/loss_func.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-05-14 02:56:09.000000 GSG-0.5.7/setup.cfg
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      810 2024-05-14 02:56:07.000000 GSG-0.5.7/setup.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-14 02:56:09.000000 GSG-0.5.7/tools/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.7/tools/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.7/tools/batch_remove.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.7/tools/evaluation.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.7/tools/parameters_dict.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.7/tools/test.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.7/tools/utils.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-19 02:21:25.000000 GSG-0.5.8/
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-19 02:21:25.000000 GSG-0.5.8/GSG.egg-info/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2940 2024-05-19 02:21:24.000000 GSG-0.5.8/GSG.egg-info/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-05-19 02:21:25.000000 GSG-0.5.8/GSG.egg-info/SOURCES.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-05-19 02:21:24.000000 GSG-0.5.8/GSG.egg-info/dependency_links.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-05-19 02:21:24.000000 GSG-0.5.8/GSG.egg-info/requires.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-05-19 02:21:24.000000 GSG-0.5.8/GSG.egg-info/top_level.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    40714 2024-05-13 12:37:54.000000 GSG-0.5.8/GSG.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2940 2024-05-19 02:21:25.000000 GSG-0.5.8/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2763 2024-05-19 02:21:17.000000 GSG-0.5.8/README.md
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-19 02:21:25.000000 GSG-0.5.8/datasets/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.8/datasets/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.8/datasets/data_util.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-19 02:21:25.000000 GSG-0.5.8/models/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.8/models/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.8/models/dot_gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.8/models/edcoder.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.8/models/gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.8/models/gcn.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.8/models/gin.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.8/models/loss_func.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-05-19 02:21:25.000000 GSG-0.5.8/setup.cfg
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      809 2024-05-19 02:17:15.000000 GSG-0.5.8/setup.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-19 02:21:25.000000 GSG-0.5.8/tools/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.8/tools/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.8/tools/batch_remove.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.8/tools/evaluation.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.8/tools/parameters_dict.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.8/tools/test.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.8/tools/utils.py
```

### Comparing `GSG-0.5.7/GSG.egg-info/PKG-INFO` & `GSG-0.5.8/GSG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GSG
-Version: 0.5.7
+Version: 0.5.8
 Home-page: https://github.com/keaml-Guan/GSG
 License: MIT Licence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GSG: A generative self-supervised graph learning framework for spatial transcriptomics
 ![GitHub Repo stars](https://img.shields.io/github/stars/keaml-Guan/GSG?style=social) ![GitHub forks](https://img.shields.io/github/forks/keaml-Guan/GSG?style=social) ![GitHub watchers](https://img.shields.io/github/watchers/keaml-Guan/GSG?style=social)
@@ -29,14 +29,14 @@
 * scikit-learn==1.0.1 
 * tqdm==4.64.1
 * matplotlib==3.5.3
 * tensorboardX==2.5.1
 * pyyaml==6.0.1
 * ploty==5.21.0
 * kaleido==0.2.1
-* igraph==0.11.4
+* igraph==0.9.8
 
 ## Citation
 
 <mark>
 Guan, R., Sun, H., Zhang, T., Wu, Z., Du, M., Liang, Y., ... & Xu, D. (2024). Generative Self-Supervised Graphs Enhance Integration, Imputation and Domains Identification of Spatial Transcriptomics.
 </mark>
```

### Comparing `GSG-0.5.7/GSG.py` & `GSG-0.5.8/GSG.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/PKG-INFO` & `GSG-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GSG
-Version: 0.5.7
+Version: 0.5.8
 Home-page: https://github.com/keaml-Guan/GSG
 License: MIT Licence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GSG: A generative self-supervised graph learning framework for spatial transcriptomics
 ![GitHub Repo stars](https://img.shields.io/github/stars/keaml-Guan/GSG?style=social) ![GitHub forks](https://img.shields.io/github/forks/keaml-Guan/GSG?style=social) ![GitHub watchers](https://img.shields.io/github/watchers/keaml-Guan/GSG?style=social)
@@ -29,14 +29,14 @@
 * scikit-learn==1.0.1 
 * tqdm==4.64.1
 * matplotlib==3.5.3
 * tensorboardX==2.5.1
 * pyyaml==6.0.1
 * ploty==5.21.0
 * kaleido==0.2.1
-* igraph==0.11.4
+* igraph==0.9.8
 
 ## Citation
 
 <mark>
 Guan, R., Sun, H., Zhang, T., Wu, Z., Du, M., Liang, Y., ... & Xu, D. (2024). Generative Self-Supervised Graphs Enhance Integration, Imputation and Domains Identification of Spatial Transcriptomics.
 </mark>
```

### Comparing `GSG-0.5.7/README.md` & `GSG-0.5.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 * scikit-learn==1.0.1 
 * tqdm==4.64.1
 * matplotlib==3.5.3
 * tensorboardX==2.5.1
 * pyyaml==6.0.1
 * ploty==5.21.0
 * kaleido==0.2.1
-* igraph==0.11.4
+* igraph==0.9.8
 
 ## Citation
 
 <mark>
 Guan, R., Sun, H., Zhang, T., Wu, Z., Du, M., Liang, Y., ... & Xu, D. (2024). Generative Self-Supervised Graphs Enhance Integration, Imputation and Domains Identification of Spatial Transcriptomics.
 </mark>
```

### Comparing `GSG-0.5.7/datasets/data_util.py` & `GSG-0.5.8/datasets/data_util.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/__init__.py` & `GSG-0.5.8/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/dot_gat.py` & `GSG-0.5.8/models/dot_gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/edcoder.py` & `GSG-0.5.8/models/edcoder.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/gat.py` & `GSG-0.5.8/models/gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/gcn.py` & `GSG-0.5.8/models/gcn.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/gin.py` & `GSG-0.5.8/models/gin.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/models/loss_func.py` & `GSG-0.5.8/models/loss_func.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/setup.py` & `GSG-0.5.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name = 'GSG',
-    version='0.5.7',
+    version='0.5.8',
     packages=find_packages(),
     python_requires='>=3.8',
     py_modules=['GSG'],
     long_description=open(os.path.join("./","README.md"), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license="MIT Licence",
     url="https://github.com/keaml-Guan/GSG",
@@ -22,10 +22,10 @@
         'scikit-learn==1.0.1',
         'tqdm==4.64.1',
         'matplotlib==3.5.3',
         'tensorboardX==2.5.1',
         'pyyaml==6.0.1',
         'plotly==5.21.0',
         'kaleido==0.2.1',
-        'igraph==0.11.4',
+        'igraph==0.9.8',
     ]
 )
```

### Comparing `GSG-0.5.7/tools/batch_remove.py` & `GSG-0.5.8/tools/batch_remove.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/tools/evaluation.py` & `GSG-0.5.8/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/tools/parameters_dict.py` & `GSG-0.5.8/tools/parameters_dict.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/tools/test.py` & `GSG-0.5.8/tools/test.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.7/tools/utils.py` & `GSG-0.5.8/tools/utils.py`

 * *Files identical despite different names*

