# Comparing `tmp/knowledge_graph_maker-0.1.2.tar.gz` & `tmp/knowledge_graph_maker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge_graph_maker-0.1.2.tar", max compression
+gzip compressed data, was "knowledge_graph_maker-0.2.0.tar", max compression
```

## Comparing `knowledge_graph_maker-0.1.2.tar` & `knowledge_graph_maker-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-05-01 08:08:04.561957 knowledge_graph_maker-0.1.2/LICENSE
--rw-r--r--   0        0        0     7551 2024-05-18 12:56:15.664626 knowledge_graph_maker-0.1.2/README.md
--rw-r--r--   0        0        0      244 2024-05-18 05:36:37.494471 knowledge_graph_maker-0.1.2/knowledge_graph_maker/__init__.py
--rw-r--r--   0        0        0     6457 2024-05-18 05:36:37.494857 knowledge_graph_maker-0.1.2/knowledge_graph_maker/graph_maker.py
--rw-r--r--   0        0        0      257 2024-05-01 07:29:51.195238 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1768 2024-05-01 07:50:57.377849 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc
--rw-r--r--   0        0        0     1657 2024-05-18 05:36:37.495037 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc
--rw-r--r--   0        0        0     1822 2024-05-18 05:36:37.495201 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2024-05-18 07:21:08.395043 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc
--rw-r--r--   0        0        0     1715 2024-05-01 07:29:51.195530 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/groq_client.py
--rw-r--r--   0        0        0     1009 2024-05-18 05:36:37.495488 knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/openai_client.py
--rw-r--r--   0        0        0     3908 2024-05-01 07:29:51.193626 knowledge_graph_maker-0.1.2/knowledge_graph_maker/logger.py
--rw-r--r--   0        0        0     2093 2024-05-04 14:44:32.548460 knowledge_graph_maker-0.1.2/knowledge_graph_maker/neo4j_graph_model.py
--rw-r--r--   0        0        0      938 2024-05-04 14:44:32.548639 knowledge_graph_maker-0.1.2/knowledge_graph_maker/types.py
--rw-r--r--   0        0        0      552 2024-05-18 14:35:01.941486 knowledge_graph_maker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8398 1970-01-01 00:00:00.000000 knowledge_graph_maker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 08:08:04.561957 knowledge_graph_maker-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7551 2024-05-18 12:56:15.664626 knowledge_graph_maker-0.2.0/README.md
+-rw-r--r--   0        0        0      244 2024-05-18 05:36:37.494471 knowledge_graph_maker-0.2.0/knowledge_graph_maker/__init__.py
+-rw-r--r--   0        0        0     6457 2024-05-18 05:36:37.494857 knowledge_graph_maker-0.2.0/knowledge_graph_maker/graph_maker.py
+-rw-r--r--   0        0        0      257 2024-05-01 07:29:51.195238 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1768 2024-05-01 07:50:57.377849 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc
+-rw-r--r--   0        0        0     1657 2024-05-18 05:36:37.495037 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc
+-rw-r--r--   0        0        0     1822 2024-05-18 05:36:37.495201 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc
+-rw-r--r--   0        0        0     1818 2024-05-18 07:21:08.395043 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc
+-rw-r--r--   0        0        0     1715 2024-05-01 07:29:51.195530 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/groq_client.py
+-rw-r--r--   0        0        0     1009 2024-05-18 05:36:37.495488 knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/openai_client.py
+-rw-r--r--   0        0        0     3908 2024-05-01 07:29:51.193626 knowledge_graph_maker-0.2.0/knowledge_graph_maker/logger.py
+-rw-r--r--   0        0        0     2093 2024-05-04 14:44:32.548460 knowledge_graph_maker-0.2.0/knowledge_graph_maker/neo4j_graph_model.py
+-rw-r--r--   0        0        0      938 2024-05-04 14:44:32.548639 knowledge_graph_maker-0.2.0/knowledge_graph_maker/types.py
+-rw-r--r--   0        0        0      552 2024-05-19 08:00:06.347175 knowledge_graph_maker-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8398 1970-01-01 00:00:00.000000 knowledge_graph_maker-0.2.0/PKG-INFO
```

### Comparing `knowledge_graph_maker-0.1.2/LICENSE` & `knowledge_graph_maker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/README.md` & `knowledge_graph_maker-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/graph_maker.py` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/graph_maker.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/groq_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/__pycache__/openai_client.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/groq_client.py` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/groq_client.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/llm_clients/openai_client.py` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/llm_clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/logger.py` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/logger.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/neo4j_graph_model.py` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/neo4j_graph_model.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/knowledge_graph_maker/types.py` & `knowledge_graph_maker-0.2.0/knowledge_graph_maker/types.py`

 * *Files identical despite different names*

### Comparing `knowledge_graph_maker-0.1.2/pyproject.toml` & `knowledge_graph_maker-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "knowledge-graph-maker"
-version = "0.1.2"
+version = "0.2.0"
 description = "Create knowledge graph out of any text using a given ontology"
 authors = ["Rahul Nayak <rahul.nyk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.26.2"
 pathlib = "^1.0.1"
 uuid = "^1.30"
 jupyterlab = "^4.0.8"
 yachalk = "^0.1.5"
-groq = "^0.5.0"
+groq = "^0.6.0"
 python-dotenv = "^1.0.1"
 neo4j = "5.19.0"
 neomodel = "^5.3.0"
 logging = "^0.4.9.6"
 openai = "^1.28.0"
```

### Comparing `knowledge_graph_maker-0.1.2/PKG-INFO` & `knowledge_graph_maker-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: knowledge-graph-maker
-Version: 0.1.2
+Version: 0.2.0
 Summary: Create knowledge graph out of any text using a given ontology
 Author: Rahul Nayak
 Author-email: rahul.nyk@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: groq (>=0.5.0,<0.6.0)
+Requires-Dist: groq (>=0.6.0,<0.7.0)
 Requires-Dist: jupyterlab (>=4.0.8,<5.0.0)
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
 Requires-Dist: neo4j (==5.19.0)
 Requires-Dist: neomodel (>=5.3.0,<6.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: openai (>=1.28.0,<2.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
```

