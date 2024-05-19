# Comparing `tmp/graphretrieval-0.1.1.tar.gz` & `tmp/graphretrieval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphretrieval-0.1.1.tar", last modified: Sun May 19 08:31:22 2024, max compression
+gzip compressed data, was "graphretrieval-0.1.2.tar", last modified: Sun May 19 08:50:19 2024, max compression
```

## Comparing `graphretrieval-0.1.1.tar` & `graphretrieval-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/GraphRetrieval/
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/GraphRetrieval/GraphRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/GraphRetrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/GraphRetrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 08:31:22.000000 graphretrieval-0.1.1/GraphRetrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:31:22.725243 graphretrieval-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-19 08:31:18.000000 graphretrieval-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:50:19.012166 graphretrieval-0.1.2/GraphRetrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/GraphRetrieval/GraphRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/GraphRetrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/GraphRetrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 08:50:19.000000 graphretrieval-0.1.2/GraphRetrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:50:19.016166 graphretrieval-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-19 08:50:14.000000 graphretrieval-0.1.2/setup.py
```

### Comparing `graphretrieval-0.1.1/GraphRetrieval/GraphRetrieval.py` & `graphretrieval-0.1.2/GraphRetrieval/GraphRetrieval.py`

 * *Files identical despite different names*

### Comparing `graphretrieval-0.1.1/README.rst` & `graphretrieval-0.1.2/README.rst`

 * *Files identical despite different names*

