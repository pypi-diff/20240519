# Comparing `tmp/pypomes_db-0.8.4.tar.gz` & `tmp/pypomes_db-0.8.5.tar.gz`

## Comparing `pypomes_db-0.8.4.tar` & `pypomes_db-0.8.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    31316 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    32487 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.5/PKG-INFO
```

### Comparing `pypomes_db-0.8.4/src/pypomes_db/__init__.py` & `pypomes_db-0.8.5/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.4/src/pypomes_db/db_common.py` & `pypomes_db-0.8.5/src/pypomes_db/db_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 # 2. alternatively, specify a comma-separated list of engines in
 #   {APP_PREFIX}_DB_ENGINES
 #   and for each engine, specify the set above, replacing 'DB' with
 #   'MSQL', 'ORCL', 'PG', and 'SQLS', respectively for the engines listed above
 
 _DB_CONN_DATA: dict = {}
 _DB_ENGINES: list[str] = []
-if env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None):
+_prefix: str = env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None)
+if _prefix:
     _default_setup: bool = True
-    _DB_ENGINES.append(env_get_str(f"{APP_PREFIX}_DB_ENGINE"))
+    _DB_ENGINES.append(_prefix)
 else:
     _default_setup: bool = False
     _engines: str = env_get_str(f"{APP_PREFIX}_DB_ENGINES", None)
     if _engines:
         _DB_ENGINES.extend(_engines.split(sep=","))
 for engine in _DB_ENGINES:
     if _default_setup:
@@ -125,14 +126,26 @@
                                             engine=engine,
                                             bind_vals=where_vals)
             errors.append(f"{count} tuples returned, at least {require_min} expected, for '{msg}'")
 
     return result
 
 
+def _db_get_param(engine: str,
+                  param: str) -> Any:
+    """
+    Return the current value of *param* being used by *engine*.
+
+    :param engine: the reference database engine
+    :param param: the reference parameter
+    :return: the parameter's current value
+    """
+    return _DB_CONN_DATA[engine].get(param)
+
+
 def _db_get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
     The connection parameters are returned as a *tuple*, with the elements
     *name*, *user*, *pwd*, *host*, *port*.
     For *oracle* engines, the extra element *client* is returned.
```

### Comparing `pypomes_db-0.8.4/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.5/src/pypomes_db/db_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# noinspection PyProtectedMember
 from logging import Logger
 from pathlib import Path
 from typing import Any
 
 from .db_common import (
     _DB_ENGINES, _DB_CONN_DATA, _assert_engine
 )
@@ -63,15 +62,15 @@
 
 
 def db_get_engines() -> list[str]:
     """
     Retrieve and return the list of configured engines.
 
     This list may include any of the supported engines:
-     *mysql*, *oracle*, *postgres*, *sqlserver*.
+    *mysql*, *oracle*, *postgres*, *sqlserver*.
 
     :return: the list of configured engines
     """
     return _DB_ENGINES
 
 
 def db_get_params(engine: str = None) -> dict:
@@ -103,14 +102,15 @@
     """
     # initialize the return variable
     result: bool = False
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     proceed: bool = True
     if curr_engine == "oracle":
         from . import oracle_pomes
         # noinspection PyProtectedMember
         proceed = oracle_pomes._initialize(errors=op_errors,
@@ -144,28 +144,32 @@
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         result = oracle_pomes._connect(errors=op_errors,
                                        logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         result = postgres_pomes._connect(errors=op_errors,
                                          logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         result = sqlserver_pomes._connect(errors=op_errors,
                                           logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
@@ -245,15 +249,15 @@
 
     require_min: int = 1 if require_nonempty else None
     reply: list[tuple] = db_select_all(errors=op_errors,
                                        sel_stmt=sel_stmt,
                                        where_vals=where_vals,
                                        require_min=require_min,
                                        require_max=1,
-                                       engine = engine,
+                                       engine=engine,
                                        conn=conn,
                                        logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return reply[0] if reply else None
@@ -288,38 +292,42 @@
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         result = oracle_pomes._select_all(errors=op_errors,
                                           sel_stmt=sel_stmt,
                                           where_vals=where_vals,
                                           require_min=require_min,
                                           require_max=require_max,
                                           conn=conn,
                                           logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         result = postgres_pomes._select_all(errors=op_errors,
                                             sel_stmt=sel_stmt,
                                             where_vals=where_vals,
                                             require_min=require_min,
                                             require_max=require_max,
                                             conn=conn,
                                             logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         result = sqlserver_pomes._select_all(errors=op_errors,
                                              sel_stmt=sel_stmt,
                                              where_vals=where_vals,
                                              require_min=require_min,
                                              require_max=require_max,
                                              conn=conn,
                                              logger=logger)
@@ -468,33 +476,38 @@
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
+    
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         result = oracle_pomes._bulk_insert(errors=op_errors,
                                            insert_stmt=insert_stmt,
                                            insert_vals=insert_vals,
                                            conn=conn,
                                            logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         result = postgres_pomes._bulk_insert(errors=op_errors,
                                              insert_stmt=insert_stmt,
                                              insert_vals=insert_vals,
                                              conn=conn,
                                              logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         result = sqlserver_pomes._bulk_insert(errors=op_errors,
                                               insert_stmt=insert_stmt,
                                               insert_vals=insert_vals,
                                               conn=conn,
                                               logger=logger)
 
     # acknowledge eventual local errors
@@ -527,41 +540,46 @@
     :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: number of LOBs effectively copied
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
+    
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         oracle_pomes._update_lob(errors=op_errors,
                                  lob_table=lob_table,
                                  lob_column=lob_column,
                                  pk_columns=pk_columns,
                                  pk_vals=pk_vals,
                                  lob_file=lob_file,
                                  chunk_size=chunk_size,
                                  conn=conn,
                                  logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         postgres_pomes._update_lob(errors=op_errors,
                                    lob_table=lob_table,
                                    lob_column=lob_column,
                                    pk_columns=pk_columns,
                                    pk_vals=pk_vals,
                                    lob_file=lob_file,
                                    chunk_size=chunk_size,
                                    conn=conn,
                                    logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         sqlserver_pomes._update_lob(errors=op_errors,
                                     lob_table=lob_table,
                                     lob_column=lob_column,
                                     pk_columns=pk_columns,
                                     pk_vals=pk_vals,
                                     lob_file=lob_file,
                                     chunk_size=chunk_size,
@@ -599,33 +617,38 @@
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
+    
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         result = oracle_pomes._execute(errors=op_errors,
                                        exc_stmt=exc_stmt,
                                        bind_vals=bind_vals,
                                        conn=conn,
                                        logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         result = postgres_pomes.db_execute(errors=op_errors,
                                            exc_stmt=exc_stmt,
                                            bind_vals=bind_vals,
                                            conn=conn,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         result = sqlserver_pomes._execute(errors=op_errors,
                                           exc_stmt=exc_stmt,
                                           bind_vals=bind_vals,
                                           conn=conn,
                                           logger=logger)
 
     # acknowledge eventual local errors
@@ -655,33 +678,38 @@
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
+    
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         result = oracle_pomes._call_function(errors=op_errors,
                                              func_name=func_name,
                                              func_vals=func_vals,
                                              conn=conn,
                                              logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         result = postgres_pomes._call_procedure(errors=op_errors,
                                                 proc_name=func_name,
                                                 proc_vals=func_vals,
                                                 conn=conn,
                                                 logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         result = sqlserver_pomes._call_procedure(errors=op_errors,
                                                  proc_name=func_name,
                                                  proc_vals=func_vals,
                                                  conn=conn,
                                                  logger=logger)
 
     # acknowledge eventual local errors
@@ -711,33 +739,38 @@
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
+    # determine the database engine
     curr_engine: str = _assert_engine(op_errors, engine)
+    
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
+        # noinspection PyProtectedMember
         result = oracle_pomes._call_procedure(errors=op_errors,
                                               proc_name=proc_name,
                                               proc_vals=proc_vals,
                                               conn=conn,
                                               logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
+        # noinspection PyProtectedMember
         result = postgres_pomes._call_procedure(errors=op_errors,
                                                 proc_name=proc_name,
                                                 proc_vals=proc_vals,
                                                 conn=conn,
                                                 logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
+        # noinspection PyProtectedMember
         result = sqlserver_pomes._call_procedure(errors=op_errors,
                                                  proc_name=proc_name,
                                                  proc_vals=proc_vals,
                                                  conn=conn,
                                                  logger=logger)
 
     # acknowledge eventual local errors
```

### Comparing `pypomes_db-0.8.4/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.5/src/pypomes_db/migration_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.4/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.5/src/pypomes_db/oracle_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.4/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.5/src/pypomes_db/postgres_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.4/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.5/src/pypomes_db/sqlserver_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.4/LICENSE` & `pypomes_db-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.4/pyproject.toml` & `pypomes_db-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.4"
+version = "0.8.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.8.4/PKG-INFO` & `pypomes_db-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.8.4
+Version: 0.8.5
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

