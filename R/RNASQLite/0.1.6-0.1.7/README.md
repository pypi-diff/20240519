# Comparing `tmp/rnasqlite-0.1.6.tar.gz` & `tmp/rnasqlite-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.6.tar", last modified: Sun May 19 00:45:34 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.7.tar", last modified: Sun May 19 01:38:40 2024, max compression
```

## Comparing `rnasqlite-0.1.6.tar` & `rnasqlite-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 00:45:34.373061 rnasqlite-0.1.6/
--rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2024-05-19 00:45:34.372049 rnasqlite-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 00:45:34.347253 rnasqlite-0.1.6/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.6/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1680 2024-05-19 00:24:51.000000 rnasqlite-0.1.6/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     2561 2024-05-19 00:44:29.000000 rnasqlite-0.1.6/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.6/RNASQLite/gene_info.csv
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.6/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:45:34.367352 rnasqlite-0.1.6/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.6/gene_info.csv
--rw-rw-rw-   0        0        0       42 2024-05-19 00:45:34.373061 rnasqlite-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-05-19 00:45:24.000000 rnasqlite-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:38:40.085247 rnasqlite-0.1.7/
+-rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2024-05-19 01:38:40.083238 rnasqlite-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 01:38:40.062461 rnasqlite-0.1.7/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.7/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1978 2024-05-19 01:38:05.000000 rnasqlite-0.1.7/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     4843 2024-05-19 01:38:07.000000 rnasqlite-0.1.7/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.7/RNASQLite/gene_info.csv
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.7/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-19 01:38:40.083238 rnasqlite-0.1.7/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 01:38:39.000000 rnasqlite-0.1.7/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.7/gene_info.csv
+-rw-rw-rw-   0        0        0       42 2024-05-19 01:38:40.085247 rnasqlite-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-19 01:38:19.000000 rnasqlite-0.1.7/setup.py
```

### Comparing `rnasqlite-0.1.6/README.md` & `rnasqlite-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.6/RNASQLite/cli.py` & `rnasqlite-0.1.7/RNASQLite/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import argparse
 import os
 import pkg_resources
-from RNASQLite.db_utils import setup_database, insert_counts_into_db, get_count_files, fetch_all_samples
+from RNASQLite.db_utils import setup_database, insert_counts_into_db, get_count_files, fetch_all_samples, fetch_filtered_samples
 from RNASQLite.process_file import process_file
 
 def main():
     parser = argparse.ArgumentParser(description='RNASQLite command line tool')
     parser.add_argument('-create', action='store_true', help='Create the SQLite database')
     parser.add_argument('-split', type=str, help='Process RNAseq counts file and split into count files')
     parser.add_argument('-load', action='store_true', help='Load counts files into the database')
     parser.add_argument('-fetch', action='store_true', help='Fetch all samples from the database')
+    parser.add_argument('-column', type=str, nargs=2, metavar=('COLUMN', 'VALUE'), help='Fetch samples by column and value')
     args = parser.parse_args()
 
     db_path = 'geo_rna_seq.db'  # SQLite 데이터베이스 파일 경로
     counts_dir = 'counts'  # Counts 파일이 저장될 디렉토리
 
     if args.create:
         setup_database(db_path)
@@ -26,12 +27,15 @@
             return
         process_file(gene_info_path, rna_seq_counts_path, counts_dir)
     elif args.load:
         count_files = get_count_files(counts_dir)
         insert_counts_into_db(db_path, count_files)
     elif args.fetch:
         fetch_all_samples(db_path)
+    elif args.column:
+        column_name, identifier_value = args.column
+        fetch_filtered_samples(db_path, column_name, identifier_value)
     else:
         print("Invalid command. Use -create, -split <file>, -load, or -fetch.")
 
 if __name__ == '__main__':
     main()
```

### Comparing `rnasqlite-0.1.6/RNASQLite/gene_info.csv` & `rnasqlite-0.1.7/RNASQLite/gene_info.csv`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.6/RNASQLite/process_file.py` & `rnasqlite-0.1.7/RNASQLite/process_file.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.6/gene_info.csv` & `rnasqlite-0.1.7/gene_info.csv`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.6/setup.py` & `rnasqlite-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RNASQLite',
-    version='0.1.6',  # 버전을 증가시킵니다.
+    version='0.1.7',  # 버전을 증가시킵니다.
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'RNASQLite=RNASQLite.cli:main',
```

