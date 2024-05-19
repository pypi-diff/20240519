# Comparing `tmp/colalamo-0.1.0.tar.gz` & `tmp/colalamo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colalamo-0.1.0.tar", last modified: Sun May 19 20:59:30 2024, max compression
+gzip compressed data, was "colalamo-0.1.1.tar", last modified: Sun May 19 21:08:48 2024, max compression
```

## Comparing `colalamo-0.1.0.tar` & `colalamo-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 20:59:30.385633 colalamo-0.1.0/
--rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 20:59:30.385021 colalamo-0.1.0/PKG-INFO
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 20:59:30.384361 colalamo-0.1.0/colalamo.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 20:59:30.000000 colalamo-0.1.0/colalamo.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      177 2024-05-19 20:59:30.000000 colalamo-0.1.0/colalamo.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 20:59:30.000000 colalamo-0.1.0/colalamo.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       43 2024-05-19 20:59:30.000000 colalamo-0.1.0/colalamo.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 20:59:30.000000 colalamo-0.1.0/colalamo.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)      775 2024-05-19 20:26:34.000000 colalamo-0.1.0/pyproject.toml
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 20:59:30.385738 colalamo-0.1.0/setup.cfg
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:08:48.505813 colalamo-0.1.1/
+-rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 21:08:48.505110 colalamo-0.1.1/PKG-INFO
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:08:48.504429 colalamo-0.1.1/colalamo.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      177 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       43 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)      778 2024-05-19 21:08:04.000000 colalamo-0.1.1/pyproject.toml
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 21:08:48.505927 colalamo-0.1.1/setup.cfg
```

### Comparing `colalamo-0.1.0/pyproject.toml` & `colalamo-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "colalamo"
-version = "0.1.0"
+version = "0.1.0001"
 description = "direct api via copilot to its large language models"
 authors = [
     { name = "tolitius" },
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["ai", "copilot", "github", "gpt", "openai", "code generation"]
```

