# Comparing `tmp/bip85-cli-0.0.1.tar.gz` & `tmp/bip85-cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bip85-cli-0.0.1.tar", last modified: Tue Sep 13 19:35:47 2022, max compression
+gzip compressed data, was "bip85-cli-0.0.2.tar", last modified: Sun May 19 19:16:57 2024, max compression
```

## Comparing `bip85-cli-0.0.1.tar` & `bip85-cli-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-13 19:35:47.598361 bip85-cli-0.0.1/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1072 2022-05-13 12:52:17.000000 bip85-cli-0.0.1/LICENSE
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3978 2022-09-13 19:35:47.598361 bip85-cli-0.0.1/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3510 2022-09-13 19:35:10.000000 bip85-cli-0.0.1/README.md
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-13 19:35:47.598361 bip85-cli-0.0.1/bip85_cli.egg-info/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3978 2022-09-13 19:35:47.000000 bip85-cli-0.0.1/bip85_cli.egg-info/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      278 2022-09-13 19:35:47.000000 bip85-cli-0.0.1/bip85_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2022-09-13 19:35:47.000000 bip85-cli-0.0.1/bip85_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       45 2022-09-13 19:35:47.000000 bip85-cli-0.0.1/bip85_cli.egg-info/entry_points.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       50 2022-09-13 19:35:47.000000 bip85-cli-0.0.1/bip85_cli.egg-info/requires.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       19 2022-09-13 19:35:47.000000 bip85-cli-0.0.1/bip85_cli.egg-info/top_level.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2114 2022-09-13 19:29:08.000000 bip85-cli-0.0.1/bip85_cli.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2022-09-13 19:35:47.598361 bip85-cli-0.0.1/bip85lib/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2022-09-13 19:26:58.000000 bip85-cli-0.0.1/bip85lib/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1954 2022-09-13 16:16:59.000000 bip85-cli-0.0.1/bip85lib/bip85.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2022-09-13 19:35:47.598361 bip85-cli-0.0.1/setup.cfg
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      996 2022-09-13 19:35:27.000000 bip85-cli-0.0.1/setup.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-19 19:16:57.428834 bip85-cli-0.0.2/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     1072 2024-05-19 19:06:10.000000 bip85-cli-0.0.2/LICENSE
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       16 2024-05-19 19:06:10.000000 bip85-cli-0.0.2/MANIFEST.in
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3978 2024-05-19 19:16:57.428834 bip85-cli-0.0.2/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3510 2024-05-19 19:06:10.000000 bip85-cli-0.0.2/README.md
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-19 19:16:57.428834 bip85-cli-0.0.2/bip85_cli.egg-info/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3978 2024-05-19 19:16:57.000000 bip85-cli-0.0.2/bip85_cli.egg-info/PKG-INFO
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      290 2024-05-19 19:16:57.000000 bip85-cli-0.0.2/bip85_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        1 2024-05-19 19:16:57.000000 bip85-cli-0.0.2/bip85_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       45 2024-05-19 19:16:57.000000 bip85-cli-0.0.2/bip85_cli.egg-info/entry_points.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       50 2024-05-19 19:16:57.000000 bip85-cli-0.0.2/bip85_cli.egg-info/requires.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       19 2024-05-19 19:16:57.000000 bip85-cli-0.0.2/bip85_cli.egg-info/top_level.txt
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     2114 2024-05-19 19:06:10.000000 bip85-cli-0.0.2/bip85_cli.py
+drwxr-xr-x   0 valerio   (1000) valerio   (1000)        0 2024-05-19 19:16:57.428834 bip85-cli-0.0.2/bip85lib/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)        0 2024-05-19 19:06:10.000000 bip85-cli-0.0.2/bip85lib/__init__.py
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     1954 2024-05-19 19:06:10.000000 bip85-cli-0.0.2/bip85lib/bip85.py
+-rw-r--r--   0 valerio   (1000) valerio   (1000)       38 2024-05-19 19:16:57.428834 bip85-cli-0.0.2/setup.cfg
+-rw-r--r--   0 valerio   (1000) valerio   (1000)      996 2024-05-19 19:11:04.000000 bip85-cli-0.0.2/setup.py
```

### Comparing `bip85-cli-0.0.1/LICENSE` & `bip85-cli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bip85-cli-0.0.1/PKG-INFO` & `bip85-cli-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bip85-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bip85 lib and cli written in python able to derive mnemonics from your master mnemonic.
 Home-page: https://github.com/valerio-vaccaro/bip85-utils
 Author: Valerio Vaccaro
 Author-email: valerio.vaccaro@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `bip85-cli-0.0.1/README.md` & `bip85-cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bip85-cli-0.0.1/bip85_cli.egg-info/PKG-INFO` & `bip85-cli-0.0.2/bip85_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bip85-cli
-Version: 0.0.1
+Version: 0.0.2
 Summary: Bip85 lib and cli written in python able to derive mnemonics from your master mnemonic.
 Home-page: https://github.com/valerio-vaccaro/bip85-utils
 Author: Valerio Vaccaro
 Author-email: valerio.vaccaro@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
```

### Comparing `bip85-cli-0.0.1/bip85_cli.py` & `bip85-cli-0.0.2/bip85_cli.py`

 * *Files identical despite different names*

### Comparing `bip85-cli-0.0.1/bip85lib/bip85.py` & `bip85-cli-0.0.2/bip85lib/bip85.py`

 * *Files identical despite different names*

### Comparing `bip85-cli-0.0.1/setup.py` & `bip85-cli-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name = 'bip85-cli',
-    version = '0.0.1',
+    version = '0.0.2',
     author = 'Valerio Vaccaro',
     author_email = 'valerio.vaccaro@gmail.com',
     license = 'MIT',
     description = 'Bip85 lib and cli written in python able to derive mnemonics from your master mnemonic.',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/valerio-vaccaro/bip85-utils',
```

