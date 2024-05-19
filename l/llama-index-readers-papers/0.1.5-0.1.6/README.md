# Comparing `tmp/llama_index_readers_papers-0.1.5.tar.gz` & `tmp/llama_index_readers_papers-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_papers-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_readers_papers-0.1.6.tar", max compression
```

## Comparing `llama_index_readers_papers-0.1.5.tar` & `llama_index_readers_papers-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2008 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/README.md
--rw-r--r--   0        0        0      186 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/__init__.py
--rw-r--r--   0        0        0      186 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/arxiv/__init__.py
--rw-r--r--   0        0        0     6302 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/arxiv/base.py
--rw-r--r--   0        0        0       17 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/pubmed/__init__.py
--rw-r--r--   0        0        0     6330 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/llama_index/readers/papers/pubmed/base.py
--rw-r--r--   0        0        0     1517 2024-05-08 15:19:55.056380 llama_index_readers_papers-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 llama_index_readers_papers-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2008 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/README.md
+-rw-r--r--   0        0        0      186 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/llama_index/readers/papers/__init__.py
+-rw-r--r--   0        0        0      186 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/llama_index/readers/papers/arxiv/__init__.py
+-rw-r--r--   0        0        0     6390 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/llama_index/readers/papers/arxiv/base.py
+-rw-r--r--   0        0        0       17 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/llama_index/readers/papers/pubmed/__init__.py
+-rw-r--r--   0        0        0     6330 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/llama_index/readers/papers/pubmed/base.py
+-rw-r--r--   0        0        0     1517 2024-05-19 03:55:13.899775 llama_index_readers_papers-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 llama_index_readers_papers-0.1.6/PKG-INFO
```

### Comparing `llama_index_readers_papers-0.1.5/README.md` & `llama_index_readers_papers-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_papers-0.1.5/llama_index/readers/papers/arxiv/base.py` & `llama_index_readers_papers-0.1.6/llama_index/readers/papers/arxiv/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,15 +143,17 @@
             paper.download_pdf(dirpath=papers_dir, filename=filename)
             logging.debug(f"> Downloading {filename}...")
 
         def get_paper_metadata(filename):
             return paper_lookup[os.path.basename(filename)]
 
         arxiv_documents = SimpleDirectoryReader(
-            papers_dir, file_metadata=get_paper_metadata
+            papers_dir,
+            file_metadata=get_paper_metadata,
+            exclude_hidden=False,  # default directory is hidden ".papers"
         ).load_data()
         # Include extra documents containing the abstracts
         abstract_documents = []
         for paper in search_results:
             d = (
                 f"The following is a summary of the paper: {paper.title}\n\nSummary:"
                 f" {paper.summary}"
```

### Comparing `llama_index_readers_papers-0.1.5/llama_index/readers/papers/pubmed/base.py` & `llama_index_readers_papers-0.1.6/llama_index/readers/papers/pubmed/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_papers-0.1.5/pyproject.toml` & `llama_index_readers_papers-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers papers integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["thejessezhang"]
 name = "llama-index-readers-papers"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 arxiv = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_papers-0.1.5/PKG-INFO` & `llama_index_readers_papers-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-papers
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index readers papers integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Maintainer: thejessezhang
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

