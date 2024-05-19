# Comparing `tmp/discorudo-1.5.tar.gz` & `tmp/discorudo-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discorudo-1.5.tar", last modified: Fri May 10 02:46:40 2024, max compression
+gzip compressed data, was "discorudo-1.6.tar", last modified: Sun May 19 13:16:26 2024, max compression
```

## Comparing `discorudo-1.5.tar` & `discorudo-1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-10 02:46:40.531108 discorudo-1.5/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-10 02:46:40.531108 discorudo-1.5/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2024-05-01 15:04:25.000000 discorudo-1.5/README.md
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-10 02:46:40.531108 discorudo-1.5/discorudo/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       75 2024-05-08 12:05:44.000000 discorudo-1.5/discorudo/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1027 2024-05-10 01:57:51.000000 discorudo-1.5/discorudo/main.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-10 02:46:40.531108 discorudo-1.5/discorudo.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-10 02:46:40.000000 discorudo-1.5/discorudo.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      222 2024-05-10 02:46:40.000000 discorudo-1.5/discorudo.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-10 02:46:40.000000 discorudo-1.5/discorudo.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2024-05-10 02:46:40.000000 discorudo-1.5/discorudo.egg-info/requires.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-05-10 02:46:40.000000 discorudo-1.5/discorudo.egg-info/top_level.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-10 02:46:40.531108 discorudo-1.5/setup.cfg
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2375 2024-05-10 02:46:27.000000 discorudo-1.5/setup.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-19 13:16:26.365017 discorudo-1.6/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-19 13:16:26.365017 discorudo-1.6/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       11 2024-05-01 15:04:25.000000 discorudo-1.6/README.md
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-19 13:16:26.361017 discorudo-1.6/discorudo/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       75 2024-05-08 12:05:44.000000 discorudo-1.6/discorudo/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1648 2024-05-19 13:15:52.000000 discorudo-1.6/discorudo/main.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-05-19 13:16:26.361017 discorudo-1.6/discorudo.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1096 2024-05-19 13:16:26.000000 discorudo-1.6/discorudo.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      222 2024-05-19 13:16:26.000000 discorudo-1.6/discorudo.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-05-19 13:16:26.000000 discorudo-1.6/discorudo.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       43 2024-05-19 13:16:26.000000 discorudo-1.6/discorudo.egg-info/requires.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       10 2024-05-19 13:16:26.000000 discorudo-1.6/discorudo.egg-info/top_level.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-05-19 13:16:26.365017 discorudo-1.6/setup.cfg
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2375 2024-05-19 13:16:14.000000 discorudo-1.6/setup.py
```

### Comparing `discorudo-1.5/PKG-INFO` & `discorudo-1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discorudo
-Version: 1.5
+Version: 1.6
 Summary: Just script on to discord
 Home-page: https://github.com/rizkychi/discorudo
 Author: rizkychi
 Author-email: rizkynhae@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/rizkychi/discorudo/
 Project-URL: Funding, https://www.paypal.me/rizkychi
```

### Comparing `discorudo-1.5/discorudo.egg-info/PKG-INFO` & `discorudo-1.6/discorudo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discorudo
-Version: 1.5
+Version: 1.6
 Summary: Just script on to discord
 Home-page: https://github.com/rizkychi/discorudo
 Author: rizkychi
 Author-email: rizkynhae@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/rizkychi/discorudo/
 Project-URL: Funding, https://www.paypal.me/rizkychi
```

### Comparing `discorudo-1.5/setup.py` & `discorudo-1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'discorudo',         # How you named your package folder (MyLib)
     packages = ['discorudo'],   # Chose the same as "name"
-    version = '1.5',      # Start with a small number and increase it with every change you make
+    version = '1.6',      # Start with a small number and increase it with every change you make
     license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description = 'Just script on to discord',   # Give a short description about your library
     long_description=long_description,            # Give a long description about your library
     long_description_content_type='text/markdown',
     author = 'rizkychi',                   # Type in your name
     author_email = 'rizkynhae@gmail.com',      # Type in your E-Mail
     url = 'https://github.com/rizkychi/discorudo',   # Provide either the link to your github or to your website
```

