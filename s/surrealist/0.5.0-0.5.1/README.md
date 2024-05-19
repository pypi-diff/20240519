# Comparing `tmp/surrealist-0.5.0.tar.gz` & `tmp/surrealist-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealist-0.5.0.tar", last modified: Wed May 15 11:06:42 2024, max compression
+gzip compressed data, was "surrealist-0.5.1.tar", last modified: Sun May 19 16:07:06 2024, max compression
```

## Comparing `surrealist-0.5.0.tar` & `surrealist-0.5.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.564814 surrealist-0.5.0/
--rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.5.0/LICENSE
--rw-rw-rw-   0        0        0    31030 2024-05-15 11:06:42.563815 surrealist-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0    29020 2024-05-15 11:06:07.000000 surrealist-0.5.0/README.md
--rw-rw-rw-   0        0        0      905 2024-05-15 11:06:07.000000 surrealist-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 11:06:42.564814 surrealist-0.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.495815 surrealist-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.507815 surrealist-0.5.0/src/surrealist/
--rw-rw-rw-   0        0        0      849 2024-04-20 09:05:50.000000 surrealist-0.5.0/src/surrealist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.518814 surrealist-0.5.0/src/surrealist/clients/
--rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.5.0/src/surrealist/clients/__init__.py
--rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.5.0/src/surrealist/clients/http_client.py
--rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.5.0/src/surrealist/clients/ws_client.py
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.525815 surrealist-0.5.0/src/surrealist/connections/
--rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.5.0/src/surrealist/connections/__init__.py
--rw-rw-rw-   0        0        0    19339 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/connections/connection.py
--rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.5.0/src/surrealist/connections/http_connection.py
--rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/connections/pool.py
--rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/connections/ws_connection.py
--rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.5.0/src/surrealist/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.530815 surrealist-0.5.0/src/surrealist/ql/
--rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.5.0/src/surrealist/ql/__init__.py
--rw-rw-rw-   0        0        0    16349 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/database.py
--rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.5.0/src/surrealist/ql/pool_database.py
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.561815 surrealist-0.5.0/src/surrealist/ql/statements/
--rw-rw-rw-   0        0        0      530 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/__init__.py
--rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.5.0/src/surrealist/ql/statements/common_statements.py
--rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/create.py
--rw-rw-rw-   0        0        0     1282 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/create_statements.py
--rw-rw-rw-   0        0        0    15142 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/define.py
--rw-rw-rw-   0        0        0     5465 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/define_index_statements.py
--rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.5.0/src/surrealist/ql/statements/delete.py
--rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.5.0/src/surrealist/ql/statements/insert.py
--rw-rw-rw-   0        0        0      496 2024-02-09 12:21:48.000000 surrealist-0.5.0/src/surrealist/ql/statements/insert_statements.py
--rw-rw-rw-   0        0        0     2967 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/ql/statements/live.py
--rw-rw-rw-   0        0        0     1289 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/live_statements.py
--rw-rw-rw-   0        0        0     1749 2024-02-19 06:06:05.000000 surrealist-0.5.0/src/surrealist/ql/statements/permissions.py
--rw-rw-rw-   0        0        0      962 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/rebuild_index.py
--rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/relate.py
--rw-rw-rw-   0        0        0     1792 2024-03-13 09:08:42.000000 surrealist-0.5.0/src/surrealist/ql/statements/remove.py
--rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.5.0/src/surrealist/ql/statements/returns.py
--rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.5.0/src/surrealist/ql/statements/select.py
--rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.5.0/src/surrealist/ql/statements/select_statements.py
--rw-rw-rw-   0        0        0     2167 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/show.py
--rw-rw-rw-   0        0        0     1457 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/simple_statements.py
--rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.5.0/src/surrealist/ql/statements/statement.py
--rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.5.0/src/surrealist/ql/statements/transaction.py
--rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.5.0/src/surrealist/ql/statements/update.py
--rw-rw-rw-   0        0        0     2016 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/update_statements.py
--rw-rw-rw-   0        0        0      621 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/statements/utils.py
--rw-rw-rw-   0        0        0     9582 2024-05-15 11:06:07.000000 surrealist-0.5.0/src/surrealist/ql/table.py
--rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.5.0/src/surrealist/result.py
--rw-rw-rw-   0        0        0     9831 2024-03-29 07:04:55.000000 surrealist-0.5.0/src/surrealist/surreal.py
--rw-rw-rw-   0        0        0     2221 2024-04-20 09:05:50.000000 surrealist-0.5.0/src/surrealist/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 11:06:42.562814 surrealist-0.5.0/src/surrealist.egg-info/
--rw-rw-rw-   0        0        0    31030 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1869 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 11:06:42.000000 surrealist-0.5.0/src/surrealist.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.366100 surrealist-0.5.1/
+-rw-rw-rw-   0        0        0     1091 2024-02-04 05:55:53.000000 surrealist-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0    31133 2024-05-19 16:07:06.365100 surrealist-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0    29123 2024-05-19 16:06:48.000000 surrealist-0.5.1/README.md
+-rw-rw-rw-   0        0        0      905 2024-05-19 16:06:48.000000 surrealist-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:07:06.366100 surrealist-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.315129 surrealist-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.324100 surrealist-0.5.1/src/surrealist/
+-rw-rw-rw-   0        0        0      849 2024-04-20 09:05:50.000000 surrealist-0.5.1/src/surrealist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.331100 surrealist-0.5.1/src/surrealist/clients/
+-rw-rw-rw-   0        0        0      124 2024-02-04 05:55:53.000000 surrealist-0.5.1/src/surrealist/clients/__init__.py
+-rw-rw-rw-   0        0        0     5044 2024-02-16 16:27:45.000000 surrealist-0.5.1/src/surrealist/clients/http_client.py
+-rw-rw-rw-   0        0        0     8117 2024-02-16 16:26:19.000000 surrealist-0.5.1/src/surrealist/clients/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.337100 surrealist-0.5.1/src/surrealist/connections/
+-rw-rw-rw-   0        0        0      198 2024-02-04 05:55:53.000000 surrealist-0.5.1/src/surrealist/connections/__init__.py
+-rw-rw-rw-   0        0        0    19339 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/connections/connection.py
+-rw-rw-rw-   0        0        0    27023 2024-03-14 16:05:03.000000 surrealist-0.5.1/src/surrealist/connections/http_connection.py
+-rw-rw-rw-   0        0        0     8023 2024-04-14 06:04:00.000000 surrealist-0.5.1/src/surrealist/connections/pool.py
+-rw-rw-rw-   0        0        0    29659 2024-04-14 06:04:00.000000 surrealist-0.5.1/src/surrealist/connections/ws_connection.py
+-rw-rw-rw-   0        0        0     2439 2024-03-14 15:59:51.000000 surrealist-0.5.1/src/surrealist/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.341100 surrealist-0.5.1/src/surrealist/ql/
+-rw-rw-rw-   0        0        0      231 2024-03-02 11:31:18.000000 surrealist-0.5.1/src/surrealist/ql/__init__.py
+-rw-rw-rw-   0        0        0    16349 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/database.py
+-rw-rw-rw-   0        0        0     3135 2024-03-02 11:31:18.000000 surrealist-0.5.1/src/surrealist/ql/pool_database.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.363100 surrealist-0.5.1/src/surrealist/ql/statements/
+-rw-rw-rw-   0        0        0      530 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/__init__.py
+-rw-rw-rw-   0        0        0     2909 2024-02-11 13:05:41.000000 surrealist-0.5.1/src/surrealist/ql/statements/common_statements.py
+-rw-rw-rw-   0        0        0     1518 2024-02-12 10:41:24.000000 surrealist-0.5.1/src/surrealist/ql/statements/create.py
+-rw-rw-rw-   0        0        0     1282 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/create_statements.py
+-rw-rw-rw-   0        0        0    15489 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/define.py
+-rw-rw-rw-   0        0        0    14628 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/define_index_statements.py
+-rw-rw-rw-   0        0        0     1213 2024-02-19 06:12:19.000000 surrealist-0.5.1/src/surrealist/ql/statements/delete.py
+-rw-rw-rw-   0        0        0     2409 2024-02-19 06:14:54.000000 surrealist-0.5.1/src/surrealist/ql/statements/insert.py
+-rw-rw-rw-   0        0        0      937 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/insert_statements.py
+-rw-rw-rw-   0        0        0     3297 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/live.py
+-rw-rw-rw-   0        0        0     1951 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/live_statements.py
+-rw-rw-rw-   0        0        0     1967 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/permissions.py
+-rw-rw-rw-   0        0        0      962 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/rebuild_index.py
+-rw-rw-rw-   0        0        0     1377 2024-02-12 10:41:24.000000 surrealist-0.5.1/src/surrealist/ql/statements/relate.py
+-rw-rw-rw-   0        0        0     2025 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/remove.py
+-rw-rw-rw-   0        0        0      825 2024-02-12 10:41:24.000000 surrealist-0.5.1/src/surrealist/ql/statements/returns.py
+-rw-rw-rw-   0        0        0     3190 2024-02-19 06:14:54.000000 surrealist-0.5.1/src/surrealist/ql/statements/select.py
+-rw-rw-rw-   0        0        0     8006 2024-02-11 12:57:39.000000 surrealist-0.5.1/src/surrealist/ql/statements/select_statements.py
+-rw-rw-rw-   0        0        0     2167 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/show.py
+-rw-rw-rw-   0        0        0     1457 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/simple_statements.py
+-rw-rw-rw-   0        0        0     3436 2024-02-16 16:23:17.000000 surrealist-0.5.1/src/surrealist/ql/statements/statement.py
+-rw-rw-rw-   0        0        0      924 2024-02-19 06:12:19.000000 surrealist-0.5.1/src/surrealist/ql/statements/transaction.py
+-rw-rw-rw-   0        0        0     1273 2024-02-19 06:12:19.000000 surrealist-0.5.1/src/surrealist/ql/statements/update.py
+-rw-rw-rw-   0        0        0     3667 2024-05-19 16:06:48.000000 surrealist-0.5.1/src/surrealist/ql/statements/update_statements.py
+-rw-rw-rw-   0        0        0      621 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/statements/utils.py
+-rw-rw-rw-   0        0        0     9582 2024-05-15 11:06:07.000000 surrealist-0.5.1/src/surrealist/ql/table.py
+-rw-rw-rw-   0        0        0     8695 2024-04-14 06:04:00.000000 surrealist-0.5.1/src/surrealist/result.py
+-rw-rw-rw-   0        0        0     9831 2024-05-19 12:47:50.000000 surrealist-0.5.1/src/surrealist/surreal.py
+-rw-rw-rw-   0        0        0     2221 2024-04-20 09:05:50.000000 surrealist-0.5.1/src/surrealist/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:07:06.364100 surrealist-0.5.1/src/surrealist.egg-info/
+-rw-rw-rw-   0        0        0    31133 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1869 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 16:07:06.000000 surrealist-0.5.1/src/surrealist.egg-info/top_level.txt
```

### Comparing `surrealist-0.5.0/LICENSE` & `surrealist-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/PKG-INFO` & `surrealist-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,15 +34,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websocket-client
 
 # README #
 
-Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro)
+Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.0)
 
 It is **synchronous** and **unofficial**, so if you need async AND/OR official client, go [here](https://github.com/surrealdb/surrealdb.py)
 
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
@@ -194,26 +194,26 @@
     print(result)
     print(table.count()) # now one record
 ```
 You can find QL examples [here](https://github.com/kotolex/surrealist/tree/master/examples/surreal_ql)
 
 One of the main features of QL-builder is that using dot you can see all statements available on each level, 
 any modern IDE will show possible statements when you type dot. 
-Thanks to this, you can not only study QL but also gain confidence that you are forming a valid query.
+Thanks to this, you can study QL and also gain confidence that you are forming a valid query.
 
 for example
 `db.account.select().limit(50).start_at(50)` analog "SELECT * FROM account LIMIT 50 START 50;"
 
 Pay attention — you can use just table name without using table() method `db.person.select()`, 
 it is readable and shorter, but in that particular case you will not get IDE suggestions.
 
 So, we recommend using table() method `db.table("person").select()` it is not much bigger, but still readable, 
 and you will get help from your IDE
 
-If you cannot form your query, you always can use a raw query via `database.raw_query` or `connection.query`
+If you cannot form your query with QL, you always can use a raw query via `database.raw_query` or `connection.query`
 It is the most efficient way, cause it allows you to do all that is possible if you have permissions.
 
 ### Iteration on Select ###
 
 When you expect a lot of data on your select query via QL-builder, you should consider using iterator, it is a simple, lazy and common way to use in python.
 
 Iterator can be used with **next** method or in **for** statement
@@ -552,17 +552,19 @@
 
 
 with DatabaseConnectionsPool("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root'), min_connections=10, 
                              max_connections=40) as db: # create pool, it creates 10 connections on start
     make_something_with_a_lot_of_threads_or_data(db) # use pool everywhere we need as a simple Database object
 ```
 
-**Note:** DatabaseConnectionsPool is NOT a singleton, it allows creating as many pools as you like, for example, for different databases or namespaces. 
+**Note 1:** DatabaseConnectionsPool is NOT a singleton, it allows creating as many pools as you like, for example, for different databases or namespaces. 
 It is your job as a developer to limit number of pools created in your application
 
+**Note 2:** DatabaseConnectionsPool uses threads, not processes
+
 **Important note:** for many and maybe the most cases, one shared connection is enough to do the job. Test it and make sure you really need a connection pool.
 
 ## Recursion and JSON in Python ##
 SurrealDb has _"no limit to the depth of any nested objects or values within"_, but in Python we have a recursion limit and
 standard json library (and str function) use recursion to load and dump objects, so if you will have deep nesting in your objects - 
 you can get RecursionLimitError.
```

### Comparing `surrealist-0.5.0/README.md` & `surrealist-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # README #
 
-Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro)
+Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.0)
 
 It is **synchronous** and **unofficial**, so if you need async AND/OR official client, go [here](https://github.com/surrealdb/surrealdb.py)
 
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
@@ -156,26 +156,26 @@
     print(result)
     print(table.count()) # now one record
 ```
 You can find QL examples [here](https://github.com/kotolex/surrealist/tree/master/examples/surreal_ql)
 
 One of the main features of QL-builder is that using dot you can see all statements available on each level, 
 any modern IDE will show possible statements when you type dot. 
-Thanks to this, you can not only study QL but also gain confidence that you are forming a valid query.
+Thanks to this, you can study QL and also gain confidence that you are forming a valid query.
 
 for example
 `db.account.select().limit(50).start_at(50)` analog "SELECT * FROM account LIMIT 50 START 50;"
 
 Pay attention — you can use just table name without using table() method `db.person.select()`, 
 it is readable and shorter, but in that particular case you will not get IDE suggestions.
 
 So, we recommend using table() method `db.table("person").select()` it is not much bigger, but still readable, 
 and you will get help from your IDE
 
-If you cannot form your query, you always can use a raw query via `database.raw_query` or `connection.query`
+If you cannot form your query with QL, you always can use a raw query via `database.raw_query` or `connection.query`
 It is the most efficient way, cause it allows you to do all that is possible if you have permissions.
 
 ### Iteration on Select ###
 
 When you expect a lot of data on your select query via QL-builder, you should consider using iterator, it is a simple, lazy and common way to use in python.
 
 Iterator can be used with **next** method or in **for** statement
@@ -514,17 +514,19 @@
 
 
 with DatabaseConnectionsPool("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root'), min_connections=10, 
                              max_connections=40) as db: # create pool, it creates 10 connections on start
     make_something_with_a_lot_of_threads_or_data(db) # use pool everywhere we need as a simple Database object
 ```
 
-**Note:** DatabaseConnectionsPool is NOT a singleton, it allows creating as many pools as you like, for example, for different databases or namespaces. 
+**Note 1:** DatabaseConnectionsPool is NOT a singleton, it allows creating as many pools as you like, for example, for different databases or namespaces. 
 It is your job as a developer to limit number of pools created in your application
 
+**Note 2:** DatabaseConnectionsPool uses threads, not processes
+
 **Important note:** for many and maybe the most cases, one shared connection is enough to do the job. Test it and make sure you really need a connection pool.
 
 ## Recursion and JSON in Python ##
 SurrealDb has _"no limit to the depth of any nested objects or values within"_, but in Python we have a recursion limit and
 standard json library (and str function) use recursion to load and dump objects, so if you will have deep nesting in your objects - 
 you can get RecursionLimitError.
```

### Comparing `surrealist-0.5.0/pyproject.toml` & `surrealist-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "surrealist"
-version = "0.5.0"
+version = "0.5.1"
 description = "Python client for SurrealDB, latest SurrealDB version compatible, all features supported"
 readme = "README.md"
 authors = [{ name = "kotolex", email = "farofwell@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `surrealist-0.5.0/src/surrealist/__init__.py` & `surrealist-0.5.1/src/surrealist/__init__.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/clients/http_client.py` & `surrealist-0.5.1/src/surrealist/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/clients/ws_client.py` & `surrealist-0.5.1/src/surrealist/clients/ws_client.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/connections/connection.py` & `surrealist-0.5.1/src/surrealist/connections/connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/connections/http_connection.py` & `surrealist-0.5.1/src/surrealist/connections/http_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/connections/pool.py` & `surrealist-0.5.1/src/surrealist/connections/pool.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/connections/ws_connection.py` & `surrealist-0.5.1/src/surrealist/connections/ws_connection.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/errors.py` & `surrealist-0.5.1/src/surrealist/errors.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/database.py` & `surrealist-0.5.1/src/surrealist/ql/database.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/pool_database.py` & `surrealist-0.5.1/src/surrealist/ql/pool_database.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/__init__.py` & `surrealist-0.5.1/src/surrealist/ql/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/common_statements.py` & `surrealist-0.5.1/src/surrealist/ql/statements/common_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/create.py` & `surrealist-0.5.1/src/surrealist/ql/statements/create.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/create_statements.py` & `surrealist-0.5.1/src/surrealist/ql/statements/create_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/define.py` & `surrealist-0.5.1/src/surrealist/ql/statements/define.py`

 * *Files 4% similar despite different names*

```diff
@@ -329,14 +329,20 @@
         self._full = False
         self._less = True
         return self
 
     def changefeed(self, duration: str, include_original: bool = False) -> "DefineTable":
         """
         Represents CHANGEFEED statement
+
+        Refer to:
+        https://surrealdb.com/docs/surrealdb/surrealql/statements/define/table#using-changefeed-clause
+
+        :param duration: valid string representation for duration, for example, "1s"
+        :param include_original: if True, then add INCLUDE ORIGINAL statement
         """
         self._changefeed = (duration, include_original)
         return self
 
     def alias(self, select: Union[str, Statement]) -> "DefineTable":
         """
         Represents AS statements, Select statement or raw string expected
@@ -381,16 +387,18 @@
                 self._type = f"RELATION IN {from_to[0]} OUT {from_to[1]}"
         else:
             self._type = "RELATION"
         return self
 
     def validate(self) -> List[str]:
         durations = ('w', 'y', 'd', 'h', 'ms', 's', 'm')
-        if self._changefeed and not any(self._changefeed.endswith(letter) for letter in durations):
-            return [f"Wrong duration {self._changefeed}, allowed postfix are (ms, s, m, h, d, w, y)"]
+        if self._changefeed:
+            actual_duration, _ = self._changefeed
+            if not any(actual_duration.endswith(letter) for letter in durations):
+                return [f"Wrong duration {actual_duration}, allowed postfix are {durations}"]
         return [OK]
 
     def _clean_str(self):
         drop = "" if not self._drop else " DROP"
         schema = ""
         if self._less:
             schema = " SCHEMALESS"
```

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/delete.py` & `surrealist-0.5.1/src/surrealist/ql/statements/delete.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/insert.py` & `surrealist-0.5.1/src/surrealist/ql/statements/insert.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/live.py` & `surrealist-0.5.1/src/surrealist/ql/statements/live.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,32 @@
         self._alias = None
         self._diff = use_diff
         self._callback = callback
         self._select = select
         self._value = None
 
     def value(self, field_name: str) -> "Live":
+        """
+        Add VALUE statement
+
+        :param field_name: field to use
+        :return: Live object
+        """
         self._value = field_name
         return self
 
     def alias(self, value_name: str, alias: str) -> "Live":
+        """
+        Add AS statement
+        @fields [ AS @alias ]
+
+        :param value_name: name of the field
+        :param alias: name of the alias
+        :return: Live object
+        """
         self._alias = (value_name, alias)
         self._diff = False
         return self
 
     def validate(self) -> List[str]:
         if self._select and any([self._value, self._diff, self._alias]):
             return ["If select is provided, value, diff and alias parameters will be ignored"]
```

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/live_statements.py` & `surrealist-0.5.1/src/surrealist/ql/statements/live_statements.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,18 +15,31 @@
 
     def run(self) -> SurrealResult:
         return self._statement._drill(self.to_str())
 
 
 class LiveUseFetch:
     def fetch(self, *args: str) -> Fetch:
+        """
+        Add fetch clause to final statement.
+        NOTE: Support for FETCH is not yet available on SurrealDb side!!!
+
+        :param args: arguments to fetch
+        :return: Fetch object
+        """
         return Fetch(self, *args)
 
 
 class Where(FinishedStatement, LiveUseFetch):
+    """
+    Represents WHERE part of the LIVE statement
+
+    Refer to:
+    https://surrealdb.com/docs/surrealdb/surrealql/statements/live#filter-the-live-query
+    """
     def __init__(self, statement: Statement, predicate: str):
         super().__init__(statement)
         self._predicate = predicate
 
     def run(self) -> SurrealResult:
         return self._statement._drill(self.to_str())
 
@@ -35,8 +48,17 @@
 
     def _clean_str(self):
         return f"{self._statement._clean_str()} WHERE {self._predicate}"
 
 
 class LiveUseWhere(LiveUseFetch):
     def where(self, predicate: str) -> Where:
+        """
+        Add WHERE clause to filter data
+
+        Refer to:
+        https://surrealdb.com/docs/surrealdb/surrealql/statements/live#filter-the-live-query
+
+        :param predicate: condition to filter data
+        :return: Where object
+        """
         return Where(self, predicate)
```

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/permissions.py` & `surrealist-0.5.1/src/surrealist/ql/statements/permissions.py`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,23 @@
     def _clean_str(self):
         result = "\n FOR ".join(f"{k} {v}" for k, v in self._kw.items())
         return f"{self._statement._clean_str()} \nPERMISSIONS \n FOR {result}"
 
 
 class CanUsePermissions:
     def permissions_none(self) -> PermissionsNone:
+        """
+        Represents PERMISSIONS NONE statement
+        """
         return PermissionsNone(self)
 
     def permissions_full(self) -> PermissionsFull:
+        """
+        Represents PERMISSIONS FULL statement
+        """
         return PermissionsFull(self)
 
     def permissions_for(self, **kwargs) -> PermissionsFor:
+        """
+        Represents PERMISSIONS FOR statement
+        """
         return PermissionsFor(self, **kwargs)
```

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/rebuild_index.py` & `surrealist-0.5.1/src/surrealist/ql/statements/rebuild_index.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/relate.py` & `surrealist-0.5.1/src/surrealist/ql/statements/relate.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/remove.py` & `surrealist-0.5.1/src/surrealist/ql/statements/remove.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,22 @@
         if type_ == "TABLE":
             self._name = table_name
 
     def validate(self) -> List[str]:
         return [OK]
 
     def if_exists(self) -> "Remove":
+        """
+        Adds IF EXISTS to a final statement
+
+        Refer to:
+        https://surrealdb.com/docs/surrealdb/surrealql/statements/remove#using-if-exists-clause-since-130
+
+        :return: Remove object
+        """
         self._on_exists = True
         return self
 
     def _clean_str(self):
         add = "" if not self._on_exists else " IF EXISTS"
         if self._type in ("TABLE", "PARAM", "USER", "ANALYZER", "SCOPE", "TOKEN"):
             what = f"{self._type}{add} {self._name}"
```

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/returns.py` & `surrealist-0.5.1/src/surrealist/ql/statements/returns.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/select.py` & `surrealist-0.5.1/src/surrealist/ql/statements/select.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/select_statements.py` & `surrealist-0.5.1/src/surrealist/ql/statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/show.py` & `surrealist-0.5.1/src/surrealist/ql/statements/show.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/simple_statements.py` & `surrealist-0.5.1/src/surrealist/ql/statements/simple_statements.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/statement.py` & `surrealist-0.5.1/src/surrealist/ql/statements/statement.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/transaction.py` & `surrealist-0.5.1/src/surrealist/ql/statements/transaction.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/update.py` & `surrealist-0.5.1/src/surrealist/ql/statements/update.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/statements/utils.py` & `surrealist-0.5.1/src/surrealist/ql/statements/utils.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/ql/table.py` & `surrealist-0.5.1/src/surrealist/ql/table.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/result.py` & `surrealist-0.5.1/src/surrealist/result.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/surreal.py` & `surrealist-0.5.1/src/surrealist/surreal.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist/utils.py` & `surrealist-0.5.1/src/surrealist/utils.py`

 * *Files identical despite different names*

### Comparing `surrealist-0.5.0/src/surrealist.egg-info/PKG-INFO` & `surrealist-0.5.1/src/surrealist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surrealist
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python client for SurrealDB, latest SurrealDB version compatible, all features supported
 Author-email: kotolex <farofwell@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -34,15 +34,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websocket-client
 
 # README #
 
-Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro)
+Surrealist is a Python tool to work with awesome [SurrealDB](https://docs.surrealdb.com/docs/intro) (support for latest version 1.5.0)
 
 It is **synchronous** and **unofficial**, so if you need async AND/OR official client, go [here](https://github.com/surrealdb/surrealdb.py)
 
 Works and tested on Ubuntu, macOS, Windows 10, can use python 3.8+ (including python 3.12)
 
 #### Key features: ####
 
@@ -194,26 +194,26 @@
     print(result)
     print(table.count()) # now one record
 ```
 You can find QL examples [here](https://github.com/kotolex/surrealist/tree/master/examples/surreal_ql)
 
 One of the main features of QL-builder is that using dot you can see all statements available on each level, 
 any modern IDE will show possible statements when you type dot. 
-Thanks to this, you can not only study QL but also gain confidence that you are forming a valid query.
+Thanks to this, you can study QL and also gain confidence that you are forming a valid query.
 
 for example
 `db.account.select().limit(50).start_at(50)` analog "SELECT * FROM account LIMIT 50 START 50;"
 
 Pay attention — you can use just table name without using table() method `db.person.select()`, 
 it is readable and shorter, but in that particular case you will not get IDE suggestions.
 
 So, we recommend using table() method `db.table("person").select()` it is not much bigger, but still readable, 
 and you will get help from your IDE
 
-If you cannot form your query, you always can use a raw query via `database.raw_query` or `connection.query`
+If you cannot form your query with QL, you always can use a raw query via `database.raw_query` or `connection.query`
 It is the most efficient way, cause it allows you to do all that is possible if you have permissions.
 
 ### Iteration on Select ###
 
 When you expect a lot of data on your select query via QL-builder, you should consider using iterator, it is a simple, lazy and common way to use in python.
 
 Iterator can be used with **next** method or in **for** statement
@@ -552,17 +552,19 @@
 
 
 with DatabaseConnectionsPool("http://127.0.0.1:8000", 'test', 'test', credentials=('root', 'root'), min_connections=10, 
                              max_connections=40) as db: # create pool, it creates 10 connections on start
     make_something_with_a_lot_of_threads_or_data(db) # use pool everywhere we need as a simple Database object
 ```
 
-**Note:** DatabaseConnectionsPool is NOT a singleton, it allows creating as many pools as you like, for example, for different databases or namespaces. 
+**Note 1:** DatabaseConnectionsPool is NOT a singleton, it allows creating as many pools as you like, for example, for different databases or namespaces. 
 It is your job as a developer to limit number of pools created in your application
 
+**Note 2:** DatabaseConnectionsPool uses threads, not processes
+
 **Important note:** for many and maybe the most cases, one shared connection is enough to do the job. Test it and make sure you really need a connection pool.
 
 ## Recursion and JSON in Python ##
 SurrealDb has _"no limit to the depth of any nested objects or values within"_, but in Python we have a recursion limit and
 standard json library (and str function) use recursion to load and dump objects, so if you will have deep nesting in your objects - 
 you can get RecursionLimitError.
```

### Comparing `surrealist-0.5.0/src/surrealist.egg-info/SOURCES.txt` & `surrealist-0.5.1/src/surrealist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

