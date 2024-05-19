# Comparing `tmp/graphretrieval-0.1.tar.gz` & `tmp/graphretrieval-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.tar", last modified: Sun May 19 07:47:23 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.1.tar", last modified: Sun May 19 08:31:22 2024, max compression
```

## Comparing `graphretrieval-0.1.tar` & `graphretrieval-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:47:23.570734 graphretrieval-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:47:23.570734 graphretrieval-0.1/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-19 07:47:19.000000 graphretrieval-0.1/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 07:47:19.000000 graphretrieval-0.1/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:47:23.570734 graphretrieval-0.1/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-19 07:47:23.000000 graphretrieval-0.1/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-19 07:47:23.000000 graphretrieval-0.1/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:47:23.000000 graphretrieval-0.1/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 07:47:23.000000 graphretrieval-0.1/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 07:47:23.000000 graphretrieval-0.1/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-19 07:47:23.570734 graphretrieval-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-19 07:47:19.000000 graphretrieval-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:47:23.570734 graphretrieval-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 07:47:19.000000 graphretrieval-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/setup.py
```

### Comparing `graphretrieval-0.1/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.1/GraphRetrieval/GraphRetrieval.py`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1/setup.py` & `graphretrieval-0.1.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup, find_packages
 
+long_description = """
+### Graph Retrieval
+"""
+
 setup(
     name='GraphRetrieval',
-    version='0.1',
+    version='0.1.1',
     description='Graph retrieval',
-    long_description='Graph retrieval',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='JVNK',
     author_email='jaya11vibhav@gmail.com',
     url='https://github.com/jayavibhavnk/GraphRetrieval',
     packages=find_packages(),
     install_requires=[
       'langchain_openai',
       'langchain',
```

