# Comparing `tmp/rnasqlite-0.1.5.tar.gz` & `tmp/rnasqlite-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnasqlite-0.1.5.tar", last modified: Sun May 19 00:26:46 2024, max compression
+gzip compressed data, was "rnasqlite-0.1.6.tar", last modified: Sun May 19 00:45:34 2024, max compression
```

## Comparing `rnasqlite-0.1.5.tar` & `rnasqlite-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 00:26:46.661095 rnasqlite-0.1.5/
--rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      418 2024-05-19 00:26:46.655203 rnasqlite-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 00:26:46.627359 rnasqlite-0.1.5/RNASQLite/
--rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.5/RNASQLite/__init__.py
--rw-rw-rw-   0        0        0     1680 2024-05-19 00:24:51.000000 rnasqlite-0.1.5/RNASQLite/cli.py
--rw-rw-rw-   0        0        0     2097 2024-05-18 13:46:51.000000 rnasqlite-0.1.5/RNASQLite/db_utils.py
--rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.5/RNASQLite/gene_info.csv
--rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.5/RNASQLite/process_file.py
-drwxrwxrwx   0        0        0        0 2024-05-19 00:26:46.655203 rnasqlite-0.1.5/RNASQLite.egg-info/
--rw-rw-rw-   0        0        0      418 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-19 00:26:46.000000 rnasqlite-0.1.5/RNASQLite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.5/gene_info.csv
--rw-rw-rw-   0        0        0       42 2024-05-19 00:26:46.661095 rnasqlite-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      816 2024-05-19 00:26:26.000000 rnasqlite-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 00:45:34.373061 rnasqlite-0.1.6/
+-rw-rw-rw-   0        0        0       23 2024-05-19 00:24:35.000000 rnasqlite-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      418 2024-05-19 00:45:34.372049 rnasqlite-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1452 2024-05-18 14:18:11.000000 rnasqlite-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 00:45:34.347253 rnasqlite-0.1.6/RNASQLite/
+-rw-rw-rw-   0        0        0       23 2024-05-18 13:34:52.000000 rnasqlite-0.1.6/RNASQLite/__init__.py
+-rw-rw-rw-   0        0        0     1680 2024-05-19 00:24:51.000000 rnasqlite-0.1.6/RNASQLite/cli.py
+-rw-rw-rw-   0        0        0     2561 2024-05-19 00:44:29.000000 rnasqlite-0.1.6/RNASQLite/db_utils.py
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.6/RNASQLite/gene_info.csv
+-rw-rw-rw-   0        0        0     3676 2024-05-18 13:46:48.000000 rnasqlite-0.1.6/RNASQLite/process_file.py
+drwxrwxrwx   0        0        0        0 2024-05-19 00:45:34.367352 rnasqlite-0.1.6/RNASQLite.egg-info/
+-rw-rw-rw-   0        0        0      418 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 00:45:34.000000 rnasqlite-0.1.6/RNASQLite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0  2497029 2024-05-18 09:24:42.000000 rnasqlite-0.1.6/gene_info.csv
+-rw-rw-rw-   0        0        0       42 2024-05-19 00:45:34.373061 rnasqlite-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      816 2024-05-19 00:45:24.000000 rnasqlite-0.1.6/setup.py
```

### Comparing `rnasqlite-0.1.5/README.md` & `rnasqlite-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.5/RNASQLite/cli.py` & `rnasqlite-0.1.6/RNASQLite/cli.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.5/RNASQLite/db_utils.py` & `rnasqlite-0.1.6/RNASQLite/db_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import sqlite3
 import os
-import pandas as pd
 
 def setup_database(db_path):
-
-
     # 데이터베이스 연결 (db 파일이 없으면 새로 생성됨)
     conn = sqlite3.connect(db_path)
     c = conn.cursor()
 
     # 테이블 생성
     c.execute('''
-    CREATE TABLE samples (
+    CREATE TABLE IF NOT EXISTS samples (
         id INTEGER PRIMARY KEY AUTOINCREMENT,
         GSE_number TEXT,
         sample_ID TEXT,
-        count_path TEXT
+        count_path TEXT,
+        UNIQUE(GSE_number, sample_ID)
     )
     ''')
 
     # 변경사항 저장
     conn.commit()
     # 연결 종료
     conn.close()
@@ -40,18 +38,28 @@
             GSE_number = parts[0]
             sample_ID = parts[-2]
             count_path = count_file_path
         else:
             print(f"Invalid filename format: {filename}")
             continue
 
+        # 중복 확인
         c.execute('''
-            INSERT INTO samples (GSE_number, sample_ID, count_path)
-            VALUES (?, ?, ?)
-        ''', (GSE_number, sample_ID, count_path))
+            SELECT COUNT(*) FROM samples WHERE GSE_number = ? AND sample_ID = ?
+        ''', (GSE_number, sample_ID))
+        result = c.fetchone()
+
+        if result[0] == 0:
+            # 중복이 아닐 경우 데이터 삽입
+            c.execute('''
+                INSERT INTO samples (GSE_number, sample_ID, count_path)
+                VALUES (?, ?, ?)
+            ''', (GSE_number, sample_ID, count_path))
+        else:
+            print(f"Duplicate entry found for GSE_number: {GSE_number}, sample_ID: {sample_ID}. Skipping insertion.")
 
     # 변경사항 저장
     conn.commit()
     # 연결 종료
     conn.close()
     print("데이터베이스에 데이터 삽입이 완료되었습니다.")
```

### Comparing `rnasqlite-0.1.5/RNASQLite/gene_info.csv` & `rnasqlite-0.1.6/RNASQLite/gene_info.csv`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.5/RNASQLite/process_file.py` & `rnasqlite-0.1.6/RNASQLite/process_file.py`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.5/gene_info.csv` & `rnasqlite-0.1.6/gene_info.csv`

 * *Files identical despite different names*

### Comparing `rnasqlite-0.1.5/setup.py` & `rnasqlite-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RNASQLite',
-    version='0.1.5',  # 버전을 증가시킵니다.
+    version='0.1.6',  # 버전을 증가시킵니다.
     packages=find_packages(),
     install_requires=[
         'pandas',
     ],
     entry_points={
         'console_scripts': [
             'RNASQLite=RNASQLite.cli:main',
```

