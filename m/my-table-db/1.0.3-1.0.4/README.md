# Comparing `tmp/my_table_db-1.0.3.tar.gz` & `tmp/my_table_db-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-1.0.3.tar", last modified: Sat May 18 20:31:33 2024, max compression
+gzip compressed data, was "my_table_db-1.0.4.tar", last modified: Sat May 18 22:54:18 2024, max compression
```

## Comparing `my_table_db-1.0.3.tar` & `my_table_db-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 20:31:33.958186 my_table_db-1.0.3/
--rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3941 2024-05-18 20:31:33.957189 my_table_db-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.3/README.md
--rw-rw-rw-   0        0        0     1906 2024-05-18 20:22:33.000000 my_table_db-1.0.3/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 20:31:33.957189 my_table_db-1.0.3/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     3941 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-18 20:31:33.000000 my_table_db-1.0.3/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 20:31:33.958186 my_table_db-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      374 2024-05-18 20:30:39.000000 my_table_db-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:54:18.592935 my_table_db-1.0.4/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3941 2024-05-18 22:54:18.591935 my_table_db-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 22:54:18.590933 my_table_db-1.0.4/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3941 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1906 2024-05-18 20:22:33.000000 my_table_db-1.0.4/my_table_db.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 22:54:18.592935 my_table_db-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-18 22:54:14.000000 my_table_db-1.0.4/setup.py
```

### Comparing `my_table_db-1.0.3/LICENSE` & `my_table_db-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.3/PKG-INFO` & `my_table_db-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.3
+Version: 1.0.4
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `my_table_db-1.0.3/README.md` & `my_table_db-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.3/main.py` & `my_table_db-1.0.4/my_table_db.py`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.3/my_table_db.egg-info/PKG-INFO` & `my_table_db-1.0.4/my_table_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.3
+Version: 1.0.4
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

