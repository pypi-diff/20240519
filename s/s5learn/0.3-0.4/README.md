# Comparing `tmp/s5learn-0.3.tar.gz` & `tmp/s5learn-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.3.tar", last modified: Sun May 19 15:46:48 2024, max compression
+gzip compressed data, was "s5learn-0.4.tar", last modified: Sun May 19 21:03:50 2024, max compression
```

## Comparing `s5learn-0.3.tar` & `s5learn-0.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 15:46:48.403739 s5learn-0.3/
--rw-rw-rw-   0        0        0       52 2024-05-19 15:46:48.403739 s5learn-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 15:46:48.388119 s5learn-0.3/s5learn/
--rw-rw-rw-   0        0        0       24 2024-05-19 09:36:27.000000 s5learn-0.3/s5learn/__init__.py
--rw-rw-rw-   0        0        0      297 2024-05-19 15:46:02.000000 s5learn-0.3/s5learn/main.py
--rw-rw-rw-   0        0        0      192 2024-05-19 14:54:13.000000 s5learn-0.3/s5learn/printtext.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:46:48.403739 s5learn-0.3/s5learn.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-19 15:46:48.000000 s5learn-0.3/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-19 15:46:48.000000 s5learn-0.3/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 15:46:48.000000 s5learn-0.3/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 15:46:48.000000 s5learn-0.3/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 15:46:48.403739 s5learn-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-05-19 15:46:02.000000 s5learn-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:03:50.805904 s5learn-0.4/
+-rw-rw-rw-   0        0        0       52 2024-05-19 21:03:50.805904 s5learn-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 21:03:50.790275 s5learn-0.4/s5learn/
+-rw-rw-rw-   0        0        0       24 2024-05-19 09:36:27.000000 s5learn-0.4/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:03:50.790275 s5learn-0.4/s5learn/data/
+-rw-rw-rw-   0        0        0      158 2024-05-19 15:00:35.000000 s5learn-0.4/s5learn/data/example.txt
+-rw-rw-rw-   0        0        0      278 2024-05-19 21:03:30.000000 s5learn-0.4/s5learn/main.py
+-rw-rw-rw-   0        0        0      197 2024-05-19 20:43:52.000000 s5learn-0.4/s5learn/printtext.py
+drwxrwxrwx   0        0        0        0 2024-05-19 21:03:50.805904 s5learn-0.4/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-19 21:03:50.000000 s5learn-0.4/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2024-05-19 21:03:50.000000 s5learn-0.4/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 21:03:50.000000 s5learn-0.4/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 21:03:50.000000 s5learn-0.4/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 21:03:50.805904 s5learn-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1817 2024-05-19 20:57:56.000000 s5learn-0.4/setup.py
```

### Comparing `s5learn-0.3/setup.py` & `s5learn-0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
-    package_data={'': ['s5learn/example.txt']}
+    package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
 #
 # with open("README.md", "r", encoding="utf-8") as fh:
```

