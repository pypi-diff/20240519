# Comparing `tmp/floatingparser-1.0.2.tar.gz` & `tmp/floatingparser-1.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatingparser-1.0.2.tar", last modified: Sun May 19 16:50:38 2024, max compression
+gzip compressed data, was "floatingparser-1.0.2.1.tar", last modified: Sun May 19 16:58:42 2024, max compression
```

## Comparing `floatingparser-1.0.2.tar` & `floatingparser-1.0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 16:50:38.436706 floatingparser-1.0.2/
--rw-rw-rw-   0        0        0     1643 2024-05-19 16:50:38.436706 floatingparser-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1352 2024-05-19 16:43:03.000000 floatingparser-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 16:50:38.420701 floatingparser-1.0.2/floatingparser/
--rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.2/floatingparser/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.2/floatingparser/floating_mail_sender.py
--rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.2/floatingparser/floating_parser.py
--rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.2/floatingparser/floating_statistics.py
--rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.2/floatingparser/floating_visualizer.py
--rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.2/floatingparser/floating_web.py
--rw-rw-rw-   0        0        0     2520 2024-05-19 16:41:01.000000 floatingparser-1.0.2/floatingparser/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 16:50:38.435706 floatingparser-1.0.2/floatingparser.egg-info/
--rw-rw-rw-   0        0        0     1643 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.2/floatingparser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2024-05-19 16:50:38.000000 floatingparser-1.0.2/floatingparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 16:50:38.437702 floatingparser-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      548 2024-05-19 16:50:30.000000 floatingparser-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:58:42.985936 floatingparser-1.0.2.1/
+-rw-rw-rw-   0        0        0     1645 2024-05-19 16:58:42.985936 floatingparser-1.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1352 2024-05-19 16:43:03.000000 floatingparser-1.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 16:58:42.969940 floatingparser-1.0.2.1/floatingparser/
+-rw-rw-rw-   0        0        0       82 2024-05-19 15:56:51.000000 floatingparser-1.0.2.1/floatingparser/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparser-1.0.2.1/floatingparser/floating_mail_sender.py
+-rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparser-1.0.2.1/floatingparser/floating_parser.py
+-rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparser-1.0.2.1/floatingparser/floating_statistics.py
+-rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparser-1.0.2.1/floatingparser/floating_visualizer.py
+-rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparser-1.0.2.1/floatingparser/floating_web.py
+-rw-rw-rw-   0        0        0     2668 2024-05-19 16:58:05.000000 floatingparser-1.0.2.1/floatingparser/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:58:42.984940 floatingparser-1.0.2.1/floatingparser.egg-info/
+-rw-rw-rw-   0        0        0     1645 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 16:14:37.000000 floatingparser-1.0.2.1/floatingparser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-05-19 16:58:42.000000 floatingparser-1.0.2.1/floatingparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:58:42.987940 floatingparser-1.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      550 2024-05-19 16:58:13.000000 floatingparser-1.0.2.1/setup.py
```

### Comparing `floatingparser-1.0.2/PKG-INFO` & `floatingparser-1.0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floatingparser
-Version: 1.0.2
+Version: 1.0.2.1
 Summary: Parser for floating server logs
 Home-page: https://github.com/Asphodell/coursework_system
 Author: Vladislav "Asphodel" Shabalin
 Author-email: vladislaus.shabalin@yandex.ru
 Description-Content-Type: text/markdown
 
 # FloatingParser System
```

### Comparing `floatingparser-1.0.2/README.md` & `floatingparser-1.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2/floatingparser/floating_mail_sender.py` & `floatingparser-1.0.2.1/floatingparser/floating_mail_sender.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2/floatingparser/floating_parser.py` & `floatingparser-1.0.2.1/floatingparser/floating_parser.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2/floatingparser/floating_statistics.py` & `floatingparser-1.0.2.1/floatingparser/floating_statistics.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2/floatingparser/floating_visualizer.py` & `floatingparser-1.0.2.1/floatingparser/floating_visualizer.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2/floatingparser/floating_web.py` & `floatingparser-1.0.2.1/floatingparser/floating_web.py`

 * *Files identical despite different names*

### Comparing `floatingparser-1.0.2/floatingparser/main.py` & `floatingparser-1.0.2.1/floatingparser/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -87,11 +87,13 @@
                             total_time_altair
                             )
 
     app.start_app() 
 
     if args.web:
         file_name = sys.argv[0]
+        print(f"FILENAME IS {file_name} !!!!!!!!!!!!!!!!!!")
+        print(rf'КОМАНДА ЭТО streamlit run {file_name} -- -p {file_path}')
         os.system(rf'streamlit run {file_name} -- -p {file_path}')
 
 if __name__ == "__main__":
     FloatingStart()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `floatingparser-1.0.2/floatingparser.egg-info/PKG-INFO` & `floatingparser-1.0.2.1/floatingparser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: floatingparser
-Version: 1.0.2
+Version: 1.0.2.1
 Summary: Parser for floating server logs
 Home-page: https://github.com/Asphodell/coursework_system
 Author: Vladislav "Asphodel" Shabalin
 Author-email: vladislaus.shabalin@yandex.ru
 Description-Content-Type: text/markdown
 
 # FloatingParser System
```

### Comparing `floatingparser-1.0.2/setup.py` & `floatingparser-1.0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
       long_description = fh.read()
 
 setup(name='floatingparser',
-      version='1.0.2',
+      version='1.0.2.1',
       author='Vladislav "Asphodel" Shabalin',
       description='Parser for floating server logs',
       long_description=long_description,  
       long_description_content_type='text/markdown',
       packages=['floatingparser'],
       author_email='vladislaus.shabalin@yandex.ru',
       url="https://github.com/Asphodell/coursework_system",
```

