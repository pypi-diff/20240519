# Comparing `tmp/rag_cli-0.2.0.tar.gz` & `tmp/rag_cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_cli-0.2.0.tar", max compression
+gzip compressed data, was "rag_cli-0.2.2.tar", max compression
```

## Comparing `rag_cli-0.2.0.tar` & `rag_cli-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-05-18 20:44:38.665564 rag_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     1906 2024-05-18 20:44:38.665564 rag_cli-0.2.0/README.md
--rw-r--r--   0        0        0     2649 2024-05-18 20:44:38.665564 rag_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-18 20:44:38.665564 rag_cli-0.2.0/src/rag_cli/__init__.py
--rw-r--r--   0        0        0     2562 2024-05-18 20:44:38.665564 rag_cli-0.2.0/src/rag_cli/cli.py
--rw-r--r--   0        0        0     1066 2024-05-18 20:44:38.665564 rag_cli-0.2.0/src/rag_cli/embedder.py
--rw-r--r--   0        0        0      850 2024-05-18 20:44:38.665564 rag_cli-0.2.0/src/rag_cli/main.py
--rw-r--r--   0        0        0      982 2024-05-18 20:44:38.665564 rag_cli-0.2.0/src/rag_cli/vector_store.py
--rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 rag_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-18 21:08:08.089534 rag_cli-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1906 2024-05-18 21:08:08.089534 rag_cli-0.2.2/README.md
+-rw-r--r--   0        0        0     2674 2024-05-18 21:08:08.089534 rag_cli-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 21:08:08.089534 rag_cli-0.2.2/src/rag_cli/__init__.py
+-rw-r--r--   0        0        0     2562 2024-05-18 21:08:08.089534 rag_cli-0.2.2/src/rag_cli/cli.py
+-rw-r--r--   0        0        0     1067 2024-05-18 21:08:08.089534 rag_cli-0.2.2/src/rag_cli/embedder.py
+-rw-r--r--   0        0        0      851 2024-05-18 21:08:08.089534 rag_cli-0.2.2/src/rag_cli/main.py
+-rw-r--r--   0        0        0      983 2024-05-18 21:08:08.089534 rag_cli-0.2.2/src/rag_cli/vector_store.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 rag_cli-0.2.2/PKG-INFO
```

### Comparing `rag_cli-0.2.0/LICENSE` & `rag_cli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rag_cli-0.2.0/README.md` & `rag_cli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rag_cli-0.2.0/pyproject.toml` & `rag_cli-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "rag-cli"
-version = "0.2.0"
+version = "0.2.2"
 description = "A project to show good CLI practices with a fully fledged RAG system."
 readme = "README.md"
-license = "GNU GPL"
+license = "GNU General Public License (GPL)"
 keywords = ["CLI", "RAG", "LLM", "vector database", "ollama"]
 authors = ["Oliver Kenyon Wilkins <okwilkins@googlemail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 qdrant-client = ">=1.9.0"
 ollama = ">=0.1.0"
```

### Comparing `rag_cli-0.2.0/src/rag_cli/cli.py` & `rag_cli-0.2.2/src/rag_cli/cli.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
+import json
 import re
 import sys
-import json
 from typing import Any
 
 
 def list_of_floats(arg: str) -> list[float]:
     """Parses a list of floats."""
     try:
         arg = arg.replace("\n", "")
```

### Comparing `rag_cli-0.2.0/src/rag_cli/embedder.py` & `rag_cli-0.2.2/src/rag_cli/embedder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import json
 import logging
 import sys
-import json
 from typing import Optional, TextIO
+
 from ollama import Client
 
 
 def run_embedder(ollama_url: str, text: Optional[str] = None, file: Optional[TextIO] = None):
     """Runs the embedder."""
 
     if text is None and file is None:
```

### Comparing `rag_cli-0.2.0/src/rag_cli/main.py` & `rag_cli-0.2.2/src/rag_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
+
+from rag_cli.cli import cli, list_of_floats
 from rag_cli.embedder import run_embedder
 from rag_cli.vector_store import run_vector_store
-from rag_cli.cli import cli, list_of_floats
 
 
 def main():
     args = cli()
 
     if args.command in ["embed"]:
         # If the file argument is not provided, read from stdin
```

### Comparing `rag_cli-0.2.0/src/rag_cli/vector_store.py` & `rag_cli-0.2.2/src/rag_cli/vector_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import sys
-from typing import Any
 import uuid
+from typing import Any
+
 from qdrant_client import QdrantClient
 from qdrant_client.models import PointStruct
 
 
 def run_vector_store(qdrant_url: str, collection_name: str, embedding: list[float], data: dict[str, Any]):
     """Store embeddings in the vector store."""
```

### Comparing `rag_cli-0.2.0/PKG-INFO` & `rag_cli-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: rag-cli
-Version: 0.2.0
+Version: 0.2.2
 Summary: A project to show good CLI practices with a fully fledged RAG system.
-License: GNU GPL
+License: GNU General Public License (GPL)
 Keywords: CLI,RAG,LLM,vector database,ollama
 Author: Oliver Kenyon Wilkins
 Author-email: okwilkins@googlemail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: rag-cli Version: 0.2.0 Summary: A project to show
-good CLI practices with a fully fledged RAG system. License: GNU GPL Keywords:
-CLI,RAG,LLM,vector database,ollama Author: Oliver Kenyon Wilkins Author-email:
-okwilkins@googlemail.com Requires-Python: >=3.8,<4.0 Classifier: License ::
-Other/Proprietary License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: ollama (>=0.1.0) Requires-Dist:
-qdrant-client (>=1.9.0) Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: rag-cli Version: 0.2.2 Summary: A project to show
+good CLI practices with a fully fledged RAG system. License: GNU General Public
+License (GPL) Keywords: CLI,RAG,LLM,vector database,ollama Author: Oliver
+Kenyon Wilkins Author-email: okwilkins@googlemail.com Requires-Python:
+>=3.8,<4.0 Classifier: License :: Other/Proprietary License Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Dist: ollama (>=0.1.0) Requires-Dist: qdrant-client (>=1.9.0) Description-
+Content-Type: text/markdown
                                    [RAG CLI]
      AA pprroojjeecctt ttoo sshhooww ggoooodd CCLLII pprraaccttiicceess wwiitthh aa ffuullllyy fflleeddggeedd RRAAGG ssyysstteemm..
                     _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_G_N_U_ _G_P_L_]
 # RAG CLI ## Installation ```bash pip install rag-cli ``` ## Commands ```bash
 sudo apt-get update && sudo apt-get install parallel jq curl ``` ```bash mkdir
 -p data/articles data/embeddings ``` ### Get Wikipedia articles ```bash
 parallel -n0 -j 10 ' curl -L -s "https://en.wikipedia.org/api/rest_v1/page/
```

