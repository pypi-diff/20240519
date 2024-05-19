# Comparing `tmp/rnasqlite-0.1.4.tar.gz` & `tmp/rnasqlite-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.4.tar", last modified: Sat May 18 14:24:34 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.5.tar", last modified: Sun May 19 00:26:46 2024, max compression
```

## Comparing `rnasqlite-0.1.4.tar` & `rnasqlite-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:24:34.204806 rnasqlite-0.1.4/
--rw-rw-rw-   0        0        0      418 2024-05-18 14:24:34.202805 rnasqlite-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 14:24:34.168287 rnasqlite-0.1.4/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.4/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1762 2024-05-18 14:23:14.000000 rnasqlite-0.1.4/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.4/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.4/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:24:34.196805 rnasqlite-0.1.4/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 14:24:34.204806 rnasqlite-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-05-18 14:24:23.000000 rnasqlite-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 00:26:46.661095 rnasqlite-0.1.5/
+-rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2024-05-19 00:26:46.655203 rnasqlite-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 00:26:46.627359 rnasqlite-0.1.5/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.5/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1680 2024-05-19 00:24:51.000000 rnasqlite-0.1.5/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.5/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.5/RNASQLite/gene_info.csv
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.5/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-19 00:26:46.655203 rnasqlite-0.1.5/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.5/gene_info.csv
+-rw-rw-rw-   0        0        0       42 2024-05-19 00:26:46.661095 rnasqlite-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-19 00:26:26.000000 rnasqlite-0.1.5/setup.py
```

### Comparing `rnasqlite-0.1.4/README.md` & `rnasqlite-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.4/RNASQLite/cli.py` & `rnasqlite-0.1.5/RNASQLite/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+import pkg_resources
 from RNASQLite.db_utils import setup_database, insert_counts_into_db, get_count_files, fetch_all_samples
 from RNASQLite.process_file import process_file
 
 def main():
     parser = argparse.ArgumentParser(description='RNASQLite command line tool')
     parser.add_argument('-create', action='store_true', help='Create the SQLite database')
     parser.add_argument('-split', type=str, help='Process RNAseq counts file and split into count files')
@@ -14,18 +15,18 @@
     db_path = 'geo_rna_seq.db'  # SQLite 데이터베이스 파일 경로
     counts_dir = 'counts'  # Counts 파일이 저장될 디렉토리
 
     if args.create:
         setup_database(db_path)
     elif args.split:
         rna_seq_counts_path = args.split
-        root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))  # 루트 디렉토리 경로
-        gene_info_path = os.path.join(root_dir, 'gene_info.csv')  # 루트 디렉토리에서 gene_info.csv 파일을 찾습니다
+        # 패키지 내부에서 gene_info.csv 파일 경로를 찾습니다
+        gene_info_path = pkg_resources.resource_filename(__name__, 'gene_info.csv')
         if not os.path.isfile(gene_info_path):
-            print(f"Error: {gene_info_path} file not found in the root directory.")
+            print(f"Error: {gene_info_path} file not found.")
             return
         process_file(gene_info_path, rna_seq_counts_path, counts_dir)
     elif args.load:
         count_files = get_count_files(counts_dir)
         insert_counts_into_db(db_path, count_files)
     elif args.fetch:
         fetch_all_samples(db_path)
```

### Comparing `rnasqlite-0.1.4/RNASQLite/db_utils.py` & `rnasqlite-0.1.5/RNASQLite/db_utils.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.4/RNASQLite/process_file.py` & `rnasqlite-0.1.5/RNASQLite/process_file.py`

 * *Files identical despite different names*

