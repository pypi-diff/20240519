# Comparing `tmp/gymconnectx-1.0.4.tar.gz` & `tmp/gymconnectx-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymconnectx-1.0.4.tar", last modified: Sun May 19 07:50:51 2024, max compression
+gzip compressed data, was "gymconnectx-1.0.5.tar", last modified: Sun May 19 07:57:40 2024, max compression
```

## Comparing `gymconnectx-1.0.4.tar` & `gymconnectx-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/gymconnectx/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/gymconnectx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/gymconnectx/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/gymconnectx/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26410 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/gymconnectx/envs/gymconnectxenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/gymconnectx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:57:40.183795 gymconnectx-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-19 07:57:40.183795 gymconnectx-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:57:40.183795 gymconnectx-1.0.5/gymconnectx/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/gymconnectx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:57:40.183795 gymconnectx-1.0.5/gymconnectx/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/gymconnectx/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26410 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/gymconnectx/envs/gymconnectxenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:57:40.183795 gymconnectx-1.0.5/gymconnectx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-19 07:57:40.000000 gymconnectx-1.0.5/gymconnectx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 07:57:40.000000 gymconnectx-1.0.5/gymconnectx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:57:40.000000 gymconnectx-1.0.5/gymconnectx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:57:40.000000 gymconnectx-1.0.5/gymconnectx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 07:57:40.000000 gymconnectx-1.0.5/gymconnectx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:57:40.183795 gymconnectx-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 07:57:35.000000 gymconnectx-1.0.5/setup.py
```

### Comparing `gymconnectx-1.0.4/PKG-INFO` & `gymconnectx-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.4
+Version: 1.0.5
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
-        Copyright (c) 2024 AI Trafic Project
+        Copyright (c) 2024 Fauzi Sholichin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `gymconnectx-1.0.4/README.md` & `gymconnectx-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.4/gymconnectx/__init__.py` & `gymconnectx-1.0.5/gymconnectx/__init__.py`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.4/gymconnectx/envs/gymconnectxenv.py` & `gymconnectx-1.0.5/gymconnectx/envs/gymconnectxenv.py`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.4/gymconnectx.egg-info/PKG-INFO` & `gymconnectx-1.0.5/gymconnectx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.4
+Version: 1.0.5
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
-        Copyright (c) 2024 AI Trafic Project
+        Copyright (c) 2024 Fauzi Sholichin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
```

### Comparing `gymconnectx-1.0.4/pyproject.toml` & `gymconnectx-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gymconnectx"
-version = "1.0.4"
+version = "1.0.5"
 description = "An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N."
 readme = "README.md"
 authors = [{ name = "Fauzi Sholichin" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `gymconnectx-1.0.4/setup.py` & `gymconnectx-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gymconnectx',
-    version='1.0.4',
+    version='1.0.5',
     description='ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.',
     url='https://github.com/fauzisho/GymConnectX',
     author='Fauzi Sholichin',
     license='MIT License',
     packages=find_packages(),
     install_requires=['gym', 'pygame', 'numpy'],
     classifiers=[
```

