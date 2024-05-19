# Comparing `tmp/colalamo-0.1.1.tar.gz` & `tmp/colalamo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colalamo-0.1.1.tar", last modified: Sun May 19 21:08:48 2024, max compression
+gzip compressed data, was "colalamo-0.1.2.tar", last modified: Sun May 19 21:13:18 2024, max compression
```

## Comparing `colalamo-0.1.1.tar` & `colalamo-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:08:48.505813 colalamo-0.1.1/
--rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 21:08:48.505110 colalamo-0.1.1/PKG-INFO
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:08:48.504429 colalamo-0.1.1/colalamo.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      177 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       43 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:08:48.000000 colalamo-0.1.1/colalamo.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)      778 2024-05-19 21:08:04.000000 colalamo-0.1.1/pyproject.toml
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 21:08:48.505927 colalamo-0.1.1/setup.cfg
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:13:18.816842 colalamo-0.1.2/
+-rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 21:13:18.816164 colalamo-0.1.2/PKG-INFO
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-05-19 21:13:18.815584 colalamo-0.1.2/colalamo.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      506 2024-05-19 21:13:18.000000 colalamo-0.1.2/colalamo.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      177 2024-05-19 21:13:18.000000 colalamo-0.1.2/colalamo.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:13:18.000000 colalamo-0.1.2/colalamo.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       52 2024-05-19 21:13:18.000000 colalamo-0.1.2/colalamo.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-05-19 21:13:18.000000 colalamo-0.1.2/colalamo.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)      787 2024-05-19 21:12:55.000000 colalamo-0.1.2/pyproject.toml
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-05-19 21:13:18.816974 colalamo-0.1.2/setup.cfg
```

### Comparing `colalamo-0.1.1/pyproject.toml` & `colalamo-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "colalamo"
-version = "0.1.0001"
+version = "0.1.0002"
 description = "direct api via copilot to its large language models"
 authors = [
     { name = "tolitius" },
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 keywords = ["ai", "copilot", "github", "gpt", "openai", "code generation"]
 
 dependencies = []
 
 [project.scripts]
-colalamo = "colalamo:main"
+colalamo = "colalamo.colalamo:main"
 
 [project.urls]
 Homepage = "https://github.com/tolitius/colalamo"
 Documentation = "https://github.com/tolitius/colalamo?tab=readme-ov-file#-colalamo"
 Repository = "https://github.com/tolitius/colalamo"
 Issues = "https://github.com/tolitius/colalamo/issues"
```

