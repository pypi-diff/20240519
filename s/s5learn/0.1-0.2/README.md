# Comparing `tmp/s5learn-0.1.tar.gz` & `tmp/s5learn-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.1.tar", last modified: Sun May 19 15:28:35 2024, max compression
+gzip compressed data, was "s5learn-0.2.tar", last modified: Sun May 19 15:41:42 2024, max compression
```

## Comparing `s5learn-0.1.tar` & `s5learn-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 15:28:35.981833 s5learn-0.1/
--rw-rw-rw-   0        0        0       52 2024-05-19 15:28:35.981833 s5learn-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 15:28:35.965513 s5learn-0.1/s5learn/
--rw-rw-rw-   0        0        0       24 2024-05-19 09:36:27.000000 s5learn-0.1/s5learn/__init__.py
--rw-rw-rw-   0        0        0      273 2024-05-19 15:00:35.000000 s5learn-0.1/s5learn/main.py
--rw-rw-rw-   0        0        0      192 2024-05-19 14:54:13.000000 s5learn-0.1/s5learn/printtext.py
-drwxrwxrwx   0        0        0        0 2024-05-19 15:28:35.981574 s5learn-0.1/s5learn.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-19 15:28:35.000000 s5learn-0.1/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-19 15:28:35.000000 s5learn-0.1/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 15:28:35.000000 s5learn-0.1/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-19 15:28:35.000000 s5learn-0.1/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 15:28:35.981833 s5learn-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1776 2024-05-19 15:27:52.000000 s5learn-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:41:42.246231 s5learn-0.2/
+-rw-rw-rw-   0        0        0       52 2024-05-19 15:41:42.238231 s5learn-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 15:41:42.220852 s5learn-0.2/s5learn/
+-rw-rw-rw-   0        0        0       24 2024-05-19 09:36:27.000000 s5learn-0.2/s5learn/__init__.py
+-rw-rw-rw-   0        0        0      287 2024-05-19 15:41:00.000000 s5learn-0.2/s5learn/main.py
+-rw-rw-rw-   0        0        0      192 2024-05-19 14:54:13.000000 s5learn-0.2/s5learn/printtext.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:41:42.238231 s5learn-0.2/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-19 15:41:41.000000 s5learn-0.2/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-19 15:41:41.000000 s5learn-0.2/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:41:41.000000 s5learn-0.2/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 15:41:41.000000 s5learn-0.2/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:41:42.246231 s5learn-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-05-19 15:41:00.000000 s5learn-0.2/setup.py
```

### Comparing `s5learn-0.1/setup.py` & `s5learn-0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.1',
-    packages=find_packages()
+    version='0.2',
+    packages=find_packages(),
+    package_data={'': ['s5learn/example.txt']}
 )
 
 
 
 # import setuptools
 #
 # with open("README.md", "r", encoding="utf-8") as fh:
```
