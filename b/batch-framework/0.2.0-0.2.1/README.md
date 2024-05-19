# Comparing `tmp/batch-framework-0.2.0.tar.gz` & `tmp/batch-framework-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-framework-0.2.0.tar", last modified: Thu Apr  4 02:38:42 2024, max compression
+gzip compressed data, was "batch-framework-0.2.1.tar", last modified: Sun May 19 15:20:43 2024, max compression
```

## Comparing `batch-framework-0.2.0.tar` & `batch-framework-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:38:42.271050 batch-framework-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 02:38:00.000000 batch-framework-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 02:38:42.271050 batch-framework-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-04 02:38:00.000000 batch-framework-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:38:42.267050 batch-framework-0.2.0/batch_framework/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/adaptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/parallize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/rdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 02:38:00.000000 batch-framework-0.2.0/batch_framework/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 02:38:42.271050 batch-framework-0.2.0/batch_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-04 02:38:42.000000 batch-framework-0.2.0/batch_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-04 02:38:42.000000 batch-framework-0.2.0/batch_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 02:38:42.000000 batch-framework-0.2.0/batch_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 02:38:42.000000 batch-framework-0.2.0/batch_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 02:38:42.000000 batch-framework-0.2.0/batch_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 02:38:42.271050 batch-framework-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-04 02:38:00.000000 batch-framework-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-19 15:19:59.000000 batch-framework-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 15:20:43.133230 batch-framework-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 15:19:59.000000 batch-framework-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.129230 batch-framework-0.2.1/batch_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/batch_framework/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/batch_framework/filesystem/dropbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/dropbox/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/filesystem/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/parallize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/rdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 15:19:59.000000 batch-framework-0.2.1/batch_framework/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 15:20:43.133230 batch-framework-0.2.1/batch_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 15:20:43.000000 batch-framework-0.2.1/batch_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 15:20:43.133230 batch-framework-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-19 15:19:59.000000 batch-framework-0.2.1/setup.py
```

### Comparing `batch-framework-0.2.0/LICENSE` & `batch-framework-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/PKG-INFO` & `batch-framework-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.0/batch_framework/adaptor.py` & `batch-framework-0.2.1/batch_framework/adaptor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/batch_framework/base.py` & `batch-framework-0.2.1/batch_framework/base.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/batch_framework/etl.py` & `batch-framework-0.2.1/batch_framework/etl.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/batch_framework/executor.py` & `batch-framework-0.2.1/batch_framework/executor.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/batch_framework/parallize.py` & `batch-framework-0.2.1/batch_framework/parallize.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/batch_framework/rdb.py` & `batch-framework-0.2.1/batch_framework/rdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,36 +49,36 @@
 
 
 class DuckDBBackend(RDB):
     def __init__(
             self, persist_fs: Optional[FileSystem] = None, db_name: str = ''):
         if persist_fs:
             assert db_name != '', 'db_name should be provided when persist_fs is provided'
-            if not isinstance(persist_fs, LocalBackend):
-                if persist_fs.check_exists(db_name):
-                    # download data to local from remote file system
-                    buff = persist_fs.download_core(db_name)
-                    lb = LocalBackend()
-                    lb.upload_core(buff, self._db_name)
-                    assert os.path.exists(
-                        './' + db_name), f'db_name: {db_name} does not exist'
+            if persist_fs.check_exists(db_name):
+                # download data to local from remote file system
+                buff = persist_fs.download_core(db_name)
+                buff.seek(0)
+                self._lb = LocalBackend('./duckdb')
+                self._lb.upload_core(buff, self._db_name)
+                assert os.path.exists(
+                    './duckdb/' + db_name), f'db_name: {db_name} does not exist'
         self._persist_fs = persist_fs
         super().__init__(db_name)
 
     @property
     def conn(self):
         """
         Get thread local used connection.
         """
         if self._conn is None:
             if self._persist_fs is None:
                 conn = duckdb.connect(database=':memory:')
             else:
                 conn = duckdb.connect(
-                    database=self._persist_fs._directory + self._db_name)
+                    database='./duckdb/' + self._db_name)
             self._conn = conn
         return self._conn
 
     def get_conn(self):
         return self.conn.cursor()
 
     def register(self, table_name: str, table: object):
@@ -95,12 +95,10 @@
         except BaseException as e:
             raise ValueError(sql) from e
 
     def commit(self):
         """
         Upload current status of duckdb to remote file system
         """
-        assert not isinstance(
-            self._persist_fs, LocalBackend), 'No need to commit for local duckdb dump storage.'
-        lb = LocalBackend()
-        buff = lb.download_core(self._db_name)
+        assert self._persist_fs is not None, 'no need to commit if there is no persist_fs for storing duckdb dump file'
+        buff = self._lb.download_core(self._db_name)
         self._persist_fs.upload_core(buff, self._db_name)
```

### Comparing `batch-framework-0.2.0/batch_framework/storage.py` & `batch-framework-0.2.1/batch_framework/storage.py`

 * *Files identical despite different names*

### Comparing `batch-framework-0.2.0/batch_framework.egg-info/PKG-INFO` & `batch-framework-0.2.1/batch_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-framework
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate Batch Framework
 Home-page: https://github.com/jeffrey82221/batch_framework
 Author: jeffreylin
 Author-email: jeffrey82221@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `batch-framework-0.2.0/setup.py` & `batch-framework-0.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,10 +60,11 @@
         'paradag',
         'dill',
         'dropboxdrivefs',
         'typing_extensions',
         'vaex',
         'tqdm',
         'types-PyYAML',
-        'PyYAML'
+        'PyYAML',
+        'split-file-reader==0.1.4'
     ]
 )
```

