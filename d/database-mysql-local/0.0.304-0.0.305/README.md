# Comparing `tmp/database_mysql_local-0.0.304.tar.gz` & `tmp/database_mysql_local-0.0.305.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.304.tar", last modified: Tue May 14 23:53:18 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.305.tar", last modified: Sun May 19 04:23:32 2024, max compression
```

## Comparing `database_mysql_local-0.0.304.tar` & `database_mysql_local-0.0.305.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:53:18.767202 database_mysql_local-0.0.304/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 23:53:18.767202 database_mysql_local-0.0.304/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:53:18.763201 database_mysql_local-0.0.304/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:53:18.767202 database_mysql_local-0.0.304/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-14 23:52:47.000000 database_mysql_local-0.0.304/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53601 2024-05-14 23:52:47.000000 database_mysql_local-0.0.304/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31055 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-14 23:52:44.000000 database_mysql_local-0.0.304/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 23:53:18.767202 database_mysql_local-0.0.304/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-14 23:53:18.000000 database_mysql_local-0.0.304/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-14 23:53:18.000000 database_mysql_local-0.0.304/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 23:53:18.000000 database_mysql_local-0.0.304/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 23:53:18.000000 database_mysql_local-0.0.304/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-14 23:53:18.000000 database_mysql_local-0.0.304/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-14 23:52:19.000000 database_mysql_local-0.0.304/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 23:53:18.767202 database_mysql_local-0.0.304/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-14 23:52:47.000000 database_mysql_local-0.0.304/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.464463 database_mysql_local-0.0.305/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51401 2024-05-19 04:23:02.000000 database_mysql_local-0.0.305/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30908 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-19 04:22:59.000000 database_mysql_local-0.0.305/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 04:23:32.000000 database_mysql_local-0.0.305/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:23:32.472463 database_mysql_local-0.0.305/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 04:22:37.000000 database_mysql_local-0.0.305/setup.py
```

### Comparing `database_mysql_local-0.0.304/PKG-INFO` & `database_mysql_local-0.0.305/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.304
+Version: 0.0.305
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.304/README.md` & `database_mysql_local-0.0.305/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.305/database_mysql_local/src/connector.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.305/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.305/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.305/database_mysql_local/src/generic_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-import os
 import re
 from datetime import datetime
 from functools import lru_cache
-from typing import Any
-from typing import Optional
+from typing import Any, Optional
 
 import mysql.connector
 from database_infrastructure_local.number_generator import NumberGenerator
 from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
 from .table_definition import table_definition
-from .utils import (process_insert_data_dict, process_update_data_dict,
-                    validate_none_select_table_name,
-                    validate_select_table_name)
+from .utils import (process_insert_data_dict, process_update_data_dict, get_where_params, where_skip_null_values,
+                    validate_none_select_table_name, validate_single_clause_value,
+                    validate_select_table_name, detect_if_is_test_data,
+                    generate_view_name, generate_column_name, get_entity_type_by_table_name)
 
 
 # TODO: this file is too big, can we break it down into smaller files?
 class GenericCRUD(metaclass=MetaLogger, object=LOGGER_CRUD_CODE_OBJECT):
     """A class that provides generic CRUD functionality.
     There are 4 main functions to create, read, update, and delete data from the database.
     The rest of the functions are helper functions or wrappers around the main functions."""
@@ -32,18 +31,18 @@
                  default_select_clause_value: str = "*", default_where: str = None, is_test_data: bool = False) -> None:
         """Initializes the GenericCRUD class. If a connection is not provided, a new connection will be created."""
         self.default_schema_name = default_schema_name
         self.connection = Connector.connect(schema_name=default_schema_name)
         self.cursor = self.connection.cursor()
         self.default_column_name = self._deprecated_id_column(default_id_column_name, default_column_name)
         self.default_table_name = default_table_name
-        self.default_view_table_name = default_view_table_name or self.generate_view_name(default_table_name)
+        self.default_view_table_name = default_view_table_name or generate_view_name(default_table_name)
         self.default_select_clause_value = default_select_clause_value
         self.default_where = default_where
-        self.is_test_data = is_test_data or self.__detect_if_is_test_data()
+        self.is_test_data = is_test_data or detect_if_is_test_data()
         self.user_context = UserContext()
 
     def _data_json_to_dict(self, data_json: dict = None) -> dict:
         if data_json is not None:
             # We let the developers migrate quietly for a week
             if datetime.now() > datetime(2024, 5, 20):
                 self.logger.warning(
@@ -52,14 +51,15 @@
 
             return data_json
 
     def _deprecated_id_column(self, id_column_name: str, column_name: str) -> str:
         if id_column_name:
             # We let the developers migrate quietly for a week
             if datetime.now() > datetime(2024, 5, 20):
+                # TODO: print the caller filename
                 self.logger.warning(
                     "GenericCRUD: id_column_name and id_column_value are deprecated and scheduled to be removed by 12/06/2024, use column_name and column_value instead.")
             return id_column_name
         return column_name
 
     def insert(self, *, schema_name: str = None, table_name: str = None, data_dict: dict = None, data_json: dict = None,
                ignore_duplicate: bool = False, commit_changes: bool = True) -> int:
@@ -166,15 +166,15 @@
           and returns the id of the new row or None if an error occurred."""
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_dict_compare = data_json_compare or self._data_json_to_dict(data_dict_compare)
         old_schema_name = self.default_schema_name
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         view_table_name = view_table_name or self.default_view_table_name
-        column_name = self.generate_column_name(table_name)
+        column_name = generate_column_name(table_name)
         self._validate_args(args=locals())
         if not data_dict:
             self.logger.warning(log_message="GenericCRUD.upsert: data_dict is empty")
             return
         if not data_dict_compare:
             return self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict)
 
@@ -270,15 +270,15 @@
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         data_dict = data_json or self._data_json_to_dict(data_dict)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
 
         if column_name:
-            where, params = self.__get_where_params(column_name, column_value)
+            where, params = get_where_params(column_name, column_value)
             self.update_by_where(schema_name=schema_name, table_name=table_name, where=where,
                                  data_dict=data_dict, params=params,
                                  limit=limit, order_by=order_by, commit_changes=commit_changes)
         else:
             raise Exception("Update by id requires an column_name")
 
     def update_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
@@ -325,19 +325,18 @@
                                                id_column_name=id_column_name, id_column_value=id_column_value)
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
                                    column_name: str = None, column_value: Any = None,
                                    id_column_name: str = None, id_column_value: Any = None) -> None:
         """Deletes data from the table by id"""
         # checks are done inside delete_by_where
-        column_name = self._deprecated_id_column(id_column_name, column_name)
+        column_name = self._deprecated_id_column(id_column_name, column_name) or self.default_column_name
         column_value = column_value or id_column_value
-        column_name = column_name or self.default_column_name
         if column_name:  # column_value can be empty
-            where, params = self.__get_where_params(column_name, column_value)
+            where, params = get_where_params(column_name, column_value)
             self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
         else:
             raise Exception("Delete by id requires an column_name and column_value.")
 
     def delete_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None) -> None:
         """Deletes data from the table by WHERE."""
@@ -368,14 +367,18 @@
         where = self.__where_security(where=where, view_name=view_table_name)
         self._validate_args(args=locals())
 
         # TODO: add ` to column names if they are not reserved words (like COUNT, ST_X(point), etc.)
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
         # TODO: If is_test_data exists in the table and is_test_data=False, add `AND is_test_data=0` to avoid users getting test data
         #   (but the tests should be allowed to access real data)
+        if (self.is_test_data and view_table_name.replace("_view", "") ==
+                self.default_view_table_name.replace("_table", "")):
+            # test data does not appear in the view, but we still wants to access it in tests (partial solution).
+            view_table_name = self.default_table_name
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
         self.cursor.execute(select_query, params)
         result = self.cursor.fetchall()
@@ -441,19 +444,14 @@
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, order_by=order_by)
         return self.convert_to_dict(result, select_clause_value)
 
-    def __validate_single_clause_value(self, select_clause_value: str = None) -> None:
-        select_clause_value = select_clause_value or self.default_select_clause_value
-        if "," in select_clause_value or select_clause_value == "*":
-            raise ValueError("select value requires a single column name")
-
     def select_one_value_by_id(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         if datetime.now() > datetime(2024, 5, 20):
             self.logger.warning(
                 "GenericCRUD.select_one_value_by_id is deprecated, use select_one_value_by_column_and_value instead.")
@@ -465,19 +463,18 @@
     def select_one_value_by_column_and_value(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         """Selects one value from the table by ID and returns it."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
-        column_name = column_name or id_column_name
-        column_value = column_value or id_column_value
-        self.__validate_single_clause_value(select_clause_value)
-        where, params = self.__get_where_params(column_name, column_value)
-        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        validate_single_clause_value(select_clause_value)
+        where, params = get_where_params(column_name, column_value)
+        where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         if result:  # TODO: the caller can't tell if not found, or found null
             return result[0]
 
     def select_one_tuple_by_where(
@@ -502,16 +499,17 @@
         return self.convert_to_dict(result, select_clause_value)
 
     def select_one_value_by_where(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "",
             skip_null_values: bool = True) -> Any:
         """Selects one value from the table based on a WHERE clause and returns it."""
-        self.__validate_single_clause_value(select_clause_value)
-        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        validate_single_clause_value(select_clause_value)
+        where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
         if result:
             return result[0]
 
     def select_multi_value_by_id(
@@ -532,28 +530,30 @@
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = "",
             skip_null_values: bool = True) -> list:
         """Selects multiple values from the table by ID and returns them as a list."""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
-        self.__validate_single_clause_value(select_clause_value)
-        where, params = self.__get_where_params(column_name, column_value)
-        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        validate_single_clause_value(select_clause_value)
+        where, params = get_where_params(column_name, column_value)
+        where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_value_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
             order_by: str = "", skip_null_values: bool = True) -> list:
-        self.__validate_single_clause_value(select_clause_value)
-        where = self.__where_skip_null_values(where, select_clause_value, skip_null_values)
+        select_clause_value = select_clause_value or self.default_select_clause_value
+        validate_single_clause_value(select_clause_value)
+        where = where_skip_null_values(where, select_clause_value, skip_null_values)
         result = self.select_multi_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, limit=limit, order_by=order_by)
         return [row[0] for row in result]
 
     def select_multi_tuple_by_id(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
@@ -680,46 +680,27 @@
                     ";" in str(x) for x in arg_value.keys())) or  # check columns
                     (not arg_name.startswith("data_") and arg_name != "params" and ";" in str(arg_value))):
                 message = f"Invalid value for {arg_name}: {arg_value} (contains ';')"
 
             if message:
                 raise Exception(message)
 
-    @staticmethod
-    def __detect_if_is_test_data() -> bool:
-        """Check if running from a Unit Test file."""
-        import inspect
-        possible_current_files = [os.path.basename(frame.filename) for frame in inspect.stack()]
-
-        for file_name in possible_current_files:
-            if file_name.startswith('test_') or file_name.endswith('_test.py') or "pytest" in file_name:
-                return True
-        return False
-
-    @staticmethod
-    def __get_entity_type_by_table_name(table_name: str) -> int or None:
-        """Returns the entity_type_id of the table."""
-        if table_name in table_definition:
-            entity_type_id = table_definition[table_name].get("entity_type_id1")
-            return entity_type_id
-
     def __add_identifier(self, data_dict: dict, table_name: str) -> None:
         # If there's an "identifier" column in the table, we want to insert a random identifier
         #  to the identifier_table and use it in the data_dict.
-        identifier_entity_type_id = self.__get_entity_type_by_table_name(table_name)
+        identifier_entity_type_id = get_entity_type_by_table_name(table_name)
         if not identifier_entity_type_id:
             return
             # TODO Please add maximum infomation to any exception i.e. table_name, data_dict ...
             # raise Exception("Could not find the entity_type_id1 for table " + table_name + " in database.table_definition_table")
 
-        identifier = NumberGenerator.get_random_identifier(schema_name="identifier",
-                                                           view_name="identifier_view",
-                                                           identifier_column_name="identifier")
+        identifier = NumberGenerator.get_random_identifier(
+            schema_name="identifier", view_name="identifier_view", identifier_column_name="identifier")
         data_dict["identifier"] = identifier
-        # TODO: use self.insert
+        # We can't use self.insert, as it would cause an infinite loop
         insert_query = "INSERT " + \
                        "INTO `identifier`.`identifier_table` (identifier, entity_type_id) " \
                        "VALUES (%s, %s);"
         self.cursor.execute(insert_query, (identifier, identifier_entity_type_id))
         self.connection.commit()
 
     # TODO: add warning logs
@@ -803,16 +784,15 @@
         #     data_dict["updated_effective_profile_id"] = self.user_context.get_effective_profile_id()
         #     data_dict["is_test_data"] = self.is_test_data
         self.logger.debug(object=locals())
         return data_dict
 
     def __log_warning(self, column_name: str, schema_name: str, table_name: str):
         """Generates a warning log message and logs it."""
-        log_message = f"{column_name} not found in {schema_name}.{table_name}"
-        self.logger.warning(log_message)
+        self.logger.warning(f"{column_name} not found in {schema_name}.{table_name}")
 
     def __where_security(self, where: str, view_name: str) -> str:
         """Adds security to the where clause."""
         '''
         if self.is_column_in_table(column_name="visibility_id", schema_name=self.schema_name, table_name=view_name):
             effective_profile_id = self.user_context.get_effective_profile_id()
             where_security = f"(visibility_id > 1 OR created_effective_profile_id = {effective_profile_id})"
@@ -836,74 +816,36 @@
             self.connection.set_schema(schema_name)
             self.default_schema_name = schema_name
 
     def close(self) -> None:
         """Closes the connection to the database (we usually do not have to call this)"""
         self.connection.close()
 
-    def _log_error_message(self, message: str, sql_statement: str, schema_name: str) -> str:
-        return (f"{message} - SQL statement: {sql_statement}. "
-                f"(user={self.connection.user}, host={self.connection.host}, schema={schema_name})")
-
-    @staticmethod
-    def generate_view_name(table_name: Optional[str]) -> Optional[str]:
-        if table_name:
-            return re.sub(r'(_table)$', '_view', table_name)
-
-    @staticmethod
-    def generate_column_name(table_name: Optional[str]) -> Optional[str]:
-        if table_name:
-            return re.sub(r'(_table)$', '_id', table_name)
-
+    # TODO: test this method
     def get_test_entity_id(self, *, entity_name: str, insert_function: callable, insert_kwargs: dict = None,
                            entity_creator: callable = None, create_kwargs: dict = None,
                            schema_name: str = None, view_name: str = None) -> int:
         """
         1. Check if there's an entity with is `is_test_data=True`.
         2. If there is, return its id.
         3. If not, create a new entity with `is_test_data=True` and return its id.
         (assuming entity_creator expects `is_test_data` as parameters,
             and returns the expected argument for insert_function)
 
         Example: get_test_entity_id(entity_name='person', entity_creator=Person, insert_function=PersonsLocal.insert)
         """
         view_name = view_name or self.default_view_table_name
         select_clause_value = entity_name + "_id"
-        fetched_result = self.select_one_dict_by_id(
+        test_entity_id = self.select_one_value_by_id(
             schema_name=schema_name or self.default_schema_name, view_table_name=view_name,
             column_name='is_test_data', column_value='1', select_clause_value=select_clause_value)
-        if fetched_result:
-            test_entity_id = fetched_result[select_clause_value]
-        else:
+        if not test_entity_id:
             insert_kwargs = insert_kwargs or {}
             create_kwargs = create_kwargs or {}
             # is_test_data from the constructor should be used in the sons to avoid duplications
             if entity_creator:
                 entity_result = entity_creator(**create_kwargs)
                 test_entity_id = insert_function(entity_result, **insert_kwargs)
             else:
                 test_entity_id = insert_function(**insert_kwargs)
         self.logger.debug(object=locals())
         return test_entity_id
-
-    def __get_where_params(self, column_name: str, column_value: Any) -> tuple:
-        column_name = column_name or self.default_column_name
-        # If we use "if column_value:" it will not work for 0, False, etc.
-        if column_value is not None:
-            where = f"`{column_name}`=%s"
-            params = (column_value,)
-        else:
-            where = f"`{column_name}` IS NULL"
-            params = None
-        return where, params
-
-    def __where_skip_null_values(self, where: str or None, select_clause_value: str,
-                                 skip_null_values: bool = False) -> str:
-        select_clause_value = select_clause_value or self.default_select_clause_value
-        if skip_null_values:
-            self.__validate_single_clause_value(select_clause_value)
-            where_skip = f"`{select_clause_value}` IS NOT NULL"
-            if where:
-                where += f" AND {where_skip}"
-            else:
-                where = where_skip
-        return where
```

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.305/database_mysql_local/src/generic_crud_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from language_remote.lang_code import LangCode
 from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_ML_CODE_OBJECT
 from .generic_crud import GenericCRUD
+from .utils import generate_column_name, generate_view_name
 
 IS_MAIN_COLUMN_NAME = "is_main"
 
 
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
@@ -121,16 +122,16 @@
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for add_value_if_not_exist")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
-        column_name = GenericCRUD.generate_column_name(table_name)
-        ml_column_name = GenericCRUD.generate_column_name(ml_table_name)
+        column_name = generate_column_name(table_name)
+        ml_column_name = generate_column_name(ml_table_name)
 
         # check if the row exists in the ml_table
         name = data_ml_dict.get("title") or data_ml_dict.get("name")
         if not name:
             raise ValueError("name or title is required for upsert_value")
         table_id = table_id or self.get_id_by_name(table_name=table_name, ml_table_name=ml_table_name, name=name,
                                                    lang_code=lang_code, column_name=column_name, order_by=order_by)
@@ -155,15 +156,15 @@
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         old_schema_name = self.default_schema_name
         self.default_schema_name = schema_name or self.default_schema_name
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
-        column_name = GenericCRUD.generate_column_name(table_name)
+        column_name = generate_column_name(table_name)
 
         if table_id is None:
             raise ValueError("table_id is required for update_value")
         if ml_table_id is None:
             raise ValueError("ml_table_id is required for update_value")
 
         old_cursor = self.cursor
@@ -177,15 +178,15 @@
             if data_dict:
                 self.update_by_id(data_dict=data_dict, table_name=table_name, column_name=column_name,
                                   id_column_value=table_id, limit=limit, order_by=order_by, commit_changes=False)
 
             data_ml_dict[column_name] = table_id
             data_ml_dict["lang_code"] = lang_code_str
             data_ml_dict[self.is_main_column_name] = is_main
-            column_name = GenericCRUD.generate_column_name(ml_table_name)
+            column_name = generate_column_name(ml_table_name)
 
             self.update_by_id(data_dict=data_ml_dict, table_name=ml_table_name, column_name=column_name,
                               id_column_value=ml_table_id, limit=limit, order_by=order_by, commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
@@ -208,16 +209,16 @@
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
-        column_name = GenericCRUD.generate_column_name(table_name)
-        ml_column_name = GenericCRUD.generate_column_name(ml_table_name)
+        column_name = generate_column_name(table_name)
+        ml_column_name = generate_column_name(ml_table_name)
 
         # check if the row exists in the ml_table
         name = data_ml_dict.get("title") or data_ml_dict.get("name")
         name_compare = name
         if not name:
             raise ValueError("name or title is required for upsert_value")
         if data_dict_compare:
@@ -252,16 +253,16 @@
         if not data_ml_dict and not data_ml_json:
             raise ValueError("data_ml_dict or data_ml_json is required for upsert_value")
         data_dict = data_json or self._data_json_to_dict(data_dict)
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
-        column_name = GenericCRUD.generate_column_name(table_name)
-        ml_column_name = GenericCRUD.generate_column_name(ml_table_name)
+        column_name = generate_column_name(table_name)
+        ml_column_name = generate_column_name(ml_table_name)
 
         # check if the row exists in the ml_table
         name_and_abbreviations = data_ml_dict.get("title") or data_ml_dict.get("name")
         if not name_and_abbreviations:
             raise ValueError("name or title is required for upsert_value")
         if data_dict_compare:
             name_and_abbreviations_compare = data_dict_compare.get("title") or data_dict_compare.get("name")
@@ -331,63 +332,63 @@
         return table_id, ml_ids_list
 
     def get_values_tuple(self, table_id: int, lang_code: LangCode = None,
                          column_name: str = None, id_column_name: str = None, select_clause_value: str = "*",
                          order_by: str = None) -> tuple:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
-        column_name = column_name or GenericCRUD.generate_column_name(self.default_table_name)
+        column_name = column_name or generate_column_name(self.default_table_name)
         result = self.select_one_tuple_by_where(where=f"{column_name}=%s AND lang_code=%s",
                                                 params=(table_id, lang_code_str),
                                                 select_clause_value=select_clause_value,
                                                 order_by=order_by)
 
         return result
 
     def get_values_dict(self, table_id: int, lang_code: LangCode = None,
                         column_name: str = None, id_column_name: str = None, order_by: str = None) -> dict:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
-        column_name = column_name or GenericCRUD.generate_column_name(
+        column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_dict_by_where(where=f"{column_name}=%s AND lang_code=%s",
                                                params=(table_id, lang_code_str),
                                                order_by=order_by or f"{column_name} DESC")
 
         return result
 
     def get_values_dict_list(self, table_id: int, lang_code: LangCode = None,
                              column_name: str = None, id_column_name: str = None,
                              order_by: str = None) -> list:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code)
-        column_name = column_name or GenericCRUD.generate_column_name(
+        column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_multi_dict_by_where(where=f"{column_name}=%s AND lang_code=%s",
                                                  params=(table_id, lang_code_str),
                                                  order_by=order_by)
         return result
 
     def get_main_values_tuple(self, table_id: int, column_name: str = None, id_column_name: str = None,
                               select_clause_value: str = "*",
                               order_by: str = None) -> tuple:
         column_name = self._deprecated_id_column(id_column_name, column_name)
-        column_name = column_name or GenericCRUD.generate_column_name(
+        column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_tuple_by_where(where=f"{column_name}=%s AND is_main=1",
                                                 params=(table_id,),
                                                 select_clause_value=select_clause_value,
                                                 order_by=order_by or f"{column_name} DESC")
 
         return result
 
     def get_main_values_dict(self, table_id: int, column_name: str = None, id_column_name: str = None,
                              select_clause_value: str = "*", order_by: str = None) -> dict:
         column_name = self._deprecated_id_column(id_column_name, column_name)
-        column_name = column_name or GenericCRUD.generate_column_name(
+        column_name = column_name or generate_column_name(
             self.default_table_name)
         result = self.select_one_dict_by_where(where=f"{column_name}=%s AND is_main=1",
                                                params=(table_id,),
                                                select_clause_value=select_clause_value,
                                                order_by=order_by)
 
         return result
@@ -395,16 +396,16 @@
     def get_id_by_name(self, name: str, table_name: str = None, ml_table_name: str = None, lang_code: LangCode = None,
                        column_name: str = None, id_column_name: str = None, order_by: str = None,
                        compare_view_name: str = None) -> Optional[int]:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
-        compare_view_name = compare_view_name or self.generate_view_name(ml_table_name)
-        column_name = column_name or GenericCRUD.generate_column_name(table_name)
+        compare_view_name = compare_view_name or generate_view_name(ml_table_name)
+        column_name = column_name or generate_column_name(table_name)
         if GenericCRUD.is_column_in_table(self, table_name=ml_table_name, column_name="title"):
             result = self.select_one_tuple_by_where(view_table_name=compare_view_name,
                                                     select_clause_value=column_name,
                                                     where="title=%s AND lang_code=%s",
                                                     params=(name, lang_code_str),
                                                     order_by=order_by)
         else:
@@ -418,16 +419,16 @@
 
     def get_ml_id_by_name(self, name: str, ml_table_name: str = None, lang_code: LangCode = None,
                           column_name: str = None, id_column_name: str = None, order_by: str = None,
                           compare_view_name: str = None) -> Optional[int]:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, name=name)
         ml_table_name = ml_table_name or self.default_ml_table_name
-        compare_view_name = compare_view_name or self.generate_view_name(ml_table_name)
-        ml_column_name = column_name or GenericCRUD.generate_column_name(ml_table_name)
+        compare_view_name = compare_view_name or generate_view_name(ml_table_name)
+        ml_column_name = column_name or generate_column_name(ml_table_name)
         if GenericCRUD.is_column_in_table(self, table_name=ml_table_name, column_name="title"):
             result = self.select_one_tuple_by_where(view_table_name=compare_view_name,
                                                     select_clause_value=ml_column_name,
                                                     where="title=%s AND lang_code=%s",
                                                     params=(name, lang_code_str),
                                                     order_by=order_by)
         else:
@@ -442,15 +443,15 @@
     def get_ml_ids_by_id(self, table_id: int, ml_table_name: str = None, lang_code: LangCode = None,
                          column_name: str = None, id_column_name: str = None,
                          ml_column_name: str = None, ml_id_column_name: str = None,
                          order_by: str = None, compare_view_name: str = None) -> list:
         column_name = self._deprecated_id_column(id_column_name, column_name)
         ml_column_name = self._deprecated_id_column(ml_id_column_name, ml_column_name)
         lang_code_str = None if lang_code is None else lang_code.value
-        compare_view_name = compare_view_name or self.generate_view_name(ml_table_name)
+        compare_view_name = compare_view_name or generate_view_name(ml_table_name)
         result = self.select_multi_tuple_by_where(view_table_name=compare_view_name,
                                                   select_clause_value=ml_column_name,
                                                   where=f"{column_name}=%s AND lang_code=%s",
                                                   params=(table_id, lang_code_str),
                                                   order_by=order_by)
         return [row[0] for row in result]
 
@@ -475,15 +476,15 @@
         view_name = re.sub(r'(_table)$', '_ml_view', table_name)
         return view_name
 
     # Change the old row with is_main=1 to is_main=0
     def _update_old_main_value_to_zero(self, table_id: int, table_name: str) -> None:
 
         data_ml_dict = {self.is_main_column_name: 0}
-        column_name = GenericCRUD.generate_column_name(table_name)
+        column_name = generate_column_name(table_name)
         where = f"{column_name}=%s AND " + self.is_main_column_name + "=1"
         self.update_by_where(table_name=self.default_ml_table_name,
                              data_dict=data_ml_dict,
                              where=where,
                              params=(table_id,))
 
     def _get_lang_code_str(self, *, name: str = None, lang_code: LangCode = None,
```

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.305/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/point.py` & `database_mysql_local-0.0.305/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.305/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.305/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.305/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.305/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.305/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.304
+Version: 0.0.305
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.304/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.305/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/pyproject.toml` & `database_mysql_local-0.0.305/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.304/setup.py` & `database_mysql_local-0.0.305/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 # TODO: we are migrating from database_mysql_local to database_mysql_local
 #  but in the meantime we want to keep both names
 old_name = "database_mysql_local"
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.304',
+    version='0.0.305',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir, old_name],
     package_dir={package_dir: f'{package_dir}/src', old_name: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

