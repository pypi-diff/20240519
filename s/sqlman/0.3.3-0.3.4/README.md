# Comparing `tmp/sqlman-0.3.3.tar.gz` & `tmp/sqlman-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlman-0.3.3.tar", last modified: Fri May 17 16:37:32 2024, max compression
+gzip compressed data, was "sqlman-0.3.4.tar", last modified: Sun May 19 04:23:12 2024, max compression
```

## Comparing `sqlman-0.3.3.tar` & `sqlman-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.740825 sqlman-0.3.3/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3982 2024-05-17 16:37:32.740593 sqlman-0.3.3/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)     3694 2024-05-17 16:37:22.000000 sqlman-0.3.3/README.md
--rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-17 16:37:32.740862 sqlman-0.3.3/setup.cfg
--rw-r--r--   0 wangtuo    (501) staff       (20)      645 2024-05-17 16:37:22.000000 sqlman-0.3.3/setup.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.738690 sqlman-0.3.3/sqlman/
--rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3.3/sqlman/__init__.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     6732 2024-05-17 16:36:11.000000 sqlman-0.3.3/sqlman/handler.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     9514 2024-05-16 11:47:03.000000 sqlman-0.3.3/sqlman/table_controller.py
--rw-r--r--   0 wangtuo    (501) staff       (20)     1362 2024-04-21 12:47:57.000000 sqlman-0.3.3/sqlman/tools.py
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.740113 sqlman-0.3.3/sqlman.egg-info/
--rw-r--r--   0 wangtuo    (501) staff       (20)     3982 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/PKG-INFO
--rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/SOURCES.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/dependency_links.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/not-zip-safe
--rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/requires.txt
--rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-17 16:37:32.000000 sqlman-0.3.3/sqlman.egg-info/top_level.txt
-drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-17 16:37:32.740254 sqlman-0.3.3/tests/
--rw-r--r--   0 wangtuo    (501) staff       (20)      371 2024-05-17 16:30:01.000000 sqlman-0.3.3/tests/test-0.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-19 04:23:12.240802 sqlman-0.3.4/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3982 2024-05-19 04:23:12.240561 sqlman-0.3.4/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3694 2024-05-17 16:37:22.000000 sqlman-0.3.4/README.md
+-rw-r--r--   0 wangtuo    (501) staff       (20)       38 2024-05-19 04:23:12.240841 sqlman-0.3.4/setup.cfg
+-rw-r--r--   0 wangtuo    (501) staff       (20)      645 2024-05-19 04:23:03.000000 sqlman-0.3.4/setup.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-19 04:23:12.239272 sqlman-0.3.4/sqlman/
+-rw-r--r--   0 wangtuo    (501) staff       (20)       60 2024-04-17 16:06:46.000000 sqlman-0.3.4/sqlman/__init__.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     6289 2024-05-19 04:18:09.000000 sqlman-0.3.4/sqlman/handler.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     9549 2024-05-19 04:18:09.000000 sqlman-0.3.4/sqlman/table_controller.py
+-rw-r--r--   0 wangtuo    (501) staff       (20)     1649 2024-05-19 03:55:46.000000 sqlman-0.3.4/sqlman/tools.py
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-19 04:23:12.240099 sqlman-0.3.4/sqlman.egg-info/
+-rw-r--r--   0 wangtuo    (501) staff       (20)     3982 2024-05-19 04:23:12.000000 sqlman-0.3.4/sqlman.egg-info/PKG-INFO
+-rw-r--r--   0 wangtuo    (501) staff       (20)      292 2024-05-19 04:23:12.000000 sqlman-0.3.4/sqlman.egg-info/SOURCES.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-19 04:23:12.000000 sqlman-0.3.4/sqlman.egg-info/dependency_links.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        1 2024-05-19 04:23:12.000000 sqlman-0.3.4/sqlman.egg-info/not-zip-safe
+-rw-r--r--   0 wangtuo    (501) staff       (20)       29 2024-05-19 04:23:12.000000 sqlman-0.3.4/sqlman.egg-info/requires.txt
+-rw-r--r--   0 wangtuo    (501) staff       (20)        7 2024-05-19 04:23:12.000000 sqlman-0.3.4/sqlman.egg-info/top_level.txt
+drwxr-xr-x   0 wangtuo    (501) staff       (20)        0 2024-05-19 04:23:12.240203 sqlman-0.3.4/tests/
+-rw-r--r--   0 wangtuo    (501) staff       (20)      371 2024-05-17 16:30:01.000000 sqlman-0.3.4/tests/test-0.py
```

### Comparing `sqlman-0.3.3/PKG-INFO` & `sqlman-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.3.3
+Version: 0.3.4
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
```

### Comparing `sqlman-0.3.3/README.md` & `sqlman-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlman-0.3.3/setup.py` & `sqlman-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='sqlman',
-    version='0.3.3',
+    version='0.3.4',
     description='告别SQL语句，python操作mysql的贴心助手',
     url='https://github.com/markadc/sqlman',
     author='WangTuo',
     author_email='markadc@126.com',
     packages=find_packages(),
     license='MIT',
     zip_safe=False,
```

### Comparing `sqlman-0.3.3/sqlman/handler.py` & `sqlman-0.3.4/sqlman/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 class Handler:
     def __init__(self, cfg):
         cfg.setdefault('host', 'localhost')
         cfg.setdefault('port', 3306)
         cfg.setdefault('charset', 'utf8mb4')
         cfg.setdefault('maxconnections', 4)
         cfg.setdefault('blocking', True)
-        self.__cfg = cfg
-        self.__pool = PooledDB(pymysql, **self.__cfg)
+        self._cfg = cfg
+        self._pool = PooledDB(pymysql, **self._cfg)
 
     def __getitem__(self, table: str):
         from sqlman.table_controller import TableController
-        return TableController(self.__cfg, table)
+        return TableController(self._cfg, table)
 
     def pick_table(self, name: str):
         return self.__getitem__(name)
 
     @staticmethod
     def panic(sql, msg):
         """错误日志"""
@@ -36,87 +36,68 @@
             sql     {}
             msg     {}
             """.format(sql, msg)
         )
 
     def open_connect(self, dict_cursor=False):
         """打开连接"""
-        con = self.__pool.connection()
+        con = self._pool.connection()
         cur = con.cursor(DictCursor) if dict_cursor else con.cursor()
         return cur, con
 
     def close_connect(self, cur, con):
         """关闭连接"""
         if cur:
             cur.close()
         if con:
             con.close()
 
-    def exe_sql(self, sql: str, args=None, mode=0, dict_cursor=True) -> dict:
+    def exe_sql(self, sql: str, args=None, get_all=None, dict_cursor=True) -> dict:
         """执行SQL"""
         cur, con = None, None
         try:
             cur, con = self.open_connect(dict_cursor)
             line = cur.execute(sql, args=args)
             con.commit()
-            query_results = None if mode == 0 else list(cur.fetchall()) if mode > 1 else cur.fetchone()
-            return build_result(status=1, affect=line, query=query_results)
-
         except Exception as e:
             self.panic(sql, e)
-            if con:
-                con.rollback()
             return build_result(status=0, error=str(e))
-
+        else:
+            query_results = None if get_all is None else list(cur.fetchall()) if get_all else cur.fetchone()
+            return build_result(status=1, affect=line, data=query_results)
         finally:
             self.close_connect(cur, con)
 
     def exem_sql(self, sql: str, args=None) -> int:
         """批量执行SQL"""
         cur, con = None, None
         try:
             cur, con = self.open_connect()
             line = cur.executemany(sql, args=args)
             con.commit()
             return line
-
         except Exception as e:
             self.panic(sql, e)
-            if con:
-                con.rollback()
             return 0
-
         finally:
             self.close_connect(cur, con)
 
-    @staticmethod
-    def _getfv(data: dict | list) -> tuple:
-        item = data if isinstance(data, dict) else data[0]
-        fs = []
-        vs = []
-        for k in item.keys():
-            fs.append('`{}`'.format(k))
-            vs.append('%s')
-        fileds = ', '.join(fs)
-        values = ', '.join(vs)
-        return fileds, values
-
     def _insert_one(self, table: str, item: dict, update: str = None, unique_index: str = None) -> int:
         """
         插入数据
         Args:
             table: 表
             item: 数据
             update: 数据重复，则更新数据
             unique_index: 唯一索引
 
         Returns:
             受影响的行数
         """
-        fields, values = self._getfv(item)
+        fields, values = getfv(item)
         new = '' if not (update or unique_index) else 'ON DUPLICATE KEY UPDATE {}'.format(
             update or '{}={}'.format(unique_index, unique_index)
         )
         sql = 'insert into {}({}) value({}) {}'.format(table, fields, values, new)
         affect = self.exe_sql(sql, args=tuple(item.values()))['affect']
         return affect
 
@@ -128,15 +109,15 @@
             items: 数据
             update: 数据重复，则更新数据
             unique_index: 唯一索引
 
         Returns:
             受影响的行数
         """
-        fields, values = self._getfv(items)
+        fields, values = getfv(items)
         new = '' if not (update or unique_index) else 'ON DUPLICATE KEY UPDATE {}'.format(
             update or '{}={}'.format(unique_index, unique_index)
         )
         sql = 'insert into {}({}) value({}) {}'.format(table, fields, values, new)
         affect = self.exem_sql(sql, args=[tuple(item.values()) for item in items])
         return affect
```

### Comparing `sqlman-0.3.3/sqlman/table_controller.py` & `sqlman-0.3.4/sqlman/table_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, cfg: dict, table: str):
         super().__init__(cfg)
         self.table = table
 
     def get_tables(self) -> list:
         """获取当前数据库的所有表"""
         sql = 'show tables'
-        data = self.exe_sql(sql, dict_cursor=False, mode=2)['query']
+        data = self.exe_sql(sql, dict_cursor=False, get_all=True)['data']
         tables = [this[0] for this in data]
         return tables
 
     def kill(self) -> bool:
         """删除这张表"""
         sql = 'DROP TABLE {}'.format(self.table)
         return self.exe_sql(sql)['status'] == 1
@@ -53,39 +53,39 @@
         """查询数据"""
         sql = 'select {} from {} {} {}'.format(
             pick,
             self.table,
             'where {}'.format(make_condition(kwargs)) if kwargs else '',
             '' if limit is None else 'limit {}'.format(limit)
         )
-        data = self.exe_sql(sql, mode=2)['query']
+        data = self.exe_sql(sql, get_all=True)['data']
         return data
 
     def query_count(self, **kwargs) -> int:
         """查询数量"""
         sql = 'select count(1) from {} {}'.format(
             self.table,
             'where {}'.format(make_condition(kwargs)) if kwargs else ''
         )
-        count = self.exe_sql(sql, mode=1)['query']['count(1)']
+        count = self.exe_sql(sql, get_all=False)['data']['count(1)']
         return count
 
     def is_exists(self, **kwargs) -> bool:
         """查询数据是否存在"""
         sql = 'select 1 from {} where {} limit 1'.format(self.table, make_condition(kwargs))
         return self.exe_sql(sql)['affect'] == 1
 
     def random(self, limit=1) -> dict | list:
         """随机返回一条或多条数据"""
         sql = 'select * from {} where id >= (rand() * (select max(id) from {})) limit {}'.format(
             self.table,
             self.table,
             limit
         )
-        data = self.exe_sql(sql, mode=limit)['query']
+        data = self.exe_sql(sql, get_all=limit)['data']
         return data
 
     def update_one(self, item: dict, depend: str) -> int:
         """
         更新数据
         Args:
             item: 数据，且含有<depend>字段
@@ -157,21 +157,21 @@
         sql = '\n'.join([head, mid, tail])
         affect = self.exe_sql(sql, args=args)['affect']
         return affect
 
     def get_min(self, field: str):
         """获取字段的最小值"""
         sql = 'select min({}) from {}'.format(field, self.table)
-        min_value = self.exe_sql(sql, mode=1, dict_cursor=False)['query'][0]
+        min_value = self.exe_sql(sql, get_all=False, dict_cursor=False)['data'][0]
         return min_value
 
     def get_max(self, field: str):
         """获取字段的最大值"""
         sql = 'select max({}) from {}'.format(field, self.table)
-        max_value = self.exe_sql(sql, mode=1, dict_cursor=False)['query'][0]
+        max_value = self.exe_sql(sql, get_all=False, dict_cursor=False)['data'][0]
         return max_value
 
     def scan(
             self, sort_field='id', pick='*',
             start: int = None, end: int = None,
             dealer=None, add_cond=None,
             once=1000, rest=0.05,
@@ -207,15 +207,15 @@
             '''.format(
                 pick, self.table,
                 sort_field, symbol, start, sort_field, end, cond,
                 sort_field,
                 once
             )
 
-            result: list = self.exe_sql(sql, mode=2)['query']
+            result: list = self.exe_sql(sql, get_all=True)['data']
             if not result:
                 self.panic(sql, '查询为空')
                 return
 
             # 输出查询日志
             if log is True:
                 params = sort_field, symbol, start, once, len(result), result[0][sort_field], result[-1][sort_field]
```

### Comparing `sqlman-0.3.3/sqlman/tools.py` & `sqlman-0.3.4/sqlman/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # -*- coding: utf-8 -*-
 
+
+def getfv(data: dict | list) -> tuple:
+    item = data if isinstance(data, dict) else data[0]
+    fs = []
+    vs = []
+    for k in item.keys():
+        fs.append('`{}`'.format(k))
+        vs.append('%s')
+    fileds = ', '.join(fs)
+    values = ', '.join(vs)
+    return fileds, values
+
+
 def get(key: str):
     def outer(func):
         def inner(*args, **kwargs):
             return func(*args, **kwargs).get(key)
 
         return inner
```

### Comparing `sqlman-0.3.3/sqlman.egg-info/PKG-INFO` & `sqlman-0.3.4/sqlman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlman
-Version: 0.3.3
+Version: 0.3.4
 Summary: 告别SQL语句，python操作mysql的贴心助手
 Home-page: https://github.com/markadc/sqlman
 Author: WangTuo
 Author-email: markadc@126.com
 License: MIT
 Keywords: Python,MySQL,Database
 Description-Content-Type: text/markdown
```

