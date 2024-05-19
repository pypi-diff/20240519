# Comparing `tmp/bunkrruploader-0.10.6.tar.gz` & `tmp/bunkrruploader-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunkrruploader-0.10.6.tar", last modified: Sat May 11 03:35:58 2024, max compression
+gzip compressed data, was "bunkrruploader-0.10.7.tar", last modified: Sun May 19 14:34:15 2024, max compression
```

## Comparing `bunkrruploader-0.10.6.tar` & `bunkrruploader-0.10.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 03:35:58.520721 bunkrruploader-0.10.6/
--rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-05-05 14:52:19.000000 bunkrruploader-0.10.6/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 03:35:58.520721 bunkrruploader-0.10.6/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)     4747 2024-05-10 03:22:16.000000 bunkrruploader-0.10.6/README.md
--rw-r--r--   0 alex      (1000) alex      (1001)     1545 2024-05-11 03:35:36.000000 bunkrruploader-0.10.6/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-11 03:35:58.520721 bunkrruploader-0.10.6/setup.cfg
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 03:35:58.520721 bunkrruploader-0.10.6/src/
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 03:35:58.520721 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-11 03:35:58.000000 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      507 2024-05-11 03:35:58.000000 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-11 03:35:58.000000 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-05-11 03:35:58.000000 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-05-11 03:35:58.000000 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-11 03:35:58.000000 bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        0 2024-05-10 02:35:40.000000 bunkrruploader-0.10.6/src/__init__.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-11 03:35:58.520721 bunkrruploader-0.10.6/src/bunkrr_uploader/
--rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-05-10 02:38:32.000000 bunkrruploader-0.10.6/src/bunkrr_uploader/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1001)    11653 2024-05-11 01:41:37.000000 bunkrruploader-0.10.6/src/bunkrr_uploader/api.py
--rw-r--r--   0 alex      (1000) alex      (1001)     5587 2024-05-11 01:44:38.000000 bunkrruploader-0.10.6/src/bunkrr_uploader/bunkrr_uploader.py
--rw-r--r--   0 alex      (1000) alex      (1001)     2176 2024-05-11 01:03:01.000000 bunkrruploader-0.10.6/src/bunkrr_uploader/cli.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1557 2024-05-11 00:32:15.000000 bunkrruploader-0.10.6/src/bunkrr_uploader/types.py
--rw-r--r--   0 alex      (1000) alex      (1001)     1492 2024-05-10 03:02:29.000000 bunkrruploader-0.10.6/src/bunkrr_uploader/util.py
--rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-05-10 02:35:41.000000 bunkrruploader-0.10.6/src/bunkrr_uploader.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-19 14:34:15.796133 bunkrruploader-0.10.7/
+-rw-r--r--   0 alex      (1000) alex      (1001)     1071 2024-05-05 14:52:19.000000 bunkrruploader-0.10.7/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-19 14:34:15.796133 bunkrruploader-0.10.7/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)     4747 2024-05-10 03:22:16.000000 bunkrruploader-0.10.7/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)     1545 2024-05-19 14:13:32.000000 bunkrruploader-0.10.7/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-19 14:34:15.796133 bunkrruploader-0.10.7/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-19 14:34:15.796133 bunkrruploader-0.10.7/src/
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-19 14:34:15.796133 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     5672 2024-05-19 14:34:15.000000 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      507 2024-05-19 14:34:15.000000 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-19 14:34:15.000000 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       55 2024-05-19 14:34:15.000000 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       13 2024-05-19 14:34:15.000000 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       25 2024-05-19 14:34:15.000000 bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        0 2024-05-10 02:35:40.000000 bunkrruploader-0.10.7/src/__init__.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-19 14:34:15.796133 bunkrruploader-0.10.7/src/bunkrr_uploader/
+-rw-r--r--   0 alex      (1000) alex      (1001)       46 2024-05-10 02:38:32.000000 bunkrruploader-0.10.7/src/bunkrr_uploader/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    11653 2024-05-11 01:41:37.000000 bunkrruploader-0.10.7/src/bunkrr_uploader/api.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     5551 2024-05-19 14:32:46.000000 bunkrruploader-0.10.7/src/bunkrr_uploader/bunkrr_uploader.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     2176 2024-05-11 01:03:01.000000 bunkrruploader-0.10.7/src/bunkrr_uploader/cli.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1557 2024-05-11 00:32:15.000000 bunkrruploader-0.10.7/src/bunkrr_uploader/types.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1492 2024-05-10 03:02:29.000000 bunkrruploader-0.10.7/src/bunkrr_uploader/util.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      113 2024-05-10 02:35:41.000000 bunkrruploader-0.10.7/src/bunkrr_uploader.py
```

### Comparing `bunkrruploader-0.10.6/LICENSE` & `bunkrruploader-0.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.6/PKG-INFO` & `bunkrruploader-0.10.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunkrrUploader
-Version: 0.10.6
+Version: 0.10.7
 Summary: Bunkrr uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/bunkrr-uploader
 Project-URL: Repository, https://github.com/alexmi256/bunkrr-uploader.git
 Keywords: bunkrr,upload,storage,parallel
```

### Comparing `bunkrruploader-0.10.6/README.md` & `bunkrruploader-0.10.7/README.md`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.6/pyproject.toml` & `bunkrruploader-0.10.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "BunkrrUploader"
-version = "0.10.6"
+version = "0.10.7"
 description = "Bunkrr uploader supporting parallel uploads"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT License"}
 keywords = ["bunkrr", "upload", "storage", "parallel"]
 authors = [
     {name = "Alex Mi", email = "alexmi3.14@gmail.com"},
```

### Comparing `bunkrruploader-0.10.6/src/BunkrrUploader.egg-info/PKG-INFO` & `bunkrruploader-0.10.7/src/BunkrrUploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BunkrrUploader
-Version: 0.10.6
+Version: 0.10.7
 Summary: Bunkrr uploader supporting parallel uploads
 Author-email: Alex Mi <alexmi3.14@gmail.com>
 Maintainer-email: Alex Mi <alexmi3.14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexmi256/bunkrr-uploader
 Project-URL: Repository, https://github.com/alexmi256/bunkrr-uploader.git
 Keywords: bunkrr,upload,storage,parallel
```

### Comparing `bunkrruploader-0.10.6/src/bunkrr_uploader/api.py` & `bunkrruploader-0.10.7/src/bunkrr_uploader/api.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.6/src/bunkrr_uploader/bunkrr_uploader.py` & `bunkrruploader-0.10.7/src/bunkrr_uploader/bunkrr_uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import csv
+import functools
 import logging
 import os
 import re
 import time
 from pathlib import Path
 from pprint import pformat, pprint
 from typing import Any, List, Optional
@@ -112,16 +113,16 @@
                 folder_id = str(created_folder["id"])
 
         if paths:
             responses = await self.api.upload_files(filtered_paths, folder_id)
             # pprint(responses)
 
             if self.options.get("save") is True and responses:
-                # TODO: This should merge them all into superset for all possible fields
-                response_fields = responses[0]["files"][0].values()
+                response_fields = list(set().union(*[x.values() for x in responses[0]["files"] if x]))
+
                 file_name = f"bunkrr_upload_{int(time.time())}.csv"
                 with open(file_name, "w", newline="") as csvfile:
                     logger.info(f"Saving uploaded files to {file_name}")
                     csv_writer = csv.DictWriter(csvfile, dialect="excel", fieldnames=response_fields)
                     csv_writer.writeheader()
                     for row in responses:
                         csv_writer.writerow(row["files"][0])
```

### Comparing `bunkrruploader-0.10.6/src/bunkrr_uploader/cli.py` & `bunkrruploader-0.10.7/src/bunkrr_uploader/cli.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.6/src/bunkrr_uploader/types.py` & `bunkrruploader-0.10.7/src/bunkrr_uploader/types.py`

 * *Files identical despite different names*

### Comparing `bunkrruploader-0.10.6/src/bunkrr_uploader/util.py` & `bunkrruploader-0.10.7/src/bunkrr_uploader/util.py`

 * *Files identical despite different names*

