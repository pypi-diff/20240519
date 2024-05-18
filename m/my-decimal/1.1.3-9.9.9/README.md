# Comparing `tmp/my_decimal-1.1.3.tar.gz` & `tmp/my_decimal-9.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_decimal-1.1.3.tar", last modified: Mon May 13 22:18:52 2024, max compression
+gzip compressed data, was "my_decimal-9.9.9.tar", last modified: Sat May 18 23:33:47 2024, max compression
```

## Comparing `my_decimal-1.1.3.tar` & `my_decimal-9.9.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 22:18:52.750656 my_decimal-1.1.3/
--rw-rw-rw-   0        0        0     1088 2024-05-05 23:21:12.000000 my_decimal-1.1.3/LICENSE
--rw-rw-rw-   0        0        0     2152 2024-05-13 22:18:52.749657 my_decimal-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2024-05-13 22:18:46.000000 my_decimal-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 22:18:52.748658 my_decimal-1.1.3/my_decimal.egg-info/
--rw-rw-rw-   0        0        0     2152 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 22:18:52.000000 my_decimal-1.1.3/my_decimal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       61 2024-05-06 17:10:58.000000 my_decimal-1.1.3/my_decimal.py
--rw-rw-rw-   0        0        0       42 2024-05-13 22:18:52.750656 my_decimal-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      381 2024-05-13 22:18:46.000000 my_decimal-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:33:47.402471 my_decimal-9.9.9/
+-rw-rw-rw-   0        0        0     1088 2024-05-05 23:21:12.000000 my_decimal-9.9.9/LICENSE
+-rw-rw-rw-   0        0        0     2354 2024-05-18 23:33:47.401470 my_decimal-9.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2117 2024-05-18 23:33:42.000000 my_decimal-9.9.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 23:33:47.400468 my_decimal-9.9.9/my_decimal.egg-info/
+-rw-rw-rw-   0        0        0     2354 2024-05-18 23:33:47.000000 my_decimal-9.9.9/my_decimal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-05-18 23:33:47.000000 my_decimal-9.9.9/my_decimal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:33:47.000000 my_decimal-9.9.9/my_decimal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-18 23:33:47.000000 my_decimal-9.9.9/my_decimal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       78 2024-05-18 23:29:47.000000 my_decimal-9.9.9/my_decimal.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:33:47.402471 my_decimal-9.9.9/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-05-18 23:29:47.000000 my_decimal-9.9.9/setup.py
```

### Comparing `my_decimal-1.1.3/LICENSE` & `my_decimal-9.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `my_decimal-1.1.3/PKG-INFO` & `my_decimal-9.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_decimal
-Version: 1.1.3
+Version: 9.9.9
 Summary: A small library for formatting decimals
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -17,14 +17,20 @@
 ```
 ***
 ## Установка
 *Функция my_decimal не требует установки дополнительных библиотек. Просто напишите в консоли*
 > `pip install my-decimal`
 ***
 ## Пример использования
+```python
+my_decimal(expression,long)
+#expression - Выражение/переменная
+#long - Число значений после точки. Если не указывать long=3
+```
+
 
 1. ### без использования дополнительных модулей
 ```python
 num1 = 0.1
 num2 = 0.2
 
 result = num1 + num2
```

### Comparing `my_decimal-1.1.3/README.md` & `my_decimal-9.9.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 ```
 ***
 ## Установка
 *Функция my_decimal не требует установки дополнительных библиотек. Просто напишите в консоли*
 > `pip install my-decimal`
 ***
 ## Пример использования
+```python
+my_decimal(expression,long)
+#expression - Выражение/переменная
+#long - Число значений после точки. Если не указывать long=3
+```
+
 
 1. ### без использования дополнительных модулей
 ```python
 num1 = 0.1
 num2 = 0.2
 
 result = num1 + num2
@@ -55,8 +61,8 @@
 ***
 ## Важно
 *Функция my_decimal предполагает, что входное выражение является числом. При передаче нечисловых значений будут возникать ошибки.*
 
 ***
 ### Автор
 
-Автор: k0ng999
+Автор: k0ng999
```

### Comparing `my_decimal-1.1.3/my_decimal.egg-info/PKG-INFO` & `my_decimal-9.9.9/my_decimal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: my_decimal
-Version: 1.1.3
+Version: 9.9.9
 Summary: A small library for formatting decimals
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -17,14 +17,20 @@
 ```
 ***
 ## Установка
 *Функция my_decimal не требует установки дополнительных библиотек. Просто напишите в консоли*
 > `pip install my-decimal`
 ***
 ## Пример использования
+```python
+my_decimal(expression,long)
+#expression - Выражение/переменная
+#long - Число значений после точки. Если не указывать long=3
+```
+
 
 1. ### без использования дополнительных модулей
 ```python
 num1 = 0.1
 num2 = 0.2
 
 result = num1 + num2
```

