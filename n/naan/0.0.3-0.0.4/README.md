# Comparing `tmp/naan-0.0.3.tar.gz` & `tmp/naan-0.0.4.tar.gz`

## Comparing `naan-0.0.3.tar` & `naan-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 naan-0.0.3/naan/__about__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 naan-0.0.3/naan/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 naan-0.0.3/naan/document.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 naan-0.0.3/naan/filesystem.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 naan-0.0.3/naan/naan.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 naan-0.0.3/naan/queries.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 naan-0.0.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 naan-0.0.3/LICENSE
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 naan-0.0.3/README.md
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 naan-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 naan-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 naan-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 naan-0.0.4/naan/__about__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 naan-0.0.4/naan/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 naan-0.0.4/naan/document.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 naan-0.0.4/naan/filesystem.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 naan-0.0.4/naan/naan.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 naan-0.0.4/naan/queries.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 naan-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 naan-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 naan-0.0.4/README.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 naan-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 naan-0.0.4/PKG-INFO
```

### Comparing `naan-0.0.3/naan/filesystem.py` & `naan-0.0.4/naan/filesystem.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # SPDX-FileCopyrightText: 2023-present Massimiliano Pippi <mpippi@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 import logging
-from pathlib import Path
 import shutil
-
+from pathlib import Path
 
 logger = logging.getLogger(__name__)
 
 DB_FILENAME_PATTERN = "{}.db"
 INDEX_FILENAME_PATTERN = "{}.faiss"
 
 
 class StorageFolder:
-    def __init__(self, path: Path, force: bool = False) -> None:
+    def __init__(self, path: Path, *, force: bool = False) -> None:
         try:
             path.mkdir(exist_ok=True)
         except FileExistsError as e:
-            logger.error(f"Path {path.name} should be a directory")
+            logger.exception("Path %s should be a directory", path.name)
             raise e from None
 
         self._path = path
+        self._name = path.name
         self._db_file = self._path / DB_FILENAME_PATTERN.format(path.name)
         self._index_file = self._path / INDEX_FILENAME_PATTERN.format(path.name)
 
         # We can assume at this point the path exists and is a directory.
         # If the folder is not empty, see if it's a valid storage
         contents = list(self._path.iterdir())
         if contents and not self.ready:
@@ -43,7 +43,11 @@
     @property
     def db_file(self):
         return self._db_file
 
     @property
     def index_file(self):
         return self._index_file
+
+    @property
+    def name(self):
+        return self._name
```

### Comparing `naan-0.0.3/.gitignore` & `naan-0.0.4/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -123,7 +123,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# naan
+naan.db
```

### Comparing `naan-0.0.3/LICENSE` & `naan-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `naan-0.0.3/pyproject.toml` & `naan-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -49,42 +49,41 @@
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
-  "coverage report",
+  "coverage report -m",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
 ]
 [tool.hatch.envs.types.scripts]
-check = "mypy --install-types --non-interactive {args:src/stocaz tests}"
+check = "mypy --install-types --non-interactive {args:src/naan tests}"
 
 [tool.coverage.run]
-source_pkgs = ["stocaz", "tests"]
+source_pkgs = ["naan", "tests"]
 branch = true
 parallel = true
 omit = [
-  "src/stocaz/__about__.py",
+  "src/naan/__about__.py",
 ]
 
 [tool.coverage.paths]
-stocaz = ["src/stocaz", "*/stocaz/src/stocaz"]
-tests = ["tests", "*/stocaz/tests"]
+tests = ["tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
@@ -96,10 +95,11 @@
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
+exclude = ["example"]
 
 [tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "parents"
```

### Comparing `naan-0.0.3/PKG-INFO` & `naan-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: naan
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/unknown/naan#readme
 Project-URL: Issues, https://github.com/unknown/naan/issues
 Project-URL: Source, https://github.com/unknown/naan
 Author-email: Massimiliano Pippi <mpippi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -26,31 +26,40 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/naan.svg)](https://pypi.org/project/naan)
 
 -----
 
 **Table of Contents**
 
 - [naan](#naan)
+  - [What is Naan?](#what-is-naan)
   - [Installation](#installation)
   - [Index data](#index-data)
   - [License](#license)
 
+## What is Naan?
+
+- Naan is a wrapper around FAISS indexes that provides metadata storage and retrieval for the vectors added to the index.
+- Naan's job is to eliminate the tedious task of keeping around the original content before it's encoded
+and added to the index.
+- Naan is NOT a vector database. All the vector-search operations are demanded to FAISS.
+
 ## Installation
 
 ```console
 pip install naan
 ```
 
 ## Index data
 
 To see Naan in action, let's first get some data to embed:
 
 ```python
+from io import StringIO
 import requests
-from sentence_transformers import SentenceTransformer
+import json
 
 
 res = requests.get("https://raw.githubusercontent.com/masci/naan/main/example/sentences.json")
 sentences = json.load(StringIO(res.text))
 ```
 
 Naan tries not to get in the way you manage your FAISS index, so the first step is always setting
@@ -58,15 +67,15 @@
 
 ```python
 from sentence_transformers import SentenceTransformer
 import faiss
 
 
 model = SentenceTransformer("bert-base-nli-mean-tokens")
-sentence_embeddings = model.encode(sentences[:100])
+sentence_embeddings = model.encode(sentences)
 dim = sentence_embeddings.shape[1]
 index = faiss.IndexFlatL2(dim)
 ```
 
 Now it's time to wrap the FAISS index with Naan and use it to index data:
 
 ```python
@@ -85,16 +94,15 @@
 # Reopen an existing Naan database
 db = NaanDB("db.naan")
 query_embeddings = model.encode(["The book is on the table"])
 # Naan's search API is the same as FAISS, let's get the 3 closest vectors
 results = db.search(query_embeddings, 3)
 for result in results:
     print(result)
-# (5799, 'Two girls are laughing and other girls are watching them')
-# (20303, 'A group of football players is running in the field')
-# (14418, 'Four boys are sitting in a muddy stream.')
-# (28922, 'A group of people playing football is running in the field')
+# Document(vector_id=11451, content='A group of people sitting around a desk.', embeddings=None)
+# Document(vector_id=2754, content='A close-up picture of a desk with a computer and papers on it.', embeddings=None)
+# Document(vector_id=11853, content='A computer on a desk.', embeddings=None)
 ```
 
 ## License
 
 `naan` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

