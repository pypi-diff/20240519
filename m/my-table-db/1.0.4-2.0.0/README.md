# Comparing `tmp/my_table_db-1.0.4.tar.gz` & `tmp/my_table_db-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-1.0.4.tar", last modified: Sat May 18 22:54:18 2024, max compression
+gzip compressed data, was "my_table_db-2.0.0.tar", last modified: Sat May 18 23:00:52 2024, max compression
```

## Comparing `my_table_db-1.0.4.tar` & `my_table_db-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 22:54:18.592935 my_table_db-1.0.4/
--rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3941 2024-05-18 22:54:18.591935 my_table_db-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 22:54:18.590933 my_table_db-1.0.4/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     3941 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-18 22:54:18.000000 my_table_db-1.0.4/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1906 2024-05-18 20:22:33.000000 my_table_db-1.0.4/my_table_db.py
--rw-rw-rw-   0        0        0       42 2024-05-18 22:54:18.592935 my_table_db-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-05-18 22:54:14.000000 my_table_db-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:00:52.212201 my_table_db-2.0.0/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3941 2024-05-18 23:00:52.211201 my_table_db-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 23:00:52.211201 my_table_db-2.0.0/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3941 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1906 2024-05-18 23:00:35.000000 my_table_db-2.0.0/my_table_db.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:00:52.212201 my_table_db-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-18 23:00:35.000000 my_table_db-2.0.0/setup.py
```

### Comparing `my_table_db-1.0.4/LICENSE` & `my_table_db-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.4/PKG-INFO` & `my_table_db-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.4
+Version: 2.0.0
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `my_table_db-1.0.4/README.md` & `my_table_db-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `my_table_db-1.0.4/my_table_db.egg-info/PKG-INFO` & `my_table_db-2.0.0/my_table_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 1.0.4
+Version: 2.0.0
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `my_table_db-1.0.4/my_table_db.py` & `my_table_db-2.0.0/my_table_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-__all__ = ['my_table_bd']
-def my_table_bd(name_arg1=None, arg1=None, name_arg2=None, arg2=None, name_arg3=None, arg3=None, arg4=None,
+__all__ = ['my_table_db']
+def my_table_db(name_arg1=None, arg1=None, name_arg2=None, arg2=None, name_arg3=None, arg3=None, arg4=None,
             name_arg4=None, name_arg5=None, arg5=None, name_arg6=None, arg6=None, name_arg7=None, arg7=None):
     if (name_arg1 and name_arg2 and name_arg3 and name_arg4 and name_arg5 and name_arg6 and name_arg7) is not None:
         return (
             f'{name_arg1}:{str(arg1):10}{'|':9}{name_arg2}:{str(arg2):10}{'|':9}{name_arg3}:{str(arg3):10}{'|':9}{arg4}:{str(name_arg4):10}{'|':9}{arg5}:{str(name_arg5):10}{'|':9}{arg6}:{str(name_arg6):10}{'|':9}{arg7}:{str(name_arg7):10}')
     elif (name_arg1 and name_arg2 and name_arg3 and name_arg4 and name_arg5 and name_arg6) is not None:
         return (
             f'{name_arg1}:{str(arg1):10}{'|':9}{name_arg2}:{str(arg2):10}{'|':9}{name_arg3}:{str(arg3):10}{'|':9}{arg4}:{str(name_arg4):10}{'|':9}{arg5}:{str(name_arg5):10}{'|':9}{arg6}:{str(name_arg6):10}')
```

