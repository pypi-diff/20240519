# Comparing `tmp/retriever_search-0.2.2.tar.gz` & `tmp/retriever_search-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriever_search-0.2.2.tar", last modified: Sun May 19 17:43:10 2024, max compression
+gzip compressed data, was "retriever_search-0.2.3.tar", last modified: Sun May 19 18:59:00 2024, max compression
```

## Comparing `retriever_search-0.2.2.tar` & `retriever_search-0.2.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.717131 retriever_search-0.2.2/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.2/LICENSE
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:43:10.716744 retriever_search-0.2.2/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.2/README.md
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.705435 retriever_search-0.2.2/retriever_search/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.2/retriever_search/DocumentIngestion.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.2/retriever_search/QueryPipeline.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/TopicModellingInit.html
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.2/retriever_search/Utils.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 17:42:24.000000 retriever_search-0.2.2/retriever_search/__init__.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.2/retriever_search/callbacks.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.713983 retriever_search-0.2.2/retriever_search/data/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/data/CountVectorizer.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/data/EmbeddedVectors.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.2/retriever_search/data/LDAModel.pkl
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.2/retriever_search/frontend_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.2/retriever_search/layout.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.2/retriever_search/search_app.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.2/retriever_search/search_server.py
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1131 2024-05-19 17:41:36.000000 retriever_search-0.2.2/retriever_search/viz_server.py
-drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 17:43:10.716206 retriever_search-0.2.2/retriever_search.egg-info/
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2293 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/PKG-INFO
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/SOURCES.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/dependency_links.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)      262 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/requires.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 17:43:10.000000 retriever_search-0.2.2/retriever_search.egg-info/top_level.txt
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 17:43:10.717229 retriever_search-0.2.2/setup.cfg
--rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1136 2024-05-19 17:43:03.000000 retriever_search-0.2.2/setup.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 18:59:00.979131 retriever_search-0.2.3/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1062 2024-04-23 05:51:14.000000 retriever_search-0.2.3/LICENSE
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 18:59:00.978770 retriever_search-0.2.3/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1512 2024-05-02 20:10:32.000000 retriever_search-0.2.3/README.md
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 18:59:00.951116 retriever_search-0.2.3/retriever_search/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     6508 2024-04-30 16:55:53.000000 retriever_search-0.2.3/retriever_search/DocumentIngestion.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1922 2024-04-24 08:53:52.000000 retriever_search-0.2.3/retriever_search/QueryPipeline.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   315320 2024-05-02 19:07:29.000000 retriever_search-0.2.3/retriever_search/TopicModellingInit.html
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      259 2024-05-02 18:52:21.000000 retriever_search-0.2.3/retriever_search/Utils.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      144 2024-05-19 18:58:36.000000 retriever_search-0.2.3/retriever_search/__init__.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     9998 2024-05-19 17:40:04.000000 retriever_search-0.2.3/retriever_search/callbacks.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 18:59:00.964483 retriever_search-0.2.3/retriever_search/data/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)   337240 2024-05-02 19:07:29.000000 retriever_search-0.2.3/retriever_search/data/CountVectorizer.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  6339926 2024-05-02 19:07:29.000000 retriever_search-0.2.3/retriever_search/data/EmbeddedVectors.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)  2102124 2024-05-02 19:07:29.000000 retriever_search-0.2.3/retriever_search/data/LDAModel.pkl
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3597 2024-05-02 19:19:42.000000 retriever_search-0.2.3/retriever_search/frontend_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2615 2024-05-02 18:56:07.000000 retriever_search-0.2.3/retriever_search/layout.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1597 2024-05-02 18:49:21.000000 retriever_search-0.2.3/retriever_search/search_app.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     3458 2024-04-30 17:09:10.000000 retriever_search-0.2.3/retriever_search/search_server.py
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1131 2024-05-19 17:41:36.000000 retriever_search-0.2.3/retriever_search/viz_server.py
+drwxr-xr-x   0 sidharthkathpal   (501) staff       (20)        0 2024-05-19 18:59:00.978246 retriever_search-0.2.3/retriever_search.egg-info/
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     2286 2024-05-19 18:59:00.000000 retriever_search-0.2.3/retriever_search.egg-info/PKG-INFO
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      698 2024-05-19 18:59:00.000000 retriever_search-0.2.3/retriever_search.egg-info/SOURCES.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)        1 2024-05-19 18:59:00.000000 retriever_search-0.2.3/retriever_search.egg-info/dependency_links.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)      255 2024-05-19 18:59:00.000000 retriever_search-0.2.3/retriever_search.egg-info/requires.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       17 2024-05-19 18:59:00.000000 retriever_search-0.2.3/retriever_search.egg-info/top_level.txt
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)       38 2024-05-19 18:59:00.979221 retriever_search-0.2.3/setup.cfg
+-rw-r--r--   0 sidharthkathpal   (501) staff       (20)     1129 2024-05-19 18:58:33.000000 retriever_search-0.2.3/setup.py
```

### Comparing `retriever_search-0.2.2/LICENSE` & `retriever_search-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/PKG-INFO` & `retriever_search-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.2
+Version: 0.2.3
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
@@ -16,15 +16,15 @@
 Requires-Dist: Flask==2.2.5
 Requires-Dist: pandas==2.2.1
 Requires-Dist: torch==2.2.1
 Requires-Dist: accelerate==0.27.2
 Requires-Dist: gradio==4.21.0
 Requires-Dist: dash==2.15.0
 Requires-Dist: plotly==5.10.0
-Requires-Dist: wordcloud==1.9.2
+Requires-Dist: wordcloud
 Requires-Dist: pyLDAvis==3.4.1
 Requires-Dist: nltk==3.7
 
 <div align="center">
 
 # Retriever
```

### Comparing `retriever_search-0.2.2/README.md` & `retriever_search-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/DocumentIngestion.py` & `retriever_search-0.2.3/retriever_search/DocumentIngestion.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/QueryPipeline.py` & `retriever_search-0.2.3/retriever_search/QueryPipeline.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/TopicModellingInit.html` & `retriever_search-0.2.3/retriever_search/TopicModellingInit.html`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/callbacks.py` & `retriever_search-0.2.3/retriever_search/callbacks.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/data/CountVectorizer.pkl` & `retriever_search-0.2.3/retriever_search/data/CountVectorizer.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/data/EmbeddedVectors.pkl` & `retriever_search-0.2.3/retriever_search/data/EmbeddedVectors.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/data/LDAModel.pkl` & `retriever_search-0.2.3/retriever_search/data/LDAModel.pkl`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/frontend_app.py` & `retriever_search-0.2.3/retriever_search/frontend_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/layout.py` & `retriever_search-0.2.3/retriever_search/layout.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/search_app.py` & `retriever_search-0.2.3/retriever_search/search_app.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/search_server.py` & `retriever_search-0.2.3/retriever_search/search_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search/viz_server.py` & `retriever_search-0.2.3/retriever_search/viz_server.py`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/retriever_search.egg-info/PKG-INFO` & `retriever_search-0.2.3/retriever_search.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriever_search
-Version: 0.2.2
+Version: 0.2.3
 Summary: Local retriever search for your use
 Home-page: https://github.com/GovML/retriever.git
 Author: Sidharth Kathpal
 Author-email: kathpal.sid@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai==2.0.0
@@ -16,15 +16,15 @@
 Requires-Dist: Flask==2.2.5
 Requires-Dist: pandas==2.2.1
 Requires-Dist: torch==2.2.1
 Requires-Dist: accelerate==0.27.2
 Requires-Dist: gradio==4.21.0
 Requires-Dist: dash==2.15.0
 Requires-Dist: plotly==5.10.0
-Requires-Dist: wordcloud==1.9.2
+Requires-Dist: wordcloud
 Requires-Dist: pyLDAvis==3.4.1
 Requires-Dist: nltk==3.7
 
 <div align="center">
 
 # Retriever
```

### Comparing `retriever_search-0.2.2/retriever_search.egg-info/SOURCES.txt` & `retriever_search-0.2.3/retriever_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retriever_search-0.2.2/setup.py` & `retriever_search-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         'Flask==2.2.5',
         'pandas==2.2.1',
         'torch==2.2.1',
         'accelerate==0.27.2',
         'gradio==4.21.0',
         'dash==2.15.0',
         'plotly==5.10.0',
-        'wordcloud==1.9.2',
+        'wordcloud',
         'pyLDAvis==3.4.1',
         'nltk==3.7',
     ],
     packages=find_packages(),
     include_package_data=True,
     package_data={'retriever_search': ['data/CountVectorizer.pkl', 'data/EmbeddedVectors.pkl', 'data/LDAModel.pkl', 'TopicModellingInit.html']}
 )
```

