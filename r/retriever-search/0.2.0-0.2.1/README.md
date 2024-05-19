# Comparing `tmp/retriever_search-0.2.0.tar.gz` & `tmp/retriever_search-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.2.0.tar", last modified: Sun May  5 16:23:08 2024, max compression
+gzip compressed data, was "retriever_search-0.2.1.tar", last modified: Sun May 19 17:14:55 2024, max compression
```

## Comparing `retriever_search-0.2.0.tar` & `retriever_search-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-05 16:23:08.797545 retriever_search-0.2.0/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.0/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-05 16:23:08.796574 retriever_search-0.2.0/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.0/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-05 16:23:08.783742 retriever_search-0.2.0/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.0/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.0/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.0/retriever_search/Utils.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       85 2024-05-05 16:22:58.000000 retriever_search-0.2.0/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9558 2024-05-02 18:56:07.000000 retriever_search-0.2.0/retriever_search/callbacks.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.0/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.0/retriever_search/layout.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.0/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.0/retriever_search/search_server.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      935 2024-05-02 19:58:24.000000 retriever_search-0.2.0/retriever_search/viz_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-05 16:23:08.795175 retriever_search-0.2.0/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      538 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      262 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-05 16:23:08.000000 retriever_search-0.2.0/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-05 16:23:08.797803 retriever_search-0.2.0/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      961 2024-05-02 20:12:06.000000 retriever_search-0.2.0/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:14:55.802447 retriever_search-0.2.1/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.1/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:14:55.802054 retriever_search-0.2.1/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.1/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:14:55.799349 retriever_search-0.2.1/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.1/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.1/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.1/retriever_search/Utils.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 17:14:30.000000 retriever_search-0.2.1/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9558 2024-05-02 18:56:07.000000 retriever_search-0.2.1/retriever_search/callbacks.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.1/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.1/retriever_search/layout.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.1/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.1/retriever_search/search_server.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      969 2024-05-05 16:38:52.000000 retriever_search-0.2.1/retriever_search/viz_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:14:55.801295 retriever_search-0.2.1/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      538 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      262 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 17:14:55.802548 retriever_search-0.2.1/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1141 2024-05-19 17:14:26.000000 retriever_search-0.2.1/setup.py
```

### Comparing `retriever_search-0.2.0/LICENSE` & `retriever_search-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/PKG-INFO` & `retriever_search-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.0
+Version: 0.2.1
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.2.0/README.md` & `retriever_search-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/DocumentIngestion.py` & `retriever_search-0.2.1/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/QueryPipeline.py` & `retriever_search-0.2.1/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/callbacks.py` & `retriever_search-0.2.1/retriever_search/callbacks.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/frontend_app.py` & `retriever_search-0.2.1/retriever_search/frontend_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/layout.py` & `retriever_search-0.2.1/retriever_search/layout.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/search_app.py` & `retriever_search-0.2.1/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/search_server.py` & `retriever_search-0.2.1/retriever_search/search_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/retriever_search/viz_server.py` & `retriever_search-0.2.1/retriever_search/viz_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import dash
 from flask import Flask
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
 #Test
 import requests
-from callbacks import get_callbacks
-from layout import Layout
+from retriever_search.callbacks import get_callbacks
+from retriever_search.layout import Layout
 import json
 import warnings
 import ast  
 
 warnings.filterwarnings("ignore")
 
 server = Flask(__name__)
```

### Comparing `retriever_search-0.2.0/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.2.1/retriever_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.0
+Version: 0.2.1
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.2.0/retriever_search.egg-info/SOURCES.txt` & `retriever_search-0.2.1/retriever_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.0/setup.py` & `retriever_search-0.2.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,8 +28,10 @@
         'dash==2.15.0',
         'plotly==5.10.0',
         'wordcloud==1.9.2',
         'pyLDAvis==3.4.1',
         'nltk==3.7',
     ],
     packages=find_packages(),
+    include_package_data=True,
+    package_data={'retriever_search': ['data/CountVectorizer.pkl', 'data/EmbeddedVectors.pkl', 'data/LDAModel.pkl', 'data/TopicModellingInit.html']}
 )
```

