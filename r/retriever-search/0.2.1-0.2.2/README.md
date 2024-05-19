# Comparing `tmp/retriever_search-0.2.1.tar.gz` & `tmp/retriever_search-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.2.1.tar", last modified: Sun May 19 17:14:55 2024, max compression
+gzip compressed data, was "retriever_search-0.2.2.tar", last modified: Sun May 19 17:43:10 2024, max compression
```

## Comparing `retriever_search-0.2.1.tar` & `retriever_search-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:14:55.802447 retriever_search-0.2.1/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.1/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:14:55.802054 retriever_search-0.2.1/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.1/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:14:55.799349 retriever_search-0.2.1/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.1/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.1/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.1/retriever_search/Utils.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 17:14:30.000000 retriever_search-0.2.1/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9558 2024-05-02 18:56:07.000000 retriever_search-0.2.1/retriever_search/callbacks.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.1/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.1/retriever_search/layout.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.1/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.1/retriever_search/search_server.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      969 2024-05-05 16:38:52.000000 retriever_search-0.2.1/retriever_search/viz_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:14:55.801295 retriever_search-0.2.1/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      538 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      262 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 17:14:55.000000 retriever_search-0.2.1/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 17:14:55.802548 retriever_search-0.2.1/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1141 2024-05-19 17:14:26.000000 retriever_search-0.2.1/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.717131 retriever_search-0.2.2/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.2/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:43:10.716744 retriever_search-0.2.2/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.2/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.705435 retriever_search-0.2.2/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.2/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.2/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/TopicModellingInit.html
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.2/retriever_search/Utils.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 17:42:24.000000 retriever_search-0.2.2/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.2/retriever_search/callbacks.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.713983 retriever_search-0.2.2/retriever_search/data/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/data/CountVectorizer.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/data/EmbeddedVectors.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/data/LDAModel.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.2/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.2/retriever_search/layout.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.2/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.2/retriever_search/search_server.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1131 2024-05-19 17:41:36.000000 retriever_search-0.2.2/retriever_search/viz_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.716206 retriever_search-0.2.2/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      262 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 17:43:10.717229 retriever_search-0.2.2/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1136 2024-05-19 17:43:03.000000 retriever_search-0.2.2/setup.py
```

### Comparing `retriever_search-0.2.1/LICENSE` & `retriever_search-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/PKG-INFO` & `retriever_search-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.1
+Version: 0.2.2
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.2.1/README.md` & `retriever_search-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/DocumentIngestion.py` & `retriever_search-0.2.2/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/QueryPipeline.py` & `retriever_search-0.2.2/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/callbacks.py` & `retriever_search-0.2.2/retriever_search/callbacks.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import re
 from nltk.corpus import stopwords
 import pickle
 import matplotlib
 import pandas as pd
 import requests
 from tqdm import tqdm
+import os
 
 
 class get_callbacks():
     def __init__(self, app, df, keyword_data):
         self.init_df = df
         self.df = df
         self.title_abs = {}
@@ -28,27 +29,33 @@
         self.get_callback()
         self.n_clicks = 0
         self.search_results = None
         #self.document_store = self.get_retriever(outputDirectory= "./500K_test/" )
 
     
     def init_data(self):
-    
+        
+        this_dir, this_filename = os.path.split(__file__)
+        print(this_dir)
         #Loading the lda_model for topic_modeling
-        with open("./data/LDAModel.pkl", "rb") as f:
+        with open(this_dir + "/data/LDAModel.pkl", "rb") as f:
             ldaModel = pickle.load(f)
 
         #Loading the Count vectorizer array
-        with open("./data/EmbeddedVectors.pkl", "rb") as f:
+        with open(this_dir + "/data/EmbeddedVectors.pkl", "rb") as f:
             dtm_tf = pickle.load(f)
 
         #Loading the Count Vectorizer object
-        with open("./data/CountVectorizer.pkl", "rb") as f:
+        with open(this_dir + "/data/CountVectorizer.pkl", "rb") as f:
             tf_vectorizer = pickle.load(f)
 
+        #ldaModel = pickle.load(importlib.resources.read_text("retriever_search", "LDAModel.pkl"))
+        #dtm_tf = pickle.load(importlib.resources.read_text("retriever_search", "mbeddedVectors.pkl"))
+        #tf_vectorizer = pickle.load(importlib.resources.read_text("retriever_search", "CountVectorizer.pkl"))
+
         return ldaModel, dtm_tf, tf_vectorizer
 
 
 
     def get_json(self,path):
         with open(path, "r") as f:
             return json.load(f)
```

### Comparing `retriever_search-0.2.1/retriever_search/frontend_app.py` & `retriever_search-0.2.2/retriever_search/frontend_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/layout.py` & `retriever_search-0.2.2/retriever_search/layout.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/search_app.py` & `retriever_search-0.2.2/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/search_server.py` & `retriever_search-0.2.2/retriever_search/search_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.1/retriever_search/viz_server.py` & `retriever_search-0.2.2/retriever_search/viz_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #Importing the Libraries
 import dash
 from flask import Flask
 import pandas as pd
 import numpy as np
 from tqdm import tqdm
+import os
 #Test
 import requests
 from retriever_search.callbacks import get_callbacks
 from retriever_search.layout import Layout
 import json
 import warnings
 import ast  
@@ -17,16 +18,18 @@
 server = Flask(__name__)
 app = dash.Dash(__name__, server=server)
 
 def get_init_df():
       return pd.DataFrame(columns = ["title", "title_abs", "doc_ids", "keyword", "emb1", "emb2"])
 
 def init_topicModel():
-   with open('./data/TopicModellingInit.html', 'r') as f:
+   this_dir, this_filename = os.path.split(__file__)
+   with open(this_dir + '/TopicModellingInit.html', 'r') as f:
       vis_html = f.read()
+   #vis_html = importlib.resources.read_binary("retriever_search", "TopicModellingInit.html")
    return vis_html
 
 vis_html = init_topicModel()
 df = get_init_df()
 keyword_data = []
```

### Comparing `retriever_search-0.2.1/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.2.2/retriever_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.1
+Version: 0.2.2
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.2.1/retriever_search.egg-info/SOURCES.txt` & `retriever_search-0.2.2/retriever_search.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 LICENSE
 README.md
 setup.py
 retriever_search/DocumentIngestion.py
 retriever_search/QueryPipeline.py
+retriever_search/TopicModellingInit.html
 retriever_search/Utils.py
 retriever_search/__init__.py
 retriever_search/callbacks.py
 retriever_search/frontend_app.py
 retriever_search/layout.py
 retriever_search/search_app.py
 retriever_search/search_server.py
 retriever_search/viz_server.py
 retriever_search.egg-info/PKG-INFO
 retriever_search.egg-info/SOURCES.txt
 retriever_search.egg-info/dependency_links.txt
 retriever_search.egg-info/requires.txt
-retriever_search.egg-info/top_level.txt
+retriever_search.egg-info/top_level.txt
+retriever_search/data/CountVectorizer.pkl
+retriever_search/data/EmbeddedVectors.pkl
+retriever_search/data/LDAModel.pkl
```

### Comparing `retriever_search-0.2.1/setup.py` & `retriever_search-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
         'plotly==5.10.0',
         'wordcloud==1.9.2',
         'pyLDAvis==3.4.1',
         'nltk==3.7',
     ],
     packages=find_packages(),
     include_package_data=True,
-    package_data={'retriever_search': ['data/CountVectorizer.pkl', 'data/EmbeddedVectors.pkl', 'data/LDAModel.pkl', 'data/TopicModellingInit.html']}
+    package_data={'retriever_search': ['data/CountVectorizer.pkl', 'data/EmbeddedVectors.pkl', 'data/LDAModel.pkl', 'TopicModellingInit.html']}
 )
```

