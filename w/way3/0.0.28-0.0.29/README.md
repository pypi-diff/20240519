# Comparing `tmp/way3-0.0.28.tar.gz` & `tmp/way3-0.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way3-0.0.28.tar", last modified: Sat May 18 09:39:58 2024, max compression
+gzip compressed data, was "way3-0.0.29.tar", last modified: Sat May 18 10:21:00 2024, max compression
```

## Comparing `way3-0.0.28.tar` & `way3-0.0.29.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.679025 way3-0.0.28/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-18 09:39:53.000000 way3-0.0.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-18 09:39:58.679025 way3-0.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-18 09:39:53.000000 way3-0.0.28/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 09:39:58.679025 way3-0.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 09:39:53.000000 way3-0.0.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 09:39:53.000000 way3-0.0.28/tests/test_file_find.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-18 09:39:53.000000 way3-0.0.28/tests/test_file_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 09:39:53.000000 way3-0.0.28/tests/test_folder_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/way3/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-18 09:39:53.000000 way3-0.0.28/way3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/way3/file_find/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_find/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_find/current_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_find/traverse_files_from_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.675025 way3-0.0.28/way3/file_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-18 09:39:53.000000 way3-0.0.28/way3/file_op/create_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.679025 way3-0.0.28/way3/folder_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:53.000000 way3-0.0.28/way3/folder_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-18 09:39:53.000000 way3-0.0.28/way3/folder_op/create_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 09:39:58.679025 way3-0.0.28/way3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 09:39:58.000000 way3-0.0.28/way3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.829621 way3-0.0.29/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-18 10:20:57.000000 way3-0.0.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-18 10:21:00.829621 way3-0.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-18 10:20:57.000000 way3-0.0.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 10:21:00.829621 way3-0.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 10:20:57.000000 way3-0.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.825621 way3-0.0.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:20:57.000000 way3-0.0.29/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-18 10:20:57.000000 way3-0.0.29/tests/test_file_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-18 10:20:57.000000 way3-0.0.29/tests/test_file_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-18 10:20:57.000000 way3-0.0.29/tests/test_folder_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.825621 way3-0.0.29/way3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-18 10:20:57.000000 way3-0.0.29/way3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.829621 way3-0.0.29/way3/file_find/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:20:57.000000 way3-0.0.29/way3/file_find/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-18 10:20:57.000000 way3-0.0.29/way3/file_find/current_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-18 10:20:57.000000 way3-0.0.29/way3/file_find/traverse_files_from_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.829621 way3-0.0.29/way3/file_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:20:57.000000 way3-0.0.29/way3/file_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-18 10:20:57.000000 way3-0.0.29/way3/file_op/create_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.829621 way3-0.0.29/way3/folder_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:20:57.000000 way3-0.0.29/way3/folder_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-18 10:20:57.000000 way3-0.0.29/way3/folder_op/create_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.829621 way3-0.0.29/way3/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 10:20:57.000000 way3-0.0.29/way3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-18 10:20:57.000000 way3-0.0.29/way3/utils/ignore_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 10:21:00.829621 way3-0.0.29/way3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-18 10:21:00.000000 way3-0.0.29/way3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-18 10:21:00.000000 way3-0.0.29/way3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 10:21:00.000000 way3-0.0.29/way3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 10:21:00.000000 way3-0.0.29/way3.egg-info/top_level.txt
```

### Comparing `way3-0.0.28/LICENSE` & `way3-0.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/PKG-INFO` & `way3-0.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.28
+Version: 0.0.29
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `way3-0.0.28/README.md` & `way3-0.0.29/README.md`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/setup.py` & `way3-0.0.29/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="way3",
-    version="0.0.28",
+    version="0.0.29",
     author="aboutmydreams",
     author_email="aboutmydreams@163.com",
     description="Simplified file path management for Python developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aboutmydreams/way3",
     packages=setuptools.find_packages(),
```

### Comparing `way3-0.0.28/tests/test_file_find.py` & `way3-0.0.29/tests/test_file_find.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/tests/test_file_op.py` & `way3-0.0.29/tests/test_file_op.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/tests/test_folder_op.py` & `way3-0.0.29/tests/test_folder_op.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/way3/__init__.py` & `way3-0.0.29/way3/__init__.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/way3/file_find/traverse_files_from_folder.py` & `way3-0.0.29/way3/file_find/traverse_files_from_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from typing import Dict, List
-from ..utils.ignore_rule import parse_gitignore, is_gitignored
+from way3.utils.ignore_rule import parse_gitignore, is_gitignored
 
 
 def get_files_in_directory(directory, should_ignore=True, ignore_file_path=None):
     """
     获取指定目录下所有文件，排除.gitignore中列出的文件
     """
```

### Comparing `way3-0.0.28/way3/file_op/create_file.py` & `way3-0.0.29/way3/file_op/create_file.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/way3/folder_op/create_folder.py` & `way3-0.0.29/way3/folder_op/create_folder.py`

 * *Files identical despite different names*

### Comparing `way3-0.0.28/way3.egg-info/PKG-INFO` & `way3-0.0.29/way3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 0.0.28
+Version: 0.0.29
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

