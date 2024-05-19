# Comparing `tmp/llmsmith-0.5.0.tar.gz` & `tmp/llmsmith-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmsmith-0.5.0.tar", max compression
+gzip compressed data, was "llmsmith-0.6.0.tar", max compression
```

## Comparing `llmsmith-0.5.0.tar` & `llmsmith-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
--rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.5.0/LICENSE
--rw-r--r--   0        0        0     1517 2024-05-07 11:18:28.748569 llmsmith-0.5.0/README.md
--rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.5.0/llmsmith/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.5.0/llmsmith/agent/__init__.py
--rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.5.0/llmsmith/agent/errors.py
--rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.5.0/llmsmith/agent/function/__init__.py
--rw-r--r--   0        0        0     5618 2024-05-07 11:09:56.773034 llmsmith-0.5.0/llmsmith/agent/function/cohere.py
--rw-r--r--   0        0        0     5926 2024-05-07 11:14:41.988980 llmsmith-0.5.0/llmsmith/agent/function/gemini.py
--rw-r--r--   0        0        0     8889 2024-05-07 11:14:54.558351 llmsmith-0.5.0/llmsmith/agent/function/openai.py
--rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.5.0/llmsmith/agent/function/options/__init__.py
--rw-r--r--   0        0        0     1985 2024-05-07 12:01:42.276643 llmsmith-0.5.0/llmsmith/agent/function/options/openai.py
--rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.5.0/llmsmith/agent/tool/__init__.py
--rw-r--r--   0        0        0      898 2024-05-06 11:04:31.823036 llmsmith-0.5.0/llmsmith/agent/tool/cohere.py
--rw-r--r--   0        0        0     1014 2024-05-07 11:15:14.677758 llmsmith-0.5.0/llmsmith/agent/tool/gemini.py
--rw-r--r--   0        0        0     2002 2024-05-07 11:15:20.017868 llmsmith-0.5.0/llmsmith/agent/tool/openai.py
--rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.5.0/llmsmith/job/__init__.py
--rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.5.0/llmsmith/job/base.py
--rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.5.0/llmsmith/job/job.py
--rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.5.0/llmsmith/reranker/__init__.py
--rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.5.0/llmsmith/reranker/base.py
--rw-r--r--   0        0        0     2849 2024-05-07 11:15:37.535755 llmsmith-0.5.0/llmsmith/reranker/cohere.py
--rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.5.0/llmsmith/reranker/options/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-07 11:15:49.065554 llmsmith-0.5.0/llmsmith/reranker/options/cohere.py
--rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.5.0/llmsmith/task/__init__.py
--rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.5.0/llmsmith/task/base.py
--rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.5.0/llmsmith/task/models.py
--rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.5.0/llmsmith/task/retrieval/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.5.0/llmsmith/task/retrieval/vector/__init__.py
--rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.5.0/llmsmith/task/retrieval/vector/base.py
--rw-r--r--   0        0        0     3715 2024-05-07 11:16:01.033751 llmsmith-0.5.0/llmsmith/task/retrieval/vector/chromadb.py
--rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/__init__.py
--rw-r--r--   0        0        0      897 2024-05-07 11:16:13.459211 llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/chromadb.py
--rw-r--r--   0        0        0     1316 2024-05-07 11:16:18.001301 llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/qdrant.py
--rw-r--r--   0        0        0     4295 2024-05-07 11:16:06.806987 llmsmith-0.5.0/llmsmith/task/retrieval/vector/qdrant.py
--rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.5.0/llmsmith/task/textgen/__init__.py
--rw-r--r--   0        0        0     3036 2024-05-07 11:16:24.273688 llmsmith-0.5.0/llmsmith/task/textgen/claude.py
--rw-r--r--   0        0        0     6108 2024-05-07 04:06:44.987359 llmsmith-0.5.0/llmsmith/task/textgen/cohere.py
--rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.5.0/llmsmith/task/textgen/errors.py
--rw-r--r--   0        0        0     7102 2024-05-07 11:16:33.346249 llmsmith-0.5.0/llmsmith/task/textgen/gemini.py
--rw-r--r--   0        0        0     6441 2024-05-07 11:16:37.844109 llmsmith-0.5.0/llmsmith/task/textgen/openai.py
--rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.5.0/llmsmith/task/textgen/options/__init__.py
--rw-r--r--   0        0        0     1489 2024-05-07 11:16:43.800922 llmsmith-0.5.0/llmsmith/task/textgen/options/claude.py
--rw-r--r--   0        0        0     2317 2024-05-07 12:16:46.722433 llmsmith-0.5.0/llmsmith/task/textgen/options/cohere.py
--rw-r--r--   0        0        0     1337 2024-05-07 11:16:51.095809 llmsmith-0.5.0/llmsmith/task/textgen/options/gemini.py
--rw-r--r--   0        0        0     1881 2024-05-07 11:16:55.681932 llmsmith-0.5.0/llmsmith/task/textgen/options/openai.py
--rw-r--r--   0        0        0     1922 2024-05-07 13:09:53.143679 llmsmith-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 llmsmith-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-03 09:01:34.959168 llmsmith-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1530 2024-05-19 16:22:27.175607 llmsmith-0.6.0/README.md
+-rw-r--r--   0        0        0       78 2024-03-15 04:21:07.861053 llmsmith-0.6.0/llmsmith/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:18:59.343170 llmsmith-0.6.0/llmsmith/agent/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-18 09:12:45.143269 llmsmith-0.6.0/llmsmith/agent/errors.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:19:30.041692 llmsmith-0.6.0/llmsmith/agent/function/__init__.py
+-rw-r--r--   0        0        0     5618 2024-05-07 11:09:56.773034 llmsmith-0.6.0/llmsmith/agent/function/cohere.py
+-rw-r--r--   0        0        0     5926 2024-05-07 11:14:41.988980 llmsmith-0.6.0/llmsmith/agent/function/gemini.py
+-rw-r--r--   0        0        0     8889 2024-05-07 11:14:54.558351 llmsmith-0.6.0/llmsmith/agent/function/openai.py
+-rw-r--r--   0        0        0        0 2024-04-23 05:43:58.075908 llmsmith-0.6.0/llmsmith/agent/function/options/__init__.py
+-rw-r--r--   0        0        0     1985 2024-05-07 12:01:42.276643 llmsmith-0.6.0/llmsmith/agent/function/options/openai.py
+-rw-r--r--   0        0        0        0 2024-04-18 05:26:07.193675 llmsmith-0.6.0/llmsmith/agent/tool/__init__.py
+-rw-r--r--   0        0        0      898 2024-05-06 11:04:31.823036 llmsmith-0.6.0/llmsmith/agent/tool/cohere.py
+-rw-r--r--   0        0        0     1014 2024-05-07 11:15:14.677758 llmsmith-0.6.0/llmsmith/agent/tool/gemini.py
+-rw-r--r--   0        0        0     2002 2024-05-07 11:15:20.017868 llmsmith-0.6.0/llmsmith/agent/tool/openai.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:47:53.187559 llmsmith-0.6.0/llmsmith/job/__init__.py
+-rw-r--r--   0        0        0     7428 2024-04-02 12:37:57.531013 llmsmith-0.6.0/llmsmith/job/base.py
+-rw-r--r--   0        0        0     8550 2024-04-03 05:58:40.426172 llmsmith-0.6.0/llmsmith/job/job.py
+-rw-r--r--   0        0        0        0 2024-04-30 12:02:50.437340 llmsmith-0.6.0/llmsmith/reranker/__init__.py
+-rw-r--r--   0        0        0      575 2024-05-02 04:19:45.995736 llmsmith-0.6.0/llmsmith/reranker/base.py
+-rw-r--r--   0        0        0     2849 2024-05-07 11:15:37.535755 llmsmith-0.6.0/llmsmith/reranker/cohere.py
+-rw-r--r--   0        0        0        0 2024-05-02 03:46:41.851482 llmsmith-0.6.0/llmsmith/reranker/options/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-07 11:15:49.065554 llmsmith-0.6.0/llmsmith/reranker/options/cohere.py
+-rw-r--r--   0        0        0        0 2024-03-14 11:03:16.994184 llmsmith-0.6.0/llmsmith/task/__init__.py
+-rw-r--r--   0        0        0     1329 2024-04-02 12:23:38.410395 llmsmith-0.6.0/llmsmith/task/base.py
+-rw-r--r--   0        0        0      437 2024-04-22 10:15:31.395712 llmsmith-0.6.0/llmsmith/task/models.py
+-rw-r--r--   0        0        0        0 2024-03-15 07:53:27.486482 llmsmith-0.6.0/llmsmith/task/retrieval/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:44:57.026421 llmsmith-0.6.0/llmsmith/task/retrieval/vector/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-01 10:16:21.291906 llmsmith-0.6.0/llmsmith/task/retrieval/vector/base.py
+-rw-r--r--   0        0        0     3715 2024-05-07 11:16:01.033751 llmsmith-0.6.0/llmsmith/task/retrieval/vector/chromadb.py
+-rw-r--r--   0        0        0        0 2024-04-09 12:03:40.797998 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-07 11:16:13.459211 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/chromadb.py
+-rw-r--r--   0        0        0     1157 2024-05-19 16:22:27.178379 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/pinecone.py
+-rw-r--r--   0        0        0     1316 2024-05-07 11:16:18.001301 llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/qdrant.py
+-rw-r--r--   0        0        0     3858 2024-05-19 16:22:27.179017 llmsmith-0.6.0/llmsmith/task/retrieval/vector/pinecone.py
+-rw-r--r--   0        0        0     4295 2024-05-07 11:16:06.806987 llmsmith-0.6.0/llmsmith/task/retrieval/vector/qdrant.py
+-rw-r--r--   0        0        0        0 2024-03-15 11:22:26.459597 llmsmith-0.6.0/llmsmith/task/textgen/__init__.py
+-rw-r--r--   0        0        0     3036 2024-05-07 11:16:24.273688 llmsmith-0.6.0/llmsmith/task/textgen/claude.py
+-rw-r--r--   0        0        0     6108 2024-05-07 04:06:44.987359 llmsmith-0.6.0/llmsmith/task/textgen/cohere.py
+-rw-r--r--   0        0        0      681 2024-04-18 12:18:54.653626 llmsmith-0.6.0/llmsmith/task/textgen/errors.py
+-rw-r--r--   0        0        0     7102 2024-05-07 11:16:33.346249 llmsmith-0.6.0/llmsmith/task/textgen/gemini.py
+-rw-r--r--   0        0        0     6441 2024-05-07 11:16:37.844109 llmsmith-0.6.0/llmsmith/task/textgen/openai.py
+-rw-r--r--   0        0        0        0 2024-03-19 08:37:09.919088 llmsmith-0.6.0/llmsmith/task/textgen/options/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-07 11:16:43.800922 llmsmith-0.6.0/llmsmith/task/textgen/options/claude.py
+-rw-r--r--   0        0        0     2317 2024-05-07 12:16:46.722433 llmsmith-0.6.0/llmsmith/task/textgen/options/cohere.py
+-rw-r--r--   0        0        0     1337 2024-05-07 11:16:51.095809 llmsmith-0.6.0/llmsmith/task/textgen/options/gemini.py
+-rw-r--r--   0        0        0     1881 2024-05-07 11:16:55.681932 llmsmith-0.6.0/llmsmith/task/textgen/options/openai.py
+-rw-r--r--   0        0        0     2028 2024-05-19 16:22:35.929832 llmsmith-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 llmsmith-0.6.0/PKG-INFO
```

### Comparing `llmsmith-0.5.0/LICENSE` & `llmsmith-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/README.md` & `llmsmith-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Here's the list of extra dependencies supported by LLMSmith:
 - `openai`
 - `claude`
 - `gemini`
 - `chromadb`
 - `qdrant`
 - `cohere`
+- `pinecone`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
 Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
```

### Comparing `llmsmith-0.5.0/llmsmith/agent/function/cohere.py` & `llmsmith-0.6.0/llmsmith/agent/function/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/agent/function/gemini.py` & `llmsmith-0.6.0/llmsmith/agent/function/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/agent/function/openai.py` & `llmsmith-0.6.0/llmsmith/agent/function/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/agent/function/options/openai.py` & `llmsmith-0.6.0/llmsmith/agent/function/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/agent/tool/cohere.py` & `llmsmith-0.6.0/llmsmith/agent/tool/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/agent/tool/gemini.py` & `llmsmith-0.6.0/llmsmith/agent/tool/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/agent/tool/openai.py` & `llmsmith-0.6.0/llmsmith/agent/tool/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/job/base.py` & `llmsmith-0.6.0/llmsmith/job/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/job/job.py` & `llmsmith-0.6.0/llmsmith/job/job.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/reranker/base.py` & `llmsmith-0.6.0/llmsmith/reranker/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/reranker/cohere.py` & `llmsmith-0.6.0/llmsmith/reranker/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/reranker/options/cohere.py` & `llmsmith-0.6.0/llmsmith/reranker/options/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/base.py` & `llmsmith-0.6.0/llmsmith/task/base.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/retrieval/vector/chromadb.py` & `llmsmith-0.6.0/llmsmith/task/retrieval/vector/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/chromadb.py` & `llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/chromadb.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/retrieval/vector/options/qdrant.py` & `llmsmith-0.6.0/llmsmith/task/retrieval/vector/options/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/retrieval/vector/qdrant.py` & `llmsmith-0.6.0/llmsmith/task/retrieval/vector/qdrant.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/claude.py` & `llmsmith-0.6.0/llmsmith/task/textgen/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/cohere.py` & `llmsmith-0.6.0/llmsmith/task/textgen/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/errors.py` & `llmsmith-0.6.0/llmsmith/task/textgen/errors.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/gemini.py` & `llmsmith-0.6.0/llmsmith/task/textgen/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/openai.py` & `llmsmith-0.6.0/llmsmith/task/textgen/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/options/claude.py` & `llmsmith-0.6.0/llmsmith/task/textgen/options/claude.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/options/cohere.py` & `llmsmith-0.6.0/llmsmith/task/textgen/options/cohere.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/options/gemini.py` & `llmsmith-0.6.0/llmsmith/task/textgen/options/gemini.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/llmsmith/task/textgen/options/openai.py` & `llmsmith-0.6.0/llmsmith/task/textgen/options/openai.py`

 * *Files identical despite different names*

### Comparing `llmsmith-0.5.0/pyproject.toml` & `llmsmith-0.6.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "LLMSmith"
-version = "0.5.0"
+version = "0.6.0"
 description = "Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)"
 authors = ["Dheeraj Gopinath <dheeraj.gopinath@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
@@ -20,23 +20,25 @@
 chromadb-client = {version = "^0.4.25.dev0", optional = true}
 onnxruntime = {version = "^1.17.1", optional = true}
 protobuf = {version = "3.20.3", optional = true}
 tokenizers = {version = "^0.15.2", optional = true}
 python-dotenv = "^1.0.1"
 qdrant-client = {version = "^1.8.2", optional = true}
 cohere = {version = "^5.3.2", optional = true}
+pinecone-client = {version = "^4.1.0", optional = true}
 
 [tool.poetry.extras]
 openai = ["openai"]
 claude = ["anthropic"]
 gemini = ["google-generativeai"]
 chromadb = ["chromadb-client", "onnxruntime", "protobuf", "tokenizers"]
 qdrant = ["qdrant-client"]
 cohere = ["cohere"]
-all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client", "cohere"]
+pinecone = ["pinecone-client"]
+all = ["openai", "anthropic", "google-generativeai", "chromadb-client", "onnxruntime", "protobuf", "tokenizers", "qdrant-client", "cohere", "pinecone-client"]
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.2"
 black = "^24.2.0"
```

### Comparing `llmsmith-0.5.0/PKG-INFO` & `llmsmith-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLMSmith
-Version: 0.5.0
+Version: 0.6.0
 Summary: Lightweight Python library designed for developing functionalities powered by Large Language Models (LLMs)
 Author: Dheeraj Gopinath
 Author-email: dheeraj.gopinath@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: all
 Provides-Extra: chromadb
 Provides-Extra: claude
 Provides-Extra: cohere
 Provides-Extra: gemini
 Provides-Extra: openai
+Provides-Extra: pinecone
 Provides-Extra: qdrant
 Requires-Dist: anthropic (>=0.19.2,<0.20.0) ; extra == "claude" or extra == "all"
 Requires-Dist: chromadb-client (>=0.4.25.dev0,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: cohere (>=5.3.2,<6.0.0) ; extra == "cohere" or extra == "all"
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
 Requires-Dist: onnxruntime (>=1.17.1,<2.0.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: openai (>=1.23.2,<2.0.0) ; extra == "openai" or extra == "all"
+Requires-Dist: pinecone-client (>=4.1.0,<5.0.0) ; extra == "pinecone" or extra == "all"
 Requires-Dist: protobuf (==3.20.3) ; extra == "chromadb" or extra == "all"
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: qdrant-client (>=1.8.2,<2.0.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: tokenizers (>=0.15.2,<0.16.0) ; extra == "chromadb" or extra == "all"
 Description-Content-Type: text/markdown
 
 # 🧰 LLMSmith
@@ -55,14 +57,15 @@
 Here's the list of extra dependencies supported by LLMSmith:
 - `openai`
 - `claude`
 - `gemini`
 - `chromadb`
 - `qdrant`
 - `cohere`
+- `pinecone`
 - `all` (downloads all extra dependencies)
 
 ## Example
 
 Refer [this](https://llmsmith.readthedocs.io/en/latest/examples.html) page from the documentation to see examples on how LLMSmith can be used to build LLM powered functionalities.
 
 ## Documentation
```

