# Comparing `tmp/my_table_db-2.0.0.tar.gz` & `tmp/my_table_db-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_table_db-2.0.0.tar", last modified: Sat May 18 23:00:52 2024, max compression
+gzip compressed data, was "my_table_db-2.0.1.tar", last modified: Sat May 18 23:04:52 2024, max compression
```

## Comparing `my_table_db-2.0.0.tar` & `my_table_db-2.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 23:00:52.212201 my_table_db-2.0.0/
--rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     3941 2024-05-18 23:00:52.211201 my_table_db-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3703 2024-05-18 19:59:13.000000 my_table_db-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 23:00:52.211201 my_table_db-2.0.0/my_table_db.egg-info/
--rw-rw-rw-   0        0        0     3941 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-18 23:00:52.000000 my_table_db-2.0.0/my_table_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1906 2024-05-18 23:00:35.000000 my_table_db-2.0.0/my_table_db.py
--rw-rw-rw-   0        0        0       42 2024-05-18 23:00:52.212201 my_table_db-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-05-18 23:00:35.000000 my_table_db-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:04:52.834056 my_table_db-2.0.1/
+-rw-rw-rw-   0        0        0     1086 2024-05-18 20:21:49.000000 my_table_db-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3892 2024-05-18 23:04:52.833057 my_table_db-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3654 2024-05-18 23:04:48.000000 my_table_db-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 23:04:52.832058 my_table_db-2.0.1/my_table_db.egg-info/
+-rw-rw-rw-   0        0        0     3892 2024-05-18 23:04:52.000000 my_table_db-2.0.1/my_table_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2024-05-18 23:04:52.000000 my_table_db-2.0.1/my_table_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:04:52.000000 my_table_db-2.0.1/my_table_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-18 23:04:52.000000 my_table_db-2.0.1/my_table_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1906 2024-05-18 23:00:35.000000 my_table_db-2.0.1/my_table_db.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:04:52.834056 my_table_db-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-18 23:04:48.000000 my_table_db-2.0.1/setup.py
```

### Comparing `my_table_db-2.0.0/LICENSE` & `my_table_db-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `my_table_db-2.0.0/PKG-INFO` & `my_table_db-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 2.0.0
+Version: 2.0.1
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Функция Library
 
 Этот Python-скрипт определяет функцию library, которая форматирует набор именованных аргументов и их соответствующих значений в строку. Выходная строка структурирована с определенным форматом, где каждая пара имя-значение разделена символом | и дополнена до выравнивания в столбцах.
 
 ***
-### Установка
-` pip install my_table_db `
 
 
 ## Использование
 Функция library принимает именованные аргументы (name_arg1, name_arg2, ..., name_arg7) и их соответствующие значения (arg1, arg2, ..., arg7). Она форматирует эти входные данные в аккуратную строку с каждой парой имя-значение, разделенной символом |. Функция может обрабатывать различное количество аргументов, от одного до семи пар.
 
 ***
 
@@ -35,15 +33,15 @@
 ***
 
 # Установка
 
 ` pip install my_table_db `
 
 ## Пример 1
-Пример использования функции library:
+Пример использования функции my_table_db:
 
 ```python
 from my_table_db import my_table_db
 
 print(my_table_db('ID', 1, 'Name', 'Alice', 'Salary', 50000))
 
 ```
```

### Comparing `my_table_db-2.0.0/README.md` & `my_table_db-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Функция Library
 
 Этот Python-скрипт определяет функцию library, которая форматирует набор именованных аргументов и их соответствующих значений в строку. Выходная строка структурирована с определенным форматом, где каждая пара имя-значение разделена символом | и дополнена до выравнивания в столбцах.
 
 ***
-### Установка
-` pip install my_table_db `
 
 
 ## Использование
 Функция library принимает именованные аргументы (name_arg1, name_arg2, ..., name_arg7) и их соответствующие значения (arg1, arg2, ..., arg7). Она форматирует эти входные данные в аккуратную строку с каждой парой имя-значение, разделенной символом |. Функция может обрабатывать различное количество аргументов, от одного до семи пар.
 
 ***
 
@@ -25,15 +23,15 @@
 ***
 
 # Установка
 
 ` pip install my_table_db `
 
 ## Пример 1
-Пример использования функции library:
+Пример использования функции my_table_db:
 
 ```python
 from my_table_db import my_table_db
 
 print(my_table_db('ID', 1, 'Name', 'Alice', 'Salary', 50000))
 
 ```
```

### Comparing `my_table_db-2.0.0/my_table_db.egg-info/PKG-INFO` & `my_table_db-2.0.1/my_table_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: my_table_db
-Version: 2.0.0
+Version: 2.0.1
 Summary: A small library for conclusion table db
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Функция Library
 
 Этот Python-скрипт определяет функцию library, которая форматирует набор именованных аргументов и их соответствующих значений в строку. Выходная строка структурирована с определенным форматом, где каждая пара имя-значение разделена символом | и дополнена до выравнивания в столбцах.
 
 ***
-### Установка
-` pip install my_table_db `
 
 
 ## Использование
 Функция library принимает именованные аргументы (name_arg1, name_arg2, ..., name_arg7) и их соответствующие значения (arg1, arg2, ..., arg7). Она форматирует эти входные данные в аккуратную строку с каждой парой имя-значение, разделенной символом |. Функция может обрабатывать различное количество аргументов, от одного до семи пар.
 
 ***
 
@@ -35,15 +33,15 @@
 ***
 
 # Установка
 
 ` pip install my_table_db `
 
 ## Пример 1
-Пример использования функции library:
+Пример использования функции my_table_db:
 
 ```python
 from my_table_db import my_table_db
 
 print(my_table_db('ID', 1, 'Name', 'Alice', 'Salary', 50000))
 
 ```
```

### Comparing `my_table_db-2.0.0/my_table_db.py` & `my_table_db-2.0.1/my_table_db.py`

 * *Files identical despite different names*

