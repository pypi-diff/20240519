# Comparing `tmp/floatingparser-1.0.1.tar.gz` & `tmp/floatingparser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatingparser-1.0.1.tar", last modified: Sun May 19 16:30:07 2024, max compression
+gzip compressed data, was "floatingparser-1.0.2.tar", last modified: Sun May 19 16:50:38 2024, max compression
```

## Comparing `floatingparser-1.0.1.tar` & `floatingparser-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:30:07.691169 floatingparser-1.0.1/
--rw-rw-rw-   0        0        0      148 2024-05-19 16:30:07.691169 floatingparser-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-12-03 17:16:13.000000 floatingparser-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 16:30:07.673256 floatingparser-1.0.1/floatingparser/
--rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.1/floatingparser/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.1/floatingparser/floating_mail_sender.py
--rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.1/floatingparser/floating_parser.py
--rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.1/floatingparser/floating_statistics.py
--rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.1/floatingparser/floating_visualizer.py
--rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.1/floatingparser/floating_web.py
--rw-rw-rw-   0        0        0     2558 2024-05-19 16:27:55.000000 floatingparser-1.0.1/floatingparser/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:30:07.690170 floatingparser-1.0.1/floatingparser.egg-info/
--rw-rw-rw-   0        0        0      148 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.1/floatingparser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-05-19 16:30:07.000000 floatingparser-1.0.1/floatingparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 16:30:07.693170 floatingparser-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      250 2024-05-19 16:29:47.000000 floatingparser-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:50:38.436706 floatingparser-1.0.2/
+-rw-rw-rw-   0        0        0     1643 2024-05-19 16:50:38.436706 floatingparser-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2024-05-19 16:43:03.000000 floatingparser-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 16:50:38.420701 floatingparser-1.0.2/floatingparser/
+-rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.2/floatingparser/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.2/floatingparser/floating_mail_sender.py
+-rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.2/floatingparser/floating_parser.py
+-rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.2/floatingparser/floating_statistics.py
+-rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.2/floatingparser/floating_visualizer.py
+-rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.2/floatingparser/floating_web.py
+-rw-rw-rw-   0        0        0     2520 2024-05-19 16:41:01.000000 floatingparser-1.0.2/floatingparser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:50:38.435706 floatingparser-1.0.2/floatingparser.egg-info/
+-rw-rw-rw-   0        0        0     1643 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.2/floatingparser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:50:38.437702 floatingparser-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      548 2024-05-19 16:50:30.000000 floatingparser-1.0.2/setup.py
```

### Comparing `floatingparser-1.0.1/floatingparser/floating_mail_sender.py` & `floatingparser-1.0.2/floatingparser/floating_mail_sender.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.1/floatingparser/floating_parser.py` & `floatingparser-1.0.2/floatingparser/floating_parser.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.1/floatingparser/floating_statistics.py` & `floatingparser-1.0.2/floatingparser/floating_statistics.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.1/floatingparser/floating_visualizer.py` & `floatingparser-1.0.2/floatingparser/floating_visualizer.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.1/floatingparser/floating_web.py` & `floatingparser-1.0.2/floatingparser/floating_web.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.1/floatingparser/main.py` & `floatingparser-1.0.2/floatingparser/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .floating_parser import LogParser
 from .floating_statistics import Statistics
 from .floating_visualizer import Visualizer
 from .floating_mail_sender import Sender
 from .floating_web import App
 
 
-def main():
+def FloatingStart():
     '''
     Working with modules
     '''
 
     default_logs_path = pathlib.Path().cwd() / "tfs-log.txt"
     argparser = argparse.ArgumentParser(description="Logs data to graphs")
     
@@ -86,13 +86,12 @@
                             start_stop_graph, 
                             total_time_altair
                             )
 
     app.start_app() 
 
     if args.web:
-        namik = sys.argv[0]
-        print(f'Название файла это {namik}')
-        os.system(rf'streamlit run .\main.py -- -p {file_path}')
+        file_name = sys.argv[0]
+        os.system(rf'streamlit run {file_name} -- -p {file_path}')
 
 if __name__ == "__main__":
-    main()
+    FloatingStart()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

