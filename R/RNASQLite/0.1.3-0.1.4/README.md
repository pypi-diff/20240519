# Comparing `tmp/rnasqlite-0.1.3.tar.gz` & `tmp/rnasqlite-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.3.tar", last modified: Sat May 18 14:19:56 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.4.tar", last modified: Sat May 18 14:24:34 2024, max compression
```

## Comparing `rnasqlite-0.1.3.tar` & `rnasqlite-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:19:56.554349 rnasqlite-0.1.3/
--rw-rw-rw-   0        0        0      418 2024-05-18 14:19:56.553349 rnasqlite-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 14:19:56.522825 rnasqlite-0.1.3/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.3/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1628 2024-05-18 13:59:18.000000 rnasqlite-0.1.3/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.3/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.3/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:19:56.552348 rnasqlite-0.1.3/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 14:19:56.000000 rnasqlite-0.1.3/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 14:19:56.554349 rnasqlite-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      727 2024-05-18 14:19:40.000000 rnasqlite-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:24:34.204806 rnasqlite-0.1.4/
+-rw-rw-rw-   0        0        0      418 2024-05-18 14:24:34.202805 rnasqlite-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 14:24:34.168287 rnasqlite-0.1.4/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.4/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1762 2024-05-18 14:23:14.000000 rnasqlite-0.1.4/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.4/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.4/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-18 14:24:34.196805 rnasqlite-0.1.4/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-18 14:24:34.000000 rnasqlite-0.1.4/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 14:24:34.204806 rnasqlite-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      727 2024-05-18 14:24:23.000000 rnasqlite-0.1.4/setup.py
```

### Comparing `rnasqlite-0.1.3/README.md` & `rnasqlite-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.3/RNASQLite/cli.py` & `rnasqlite-0.1.4/RNASQLite/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     db_path = 'geo_rna_seq.db'  # SQLite 데이터베이스 파일 경로
     counts_dir = 'counts'  # Counts 파일이 저장될 디렉토리
 
     if args.create:
         setup_database(db_path)
     elif args.split:
         rna_seq_counts_path = args.split
-        gene_info_path = 'gene_info.csv'  # 실행 디렉토리에서 gene_info.csv 파일을 찾습니다
+        root_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))  # 루트 디렉토리 경로
+        gene_info_path = os.path.join(root_dir, 'gene_info.csv')  # 루트 디렉토리에서 gene_info.csv 파일을 찾습니다
         if not os.path.isfile(gene_info_path):
-            print(f"Error: {gene_info_path} file not found in the current directory.")
+            print(f"Error: {gene_info_path} file not found in the root directory.")
             return
         process_file(gene_info_path, rna_seq_counts_path, counts_dir)
     elif args.load:
         count_files = get_count_files(counts_dir)
         insert_counts_into_db(db_path, count_files)
     elif args.fetch:
         fetch_all_samples(db_path)
```

### Comparing `rnasqlite-0.1.3/RNASQLite/db_utils.py` & `rnasqlite-0.1.4/RNASQLite/db_utils.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.3/RNASQLite/process_file.py` & `rnasqlite-0.1.4/RNASQLite/process_file.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.3/setup.py` & `rnasqlite-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RNASQLite',
-    version='0.1.3',  # 버전을 업데이트합니다.
+    version='0.1.4',  # 버전을 업데이트합니다.
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'RNASQLite=RNASQLite.cli:main',
```

