# Comparing `tmp/subprocess_shell-1.0.1.tar.gz` & `tmp/subprocess_shell-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocess_shell-1.0.1.tar", last modified: Fri May 10 20:33:55 2024, max compression
+gzip compressed data, was "subprocess_shell-1.0.2.tar", last modified: Sun May 19 07:43:01 2024, max compression
```

## Comparing `subprocess_shell-1.0.1.tar` & `subprocess_shell-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/
--rw-r--r--   0 arappold  (1000) arappold  (1000)     1072 2023-10-10 12:57:53.000000 subprocess_shell-1.0.1/LICENSE
--rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/PKG-INFO
--rw-r--r--   0 arappold  (1000) arappold  (1000)    18616 2024-05-09 08:30:58.000000 subprocess_shell-1.0.1/README.md
--rw-r--r--   0 arappold  (1000) arappold  (1000)      583 2024-05-10 20:29:36.000000 subprocess_shell-1.0.1/pyproject.toml
--rw-r--r--   0 arappold  (1000) arappold  (1000)       38 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/setup.cfg
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    35385 2024-05-10 20:15:10.000000 subprocess_shell-1.0.1/src/subprocess_shell/__init__.py
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/PKG-INFO
--rw-r--r--   0 arappold  (1000) arappold  (1000)      315 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/SOURCES.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)        1 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/dependency_links.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)       62 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/requires.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)       17 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/src/subprocess_shell.egg-info/top_level.txt
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-10 20:33:55.000000 subprocess_shell-1.0.1/tests/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    16050 2024-05-10 20:23:03.000000 subprocess_shell-1.0.1/tests/test_subprocess_shell.py
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)     1072 2023-10-10 12:57:53.000000 subprocess_shell-1.0.2/LICENSE
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/PKG-INFO
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    18616 2024-05-09 08:30:58.000000 subprocess_shell-1.0.2/README.md
+-rw-r--r--   0 arappold  (1000) arappold  (1000)      583 2024-05-19 07:37:08.000000 subprocess_shell-1.0.2/pyproject.toml
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       38 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/setup.cfg
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    35390 2024-05-11 12:26:54.000000 subprocess_shell-1.0.2/src/subprocess_shell/__init__.py
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell.egg-info/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell.egg-info/PKG-INFO
+-rw-r--r--   0 arappold  (1000) arappold  (1000)      315 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)        1 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       62 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell.egg-info/requires.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       17 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/src/subprocess_shell.egg-info/top_level.txt
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-19 07:43:01.000000 subprocess_shell-1.0.2/tests/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    16050 2024-05-19 07:32:48.000000 subprocess_shell-1.0.2/tests/test_subprocess_shell.py
```

### Comparing `subprocess_shell-1.0.1/LICENSE` & `subprocess_shell-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocess_shell-1.0.1/PKG-INFO` & `subprocess_shell-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess_shell
-Version: 1.0.1
+Version: 1.0.2
 Summary: A shell for subprocess
 Author-email: Andreas Rappold <not_evil@rappold1.at>
 License: MIT License
         
         Copyright (c) 2023 Andreas Rappold
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `subprocess_shell-1.0.1/README.md` & `subprocess_shell-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `subprocess_shell-1.0.1/pyproject.toml` & `subprocess_shell-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "subprocess_shell"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Andreas Rappold", email="not_evil@rappold1.at" },
 ]
 description = "A shell for subprocess"
 readme = "README.md"
 
 [project.license]
```

### Comparing `subprocess_shell-1.0.1/src/subprocess_shell/__init__.py` & `subprocess_shell-1.0.2/src/subprocess_shell/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
             previous_bytes = b""
             for bytes in itertools.chain([object], objects):
                 bytes = previous_bytes + bytes
                 try:
                     string = bytes.decode()
 
                 except UnicodeDecodeError:
-                    for index in range(-3, 0):
+                    for index in range(-1, -4, -1):
                         try:
                             string = bytes[:index].decode()
 
                         except UnicodeDecodeError:
                             pass
 
                         else:
```

### Comparing `subprocess_shell-1.0.1/src/subprocess_shell.egg-info/PKG-INFO` & `subprocess_shell-1.0.2/src/subprocess_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess_shell
-Version: 1.0.1
+Version: 1.0.2
 Summary: A shell for subprocess
 Author-email: Andreas Rappold <not_evil@rappold1.at>
 License: MIT License
         
         Copyright (c) 2023 Andreas Rappold
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `subprocess_shell-1.0.1/tests/test_subprocess_shell.py` & `subprocess_shell-1.0.2/tests/test_subprocess_shell.py`

 * *Files identical despite different names*

