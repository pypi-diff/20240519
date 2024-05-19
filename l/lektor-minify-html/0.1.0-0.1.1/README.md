# Comparing `tmp/lektor-minify-html-0.1.0.tar.gz` & `tmp/lektor_minify_html-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-minify-html-0.1.0.tar", last modified: Wed Apr 10 23:05:07 2024, max compression
+gzip compressed data, was "lektor_minify_html-0.1.1.tar", last modified: Sun May 19 01:07:54 2024, max compression
```

## Comparing `lektor-minify-html-0.1.0.tar` & `lektor_minify_html-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-10 23:05:07.000000 lektor-minify-html-0.1.0/lektor_minify_html.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/lektor_minify_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 23:05:07.428490 lektor-minify-html-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 23:05:02.000000 lektor-minify-html-0.1.0/tests/test_lektor_minify_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:07:54.218867 lektor_minify_html-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-19 01:07:46.000000 lektor_minify_html-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-19 01:07:54.218867 lektor_minify_html-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-19 01:07:46.000000 lektor_minify_html-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:07:54.218867 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-19 01:07:54.000000 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-19 01:07:54.000000 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:07:54.000000 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 01:07:54.000000 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 01:07:54.000000 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 01:07:54.000000 lektor_minify_html-0.1.1/lektor_minify_html.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-19 01:07:46.000000 lektor_minify_html-0.1.1/lektor_minify_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-19 01:07:46.000000 lektor_minify_html-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 01:07:54.218867 lektor_minify_html-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:07:54.218867 lektor_minify_html-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-19 01:07:46.000000 lektor_minify_html-0.1.1/tests/test_lektor_minify_html.py
```

### Comparing `lektor-minify-html-0.1.0/LICENSE` & `lektor_minify_html-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-minify-html-0.1.0/PKG-INFO` & `lektor_minify_html-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-minify-html
-Version: 0.1.0
+Version: 0.1.1
 Summary: Minify content using minify-html
 Author: seralot
 License: MIT License
         
         Copyright (c) 2024 Sergio Alonso
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lektor-minify-html-0.1.0/README.md` & `lektor_minify_html-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lektor-minify-html-0.1.0/lektor_minify_html.egg-info/PKG-INFO` & `lektor_minify_html-0.1.1/lektor_minify_html.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lektor-minify-html
-Version: 0.1.0
+Version: 0.1.1
 Summary: Minify content using minify-html
 Author: seralot
 License: MIT License
         
         Copyright (c) 2024 Sergio Alonso
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lektor-minify-html-0.1.0/lektor_minify_html.py` & `lektor_minify_html-0.1.1/lektor_minify_html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 from lektor.pluginsystem import Plugin
 import minify_html
 
 class MinifyHtmlPlugin(Plugin):
     name = 'Lektor minify html'
     description = u'Minify content using minify-html'
 
@@ -17,12 +16,16 @@
 
     def on_after_build(self, builder, **extra) -> None:
         if not len(extra["prog"].artifacts):
             return
 
         dst_filename = extra["prog"].artifacts[0].dst_filename
 
-        with open(dst_filename, 'r+') as file:
-            html_content = file.read()
-            file.seek(0)
-            file.write(self.minify(html_content))
-            file.truncate()
+        try:
+            with open(dst_filename, 'r+') as file:
+                html_content = file.read()
+                file.seek(0)
+                file.write(self.minify(html_content))
+                file.truncate()
+        except UnicodeDecodeError:
+            # Minification is skipped.
+            return
```

### Comparing `lektor-minify-html-0.1.0/pyproject.toml` & `lektor_minify_html-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lektor-minify-html"
-version = "0.1.0"
+version = "0.1.1"
 license = {file = "LICENSE"}
 authors = [{ name = "seralot"}]
 description = "Minify content using minify-html"
 readme = "README.md"
 dependencies = ["minify-html"]
 
 [project.urls]
```

