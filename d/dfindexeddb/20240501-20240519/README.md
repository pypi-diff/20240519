# Comparing `tmp/dfindexeddb-20240501.tar.gz` & `tmp/dfindexeddb-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfindexeddb-20240501.tar", last modified: Tue May  7 01:16:25 2024, max compression
+gzip compressed data, was "dfindexeddb-20240519.tar", last modified: Sun May 19 07:36:06 2024, max compression
```

## Comparing `dfindexeddb-20240501.tar` & `dfindexeddb-20240519.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.428833 dfindexeddb-20240501/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-07 01:16:19.000000 dfindexeddb-20240501/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 01:16:19.000000 dfindexeddb-20240501/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    18496 2024-05-07 01:16:25.428833 dfindexeddb-20240501/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4675 2024-05-07 01:16:19.000000 dfindexeddb-20240501/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.420833 dfindexeddb-20240501/dfindexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32122 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/blink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    47366 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/v8.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/firefox/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/firefox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    21595 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/safari/webkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/indexeddb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb/leveldb/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/ldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9209 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/leveldb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-07 01:16:19.000000 dfindexeddb-20240501/dfindexeddb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 01:16:25.424833 dfindexeddb-20240501/dfindexeddb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18496 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-07 01:16:25.000000 dfindexeddb-20240501/dfindexeddb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-07 01:16:19.000000 dfindexeddb-20240501/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 01:16:25.428833 dfindexeddb-20240501/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-07 01:16:19.000000 dfindexeddb-20240501/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.508549 dfindexeddb-20240519/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 07:36:02.000000 dfindexeddb-20240519/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 07:36:02.000000 dfindexeddb-20240519/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    18814 2024-05-19 07:36:06.508549 dfindexeddb-20240519/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-05-19 07:36:02.000000 dfindexeddb-20240519/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.500549 dfindexeddb-20240519/dfindexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.504549 dfindexeddb-20240519/dfindexeddb/indexeddb/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.504549 dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/blink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47578 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22102 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/v8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.504549 dfindexeddb-20240519/dfindexeddb/indexeddb/firefox/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/firefox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.504549 dfindexeddb-20240519/dfindexeddb/indexeddb/safari/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/safari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/safari/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/safari/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21969 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/safari/webkit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/indexeddb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.504549 dfindexeddb-20240519/dfindexeddb/leveldb/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/ldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.508549 dfindexeddb-20240519/dfindexeddb/leveldb/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/plugins/chrome_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/plugins/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/plugins/notification_database_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/leveldb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-19 07:36:02.000000 dfindexeddb-20240519/dfindexeddb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:36:06.508549 dfindexeddb-20240519/dfindexeddb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18814 2024-05-19 07:36:06.000000 dfindexeddb-20240519/dfindexeddb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-19 07:36:06.000000 dfindexeddb-20240519/dfindexeddb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:36:06.000000 dfindexeddb-20240519/dfindexeddb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-19 07:36:06.000000 dfindexeddb-20240519/dfindexeddb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 07:36:06.000000 dfindexeddb-20240519/dfindexeddb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 07:36:06.000000 dfindexeddb-20240519/dfindexeddb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-19 07:36:02.000000 dfindexeddb-20240519/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:36:06.508549 dfindexeddb-20240519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-19 07:36:02.000000 dfindexeddb-20240519/setup.py
```

### Comparing `dfindexeddb-20240501/LICENSE` & `dfindexeddb-20240519/LICENSE`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/PKG-INFO` & `dfindexeddb-20240519/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240501
+Version: 20240519
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,14 +215,17 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: python-snappy==0.6.1
 Requires-Dist: zstd==1.5.5.1
+Provides-Extra: plugins
+Requires-Dist: protobuf; extra == "plugins"
+Requires-Dist: dfdatetime; extra == "plugins"
 
 # dfIndexeddb
 
 dfindexeddb is an experimental Python tool for performing digital forensic
 analysis of IndexedDB and LevelDB files.
 
 It parses LevelDB, IndexedDB and JavaScript structures from these files without
@@ -251,14 +254,20 @@
 
 ```
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install dfindexeddb
 ```
 
+To also install the dependencies for leveldb/indexeddb plugins, run
+```
+    $ pip install 'dfindexeddb[plugins]'
+```
+
+
 ## Installation from source
 
 1. [Linux] Install the snappy compression development package
 
 ```
     $ sudo apt install libsnappy-dev
 ```
@@ -269,14 +278,19 @@
 
 ```
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install .
 ```
 
+To also install the dependencies for leveldb/indexeddb plugins, run
+```
+    $ pip install '.[plugins]'
+```
+
 ## Usage
 
 Two CLI tools for parsing IndexedDB/LevelDB files are available after
 installation:
 
 
 ### IndexedDB
@@ -355,15 +369,23 @@
 ```
 
 #### Examples
 
 To parse records from a LevelDB folder, use the following command:
 
 ```
-dfindexeddb db -s SOURCE
+dfleveldb db -s SOURCE
+```
+
+To parse records from a LevelDB folder, and use the sequence number to 
+determine recovered records and output as JSON, use the
+following command:
+
+```
+dfleveldb db -s SOURCE --use_sequence_number
 ```
 
 To parse blocks / physical records/ write batches / internal key records from a
 LevelDB log (.log) file, use the following command, specifying the type (block,
 physical_records, etc) via the `-t` option.  By default, internal key records are parsed:
 
 ```
@@ -379,19 +401,18 @@
 ```
 
 To parse version edit records from a Descriptor (MANIFEST) file, use the
 following command:
 
 ```
 $ dfleveldb descriptor -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,versionedit} | -v]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,physical_records,versionedit}, --structure_type {blocks,physical_records,versionedit}
-                        Parses the specified structure. Default is versionedit.
-  -v, --version_history
-                        Parses the leveldb version history.
 ```
+
+#### Plugins
+
+To apply a plugin parser for a leveldb file/folder, add the 
+`--plugin [Plugin Name]` argument.  Currently, there is support for the 
+following artifacts:
+
+| Plugin Name | Artifact Name |
+| -------- | ------- |
+| `ChromeNotificationRecord` | Chrome/Chromium Notifications |
```

### Comparing `dfindexeddb-20240501/README.md` & `dfindexeddb-20240519/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 
 ```
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install dfindexeddb
 ```
 
+To also install the dependencies for leveldb/indexeddb plugins, run
+```
+    $ pip install 'dfindexeddb[plugins]'
+```
+
+
 ## Installation from source
 
 1. [Linux] Install the snappy compression development package
 
 ```
     $ sudo apt install libsnappy-dev
 ```
@@ -47,14 +53,19 @@
 
 ```
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install .
 ```
 
+To also install the dependencies for leveldb/indexeddb plugins, run
+```
+    $ pip install '.[plugins]'
+```
+
 ## Usage
 
 Two CLI tools for parsing IndexedDB/LevelDB files are available after
 installation:
 
 
 ### IndexedDB
@@ -133,15 +144,23 @@
 ```
 
 #### Examples
 
 To parse records from a LevelDB folder, use the following command:
 
 ```
-dfindexeddb db -s SOURCE
+dfleveldb db -s SOURCE
+```
+
+To parse records from a LevelDB folder, and use the sequence number to 
+determine recovered records and output as JSON, use the
+following command:
+
+```
+dfleveldb db -s SOURCE --use_sequence_number
 ```
 
 To parse blocks / physical records/ write batches / internal key records from a
 LevelDB log (.log) file, use the following command, specifying the type (block,
 physical_records, etc) via the `-t` option.  By default, internal key records are parsed:
 
 ```
@@ -157,19 +176,18 @@
 ```
 
 To parse version edit records from a Descriptor (MANIFEST) file, use the
 following command:
 
 ```
 $ dfleveldb descriptor -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,versionedit} | -v]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,physical_records,versionedit}, --structure_type {blocks,physical_records,versionedit}
-                        Parses the specified structure. Default is versionedit.
-  -v, --version_history
-                        Parses the leveldb version history.
 ```
+
+#### Plugins
+
+To apply a plugin parser for a leveldb file/folder, add the 
+`--plugin [Plugin Name]` argument.  Currently, there is support for the 
+following artifacts:
+
+| Plugin Name | Artifact Name |
+| -------- | ------- |
+| `ChromeNotificationRecord` | Chrome/Chromium Notifications |
```

### Comparing `dfindexeddb-20240501/dfindexeddb/__init__.py` & `dfindexeddb-20240519/dfindexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/errors.py` & `dfindexeddb-20240519/dfindexeddb/errors.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/__init__.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/__init__.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/blink.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/blink.py`

 * *Files 2% similar despite different names*

```diff
@@ -776,14 +776,17 @@
     return RTCEncodedVideoFrame(index=index)
 
   def _ReadCryptoKey(self) -> CryptoKey:
     """Reads a CryptoKey from the current position.
 
     Returns:
       A parsed CryptoKey.
+
+    Raises:
+      ParserError: if there is an unexpected CryptoKeySubTag.
     """
     _, raw_key_byte = self.deserializer.decoder.DecodeUint8()
     key_byte = definitions.CryptoKeySubTag(raw_key_byte)
     if key_byte == definitions.CryptoKeySubTag.AES_KEY:
       key_type, algorithm_parameters = self._ReadAESKey()
     elif key_byte == definitions.CryptoKeySubTag.HMAC_KEY:
       key_type, algorithm_parameters = self._ReadHMACKey()
@@ -791,14 +794,16 @@
       key_type, algorithm_parameters = self._ReadRSAHashedKey()
     elif key_byte == definitions.CryptoKeySubTag.EC_KEY:
       key_type, algorithm_parameters = self._ReadECKey()
     elif key_byte == definitions.CryptoKeySubTag.ED25519_KEY:
       key_type, algorithm_parameters = self._ReadED25519Key()
     elif key_byte == definitions.CryptoKeySubTag.NO_PARAMS_KEY:
       key_type, algorithm_parameters = self.ReadNoParamsKey()
+    else:
+      raise errors.ParserError('Unexpected CryptoKeySubTag')
 
     _, raw_usages = self.deserializer.decoder.DecodeUint32Varint()
     usages = definitions.CryptoKeyUsage(raw_usages)
 
     extractable = bool(raw_usages & definitions.CryptoKeyUsage.EXTRACTABLE)
     _, key_data_length = self.deserializer.decoder.DecodeUint32Varint()
```

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/definitions.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/record.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1271,22 +1271,25 @@
       if object_type == definitions.ExternalObjectType.FILE:
         _, filename = decoder.DecodeStringWithLength()
         _, last_modified = decoder.DecodeVarint()
       else:
         filename = None
         last_modified = None
       token = None
-    elif (object_type ==
-        definitions.ExternalObjectType.FILE_SYSTEM_ACCESS_HANDLE):
+    else:
+      if (object_type ==
+          definitions.ExternalObjectType.FILE_SYSTEM_ACCESS_HANDLE):
+        _, token = decoder.DecodeBlobWithLength()
+      else:
+        token = None
       blob_number = None
       mime_type = None
       size = None
       filename = None
       last_modified = None
-      _, token = decoder.DecodeBlobWithLength()
 
     return cls(offset=base_offset + offset, object_type=object_type,
         blob_number=blob_number, mime_type=mime_type, size=size,
         filename=filename, last_modified=last_modified, token=token)
 
 
 @dataclass
@@ -1413,28 +1416,30 @@
     """
     if not foldername or not foldername.is_dir():
       raise ValueError(f'{foldername} is None or not a directory')
     self.foldername = foldername
 
   def GetRecords(
       self,
-      use_manifest: bool = False
+      use_manifest: bool = False,
+      use_sequence_number: bool = False
   ) -> Generator[IndexedDBRecord, None, None]:
     """Yield LevelDBRecords.
 
     Args:
       use_manifest: True to use the current manifest in the folder as a means to
           find the active file set.
-
+      use_sequence_number: True to use the sequence number to determine the
     Yields:
       IndexedDBRecord.
     """
     leveldb_folder_reader = record.FolderReader(self.foldername)
     for leveldb_record in leveldb_folder_reader.GetRecords(
-        use_manifest=use_manifest):
+        use_manifest=use_manifest,
+        use_sequence_number=use_sequence_number):
       try:
         yield IndexedDBRecord.FromLevelDBRecord(
             leveldb_record)
       except(
           errors.ParserError,
           errors.DecoderError,
           NotImplementedError) as err:
```

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/chromium/v8.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/chromium/v8.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/cli.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import argparse
 import dataclasses
 import enum
 from datetime import datetime
 import json
 import pathlib
 
+from dfindexeddb import utils
 from dfindexeddb import version
 from dfindexeddb.indexeddb.chromium import blink
 from dfindexeddb.indexeddb.chromium import record as chromium_record
 from dfindexeddb.indexeddb.chromium import v8
 from dfindexeddb.indexeddb.safari import record as safari_record
 
 
@@ -32,15 +33,15 @@
     '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~.')
 
 
 class Encoder(json.JSONEncoder):
   """A JSON encoder class for dfindexeddb fields."""
   def default(self, o):
     if dataclasses.is_dataclass(o):
-      o_dict = dataclasses.asdict(o)
+      o_dict = utils.asdict(o)
       return o_dict
     if isinstance(o, bytes):
       out = []
       for x in o:
         if chr(x) not in _VALID_PRINTABLE_CHARACTERS:
           out.append(f'\\x{x:02X}')
         else:
@@ -79,15 +80,17 @@
     _Output(blink_value, output=args.output)
 
 
 def DbCommand(args):
   """The CLI for processing a directory as IndexedDB."""
   if args.format in ('chrome', 'chromium'):
     for db_record in chromium_record.FolderReader(
-        args.source).GetRecords(use_manifest=args.use_manifest):
+        args.source).GetRecords(
+            use_manifest=args.use_manifest,
+            use_sequence_number=args.use_sequence_number):
       _Output(db_record, output=args.output)
   elif args.format == 'safari':
     for db_record in safari_record.FileReader(args.source).Records():
       _Output(db_record, output=args.output)
 
 
 def LdbCommand(args):
@@ -135,24 +138,31 @@
   parser_db.add_argument(
       '-s', '--source',
       required=True,
       type=pathlib.Path,
       help=(
         'The source IndexedDB folder (for chrome/chromium) '
         'or file (for safari).'))
+  recover_group = parser_db.add_mutually_exclusive_group()
+  recover_group.add_argument(
+      '--use_manifest',
+      action='store_true',
+      help='Use manifest file to determine active/deleted records.')
+  recover_group.add_argument(
+      '--use_sequence_number',
+      action='store_true',
+      help=(
+          'Use sequence number and file offset to determine active/deleted '
+          'records.'))
   parser_db.add_argument(
       '--format',
       required=True,
       choices=['chromium', 'chrome', 'safari'],
       help='The type of IndexedDB to parse.')
   parser_db.add_argument(
-      '--use_manifest',
-      action='store_true',
-      help='Use manifest file to determine active/deleted records.')
-  parser_db.add_argument(
       '-o',
       '--output',
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
```

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/firefox/__init__.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/firefox/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/safari/__init__.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/safari/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/safari/definitions.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/safari/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/safari/record.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/safari/record.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/indexeddb/safari/webkit.py` & `dfindexeddb-20240519/dfindexeddb/indexeddb/safari/webkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,15 @@
       the JavaScript array.
 
     Raises:
       ParserError if an invalid Terminator tag was found.
     """
     _, length = self.decoder.DecodeUint32()
     array = JSArray()
+    self.object_pool.append(array)
     for _ in range(length):
       _, _ = self.decoder.DecodeUint32()
       _, value = self.DecodeValue()
       array.append(value)
 
     offset, terminator_tag = self.decoder.DecodeUint32()
     if terminator_tag != definitions.TerminatorTag:
@@ -310,21 +311,21 @@
       raise errors.ParserError(f'Terminator tag not found at offset {offset}.')
     return array
 
   def DecodeObject(self) -> Dict[str, Any]:
     """Decodes an Object value."""
     tag = self.PeekTag()
     js_object = {}
+    self.object_pool.append(js_object)
     while tag != definitions.TerminatorTag:
       name = self.DecodeStringData()
       _, value = self.DecodeValue()
       js_object[name] = value
       tag = self.PeekTag()
     _ = self.decoder.DecodeUint32()
-    self.object_pool.append(js_object)
     return js_object
 
   def DecodeStringData(self) -> str:
     """Decodes a StringData value.
 
     Returns:
       A JavaScript array.
@@ -338,19 +339,19 @@
     """
     peeked_tag = self.PeekTag()
     if peeked_tag == definitions.TerminatorTag:
       raise errors.ParserError('Unexpected TerminatorTag found')
 
     if peeked_tag == definitions.StringPoolTag:
       _ = self.decoder.DecodeUint32()
-      if len(self.constant_pool) < 0xff:
+      if len(self.constant_pool) <= 0xff:
         _, cp_index = self.decoder.DecodeUint8()
-      elif len(self.constant_pool) < 0xffff:
+      elif len(self.constant_pool) <= 0xffff:
         _, cp_index = self.decoder.DecodeUint16()
-      elif len(self.constant_pool) < 0xffffffff:
+      elif len(self.constant_pool) <= 0xffffffff:
         _, cp_index = self.decoder.DecodeUint32()
       else:
         raise errors.ParserError('Unexpected constant pool size value.')
       return self.constant_pool[cp_index]
 
     _, length_with_8bit_flag = self.decoder.DecodeUint32()
     if length_with_8bit_flag == definitions.TerminatorTag:
@@ -446,14 +447,15 @@
     flags = self.DecodeStringData()
     return RegExp(pattern=pattern, flags=flags)
 
   def DecodeMapData(self) -> dict:
     """Decodes a Map value."""
     tag = self.PeekSerializationTag()
     js_map = {}   # TODO: make this into a JSMap (like JSArray/JSSet)
+    self.object_pool.append(js_map)
 
     while tag != definitions.SerializationTag.NON_MAP_PROPERTIES:
       _, key = self.DecodeValue()
       _, value = self.DecodeValue()
       js_map[key] = value
       tag = self.PeekSerializationTag()
 
@@ -464,21 +466,21 @@
     while pool_tag != definitions.TerminatorTag:
       name = self.DecodeStringData()
       value = self.DecodeValue()
       js_map[name] = value
       pool_tag = self.PeekTag()
 
     _, tag = self.decoder.DecodeUint32()
-
     return js_map
 
   def DecodeSetData(self) -> JSSet:
     """Decodes a SetData value."""
     tag = self.PeekSerializationTag()
     js_set = JSSet()
+    self.object_pool.append(js_set)
 
     while tag != definitions.SerializationTag.NON_SET_PROPERTIES:
       _, key = self.DecodeValue()
       js_set.add(key)
       tag = self.PeekSerializationTag()
 
     # consume the NonSetPropertiesTag
@@ -536,16 +538,21 @@
   def DecodeSharedArrayBuffer(self) -> int:
     """Decodes an SharedArrayBuffer value."""
     _, value = self.decoder.DecodeUint32()
     return value
 
   def DecodeObjectReference(self) -> Any:
     """Decodes an ObjectReference value."""
-    _, object_ref = self.decoder.DecodeUint8()
-    return self.object_pool[object_ref - 1]
+    if len(self.object_pool) < 0xFF:
+      _, object_ref = self.decoder.DecodeUint8()
+    elif len(self.object_pool) < 0xFFFF:
+      _, object_ref = self.decoder.DecodeUint16()
+    else:  # if len(self.object_pool) < 0xFFFFFFFF:
+      _, object_ref = self.decoder.DecodeUint32()
+    return self.object_pool[object_ref]
 
   def DecodeArrayBufferView(self) -> ArrayBufferView:
     """Decodes an ArrayBufferView value.
 
     Returns:
       an ArrayBufferView.
 
@@ -637,14 +644,15 @@
       value = self.DecodeRegExp()
     elif tag == definitions.SerializationTag.OBJECT_REFERENCE:
       value = self.DecodeObjectReference()
     elif tag == definitions.SerializationTag.ARRAY_BUFFER:
       value = self.DecodeArrayBuffer()
     elif tag == definitions.SerializationTag.ARRAY_BUFFER_VIEW:
       value = self.DecodeArrayBufferView()
+      self.object_pool.append(value)
     elif tag == definitions.SerializationTag.ARRAY_BUFFER_TRANSFER:
       value = self.DecodeArrayBufferTransfer()
     elif tag == definitions.SerializationTag.TRUE_OBJECT:
       self.object_pool.append(True)
       value = True
     elif tag == definitions.SerializationTag.FALSE_OBJECT:
       self.object_pool.append(False)
```

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/__init__.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/__init__.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/cli.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,33 +15,35 @@
 """A CLI tool for leveldb files."""
 import argparse
 import dataclasses
 from datetime import datetime
 import json
 import pathlib
 
+from dfindexeddb import utils
 from dfindexeddb import version
 from dfindexeddb.leveldb import descriptor
 from dfindexeddb.leveldb import ldb
 from dfindexeddb.leveldb import log
 from dfindexeddb.leveldb import record
+from dfindexeddb.leveldb.plugins import manager
 
 
 _VALID_PRINTABLE_CHARACTERS = (
     ' abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789' +
     '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~.')
 
 
 class Encoder(json.JSONEncoder):
   """A JSON encoder class for dfleveldb fields."""
 
   def default(self, o):
     """Returns a serializable object for o."""
     if dataclasses.is_dataclass(o):
-      o_dict = dataclasses.asdict(o)
+      o_dict = utils.asdict(o)
       return o_dict
     if isinstance(o, bytes):
       out = []
       for x in o:
         if chr(x) not in _VALID_PRINTABLE_CHARACTERS:
           out.append(f'\\x{x:02X}')
         else:
@@ -62,39 +64,79 @@
     print(json.dumps(structure, cls=Encoder))
   elif output == 'repr':
     print(structure)
 
 
 def DbCommand(args):
   """The CLI for processing leveldb folders."""
+  if args.plugin and args.plugin == 'list':
+    for plugin, _ in manager.LeveldbPluginManager.GetPlugins():
+      print(plugin)
+    return
+
+  if args.plugin:
+    plugin_class = manager.LeveldbPluginManager.GetPlugin(args.plugin)
+  else:
+    plugin_class = None
+
   for leveldb_record in record.FolderReader(
-      args.source).GetRecords(use_manifest=args.use_manifest):
-    _Output(leveldb_record, output=args.output)
+      args.source).GetRecords(
+          use_manifest=args.use_manifest,
+          use_sequence_number=args.use_sequence_number):
+    if plugin_class:
+      plugin_record = plugin_class.FromLevelDBRecord(leveldb_record)
+      _Output(plugin_record, output=args.output)
+    else:
+      _Output(leveldb_record, output=args.output)
 
 
 def LdbCommand(args):
   """The CLI for processing ldb files."""
+  if args.plugin and args.plugin == 'list':
+    for plugin, _ in manager.LeveldbPluginManager.GetPlugins():
+      print(plugin)
+    return
+
+  if args.plugin:
+    plugin_class = manager.LeveldbPluginManager.GetPlugin(args.plugin)
+  else:
+    plugin_class = None
+
   ldb_file = ldb.FileReader(args.source)
 
   if args.structure_type == 'blocks':
     # Prints block information.
     for block in ldb_file.GetBlocks():
       _Output(block, output=args.output)
 
   elif args.structure_type == 'records' or not args.structure_type:
     # Prints key value record information.
     for key_value_record in ldb_file.GetKeyValueRecords():
-      _Output(key_value_record, output=args.output)
+      if plugin_class:
+        plugin_record = plugin_class.FromKeyValueRecord(key_value_record)
+        _Output(plugin_record, output=args.output)
+      else:
+        _Output(key_value_record, output=args.output)
 
   else:
     print(f'{args.structure_type} is not supported for ldb files.')
 
 
 def LogCommand(args):
   """The CLI for processing log files."""
+  if args.plugin and args.plugin == 'list':
+    for plugin, _ in manager.LeveldbPluginManager.GetPlugins():
+      print(plugin)
+    return
+
+  if args.plugin:
+    plugin_class = manager.LeveldbPluginManager.GetPlugin(args.plugin)
+  else:
+    plugin_class = None
+
   log_file = log.FileReader(args.source)
 
   if args.structure_type == 'blocks':
     # Prints block information.
     for block in log_file.GetBlocks():
       _Output(block, output=args.output)
 
@@ -108,15 +150,19 @@
     for batch in log_file.GetWriteBatches():
       _Output(batch, output=args.output)
 
   elif (args.structure_type in ('parsed_internal_key', 'records')
         or not args.structure_type):
     # Prints key value record information.
     for internal_key_record in log_file.GetParsedInternalKeys():
-      _Output(internal_key_record, output=args.output)
+      if plugin_class:
+        plugin_record = plugin_class.FromKeyValueRecord(internal_key_record)
+        _Output(plugin_record, output=args.output)
+      else:
+        _Output(internal_key_record, output=args.output)
 
   else:
     print(f'{args.structure_type} is not supported for log files.')
 
 
 def DescriptorCommand(args):
   """The CLI for processing descriptor (MANIFEST) files."""
@@ -140,14 +186,15 @@
         or not args.structure_type):
     for version_edit in manifest_file.GetVersionEdits():
       _Output(version_edit, output=args.output)
 
   else:
     print(f'{args.structure_type} is not supported for descriptor files.')
 
+
 def App():
   """The CLI app entrypoint for parsing leveldb files."""
   parser = argparse.ArgumentParser(
       prog='dfleveldb',
       description='A cli tool for parsing leveldb files',
       epilog=f'Version {version.GetVersion()}')
 
@@ -156,27 +203,37 @@
   parser_db = subparsers.add_parser(
       'db', help='Parse a directory as leveldb.')
   parser_db.add_argument(
       '-s', '--source',
       required=True,
       type=pathlib.Path,
       help='The source leveldb directory')
-  parser_db.add_argument(
+  recover_group = parser_db.add_mutually_exclusive_group()
+  recover_group.add_argument(
       '--use_manifest',
       action='store_true',
       help='Use manifest file to determine active/deleted records.')
+  recover_group.add_argument(
+      '--use_sequence_number',
+      action='store_true',
+      help=(
+          'Use sequence number and file offset to determine active/deleted '
+          'records.'))
   parser_db.add_argument(
       '-o',
       '--output',
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
+  parser_db.add_argument(
+      '--plugin',
+      help='Use plugin to parse records.')
   parser_db.set_defaults(func=DbCommand)
 
   parser_log = subparsers.add_parser(
       'log', help='Parse a leveldb log file.')
   parser_log.add_argument(
       '-s', '--source',
       required=True,
@@ -188,14 +245,17 @@
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
   parser_log.add_argument(
+      '--plugin',
+      help='Use plugin to parse records.')
+  parser_log.add_argument(
       '-t',
       '--structure_type',
       choices=[
           'blocks',
           'physical_records',
           'write_batches',
           'parsed_internal_key'],
@@ -215,14 +275,17 @@
       choices=[
           'json',
           'jsonl',
           'repr'],
       default='json',
       help='Output format.  Default is json')
   parser_ldb.add_argument(
+      '--plugin',
+      help='Use plugin to parse records.')
+  parser_ldb.add_argument(
       '-t',
       '--structure_type',
       choices=[
           'blocks',
           'records'],
       help='Parses the specified structure.  Default is records.')
   parser_ldb.set_defaults(func=LdbCommand)
```

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/definitions.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/definitions.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/descriptor.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/descriptor.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/ldb.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/ldb.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/log.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,28 +148,30 @@
   contents_offset: int
 
   PHYSICAL_HEADER_LENGTH = 7
 
   @classmethod
   def FromDecoder(
       cls, decoder: utils.LevelDBDecoder, base_offset: int = 0
-  ) -> PhysicalRecord:
+  ) -> Optional[PhysicalRecord]:
     """Decodes a PhysicalRecord from the current position of a LevelDBDecoder.
 
     Args:
       decoder: the LevelDBDecoder.
       base_offset: the base offset of the WriteBatch from which the data is
           read from.
 
     Returns:
-      A PhysicalRecord.
+      A PhysicalRecord or None if the parsed header is 0.
     """
     offset, checksum = decoder.DecodeUint32()
     _, length = decoder.DecodeUint16()
     _, record_type_byte = decoder.DecodeUint8()
+    if checksum == 0 or length == 0 or record_type_byte == 0:
+      return None
     try:
       record_type = definitions.LogFilePhysicalRecordType(record_type_byte)
     except ValueError as error:
       raise errors.ParserError(
           f'Error parsing record type of Physical Record at offset '
           f'{offset + base_offset}') from error
     contents_offset, contents = decoder.ReadBytes(length)
@@ -202,15 +204,19 @@
     Yields:
       LogFileRecord
     """
     buffer = io.BytesIO(self.data)
     buffer_length = len(self.data)
 
     while buffer.tell() + PhysicalRecord.PHYSICAL_HEADER_LENGTH < buffer_length:
-      yield PhysicalRecord.FromStream(buffer, base_offset=self.offset)
+      record = PhysicalRecord.FromStream(buffer, base_offset=self.offset)
+      if record:
+        yield record
+      else:
+        return
 
   @classmethod
   def FromStream(cls, stream: BinaryIO) -> Optional[Block]:
     """Parses a Block from a binary stream.
 
     Args:
       stream: the binary stream to be parsed.
```

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/record.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """A module for records from LevelDB files."""
 from __future__ import annotations
+from collections import defaultdict
 import dataclasses
 import pathlib
 import re
 import sys
 from typing import Generator, Optional, Union
 
 from dfindexeddb import errors
@@ -293,25 +294,56 @@
     for ldb_file in self.LdbFiles():
       if ldb_file in processed_files:
         continue
       for record in self._GetLdbRecords(filename=ldb_file):
         record.recovered = True
         yield record
 
+  def _RecordsBySequenceNumber(self) -> Generator[LevelDBRecord, None, None]:
+    """Yields LevelDBRecords using the sequence number and file offset.
+
+    Yields:
+      LevelDBRecords.
+    """
+    unsorted_records = defaultdict(list)
+
+    for filename in self.foldername.iterdir():
+      for leveldb_record in LevelDBRecord.FromFile(filename):
+        if leveldb_record:
+          unsorted_records[leveldb_record.record.key].append(leveldb_record)
+    for _, unsorted_records in unsorted_records.items():
+      num_unsorted_records = len(unsorted_records)
+      if num_unsorted_records == 1:
+        unsorted_records[0].recovered = False
+        yield unsorted_records[0]
+      else:
+        for i, record in enumerate(sorted(
+            unsorted_records, key=lambda x: (
+                x.record.sequence_number, x.record.offset)),
+            start=1):
+          if i == num_unsorted_records:
+            record.recovered = False
+          else:
+            record.recovered = True
+          yield record
+
   def GetRecords(
       self,
-      use_manifest: bool = False
+      use_manifest: bool = False,
+      use_sequence_number: bool = False
   ) -> Generator[LevelDBRecord, None, None]:
     """Yield LevelDBRecords.
 
     Args:
       use_manifest: True to use the current manifest in the folder as a means to
           find the active file set.
 
     Yields:
       LevelDBRecords.
     """
     if use_manifest:
       yield from self._RecordsByManifest()
+    elif use_sequence_number:
+      yield from self._RecordsBySequenceNumber()
     else:
       for filename in self.foldername.iterdir():
         yield from LevelDBRecord.FromFile(filename)
```

### Comparing `dfindexeddb-20240501/dfindexeddb/leveldb/utils.py` & `dfindexeddb-20240519/dfindexeddb/leveldb/utils.py`

 * *Files identical despite different names*

### Comparing `dfindexeddb-20240501/dfindexeddb/utils.py` & `dfindexeddb-20240519/dfindexeddb/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utilities for dfindexeddb."""
 from __future__ import annotations
+import copy
+import dataclasses
 import io
 import os
 import struct
 from typing import BinaryIO, Tuple, Type, TypeVar
 
 
 from dfindexeddb import errors
@@ -255,7 +257,39 @@
       base_offset: the base offset of the raw data.
 
     Returns:
       The class instance.
     """
     stream = io.BytesIO(raw_data)
     return cls.FromStream(stream=stream, base_offset=base_offset)
+
+
+def asdict(obj, *, dict_factory=dict):  # pylint: disable=invalid-name
+  """Custom implementation of the asdict dataclasses method to include the
+  class name under the __type__ attribute name.
+  """
+  if not dataclasses.is_dataclass(obj):
+    raise TypeError("asdict() should be called on dataclass instances")
+  return _asdict_inner(obj, dict_factory)
+
+
+def _asdict_inner(obj, dict_factory):
+  """Custom implementation of the _asdict_inner dataclasses method."""
+  if dataclasses.is_dataclass(obj):
+    result = [('__type__', obj.__class__.__name__)]
+    for f in dataclasses.fields(obj):
+      value = _asdict_inner(getattr(obj, f.name), dict_factory)
+      result.append((f.name, value))
+    return dict_factory(result)
+
+  if isinstance(obj, tuple) and hasattr(obj, '_fields'):
+    return type(obj)(*[_asdict_inner(v, dict_factory) for v in obj])
+
+  if isinstance(obj, (list, tuple)):
+    return type(obj)(_asdict_inner(v, dict_factory) for v in obj)
+
+  if isinstance(obj, dict):
+    return type(obj)((_asdict_inner(k, dict_factory),
+                      _asdict_inner(v, dict_factory))
+                      for k, v in obj.items())
+
+  return copy.deepcopy(obj)
```

### Comparing `dfindexeddb-20240501/dfindexeddb/version.py` & `dfindexeddb-20240519/dfindexeddb/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Version information for dfIndexeddb."""
 
 
-__version__ = "20240501"
+__version__ = "20240519"
 
 
 def GetVersion():
   """Returns the version information."""
   return __version__
```

### Comparing `dfindexeddb-20240501/dfindexeddb.egg-info/PKG-INFO` & `dfindexeddb-20240519/dfindexeddb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfindexeddb
-Version: 20240501
+Version: 20240519
 Summary: dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files.
 Author-email: Syd Pleno <sydp@google.com>
 Maintainer-email: dfIndexeddb Developers <dfindexeddb-dev@googlegroups.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,14 +215,17 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: python-snappy==0.6.1
 Requires-Dist: zstd==1.5.5.1
+Provides-Extra: plugins
+Requires-Dist: protobuf; extra == "plugins"
+Requires-Dist: dfdatetime; extra == "plugins"
 
 # dfIndexeddb
 
 dfindexeddb is an experimental Python tool for performing digital forensic
 analysis of IndexedDB and LevelDB files.
 
 It parses LevelDB, IndexedDB and JavaScript structures from these files without
@@ -251,14 +254,20 @@
 
 ```
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install dfindexeddb
 ```
 
+To also install the dependencies for leveldb/indexeddb plugins, run
+```
+    $ pip install 'dfindexeddb[plugins]'
+```
+
+
 ## Installation from source
 
 1. [Linux] Install the snappy compression development package
 
 ```
     $ sudo apt install libsnappy-dev
 ```
@@ -269,14 +278,19 @@
 
 ```
     $ python3 -m venv .venv
     $ source .venv/bin/activate
     $ pip install .
 ```
 
+To also install the dependencies for leveldb/indexeddb plugins, run
+```
+    $ pip install '.[plugins]'
+```
+
 ## Usage
 
 Two CLI tools for parsing IndexedDB/LevelDB files are available after
 installation:
 
 
 ### IndexedDB
@@ -355,15 +369,23 @@
 ```
 
 #### Examples
 
 To parse records from a LevelDB folder, use the following command:
 
 ```
-dfindexeddb db -s SOURCE
+dfleveldb db -s SOURCE
+```
+
+To parse records from a LevelDB folder, and use the sequence number to 
+determine recovered records and output as JSON, use the
+following command:
+
+```
+dfleveldb db -s SOURCE --use_sequence_number
 ```
 
 To parse blocks / physical records/ write batches / internal key records from a
 LevelDB log (.log) file, use the following command, specifying the type (block,
 physical_records, etc) via the `-t` option.  By default, internal key records are parsed:
 
 ```
@@ -379,19 +401,18 @@
 ```
 
 To parse version edit records from a Descriptor (MANIFEST) file, use the
 following command:
 
 ```
 $ dfleveldb descriptor -s SOURCE [-o {json,jsonl,repr}] [-t {blocks,physical_records,versionedit} | -v]
-
-options:
-  -h, --help            show this help message and exit
-  -s SOURCE, --source SOURCE
-                        The source leveldb file
-  -o {json,jsonl,repr}, --output {json,jsonl,repr}
-                        Output format. Default is json
-  -t {blocks,physical_records,versionedit}, --structure_type {blocks,physical_records,versionedit}
-                        Parses the specified structure. Default is versionedit.
-  -v, --version_history
-                        Parses the leveldb version history.
 ```
+
+#### Plugins
+
+To apply a plugin parser for a leveldb file/folder, add the 
+`--plugin [Plugin Name]` argument.  Currently, there is support for the 
+following artifacts:
+
+| Plugin Name | Artifact Name |
+| -------- | ------- |
+| `ChromeNotificationRecord` | Chrome/Chromium Notifications |
```

### Comparing `dfindexeddb-20240501/dfindexeddb.egg-info/SOURCES.txt` & `dfindexeddb-20240519/dfindexeddb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,8 +29,13 @@
 dfindexeddb/leveldb/__init__.py
 dfindexeddb/leveldb/cli.py
 dfindexeddb/leveldb/definitions.py
 dfindexeddb/leveldb/descriptor.py
 dfindexeddb/leveldb/ldb.py
 dfindexeddb/leveldb/log.py
 dfindexeddb/leveldb/record.py
-dfindexeddb/leveldb/utils.py
+dfindexeddb/leveldb/utils.py
+dfindexeddb/leveldb/plugins/__init__.py
+dfindexeddb/leveldb/plugins/chrome_notifications.py
+dfindexeddb/leveldb/plugins/interface.py
+dfindexeddb/leveldb/plugins/manager.py
+dfindexeddb/leveldb/plugins/notification_database_data_pb2.py
```

### Comparing `dfindexeddb-20240501/pyproject.toml` & `dfindexeddb-20240519/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfindexeddb"
-version = "20240501"
+version = "20240519"
 requires-python = ">=3.8"
 description = "dfindexeddb is an experimental Python tool for performing digital forensic analysis of IndexedDB and leveldb files."
 license = {file = "LICENSE"}
 authors = [{name = "Syd Pleno", email = "sydp@google.com"}]
 maintainers = [
   {name = "dfIndexeddb Developers", email = "dfindexeddb-dev@googlegroups.com"},
 ]
@@ -18,26 +18,30 @@
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Programming Language :: Python',
 ]
 
+[project.optional-dependencies]
+plugins = ["protobuf", "dfdatetime"]
+
 [project.scripts]
 dfindexeddb = "dfindexeddb.indexeddb.cli:App"
 dfleveldb = "dfindexeddb.leveldb.cli:App"
 
 [tool.setuptools]
 packages = [
-  "dfindexeddb", 
-  "dfindexeddb.indexeddb", 
+  "dfindexeddb",
+  "dfindexeddb.indexeddb",
   "dfindexeddb.indexeddb.chromium",
   "dfindexeddb.indexeddb.firefox",
-  "dfindexeddb.indexeddb.safari", 
+  "dfindexeddb.indexeddb.safari",
   "dfindexeddb.leveldb",
+  "dfindexeddb.leveldb.plugins",
 ]
 
 [project.urls]
 Homepage = "https://github.com/google/dfindexeddb"
 Documentation = "https://github.com/google/dfindexeddb/tree/main/docs"
 Repository = "https://github.com/google/dfindexeddb"
 "Bug Tracker" = "https://github.com/google/dfindexeddb/issues"
```

### Comparing `dfindexeddb-20240501/setup.py` & `dfindexeddb-20240519/setup.py`

 * *Files identical despite different names*

