# Comparing `tmp/floatingparser-1.0.tar.gz` & `tmp/floatingparser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatingparser-1.0.tar", last modified: Sun May 19 16:15:08 2024, max compression
+gzip compressed data, was "floatingparser-1.0.1.tar", last modified: Sun May 19 16:30:07 2024, max compression
```

## Comparing `floatingparser-1.0.tar` & `floatingparser-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:08.161720 floatingparser-1.0/
--rw-rw-rw-   0        0        0      146 2024-05-19 16:15:08.161720 floatingparser-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-12-03 17:16:13.000000 floatingparser-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:08.140929 floatingparser-1.0/floatingparser/
--rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0/floatingparser/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0/floatingparser/floating_mail_sender.py
--rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0/floatingparser/floating_parser.py
--rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0/floatingparser/floating_statistics.py
--rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0/floatingparser/floating_visualizer.py
--rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0/floatingparser/floating_web.py
--rw-rw-rw-   0        0        0     2455 2024-05-19 16:03:57.000000 floatingparser-1.0/floatingparser/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:15:08.160714 floatingparser-1.0/floatingparser.egg-info/
--rw-rw-rw-   0        0        0      146 2024-05-19 16:15:08.000000 floatingparser-1.0/floatingparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-05-19 16:15:08.000000 floatingparser-1.0/floatingparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:15:08.000000 floatingparser-1.0/floatingparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0/floatingparser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-05-19 16:15:08.000000 floatingparser-1.0/floatingparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 16:15:08.163714 floatingparser-1.0/setup.cfg
--rw-rw-rw-   0        0        0      248 2024-05-19 16:15:03.000000 floatingparser-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:30:07.691169 floatingparser-1.0.1/
+-rw-rw-rw-   0        0        0      148 2024-05-19 16:30:07.691169 floatingparser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-12-03 17:16:13.000000 floatingparser-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 16:30:07.673256 floatingparser-1.0.1/floatingparser/
+-rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.1/floatingparser/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.1/floatingparser/floating_mail_sender.py
+-rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.1/floatingparser/floating_parser.py
+-rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.1/floatingparser/floating_statistics.py
+-rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.1/floatingparser/floating_visualizer.py
+-rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.1/floatingparser/floating_web.py
+-rw-rw-rw-   0        0        0     2558 2024-05-19 16:27:55.000000 floatingparser-1.0.1/floatingparser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:30:07.690170 floatingparser-1.0.1/floatingparser.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.1/floatingparser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:30:07.693170 floatingparser-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      250 2024-05-19 16:29:47.000000 floatingparser-1.0.1/setup.py
```

### Comparing `floatingparser-1.0/floatingparser/floating_mail_sender.py` & `floatingparser-1.0.1/floatingparser/floating_mail_sender.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0/floatingparser/floating_parser.py` & `floatingparser-1.0.1/floatingparser/floating_parser.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0/floatingparser/floating_statistics.py` & `floatingparser-1.0.1/floatingparser/floating_statistics.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0/floatingparser/floating_visualizer.py` & `floatingparser-1.0.1/floatingparser/floating_visualizer.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0/floatingparser/floating_web.py` & `floatingparser-1.0.1/floatingparser/floating_web.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0/floatingparser/main.py` & `floatingparser-1.0.1/floatingparser/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Starting the Data Analytics System
 '''
 
 import argparse
 import pathlib
 from datetime import date
 import os
+import sys
 
 from .floating_parser import LogParser
 from .floating_statistics import Statistics
 from .floating_visualizer import Visualizer
 from .floating_mail_sender import Sender
 from .floating_web import App
 
@@ -85,11 +86,13 @@
                             start_stop_graph, 
                             total_time_altair
                             )
 
     app.start_app() 
 
     if args.web:
+        namik = sys.argv[0]
+        print(f'Название файла это {namik}')
         os.system(rf'streamlit run .\main.py -- -p {file_path}')
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

