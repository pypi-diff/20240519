# Comparing `tmp/my_table_db-1.0.2.tar.gz` & `tmp/my_table_db-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-1.0.2.tar", last modified: Sat May 18 20:22:52 2024, max compression
+gzip compressed data, was "my_table_db-1.0.3.tar", last modified: Sat May 18 20:31:33 2024, max compression
```

## Comparing `my_table_db-1.0.2.tar` & `my_table_db-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 20:22:52.560645 my_table_db-1.0.2/
--rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3941 2024-05-18 20:22:52.559645 my_table_db-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.2/README.md
--rw-rw-rw-   0        0        0     1906 2024-05-18 20:22:33.000000 my_table_db-1.0.2/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:22:52.558643 my_table_db-1.0.2/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     3941 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-18 20:22:52.000000 my_table_db-1.0.2/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 20:22:52.560645 my_table_db-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-05-18 20:22:50.000000 my_table_db-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:31:33.958186 my_table_db-1.0.3/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3941 2024-05-18 20:31:33.957189 my_table_db-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1906 2024-05-18 20:22:33.000000 my_table_db-1.0.3/main.py
+drwxrwxrwx   0        0        0        0 2024-05-18 20:31:33.957189 my_table_db-1.0.3/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3941 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 20:31:33.958186 my_table_db-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      374 2024-05-18 20:30:39.000000 my_table_db-1.0.3/setup.py
```

### Comparing `my_table_db-1.0.2/LICENSE` & `my_table_db-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.2/PKG-INFO` & `my_table_db-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `my_table_db-1.0.2/README.md` & `my_table_db-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.2/main.py` & `my_table_db-1.0.3/main.py`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.2/my_table_db.egg-info/PKG-INFO` & `my_table_db-1.0.3/my_table_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

