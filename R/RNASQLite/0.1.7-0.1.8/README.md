# Comparing `tmp/rnasqlite-0.1.7.tar.gz` & `tmp/rnasqlite-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.7.tar", last modified: Sun May 19 01:38:40 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.8.tar", last modified: Sun May 19 01:41:21 2024, max compression
```

## Comparing `rnasqlite-0.1.7.tar` & `rnasqlite-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 01:38:40.085247 rnasqlite-0.1.7/
--rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2024-05-19 01:38:40.083238 rnasqlite-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 01:38:40.062461 rnasqlite-0.1.7/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.7/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1978 2024-05-19 01:38:05.000000 rnasqlite-0.1.7/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     4843 2024-05-19 01:38:07.000000 rnasqlite-0.1.7/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.7/RNASQLite/gene_info.csv
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.7/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-19 01:38:40.083238 rnasqlite-0.1.7/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.7/gene_info.csv
--rw-rw-rw-   0        0        0       42 2024-05-19 01:38:40.085247 rnasqlite-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-05-19 01:38:19.000000 rnasqlite-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:41:21.261994 rnasqlite-0.1.8/
+-rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2024-05-19 01:41:21.261994 rnasqlite-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 01:41:21.237703 rnasqlite-0.1.8/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.8/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1978 2024-05-19 01:38:05.000000 rnasqlite-0.1.8/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     4864 2024-05-19 01:41:07.000000 rnasqlite-0.1.8/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.8/RNASQLite/gene_info.csv
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.8/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:41:21.261464 rnasqlite-0.1.8/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-19 01:41:21.000000 rnasqlite-0.1.8/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-19 01:41:21.000000 rnasqlite-0.1.8/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 01:41:21.000000 rnasqlite-0.1.8/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-19 01:41:21.000000 rnasqlite-0.1.8/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 01:41:21.000000 rnasqlite-0.1.8/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 01:41:21.000000 rnasqlite-0.1.8/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.8/gene_info.csv
+-rw-rw-rw-   0        0        0       42 2024-05-19 01:41:21.261994 rnasqlite-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-19 01:41:10.000000 rnasqlite-0.1.8/setup.py
```

### Comparing `rnasqlite-0.1.7/README.md` & `rnasqlite-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.7/RNASQLite/cli.py` & `rnasqlite-0.1.8/RNASQLite/cli.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.7/RNASQLite/db_utils.py` & `rnasqlite-0.1.8/RNASQLite/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sqlite3
 import os
+import pandas as pd
 
 def setup_database(db_path):
     # 데이터베이스 연결 (db 파일이 없으면 새로 생성됨)
     conn = sqlite3.connect(db_path)
     c = conn.cursor()
 
     # 테이블 생성
```

### Comparing `rnasqlite-0.1.7/RNASQLite/gene_info.csv` & `rnasqlite-0.1.8/RNASQLite/gene_info.csv`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.7/RNASQLite/process_file.py` & `rnasqlite-0.1.8/RNASQLite/process_file.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.7/gene_info.csv` & `rnasqlite-0.1.8/gene_info.csv`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.7/setup.py` & `rnasqlite-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RNASQLite',
-    version='0.1.7',  # 버전을 증가시킵니다.
+    version='0.1.8',  # 버전을 증가시킵니다.
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'RNASQLite=RNASQLite.cli:main',
```

