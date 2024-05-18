# Comparing `tmp/folder_indexer-0.1.0.tar.gz` & `tmp/folder_indexer-0.1.1.tar.gz`

## Comparing `folder_indexer-0.1.0.tar` & `folder_indexer-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/requirements.txt
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/src/folder_indexer/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/src/folder_indexer/__main__.py
--rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/src/folder_indexer/indexer.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/.gitignore
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/LICENSE
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/README.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 folder_indexer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/src/folder_indexer/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/src/folder_indexer/__main__.py
+-rw-r--r--   0        0        0    17032 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/src/folder_indexer/indexer.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/README.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 folder_indexer-0.1.1/PKG-INFO
```

### Comparing `folder_indexer-0.1.0/src/folder_indexer/indexer.py` & `folder_indexer-0.1.1/src/folder_indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `folder_indexer-0.1.0/.gitignore` & `folder_indexer-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `folder_indexer-0.1.0/LICENSE` & `folder_indexer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `folder_indexer-0.1.0/README.md` & `folder_indexer-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# file-indexer-py
+# folder-indexer-py
 A Python script to index a large folder into a parquet file, along with metadata
 
 ## Description
 
 This script is useful for searching for files stored on a reasonably slow disk
 from backups, especially in where you aren't sure about the files are are
 searching for.
 
 Use tools like DBeaver and DuckDB to query and explore the generated index.
 
 ## Usage
 
 ```bash
-pip install file_indexer
+pip install folder_indexer
 
-python3 -m file_indexer -i /path/to/input/folder -o /path/to/output/folder
+python3 -m folder_indexer -i /path/to/input/folder -o /path/to/output/folder
 # --or--
-file_indexer -i /path/to/input/folder -o /path/to/output/folder
+folder_indexer -i /path/to/input/folder -o /path/to/output/folder
 ```
 
 ## Metadata Indexed and Output
 
 The output parquet files have the following columns:
 
     * file_path
@@ -34,10 +34,10 @@
     * date_accessed
     * magic_file_type_1
     * first_100_bytes
     * last_100_bytes
     * timestamp_crawled
     * indexing_start_timestamp
 
-The parquet files are stored to the output folder with the following naming convention: `partial_file_index_{datetime}.parquet`
+The generated parquet files are stored to the output folder with the following naming convention: `partial_file_index_{datetime}.parquet`
 
 At the end of the execution, the individual parquet files are unioned into a single parquet file, with the following name: `00_complete_file_index.parquet`
```

### Comparing `folder_indexer-0.1.0/pyproject.toml` & `folder_indexer-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "folder_indexer"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "RecRanger", email = "RecRanger+package@proton.me" }]
 description = "A Python script to index a large folder into a parquet file, along with metadata"
 readme = "README.md"
 license = "BSD-3-Clause"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `folder_indexer-0.1.0/PKG-INFO` & `folder_indexer-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: folder_indexer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python script to index a large folder into a parquet file, along with metadata
 Project-URL: Homepage, https://github.com/RecRanger/folder-indexer-py
 Project-URL: Issues, https://github.com/RecRanger/folder-indexer-py/issues
 Author-email: RecRanger <RecRanger+package@proton.me>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
@@ -16,33 +16,33 @@
 Requires-Dist: python-magic
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# file-indexer-py
+# folder-indexer-py
 A Python script to index a large folder into a parquet file, along with metadata
 
 ## Description
 
 This script is useful for searching for files stored on a reasonably slow disk
 from backups, especially in where you aren't sure about the files are are
 searching for.
 
 Use tools like DBeaver and DuckDB to query and explore the generated index.
 
 ## Usage
 
 ```bash
-pip install file_indexer
+pip install folder_indexer
 
-python3 -m file_indexer -i /path/to/input/folder -o /path/to/output/folder
+python3 -m folder_indexer -i /path/to/input/folder -o /path/to/output/folder
 # --or--
-file_indexer -i /path/to/input/folder -o /path/to/output/folder
+folder_indexer -i /path/to/input/folder -o /path/to/output/folder
 ```
 
 ## Metadata Indexed and Output
 
 The output parquet files have the following columns:
 
     * file_path
@@ -56,10 +56,10 @@
     * date_accessed
     * magic_file_type_1
     * first_100_bytes
     * last_100_bytes
     * timestamp_crawled
     * indexing_start_timestamp
 
-The parquet files are stored to the output folder with the following naming convention: `partial_file_index_{datetime}.parquet`
+The generated parquet files are stored to the output folder with the following naming convention: `partial_file_index_{datetime}.parquet`
 
 At the end of the execution, the individual parquet files are unioned into a single parquet file, with the following name: `00_complete_file_index.parquet`
```

