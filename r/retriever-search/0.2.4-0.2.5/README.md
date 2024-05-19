# Comparing `tmp/retriever_search-0.2.4.tar.gz` & `tmp/retriever_search-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.2.4.tar", last modified: Sun May 19 19:42:42 2024, max compression
+gzip compressed data, was "retriever_search-0.2.5.tar", last modified: Sun May 19 21:00:24 2024, max compression
```

## Comparing `retriever_search-0.2.4.tar` & `retriever_search-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 19:42:42.073857 retriever_search-0.2.4/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.4/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 19:42:42.073439 retriever_search-0.2.4/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.4/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 19:42:42.053360 retriever_search-0.2.4/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.4/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.4/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.4/retriever_search/TopicModellingInit.html
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.4/retriever_search/Utils.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 19:40:39.000000 retriever_search-0.2.4/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.4/retriever_search/callbacks.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 19:42:42.063313 retriever_search-0.2.4/retriever_search/data/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.4/retriever_search/data/CountVectorizer.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.4/retriever_search/data/EmbeddedVectors.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.4/retriever_search/data/LDAModel.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3622 2024-05-19 19:42:34.000000 retriever_search-0.2.4/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.4/retriever_search/layout.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.4/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3491 2024-05-19 19:41:40.000000 retriever_search-0.2.4/retriever_search/search_server.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1131 2024-05-19 17:41:36.000000 retriever_search-0.2.4/retriever_search/viz_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 19:42:42.072901 retriever_search-0.2.4/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 19:42:42.000000 retriever_search-0.2.4/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-19 19:42:42.000000 retriever_search-0.2.4/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 19:42:42.000000 retriever_search-0.2.4/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      255 2024-05-19 19:42:42.000000 retriever_search-0.2.4/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 19:42:42.000000 retriever_search-0.2.4/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 19:42:42.073961 retriever_search-0.2.4/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1129 2024-05-19 19:01:43.000000 retriever_search-0.2.4/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.120120 retriever_search-0.2.5/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.5/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 21:00:24.119756 retriever_search-0.2.5/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.5/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.093565 retriever_search-0.2.5/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.5/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.5/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/TopicModellingInit.html
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.5/retriever_search/Utils.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 21:00:18.000000 retriever_search-0.2.5/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.5/retriever_search/callbacks.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.103960 retriever_search-0.2.5/retriever_search/data/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/data/CountVectorizer.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/data/EmbeddedVectors.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.5/retriever_search/data/LDAModel.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3623 2024-05-19 19:45:03.000000 retriever_search-0.2.5/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.5/retriever_search/layout.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.5/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3491 2024-05-19 19:41:40.000000 retriever_search-0.2.5/retriever_search/search_server.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1174 2024-05-19 20:59:49.000000 retriever_search-0.2.5/retriever_search/viz_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 21:00:24.119270 retriever_search-0.2.5/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      255 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 21:00:24.000000 retriever_search-0.2.5/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 21:00:24.120210 retriever_search-0.2.5/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1129 2024-05-19 19:01:43.000000 retriever_search-0.2.5/setup.py
```

### Comparing `retriever_search-0.2.4/LICENSE` & `retriever_search-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/PKG-INFO` & `retriever_search-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.4
+Version: 0.2.5
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.2.4/README.md` & `retriever_search-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/DocumentIngestion.py` & `retriever_search-0.2.5/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/QueryPipeline.py` & `retriever_search-0.2.5/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/TopicModellingInit.html` & `retriever_search-0.2.5/retriever_search/TopicModellingInit.html`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/callbacks.py` & `retriever_search-0.2.5/retriever_search/callbacks.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/data/CountVectorizer.pkl` & `retriever_search-0.2.5/retriever_search/data/CountVectorizer.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/data/EmbeddedVectors.pkl` & `retriever_search-0.2.5/retriever_search/data/EmbeddedVectors.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/data/LDAModel.pkl` & `retriever_search-0.2.5/retriever_search/data/LDAModel.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/frontend_app.py` & `retriever_search-0.2.5/retriever_search/frontend_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,12 +80,12 @@
                     gr.Markdown("# Analyse your searched data")
                     
                     src_val = self.analysis_link
                     html = ("<iframe id=\"iframeid\" src=" + src_val + "\ width=1200 height=2000>")
                     out1 = gr.HTML(html)
 
 
-        demo.launch(share=True) 
+        demo.launch(share=False) 
 
 def run_frontend():
     gradio_obj = gradio_app("http://127.0.0.1:5000", "http://127.0.0.1:8055")
     gradio_obj.gradio_launch()
```

### Comparing `retriever_search-0.2.4/retriever_search/layout.py` & `retriever_search-0.2.5/retriever_search/layout.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/search_app.py` & `retriever_search-0.2.5/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/search_server.py` & `retriever_search-0.2.5/retriever_search/search_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/retriever_search/viz_server.py` & `retriever_search-0.2.5/retriever_search/viz_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #Test
 import requests
 from retriever_search.callbacks import get_callbacks
 from retriever_search.layout import Layout
 import json
 import warnings
 import ast  
+import nltk
 
 warnings.filterwarnings("ignore")
 
 server = Flask(__name__)
 app = dash.Dash(__name__, server=server)
 
 def get_init_df():
@@ -36,10 +37,11 @@
 
 def get_json(path):
    with open(path, "r") as f:
       return json.load(f) 
 
 
 def run_viz_server():
+    nltk.download('stopwords')
     call_b = get_callbacks(app, df, keyword_data)
     app.layout = Layout(df, vis_html, keyword_data).layout
     app.run_server(debug=False, host = "127.0.0.1",port=8055)
```

### Comparing `retriever_search-0.2.4/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.2.5/retriever_search.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.4
+Version: 0.2.5
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
```

### Comparing `retriever_search-0.2.4/retriever_search.egg-info/SOURCES.txt` & `retriever_search-0.2.5/retriever_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.4/setup.py` & `retriever_search-0.2.5/setup.py`

 * *Files identical despite different names*

