# Comparing `tmp/floatingparser-1.0.2.1.tar.gz` & `tmp/floatingparser-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatingparser-1.0.2.1.tar", last modified: Sun May 19 16:58:42 2024, max compression
+gzip compressed data, was "floatingparser-1.0.2.2.tar", last modified: Sun May 19 17:10:15 2024, max compression
```

## Comparing `floatingparser-1.0.2.1.tar` & `floatingparser-1.0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:58:42.985936 floatingparser-1.0.2.1/
--rw-rw-rw-   0        0        0     1645 2024-05-19 16:58:42.985936 floatingparser-1.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2024-05-19 16:43:03.000000 floatingparser-1.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 16:58:42.969940 floatingparser-1.0.2.1/floatingparser/
--rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.2.1/floatingparser/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.2.1/floatingparser/floating_mail_sender.py
--rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.2.1/floatingparser/floating_parser.py
--rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.2.1/floatingparser/floating_statistics.py
--rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.2.1/floatingparser/floating_visualizer.py
--rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.2.1/floatingparser/floating_web.py
--rw-rw-rw-   0        0        0     2668 2024-05-19 16:58:05.000000 floatingparser-1.0.2.1/floatingparser/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:58:42.984940 floatingparser-1.0.2.1/floatingparser.egg-info/
--rw-rw-rw-   0        0        0     1645 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.2.1/floatingparser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 16:58:42.987940 floatingparser-1.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      550 2024-05-19 16:58:13.000000 floatingparser-1.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:10:15.568586 floatingparser-1.0.2.2/
+-rw-rw-rw-   0        0        0     1739 2024-05-19 17:10:15.568586 floatingparser-1.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2024-05-19 16:43:03.000000 floatingparser-1.0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:10:15.544585 floatingparser-1.0.2.2/floatingparser/
+-rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.2.2/floatingparser/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.2.2/floatingparser/floating_mail_sender.py
+-rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.2.2/floatingparser/floating_parser.py
+-rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.2.2/floatingparser/floating_statistics.py
+-rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.2.2/floatingparser/floating_visualizer.py
+-rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.2.2/floatingparser/floating_web.py
+-rw-rw-rw-   0        0        0     2668 2024-05-19 16:58:05.000000 floatingparser-1.0.2.2/floatingparser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:10:15.567586 floatingparser-1.0.2.2/floatingparser.egg-info/
+-rw-rw-rw-   0        0        0     1739 2024-05-19 17:10:15.000000 floatingparser-1.0.2.2/floatingparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-05-19 17:10:15.000000 floatingparser-1.0.2.2/floatingparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:10:15.000000 floatingparser-1.0.2.2/floatingparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.2.2/floatingparser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2024-05-19 17:10:15.000000 floatingparser-1.0.2.2/floatingparser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-19 17:10:15.000000 floatingparser-1.0.2.2/floatingparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:10:15.570585 floatingparser-1.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-19 17:09:46.000000 floatingparser-1.0.2.2/setup.py
```

### Comparing `floatingparser-1.0.2.1/PKG-INFO` & `floatingparser-1.0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: floatingparser
-Version: 1.0.2.1
-Summary: Parser for floating server logs
-Home-page: https://github.com/Asphodell/coursework_system
-Author: Vladislav "Asphodel" Shabalin
-Author-email: vladislaus.shabalin@yandex.ru
-Description-Content-Type: text/markdown
-
 # FloatingParser System
 
 floatingparser — это библиотека для обработки логов FloatingServer, которая позволяет создать статистику по журналам событий. О
 
  *  * Особенности: *  * 
 
 -  *  * Простота использования: *  * python "file_name.py" [args]
@@ -31,8 +22,8 @@
    
    parser = fp.FloatingStart()
 
 4. Запустите программу через коммандную строку и укажите нужные аргументы*:
    
    python "file_name.py" [args]
 
-*-Список аргументов можно вывести с помощью --help (-h)
+*-Список аргументов можно вывести с помощью --help (-h)
```

### Comparing `floatingparser-1.0.2.1/floatingparser/floating_mail_sender.py` & `floatingparser-1.0.2.2/floatingparser/floating_mail_sender.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2.1/floatingparser/floating_parser.py` & `floatingparser-1.0.2.2/floatingparser/floating_parser.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2.1/floatingparser/floating_statistics.py` & `floatingparser-1.0.2.2/floatingparser/floating_statistics.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2.1/floatingparser/floating_visualizer.py` & `floatingparser-1.0.2.2/floatingparser/floating_visualizer.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2.1/floatingparser/floating_web.py` & `floatingparser-1.0.2.2/floatingparser/floating_web.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2.1/floatingparser/main.py` & `floatingparser-1.0.2.2/floatingparser/main.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2.1/floatingparser.egg-info/PKG-INFO` & `floatingparser-1.0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: floatingparser
-Version: 1.0.2.1
+Version: 1.0.2.2
 Summary: Parser for floating server logs
 Home-page: https://github.com/Asphodell/coursework_system
 Author: Vladislav "Asphodel" Shabalin
 Author-email: vladislaus.shabalin@yandex.ru
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: plotly
+Requires-Dist: streamlit
 
 # FloatingParser System
 
 floatingparser — это библиотека для обработки логов FloatingServer, которая позволяет создать статистику по журналам событий. О
 
  *  * Особенности: *  *
```

