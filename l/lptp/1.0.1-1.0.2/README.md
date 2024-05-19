# Comparing `tmp/lptp-1.0.1.tar.gz` & `tmp/lptp-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptp-1.0.1.tar", last modified: Sun May 19 19:21:03 2024, max compression
+gzip compressed data, was "lptp-1.0.2.tar", last modified: Sun May 19 19:26:30 2024, max compression
```

## Comparing `lptp-1.0.1.tar` & `lptp-1.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.727985 lptp-1.0.1/
--rw-rw-rw-   0        0        0     1091 2024-03-16 13:37:55.000000 lptp-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2564 2024-05-19 19:21:03.726989 lptp-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1952 2024-05-19 18:38:57.000000 lptp-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-19 19:21:03.729985 lptp-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-05-19 19:21:01.000000 lptp-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.625978 lptp-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.628460 lptp-1.0.1/src/lptp/
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.669068 lptp-1.0.1/src/lptp/client/
--rw-rw-rw-   0        0        0       30 2024-03-16 22:02:51.000000 lptp-1.0.1/src/lptp/client/__init__.py
--rw-rw-rw-   0        0        0     3961 2024-03-24 19:27:55.000000 lptp-1.0.1/src/lptp/client/client.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.676174 lptp-1.0.1/src/lptp/exceptions/
--rw-rw-rw-   0        0        0      151 2024-03-18 17:29:57.000000 lptp-1.0.1/src/lptp/exceptions/__init__.py
--rw-rw-rw-   0        0        0      296 2024-03-17 19:57:15.000000 lptp-1.0.1/src/lptp/exceptions/base.py
--rw-rw-rw-   0        0        0      518 2024-03-24 19:25:54.000000 lptp-1.0.1/src/lptp/exceptions/client.py
--rw-rw-rw-   0        0        0      204 2024-03-17 19:47:57.000000 lptp-1.0.1/src/lptp/exceptions/data.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.687096 lptp-1.0.1/src/lptp/server/
--rw-rw-rw-   0        0        0       94 2024-03-18 20:12:29.000000 lptp-1.0.1/src/lptp/server/__init__.py
--rw-rw-rw-   0        0        0     2263 2024-03-25 11:35:16.000000 lptp-1.0.1/src/lptp/server/file_generator.py
--rw-rw-rw-   0        0        0      129 2024-03-16 22:06:11.000000 lptp-1.0.1/src/lptp/server/log.py
--rw-rw-rw-   0        0        0     2355 2024-03-24 11:21:51.000000 lptp-1.0.1/src/lptp/server/manager.py
--rw-rw-rw-   0        0        0     4551 2024-03-25 12:19:04.000000 lptp-1.0.1/src/lptp/server/procedure.py
--rw-rw-rw-   0        0        0     6191 2024-03-24 19:38:41.000000 lptp-1.0.1/src/lptp/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.690098 lptp-1.0.1/src/lptp/types/
--rw-rw-rw-   0        0        0       42 2024-03-17 19:55:57.000000 lptp-1.0.1/src/lptp/types/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.703227 lptp-1.0.1/src/lptp/types/packets/
--rw-rw-rw-   0        0        0      180 2024-03-17 17:44:08.000000 lptp-1.0.1/src/lptp/types/packets/__init__.py
--rw-rw-rw-   0        0        0     2005 2024-03-23 12:22:42.000000 lptp-1.0.1/src/lptp/types/packets/auth.py
--rw-rw-rw-   0        0        0     1930 2024-03-24 11:23:43.000000 lptp-1.0.1/src/lptp/types/packets/base.py
--rw-rw-rw-   0        0        0      268 2024-03-16 22:26:59.000000 lptp-1.0.1/src/lptp/types/packets/exit.py
--rw-rw-rw-   0        0        0     1606 2024-03-17 20:15:02.000000 lptp-1.0.1/src/lptp/types/packets/procedure.py
--rw-rw-rw-   0        0        0      208 2024-03-23 12:24:30.000000 lptp-1.0.1/src/lptp/types/packets/status.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.709750 lptp-1.0.1/src/lptp/types/pds/
--rw-rw-rw-   0        0        0       86 2024-03-17 19:19:39.000000 lptp-1.0.1/src/lptp/types/pds/__init__.py
--rw-rw-rw-   0        0        0     2316 2024-03-17 20:24:49.000000 lptp-1.0.1/src/lptp/types/pds/field.py
--rw-rw-rw-   0        0        0     1974 2024-03-25 11:41:41.000000 lptp-1.0.1/src/lptp/types/pds/pds.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.723018 lptp-1.0.1/src/lptp/types/pds/types/
--rw-rw-rw-   0        0        0      195 2024-05-19 18:18:49.000000 lptp-1.0.1/src/lptp/types/pds/types/__init__.py
--rw-rw-rw-   0        0        0     1600 2024-05-19 18:19:11.000000 lptp-1.0.1/src/lptp/types/pds/types/base.py
--rw-rw-rw-   0        0        0      347 2024-03-25 12:14:51.000000 lptp-1.0.1/src/lptp/types/pds/types/bool.py
--rw-rw-rw-   0        0        0      583 2024-03-25 12:02:32.000000 lptp-1.0.1/src/lptp/types/pds/types/int.py
--rw-rw-rw-   0        0        0     1510 2024-03-25 12:02:36.000000 lptp-1.0.1/src/lptp/types/pds/types/list.py
--rw-rw-rw-   0        0        0     2894 2024-05-19 18:18:24.000000 lptp-1.0.1/src/lptp/types/pds/types/other.py
--rw-rw-rw-   0        0        0      519 2024-03-25 12:02:40.000000 lptp-1.0.1/src/lptp/types/pds/types/str.py
-drwxrwxrwx   0        0        0        0 2024-05-19 19:21:03.725262 lptp-1.0.1/src/lptp.egg-info/
--rw-rw-rw-   0        0        0     2564 2024-05-19 19:21:03.000000 lptp-1.0.1/src/lptp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1046 2024-05-19 19:21:03.000000 lptp-1.0.1/src/lptp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 19:21:03.000000 lptp-1.0.1/src/lptp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-19 19:21:03.000000 lptp-1.0.1/src/lptp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:30.044796 lptp-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-16 13:37:55.000000 lptp-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2563 2024-05-19 19:26:30.044254 lptp-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1952 2024-05-19 18:38:57.000000 lptp-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-19 19:26:30.048776 lptp-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      812 2024-05-19 19:26:17.000000 lptp-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:29.914029 lptp-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:29.916928 lptp-1.0.2/src/lptp/
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:29.957416 lptp-1.0.2/src/lptp/client/
+-rw-rw-rw-   0        0        0       30 2024-03-16 22:02:51.000000 lptp-1.0.2/src/lptp/client/__init__.py
+-rw-rw-rw-   0        0        0     3961 2024-03-24 19:27:55.000000 lptp-1.0.2/src/lptp/client/client.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:29.971339 lptp-1.0.2/src/lptp/exceptions/
+-rw-rw-rw-   0        0        0      151 2024-03-18 17:29:57.000000 lptp-1.0.2/src/lptp/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      296 2024-03-17 19:57:15.000000 lptp-1.0.2/src/lptp/exceptions/base.py
+-rw-rw-rw-   0        0        0      518 2024-03-24 19:25:54.000000 lptp-1.0.2/src/lptp/exceptions/client.py
+-rw-rw-rw-   0        0        0      204 2024-03-17 19:47:57.000000 lptp-1.0.2/src/lptp/exceptions/data.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:29.987338 lptp-1.0.2/src/lptp/server/
+-rw-rw-rw-   0        0        0       94 2024-03-18 20:12:29.000000 lptp-1.0.2/src/lptp/server/__init__.py
+-rw-rw-rw-   0        0        0     2263 2024-03-25 11:35:16.000000 lptp-1.0.2/src/lptp/server/file_generator.py
+-rw-rw-rw-   0        0        0      129 2024-03-16 22:06:11.000000 lptp-1.0.2/src/lptp/server/log.py
+-rw-rw-rw-   0        0        0     2355 2024-03-24 11:21:51.000000 lptp-1.0.2/src/lptp/server/manager.py
+-rw-rw-rw-   0        0        0     4551 2024-03-25 12:19:04.000000 lptp-1.0.2/src/lptp/server/procedure.py
+-rw-rw-rw-   0        0        0     6191 2024-03-24 19:38:41.000000 lptp-1.0.2/src/lptp/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:29.989338 lptp-1.0.2/src/lptp/types/
+-rw-rw-rw-   0        0        0       42 2024-03-17 19:55:57.000000 lptp-1.0.2/src/lptp/types/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:30.010419 lptp-1.0.2/src/lptp/types/packets/
+-rw-rw-rw-   0        0        0      180 2024-03-17 17:44:08.000000 lptp-1.0.2/src/lptp/types/packets/__init__.py
+-rw-rw-rw-   0        0        0     2005 2024-03-23 12:22:42.000000 lptp-1.0.2/src/lptp/types/packets/auth.py
+-rw-rw-rw-   0        0        0     1930 2024-03-24 11:23:43.000000 lptp-1.0.2/src/lptp/types/packets/base.py
+-rw-rw-rw-   0        0        0      268 2024-03-16 22:26:59.000000 lptp-1.0.2/src/lptp/types/packets/exit.py
+-rw-rw-rw-   0        0        0     1606 2024-03-17 20:15:02.000000 lptp-1.0.2/src/lptp/types/packets/procedure.py
+-rw-rw-rw-   0        0        0      208 2024-03-23 12:24:30.000000 lptp-1.0.2/src/lptp/types/packets/status.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:30.019038 lptp-1.0.2/src/lptp/types/pds/
+-rw-rw-rw-   0        0        0       86 2024-03-17 19:19:39.000000 lptp-1.0.2/src/lptp/types/pds/__init__.py
+-rw-rw-rw-   0        0        0     2316 2024-03-17 20:24:49.000000 lptp-1.0.2/src/lptp/types/pds/field.py
+-rw-rw-rw-   0        0        0     1974 2024-03-25 11:41:41.000000 lptp-1.0.2/src/lptp/types/pds/pds.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:30.039265 lptp-1.0.2/src/lptp/types/pds/types/
+-rw-rw-rw-   0        0        0      195 2024-05-19 18:18:49.000000 lptp-1.0.2/src/lptp/types/pds/types/__init__.py
+-rw-rw-rw-   0        0        0     1600 2024-05-19 18:19:11.000000 lptp-1.0.2/src/lptp/types/pds/types/base.py
+-rw-rw-rw-   0        0        0      347 2024-03-25 12:14:51.000000 lptp-1.0.2/src/lptp/types/pds/types/bool.py
+-rw-rw-rw-   0        0        0      583 2024-03-25 12:02:32.000000 lptp-1.0.2/src/lptp/types/pds/types/int.py
+-rw-rw-rw-   0        0        0     1510 2024-03-25 12:02:36.000000 lptp-1.0.2/src/lptp/types/pds/types/list.py
+-rw-rw-rw-   0        0        0     2894 2024-05-19 18:18:24.000000 lptp-1.0.2/src/lptp/types/pds/types/other.py
+-rw-rw-rw-   0        0        0      519 2024-03-25 12:02:40.000000 lptp-1.0.2/src/lptp/types/pds/types/str.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:26:30.043254 lptp-1.0.2/src/lptp.egg-info/
+-rw-rw-rw-   0        0        0     2563 2024-05-19 19:26:29.000000 lptp-1.0.2/src/lptp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2024-05-19 19:26:29.000000 lptp-1.0.2/src/lptp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 19:26:29.000000 lptp-1.0.2/src/lptp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-19 19:26:29.000000 lptp-1.0.2/src/lptp.egg-info/top_level.txt
```

### Comparing `lptp-1.0.1/LICENSE` & `lptp-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/PKG-INFO` & `lptp-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lptp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Данный протокол является протоколом RPC вида и служит для вызова процедур на удалённом сервере. Проект является исключительно учебным и не рекомендуется для реального использования.
 Home-page: https://github.com/Zoom-Developer/LPTP
 Author: zoomdev
-Author-email: zoomdeveloper@ayandex.ru
+Author-email: zoomdeveloper@yandex.ru
 Keywords: rpc
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lite Procedure Transfer Protocol (LPTP)
 *Данный протокол является протоколом RPC вида и служит для вызова процедур на удалённом сервере. Проект является исключительно учебным и не рекомендуется для реального использования.*
```

### Comparing `lptp-1.0.1/README.md` & `lptp-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/setup.py` & `lptp-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 def readme():
   with open('README.md', 'r', encoding="utf8") as f:
     return f.read()
 
 setup(
     name='lptp',
-    version='1.0.1',
+    version='1.0.2',
     author='zoomdev',
-    author_email='zoomdeveloper@ayandex.ru',
+    author_email='zoomdeveloper@yandex.ru',
     description='Данный протокол является протоколом RPC вида и служит для вызова процедур на удалённом сервере. Проект является исключительно учебным и не рекомендуется для реального использования.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     package_dir={"": "src"},
     keywords='rpc',
     url="https://github.com/Zoom-Developer/LPTP",
     python_requires='>=3.10'
```

### Comparing `lptp-1.0.1/src/lptp/client/client.py` & `lptp-1.0.2/src/lptp/client/client.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/exceptions/client.py` & `lptp-1.0.2/src/lptp/exceptions/client.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/server/file_generator.py` & `lptp-1.0.2/src/lptp/server/file_generator.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/server/manager.py` & `lptp-1.0.2/src/lptp/server/manager.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/server/procedure.py` & `lptp-1.0.2/src/lptp/server/procedure.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/server/server.py` & `lptp-1.0.2/src/lptp/server/server.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/packets/auth.py` & `lptp-1.0.2/src/lptp/types/packets/auth.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/packets/base.py` & `lptp-1.0.2/src/lptp/types/packets/base.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/packets/procedure.py` & `lptp-1.0.2/src/lptp/types/packets/procedure.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/field.py` & `lptp-1.0.2/src/lptp/types/pds/field.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/pds.py` & `lptp-1.0.2/src/lptp/types/pds/pds.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/types/base.py` & `lptp-1.0.2/src/lptp/types/pds/types/base.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/types/int.py` & `lptp-1.0.2/src/lptp/types/pds/types/int.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/types/list.py` & `lptp-1.0.2/src/lptp/types/pds/types/list.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/types/other.py` & `lptp-1.0.2/src/lptp/types/pds/types/other.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp/types/pds/types/str.py` & `lptp-1.0.2/src/lptp/types/pds/types/str.py`

 * *Files identical despite different names*

### Comparing `lptp-1.0.1/src/lptp.egg-info/PKG-INFO` & `lptp-1.0.2/src/lptp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lptp
-Version: 1.0.1
+Version: 1.0.2
 Summary: Данный протокол является протоколом RPC вида и служит для вызова процедур на удалённом сервере. Проект является исключительно учебным и не рекомендуется для реального использования.
 Home-page: https://github.com/Zoom-Developer/LPTP
 Author: zoomdev
-Author-email: zoomdeveloper@ayandex.ru
+Author-email: zoomdeveloper@yandex.ru
 Keywords: rpc
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Lite Procedure Transfer Protocol (LPTP)
 *Данный протокол является протоколом RPC вида и служит для вызова процедур на удалённом сервере. Проект является исключительно учебным и не рекомендуется для реального использования.*
```

### Comparing `lptp-1.0.1/src/lptp.egg-info/SOURCES.txt` & `lptp-1.0.2/src/lptp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

