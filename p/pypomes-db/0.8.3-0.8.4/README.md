# Comparing `tmp/pypomes_db-0.8.3.tar.gz` & `tmp/pypomes_db-0.8.4.tar.gz`

## Comparing `pypomes_db-0.8.3.tar` & `pypomes_db-0.8.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/__init__.py
--rw-r--r--   0        0        0    11829 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/db_common.py
--rw-r--r--   0        0        0    31355 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/db_pomes.py
--rw-r--r--   0        0        0    18602 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/migration_pomes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/mysql_pomes.py
--rw-r--r--   0        0        0    16125 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/oracle_pomes.py
--rw-r--r--   0        0        0    15231 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/postgres_pomes.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/src/pypomes_db/sqlserver_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/README.md
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/__init__.py
+-rw-r--r--   0        0        0    11999 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/db_common.py
+-rw-r--r--   0        0        0    31316 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/db_pomes.py
+-rw-r--r--   0        0        0    18598 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/migration_pomes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/mysql_pomes.py
+-rw-r--r--   0        0        0    16025 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/oracle_pomes.py
+-rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/postgres_pomes.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/src/pypomes_db/sqlserver_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/README.md
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 pypomes_db-0.8.4/PKG-INFO
```

### Comparing `pypomes_db-0.8.3/src/pypomes_db/__init__.py` & `pypomes_db-0.8.4/src/pypomes_db/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.3/src/pypomes_db/db_common.py` & `pypomes_db-0.8.4/src/pypomes_db/db_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 _DB_CONN_DATA: dict = {}
 _DB_ENGINES: list[str] = []
 if env_get_str(f"{APP_PREFIX}_DB_ENGINE",  None):
     _default_setup: bool = True
     _DB_ENGINES.append(env_get_str(f"{APP_PREFIX}_DB_ENGINE"))
 else:
     _default_setup: bool = False
-    _engines = env_get_str(f"{APP_PREFIX}_DB_ENGINES", None)
+    _engines: str = env_get_str(f"{APP_PREFIX}_DB_ENGINES", None)
     if _engines:
         _DB_ENGINES.extend(_engines.split(sep=","))
 for engine in _DB_ENGINES:
     if _default_setup:
         _tag = "DB"
         _default_setup = False
     else:
@@ -131,28 +131,30 @@
 
 def _db_get_params(engine: str) -> tuple:
     """
     Return the current connection parameters being used for *engine*.
 
     The connection parameters are returned as a *tuple*, with the elements
     *name*, *user*, *pwd*, *host*, *port*.
+    For *oracle* engines, the extra element *client* is returned.
+    For *sqlserver* engines, the extra element *driver* is returned.
     The meaning of some parameters may vary between different database engines.
 
     :param engine: the reference database engine
     :return: the current connection parameters for the engine
     """
-    name: str = _DB_CONN_DATA[engine]["name"]
-    user: str = _DB_CONN_DATA[engine]["user"]
-    pwd: str = _DB_CONN_DATA[engine]["pwd"]
-    host: str = _DB_CONN_DATA[engine]["host"]
-    port: int = _DB_CONN_DATA[engine]["port"]
+    name: str = _DB_CONN_DATA[engine].get("name")
+    user: str = _DB_CONN_DATA[engine].get("user")
+    pwd: str = _DB_CONN_DATA[engine].get("pwd")
+    host: str = _DB_CONN_DATA[engine].get("host")
+    port: int = _DB_CONN_DATA[engine].get("port")
 
     result: tuple
     if engine == "sqlserver":
-        driver: str = _DB_CONN_DATA[engine]["driver"]
+        driver: str = _DB_CONN_DATA[engine].get("driver")
         result = (name, user, pwd, host, port, driver)
     else:
         result = (name, user, pwd, host, port)
 
     return result
 
 
@@ -161,16 +163,16 @@
     """
     Format and return the error message corresponding to the exception raised while accessing the database.
 
     :param exception: the exception raised
     :param engine: the reference database engine
     :return: the formatted error message
     """
-    name: str = _DB_CONN_DATA[engine]["name"]
-    host: str = _DB_CONN_DATA[engine]["host"]
+    name: str = _DB_CONN_DATA[engine].get("name")
+    host: str = _DB_CONN_DATA[engine].get("host")
     return f"Error accessing '{name}' at '{host}': {str_sanitize(f'{exception}')}"
 
 
 def _db_log(logger: Logger,
             engine: str,
             err_msg: str = None,
             level: int = DEBUG,
@@ -181,15 +183,15 @@
     Log *err_msg* and add it to *errors*, or else log the executed query, whichever is applicable.
 
     :param logger: the logger object
     :param engine: the reference database engine
     :param err_msg: the error message to log
     :param level: log level (defaults to DEBUG)
     :param errors: optional incidental errors
-    :param stmt: optional the query statement
+    :param stmt: optional query statement
     :param bind_vals: optional bind values for the query statement
     """
     if err_msg:
         if logger:
             logger.log(level, err_msg)
         if isinstance(errors, list):
             errors.append(err_msg)
```

### Comparing `pypomes_db-0.8.3/src/pypomes_db/db_pomes.py` & `pypomes_db-0.8.4/src/pypomes_db/db_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# noinspection PyProtectedMember
 from logging import Logger
 from pathlib import Path
 from typing import Any
 
 from .db_common import (
     _DB_ENGINES, _DB_CONN_DATA, _assert_engine
 )
@@ -71,17 +72,19 @@
     :return: the list of configured engines
     """
     return _DB_ENGINES
 
 
 def db_get_params(engine: str = None) -> dict:
     """
-    Return the connection parameters a *dict*.
+    Return the connection parameters as a *dict*.
 
     The returned *dict* contains the keys *name*, *user*, *pwd*, *host*, *port*.
+    For *oracle* engines, the returned *dict* contains the extra key *client*.
+    For *sqlserver* engines, the  returned *dict* contains the extra key *driver*.
     The meaning of these parameters may vary between different database engines.
 
     :param engine: the database engine
     :return: the current connection parameters for the engine
     """
     curr_engine: str = _DB_ENGINES[0] if not engine and _DB_ENGINES else engine
     return _DB_CONN_DATA.get(engine or curr_engine)
@@ -90,15 +93,15 @@
 def db_assert_connection(errors: list[str] | None,
                          engine: str = None,
                          logger: Logger = None) -> bool:
     """
     Determine whether the *engine*'s current configuration allows for a safe connection.
 
     :param errors: incidental errors
-    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
     :param logger: optional logger
     :return: True if the trial connection succeeded, False otherwise
     """
     # initialize the return variable
     result: bool = False
 
     # initialize the local errors list
@@ -106,16 +109,16 @@
 
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     proceed: bool = True
     if curr_engine == "oracle":
         from . import oracle_pomes
         # noinspection PyProtectedMember
-        proceed = oracle_pomes.initialize(errors=op_errors,
-                                          logger=logger)
+        proceed = oracle_pomes._initialize(errors=op_errors,
+                                           logger=logger)
     if proceed:
         conn: Any = db_connect(errors=op_errors,
                                engine=curr_engine,
                                logger=logger)
         if conn:
             conn.close()
             result = True
@@ -131,15 +134,15 @@
                logger: Logger = None) -> Any:
     """
     Obtain and return a connection to the database, or *None* if the connection cannot be obtained.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
-    :param engine: the database engine to use (uses the default engine, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
     :param logger: optional logger
     :return: the connection to the database
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
@@ -147,24 +150,24 @@
 
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_connect(errors=op_errors,
-                                         logger=logger)
+        result = oracle_pomes._connect(errors=op_errors,
+                                       logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_connect(errors=op_errors,
-                                           logger=logger)
+        result = postgres_pomes._connect(errors=op_errors,
+                                         logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_connect(errors=op_errors,
-                                            logger=logger)
+        result = sqlserver_pomes._connect(errors=op_errors,
+                                          logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -182,16 +185,16 @@
     If more than one, the attributes are concatenated by the *AND* logical connector.
     The targer database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param table: the table to be searched
     :param where_attrs: the search attributes
     :param where_vals: the values for the search attributes
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: True if at least one tuple was found
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     # noinspection PyDataSource
@@ -228,16 +231,16 @@
     in a specific tuple. In case of error, or if the search is empty, *None* is returned.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: values to be associated with the search criteria
     :param require_nonempty: defines whether an empty search should be considered an error
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     require_min: int = 1 if require_nonempty else None
@@ -274,16 +277,16 @@
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # initialize the local errors list
@@ -291,39 +294,39 @@
 
     curr_engine: str = _assert_engine(errors=op_errors,
                                       engine=engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_select_all(errors=op_errors,
+        result = oracle_pomes._select_all(errors=op_errors,
+                                          sel_stmt=sel_stmt,
+                                          where_vals=where_vals,
+                                          require_min=require_min,
+                                          require_max=require_max,
+                                          conn=conn,
+                                          logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes._select_all(errors=op_errors,
                                             sel_stmt=sel_stmt,
                                             where_vals=where_vals,
                                             require_min=require_min,
                                             require_max=require_max,
                                             conn=conn,
                                             logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_select_all(errors=op_errors,
-                                              sel_stmt=sel_stmt,
-                                              where_vals=where_vals,
-                                              require_min=require_min,
-                                              require_max=require_max,
-                                              conn=conn,
-                                              logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_select_all(errors=op_errors,
-                                               sel_stmt=sel_stmt,
-                                               where_vals=where_vals,
-                                               require_min=require_min,
-                                               require_max=require_max,
-                                               conn=conn,
-                                               logger=logger)
+        result = sqlserver_pomes._select_all(errors=op_errors,
+                                             sel_stmt=sel_stmt,
+                                             where_vals=where_vals,
+                                             require_min=require_min,
+                                             require_max=require_max,
+                                             conn=conn,
+                                             logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -337,16 +340,16 @@
     Insert a tuple, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the values to be inserted
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of inserted tuples (0 ou 1), or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
@@ -376,16 +379,16 @@
     The values for selecting the tuples to be updated are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param update_stmt: the UPDATE command
     :param update_vals: the values for the update operation
     :param where_vals: the values to be associated with the search criteria
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of updated tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     bind_vals: tuple | None = None
@@ -419,16 +422,16 @@
 
     The values for selecting the tuples to be deleted are in *where_vals*.
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param delete_stmt: the DELETE command
     :param where_vals: the values to be associated with the search criteria
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of deleted tuples, or None if an error occurred
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     result: int = db_execute(errors=op_errors,
@@ -454,49 +457,49 @@
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_bulk_insert(errors=op_errors,
+        result = oracle_pomes._bulk_insert(errors=op_errors,
+                                           insert_stmt=insert_stmt,
+                                           insert_vals=insert_vals,
+                                           conn=conn,
+                                           logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes._bulk_insert(errors=op_errors,
                                              insert_stmt=insert_stmt,
                                              insert_vals=insert_vals,
                                              conn=conn,
                                              logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_bulk_insert(errors=op_errors,
-                                               insert_stmt=insert_stmt,
-                                               insert_vals=insert_vals,
-                                               conn=conn,
-                                               logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_bulk_insert(errors=op_errors,
-                                                insert_stmt=insert_stmt,
-                                                insert_vals=insert_vals,
-                                                conn=conn,
-                                                logger=logger)
+        result = sqlserver_pomes._bulk_insert(errors=op_errors,
+                                              insert_stmt=insert_stmt,
+                                              insert_vals=insert_vals,
+                                              conn=conn,
+                                              logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -516,58 +519,58 @@
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: number of LOBs effectively copied
     """
     # initialize the local errors list
     op_errors: list[str] = []
 
     curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        oracle_pomes.db_update_lob(errors=op_errors,
+        oracle_pomes._update_lob(errors=op_errors,
+                                 lob_table=lob_table,
+                                 lob_column=lob_column,
+                                 pk_columns=pk_columns,
+                                 pk_vals=pk_vals,
+                                 lob_file=lob_file,
+                                 chunk_size=chunk_size,
+                                 conn=conn,
+                                 logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        postgres_pomes._update_lob(errors=op_errors,
                                    lob_table=lob_table,
                                    lob_column=lob_column,
                                    pk_columns=pk_columns,
                                    pk_vals=pk_vals,
                                    lob_file=lob_file,
                                    chunk_size=chunk_size,
                                    conn=conn,
                                    logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        postgres_pomes.db_update_lob(errors=op_errors,
-                                     lob_table=lob_table,
-                                     lob_column=lob_column,
-                                     pk_columns=pk_columns,
-                                     pk_vals=pk_vals,
-                                     lob_file=lob_file,
-                                     chunk_size=chunk_size,
-                                     conn=conn,
-                                     logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        sqlserver_pomes.db_update_lob(errors=op_errors,
-                                      lob_table=lob_table,
-                                      lob_column=lob_column,
-                                      pk_columns=pk_columns,
-                                      pk_vals=pk_vals,
-                                      lob_file=lob_file,
-                                      chunk_size=chunk_size,
-                                      conn=conn,
-                                      logger=logger)
+        sqlserver_pomes._update_lob(errors=op_errors,
+                                    lob_table=lob_table,
+                                    lob_column=lob_column,
+                                    pk_columns=pk_columns,
+                                    pk_vals=pk_vals,
+                                    lob_file=lob_file,
+                                    chunk_size=chunk_size,
+                                    conn=conn,
+                                    logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
 
 def db_execute(errors: list[str] | None,
                exc_stmt: str,
@@ -585,49 +588,49 @@
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_execute(errors=op_errors,
-                                         exc_stmt=exc_stmt,
-                                         bind_vals=bind_vals,
-                                         conn=conn,
-                                         logger=logger)
+        result = oracle_pomes._execute(errors=op_errors,
+                                       exc_stmt=exc_stmt,
+                                       bind_vals=bind_vals,
+                                       conn=conn,
+                                       logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
         result = postgres_pomes.db_execute(errors=op_errors,
                                            exc_stmt=exc_stmt,
                                            bind_vals=bind_vals,
                                            conn=conn,
                                            logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_execute(errors=op_errors,
-                                            exc_stmt=exc_stmt,
-                                            bind_vals=bind_vals,
-                                            conn=conn,
-                                            logger=logger)
+        result = sqlserver_pomes._execute(errors=op_errors,
+                                          exc_stmt=exc_stmt,
+                                          bind_vals=bind_vals,
+                                          conn=conn,
+                                          logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -641,49 +644,49 @@
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_call_function(errors=op_errors,
-                                               func_name=func_name,
-                                               func_vals=func_vals,
-                                               conn=conn,
-                                               logger=logger)
+        result = oracle_pomes._call_function(errors=op_errors,
+                                             func_name=func_name,
+                                             func_vals=func_vals,
+                                             conn=conn,
+                                             logger=logger)
     elif curr_engine == "postgres":
         from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors=op_errors,
-                                                  proc_name=func_name,
-                                                  proc_vals=func_vals,
-                                                  conn=conn,
-                                                  logger=logger)
+        result = postgres_pomes._call_procedure(errors=op_errors,
+                                                proc_name=func_name,
+                                                proc_vals=func_vals,
+                                                conn=conn,
+                                                logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors=op_errors,
-                                                   proc_name=func_name,
-                                                   proc_vals=func_vals,
-                                                   conn=conn,
-                                                   logger=logger)
+        result = sqlserver_pomes._call_procedure(errors=op_errors,
+                                                 proc_name=func_name,
+                                                 proc_vals=func_vals,
+                                                 conn=conn,
+                                                 logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
 
 
@@ -697,47 +700,47 @@
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     The target database engine, default or specified, must have been previously configured.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
-    :param engine: the database engine to use (uses the default engine, if not specified)
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param engine: the database engine to use (uses the default engine, if not provided)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: Any = None
 
     # initialize the local errors list
     op_errors: list[str] = []
 
     curr_engine: str = _assert_engine(op_errors, engine)
     if curr_engine == "mysql":
         pass
     elif curr_engine == "oracle":
         from . import oracle_pomes
-        result = oracle_pomes.db_call_procedure(errors=op_errors,
+        result = oracle_pomes._call_procedure(errors=op_errors,
+                                              proc_name=proc_name,
+                                              proc_vals=proc_vals,
+                                              conn=conn,
+                                              logger=logger)
+    elif curr_engine == "postgres":
+        from . import postgres_pomes
+        result = postgres_pomes._call_procedure(errors=op_errors,
                                                 proc_name=proc_name,
                                                 proc_vals=proc_vals,
                                                 conn=conn,
                                                 logger=logger)
-    elif curr_engine == "postgres":
-        from . import postgres_pomes
-        result = postgres_pomes.db_call_procedure(errors=op_errors,
-                                                  proc_name=proc_name,
-                                                  proc_vals=proc_vals,
-                                                  conn=conn,
-                                                  logger=logger)
     elif curr_engine == "sqlserver":
         from . import sqlserver_pomes
-        result = sqlserver_pomes.db_call_procedure(errors=op_errors,
-                                                   proc_name=proc_name,
-                                                   proc_vals=proc_vals,
-                                                   conn=conn,
-                                                   logger=logger)
+        result = sqlserver_pomes._call_procedure(errors=op_errors,
+                                                 proc_name=proc_name,
+                                                 proc_vals=proc_vals,
+                                                 conn=conn,
+                                                 logger=logger)
 
     # acknowledge eventual local errors
     errors.extend(op_errors)
 
     return result
```

### Comparing `pypomes_db-0.8.3/src/pypomes_db/migration_pomes.py` & `pypomes_db-0.8.4/src/pypomes_db/migration_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     :param errors: incidental error messages
     :param source_engine: the source database engine type
     :param source_table: the origin table
     :param source_columns: the colums to be migrated
     :param target_engine: the destination database engine type
     :param target_table: the table to write the data to (defaults to the source table)
     :param target_columns: the columns to write the data to (defaults to the source columns)
-    :param source_conn: the connection to the source database (obtains a new one, if not specified)
-    :param target_conn: the connection to the destination database (obtains a new one, if not specified)
+    :param source_conn: the connection to the source database (obtains a new one, if not provided)
+    :param target_conn: the connection to the destination database (obtains a new one, if not provided)
     :param where_clause: the criteria for tuple selection
     :param batch_size: the maximum number of tuples to migrate in each batch, or 0 or None for no limit
     :param logger: optional logger
     :return: the number of tuples effectively migrated
     """
     # initialize the return variable
     result: int = 0
@@ -227,16 +227,16 @@
     :param source_table: the table holding the LOBs
     :param source_lob_column: the column holding the LOB
     :param source_pk_columns: columns making up a primary key, or a unique identifier for a tuple, in source database
     :param target_engine: the destination database engine type
     :param target_table: the table to write the lob to (defaults to the source table)
     :param target_lob_column: the column to write the lob to (defaults to the source column)
     :param target_pk_columns: columns making up a primary key, or a unique identifier for a tuple, in target database
-    :param source_conn: the connection to the source database (obtains a new one, if not specified)
-    :param target_conn: the connection to the destination database (obtains a new one, if not specified)
+    :param source_conn: the connection to the source database (obtains a new one, if not provided)
+    :param target_conn: the connection to the destination database (obtains a new one, if not provided)
     :param where_clause: the criteria for tuple selection
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
     :param logger: optional logger
     :return: the number of LOBs effectively migrated
     """
     # initialize the return variable
     result: int = 0
```

### Comparing `pypomes_db-0.8.3/src/pypomes_db/oracle_pomes.py` & `pypomes_db-0.8.4/src/pypomes_db/oracle_pomes.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from .db_common import (
     _DB_CONN_DATA,
     _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
-def db_connect(errors: list[str],
-               logger: Logger) -> Connection:
+def _connect(errors: list[str],
+             logger: Logger) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -44,44 +44,44 @@
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_all(errors: list[str],
-                  sel_stmt: str,
-                  where_vals: tuple,
-                  require_min: int,
-                  require_max: int,
-                  conn: Connection,
-                  logger: Logger) -> list[tuple]:
+def _select_all(errors: list[str],
+                sel_stmt: str,
+                where_vals: tuple,
+                require_min: int,
+                require_max: int,
+                conn: Connection,
+                logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = f"{sel_stmt} FETCH NEXT {require_max} ROWS ONLY"
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
@@ -123,39 +123,39 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str],
-                   insert_stmt: str,
-                   insert_vals: list[tuple],
-                   conn: Connection,
-                   logger: Logger) -> int:
+def _bulk_insert(errors: list[str],
+                 insert_stmt: str,
+                 insert_vals: list[tuple],
+                 conn: Connection,
+                 logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The binding must be done by position. Thus, the *VALUES* clause in *insert_stmt*
     must contain as many ':n' placeholders as there are elements in the tuples found in the
     list provided in *insert_vals*, where 'n' is the 1-based position of the data in the tuple.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.executemany(statement=insert_stmt,
                                parameters=insert_vals)
@@ -179,39 +179,39 @@
                 errors=errors,
                 stmt=insert_stmt,
                 bind_vals=insert_vals[0])
 
     return result
 
 
-def db_update_lob(errors: list[str],
-                  lob_table: str,
-                  lob_column: str,
-                  pk_columns: list[str],
-                  pk_vals: tuple,
-                  lob_file: str | Path,
-                  chunk_size: int,
-                  conn: Connection,
-                  logger: Logger) -> None:
+def _update_lob(errors: list[str],
+                lob_table: str,
+                lob_column: str,
+                pk_columns: list[str],
+                pk_vals: tuple,
+                lob_file: str | Path,
+                chunk_size: int,
+                conn: Connection,
+                logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
@@ -256,43 +256,43 @@
                 err_msg=err_msg,
                 engine="oracle",
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def db_execute(errors: list[str],
-               exc_stmt: str,
-               bind_vals: tuple,
-               conn: Connection,
-               logger: Logger) -> int:
+def _execute(errors: list[str],
+             exc_stmt: str,
+             bind_vals: tuple,
+             conn: Connection,
+             logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
     The optional bind values for this operation are in *bind_vals*.
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(statement=exc_stmt,
                            parameters=bind_vals)
@@ -319,57 +319,57 @@
                 bind_vals=bind_vals)
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
 # noinspection PyUnusedLocal
-def db_call_function(errors: list[str],
-                     func_name: str,
-                     func_vals: tuple,
-                     conn: Connection,
-                     logger: Logger) -> list[tuple]:
+def _call_function(errors: list[str],
+                   func_name: str,
+                   func_vals: tuple,
+                   conn: Connection,
+                   logger: Logger) -> list[tuple]:
     """
     Execute the stored function *func_name* in the database, with the parameters given in *func_vals*.
 
     :param errors: incidental error messages
     :param func_name: name of the stored function
     :param func_vals: parameters for the stored function
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the function
     """
     # initialize the return variable
     result: list[tuple] = []
 
     return result
 
 
 # TODO: see https://python-oracledb.readthedocs.io/en/latest/user_guide/plsql_execution.html
-def db_call_procedure(errors: list[str],
-                      proc_name: str,
-                      proc_vals: tuple,
-                      conn: Connection,
-                      logger: Logger) -> list[tuple]:
+def _call_procedure(errors: list[str],
+                    proc_name: str,
+                    proc_vals: tuple,
+                    conn: Connection,
+                    logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.callproc(name=proc_name,
@@ -398,16 +398,16 @@
                 stmt=proc_name,
                 bind_vals=proc_vals)
 
     return result
 
 __is_initialized: str | None = None
 
-def initialize(errors: list[str],
-               logger: Logger) -> bool:
+def _initialize(errors: list[str],
+                logger: Logger) -> bool:
     """
     Prepare the oracle engine to access the database throught the installed client software.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: False if an error happened, True otherwise
     """
```

### Comparing `pypomes_db-0.8.3/src/pypomes_db/postgres_pomes.py` & `pypomes_db-0.8.4/src/pypomes_db/postgres_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from .db_common import (
     _db_assert_query_quota, _db_get_params,
     _db_log, _db_except_msg, _db_remove_nulls
 )
 
 
-def db_connect(errors: list[str],
-               logger: Logger = None) -> connection:
+def _connect(errors: list[str],
+             logger: Logger = None) -> connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -47,44 +47,44 @@
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_all(errors: list[str],
-                  sel_stmt: str,
-                  where_vals: tuple,
-                  require_min: int,
-                  require_max: int,
-                  conn: connection,
-                  logger: Logger) -> list[tuple]:
+def _select_all(errors: list[str],
+                sel_stmt: str,
+                where_vals: tuple,
+                require_min: int,
+                require_max: int,
+                conn: connection,
+                logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: list of tuples containing the search result, or [] if the search is empty
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     if isinstance(require_max, int) and require_max >= 0:
         sel_stmt += f" LIMIT {require_max}"
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
@@ -125,39 +125,39 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str],
-                   insert_stmt: str,
-                   insert_vals: list[tuple],
-                   conn: connection,
-                   logger: Logger) -> int:
+def _bulk_insert(errors: list[str],
+                 insert_stmt: str,
+                 insert_vals: list[tuple],
+                 conn: connection,
+                 logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must be simply *VALUES %s*.
     Note that, after the execution of *execute_values*, the *cursor.rowcount* property
     will not contain a total result, and thus the value 1 (one) is returned on success.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # execute the bulk insert
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             execute_values(cur=cursor,
@@ -183,19 +183,19 @@
                 if cleaned_row:
                     # yes, register it
                     cleaned_rows.append((inx, cleaned_row))
             # replace the cleaned rows
             for cleaned_row in cleaned_rows:
                 insert_vals[cleaned_row[0]] = tuple(cleaned_row[1])
             # bulk insert the cleaned data
-            db_bulk_insert(errors=errors,
-                           insert_stmt=insert_stmt,
-                           insert_vals=insert_vals,
-                           conn=conn,
-                           logger=logger)
+            _bulk_insert(errors=errors,
+                         insert_stmt=insert_stmt,
+                         insert_vals=insert_vals,
+                         conn=conn,
+                         logger=logger)
     except Exception as e:
         if curr_conn:
             curr_conn.rollback()
         err_msg = _db_except_msg(exception=e,
                                  engine="postgres")
     finally:
         # close the connection, if locally acquired
@@ -209,39 +209,39 @@
                 err_msg=err_msg,
                 errors=errors,
                 stmt=insert_stmt)
 
     return result
 
 
-def db_update_lob(errors: list[str],
-                  lob_table: str,
-                  lob_column: str,
-                  pk_columns: list[str],
-                  pk_vals: tuple,
-                  lob_file: str | Path,
-                  chunk_size: int,
-                  conn: connection,
-                  logger: Logger) -> None:
+def _update_lob(errors: list[str],
+                lob_table: str,
+                lob_column: str,
+                pk_columns: list[str],
+                pk_vals: tuple,
+                lob_file: str | Path,
+                chunk_size: int,
+                conn: connection,
+                logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
@@ -302,24 +302,24 @@
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(query=f"{exc_stmt};",
                            vars=bind_vals)
@@ -345,35 +345,35 @@
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
 
-def db_call_procedure(errors: list[str],
-                      proc_name: str,
-                      proc_vals: tuple,
-                      conn: connection,
-                      logger: Logger) -> list[tuple]:
+def _call_procedure(errors: list[str],
+                    proc_name: str,
+                    proc_vals: tuple,
+                    conn: connection,
+                    logger: Logger) -> list[tuple]:
     """
     Execute the stored procedure *proc_name*, with the arguments given in *proc_vals*.
 
     :param errors:  incidental error messages
     :param proc_name: the name of the sotred procedure
     :param proc_vals: the arguments to be passed
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] = [()]
 
     # make sure to have a connection
-    curr_conn: connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # build the command
     proc_stmt: str = f"{proc_name}(" + "%s, " * (len(proc_vals) - 1) + "%s)"
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
```

### Comparing `pypomes_db-0.8.3/src/pypomes_db/sqlserver_pomes.py` & `pypomes_db-0.8.4/src/pypomes_db/sqlserver_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from pathlib import Path
 
 from .db_common import (
     _db_assert_query_quota, _db_get_params, _db_log, _db_except_msg
 )
 
 
-def db_connect(errors: list[str],
-               logger: Logger = None) -> Connection:
+def _connect(errors: list[str],
+             logger: Logger = None) -> Connection:
     """
     Obtain and return a connection to the database, or *None* if the connection could not be obtained.
 
     :param errors: incidental error messages
     :param logger: optional logger
     :return: the connection to the database
     """
@@ -43,44 +43,44 @@
             err_msg=err_msg,
             errors=errors,
             stmt=f"Connecting to '{name}' at '{host}'")
 
     return result
 
 
-def db_select_all(errors: list[str],
-                  sel_stmt: str,
-                  where_vals: tuple,
-                  require_min: int,
-                  require_max: int,
-                  conn: Connection,
-                  logger: Logger) -> list[tuple]:
+def _select_all(errors: list[str],
+                sel_stmt: str,
+                where_vals: tuple,
+                require_min: int,
+                require_max: int,
+                conn: Connection,
+                logger: Logger) -> list[tuple]:
     """
     Search the database and return all tuples that satisfy the *sel_stmt* search command.
 
     The command can optionally contain search criteria, with respective values given
     in *where_vals*. The list of values for an attribute with the *IN* clause must be contained
     in a specific tuple. If not positive integers, *require_min* and *require_max* are ignored.
     If the search is empty, an empty list is returned.
 
     :param errors: incidental error messages
     :param sel_stmt: SELECT command for the search
     :param where_vals: the values to be associated with the search criteria
     :param require_min: optionally defines the minimum number of tuples to be returned
     :param require_max: optionally defines the maximum number of tuples to be returned
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: tuple containing the search result, [] if the search was empty, or None if there was an error
     """
     # initialize the return variable
     result: list[tuple] = []
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     err_msg: str | None = None
     if isinstance(require_max, int) and require_max > 0:
         sel_stmt: str = sel_stmt.replace("SELECT", f"SELECT TOP {require_max}", 1)
 
     try:
         # obtain a cursor and execute the operation
@@ -120,38 +120,38 @@
                 errors=errors,
                 stmt=sel_stmt,
                 bind_vals=where_vals)
 
     return result
 
 
-def db_bulk_insert(errors: list[str],
-                   insert_stmt: str,
-                   insert_vals: list[tuple],
-                   conn: Connection,
-                   logger: Logger) -> int:
+def _bulk_insert(errors: list[str],
+                 insert_stmt: str,
+                 insert_vals: list[tuple],
+                 conn: Connection,
+                 logger: Logger) -> int:
     """
     Insert the tuples, with values defined in *insert_vals*, into the database.
 
     The *VALUES* clause in *insert_stmt* must contain as many '%s' placeholders
     as there are elements in the tuples found in the list provided in *insert_vals*.
 
     :param errors: incidental error messages
     :param insert_stmt: the INSERT command
     :param insert_vals: the list of values to be inserted
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the number of inserted tuples, or None if an error occurred
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and perform the operation
         with curr_conn.cursor() as cursor:
             cursor.fast_executemany = True
             try:
@@ -179,39 +179,39 @@
                 errors=errors,
                 stmt=insert_stmt,
                 bind_vals=insert_vals[0])
 
     return result
 
 
-def db_update_lob(errors: list[str],
-                  lob_table: str,
-                  lob_column: str,
-                  pk_columns: list[str],
-                  pk_vals: tuple,
-                  lob_file: str | Path,
-                  chunk_size: int,
-                  conn: Connection,
-                  logger: Logger) -> None:
+def _update_lob(errors: list[str],
+                lob_table: str,
+                lob_column: str,
+                pk_columns: list[str],
+                pk_vals: tuple,
+                lob_file: str | Path,
+                chunk_size: int,
+                conn: Connection,
+                logger: Logger) -> None:
     """
     Update a large binary objects (LOB) in the given table and column.
 
     :param errors: incidental error messages
     :param lob_table: the table to be update with the new LOB
     :param lob_column: the column to be updated with the new LOB
     :param pk_columns: columns making up a primary key, or a unique identifier for the tuple
     :param pk_vals: values with which to locate the tuple to be updated
     :param lob_file: file holding the LOB (a file object or a valid path)
     :param chunk_size: size in bytes of the data chunk to read/write, or 0 or None for no limit
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     """
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # make sure to have a data file
     data_file: Path = Path(lob_file) if isinstance(lob_file, str) else lob_file
 
     # normalize the chunk size
     if not chunk_size:
         chunk_size = -1
@@ -253,43 +253,43 @@
                 engine="sqlserver",
                 err_msg=err_msg,
                 errors=errors,
                 stmt=update_stmt,
                 bind_vals=pk_vals)
 
 
-def db_execute(errors: list[str],
-               exc_stmt: str,
-               bind_vals: tuple,
-               conn: Connection,
-               logger: Logger) -> int:
+def _execute(errors: list[str],
+             exc_stmt: str,
+             bind_vals: tuple,
+             conn: Connection,
+             logger: Logger) -> int:
     """
     Execute the command *exc_stmt* on the database.
 
     This command might be a DML ccommand modifying the database, such as
     inserting, updating or deleting tuples, or it might be a DDL statement,
     or it might even be an environment-related command.
     The optional bind values for this operation are in *bind_vals*.
     The value returned is the value obtained from the execution of *exc_stmt*.
     It might be the number of inserted, modified, or deleted tuples,
     ou None if an error occurred.
 
     :param errors: incidental error messages
     :param exc_stmt: the command to execute
     :param bind_vals: optional bind values
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the return value from the command execution
     """
     # initialize the return variable
     result: int | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     err_msg: str | None = None
     try:
         # obtain a cursor and execute the operation
         with curr_conn.cursor() as cursor:
             cursor.execute(exc_stmt, bind_vals)
             result = cursor.rowcount
@@ -313,35 +313,35 @@
                 errors=errors,
                 stmt=exc_stmt,
                 bind_vals=bind_vals)
 
     return result
 
 
-def db_call_procedure(errors: list[str],
-                      proc_name: str,
-                      proc_vals: tuple,
-                      conn: Connection,
-                      logger: Logger = None) -> list[tuple]:
+def _call_procedure(errors: list[str],
+                    proc_name: str,
+                    proc_vals: tuple,
+                    conn: Connection,
+                    logger: Logger = None) -> list[tuple]:
     """
     Execute the stored procedure *proc_name* in the database, with the parameters given in *proc_vals*.
 
     :param errors: incidental error messages
     :param proc_name: name of the stored procedure
     :param proc_vals: parameters for the stored procedure
-    :param conn: optional connection to use (obtains a new one, if not specified)
+    :param conn: optional connection to use (obtains a new one, if not provided)
     :param logger: optional logger
     :return: the data returned by the procedure
     """
     # initialize the return variable
     result: list[tuple] | None = None
 
     # make sure to have a connection
-    curr_conn: Connection = conn or db_connect(errors=errors,
-                                               logger=logger)
+    curr_conn: Connection = conn or _connect(errors=errors,
+                                             logger=logger)
 
     # build the command
     proc_stmt: str | None = None
 
     # execute the stored procedure
     err_msg: str | None = None
     try:
```

### Comparing `pypomes_db-0.8.3/LICENSE` & `pypomes_db-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_db-0.8.3/pyproject.toml` & `pypomes_db-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_db"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (database modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_db-0.8.3/PKG-INFO` & `pypomes_db-0.8.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_db
-Version: 0.8.3
+Version: 0.8.4
 Summary: A collection of Python pomes, pennyeach (database modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-DB
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-DB/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

