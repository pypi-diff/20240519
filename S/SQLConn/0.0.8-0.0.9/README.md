# Comparing `tmp/SQLConn-0.0.8.tar.gz` & `tmp/SQLConn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLConn-0.0.8.tar", last modified: Mon May 13 02:14:36 2024, max compression
+gzip compressed data, was "SQLConn-0.0.9.tar", last modified: Mon May 13 02:17:50 2024, max compression
```

## Comparing `SQLConn-0.0.8.tar` & `SQLConn-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:14:36.890690 SQLConn-0.0.8/
--rw-rw-rw-   0        0        0    10743 2024-05-13 02:14:36.889696 SQLConn-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10235 2024-05-13 02:11:10.000000 SQLConn-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 02:14:36.882692 SQLConn-0.0.8/SQLConn/
--rw-rw-rw-   0        0        0     5583 2024-05-06 10:21:39.000000 SQLConn-0.0.8/SQLConn/SQLConn.py
--rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.8/SQLConn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:14:36.888691 SQLConn-0.0.8/SQLConn.egg-info/
--rw-rw-rw-   0        0        0    10743 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-13 02:14:36.000000 SQLConn-0.0.8/SQLConn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 02:14:36.890690 SQLConn-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      774 2024-05-13 02:14:28.000000 SQLConn-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:50.288817 SQLConn-0.0.9/
+-rw-rw-rw-   0        0        0    10743 2024-05-13 02:17:50.287817 SQLConn-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10235 2024-05-13 02:11:10.000000 SQLConn-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:50.279816 SQLConn-0.0.9/SQLConn/
+-rw-rw-rw-   0        0        0     5810 2024-05-13 02:17:15.000000 SQLConn-0.0.9/SQLConn/SQLConn.py
+-rw-rw-rw-   0        0        0      293 2024-05-06 09:40:40.000000 SQLConn-0.0.9/SQLConn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:17:50.285816 SQLConn-0.0.9/SQLConn.egg-info/
+-rw-rw-rw-   0        0        0    10743 2024-05-13 02:17:50.000000 SQLConn-0.0.9/SQLConn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-05-13 02:17:50.000000 SQLConn-0.0.9/SQLConn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:17:50.000000 SQLConn-0.0.9/SQLConn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-13 02:17:50.000000 SQLConn-0.0.9/SQLConn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 02:17:50.000000 SQLConn-0.0.9/SQLConn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:17:50.289816 SQLConn-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      774 2024-05-13 02:17:33.000000 SQLConn-0.0.9/setup.py
```

### Comparing `SQLConn-0.0.8/PKG-INFO` & `SQLConn-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: sqlalchemy
```

### Comparing `SQLConn-0.0.8/README.md` & `SQLConn-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `SQLConn-0.0.8/SQLConn/SQLConn.py` & `SQLConn-0.0.9/SQLConn/SQLConn.py`

 * *Files 10% similar despite different names*

```diff
@@ -91,26 +91,32 @@
         self.__port=int(port)
         self._conn=pymssql.connect(host=self.__host,user=self.__user,password=self.__password,database=self.__database,port=self.__port)
         
     @property
     def URL(self):
         return f'mssql+pyodbc://{self.__user}:{self.__password}@{self.__host}:{self.__port}/{self.__database}'
 class OracleConn(SQLConn):
-    def __init__(self,password:str,host:str='127.0.0.1',user:str="system",database:str="xe",port:str|int=1521) -> None:
-        super().__init__()
-        self.__host=host
-        self.__user=user
-        self.__password=password
-        self.__database=database
-        self.__port=int(port)
-        self._conn=cx_Oracle.connect(self.__user,self.__password,f'{self.__host}:{self.__port}/{self.__database}')
+    def __init__(self, password: str, host: str = '127.0.0.1', user: str = "system", database: str = "xe", port: str | int = 1521) -> None:
+        try:
+            import cx_Oracle
+        except ImportError:
+            raise ImportError("cx_Oracle is not installed. Please install it using 'pip install SQLConn[oracle]'")
         
+        super().__init__()
+        self.__host = host
+        self.__user = user
+        self.__password = password
+        self.__database = database
+        self.__port = int(port)
+        self._conn = cx_Oracle.connect(self.__user, self.__password, f'{self.__host}:{self.__port}/{self.__database}')
+
     @property
     def URL(self):
         return f'oracle+cx_oracle://{self.__user}:{self.__password}@{self.__host}:{self.__port}/?service_name={self.__database}'
+
 class PostgresqlConn(SQLConn):
     def __init__(self,password:str,host:str='127.0.0.1',user:str="postgres",database:str="postgres",port:str|int=5432) -> None:
         super().__init__()
         self.__host=host
         self.__user=user
         self.__password=password
         self.__database=database
```

### Comparing `SQLConn-0.0.8/SQLConn.egg-info/PKG-INFO` & `SQLConn-0.0.9/SQLConn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLConn
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package facilitates easy SQL database integration.
 Home-page: https://github.com/janyoungjin/SQLConn
 Author: janyoungjin
 Keywords: mysql,postgresql,sqlite,mssql,oracle,sql
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: sqlalchemy
```

### Comparing `SQLConn-0.0.8/setup.py` & `SQLConn-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='SQLConn',
-    version='0.0.8',
+    version='0.0.9',
     description='This package facilitates easy SQL database integration.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='janyoungjin',
     install_requires=[
         'pandas',
         'sqlalchemy',
```

