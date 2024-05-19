# Comparing `tmp/reasonify_headless-0.1.0a1.tar.gz` & `tmp/reasonify_headless-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.1.0a1.tar", last modified: Sat May 18 15:58:53 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a2.tar", last modified: Sun May 19 13:47:54 2024, max compression
```

## Comparing `reasonify_headless-0.1.0a1.tar` & `reasonify_headless-0.1.0a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1265 2024-05-18 15:58:53.462361 reasonify_headless-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0     1971 2024-05-18 15:03:23.548088 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/core/loop.py
--rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/__init__.py
--rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/async.yaml
--rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/date.yaml
--rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/dir.yaml
--rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/simple_ask.yaml
--rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/models/shot.py
--rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/__init__.py
--rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/chat.j2
--rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/main.j2
--rw-r--r--   0        0        0      242 2024-05-18 14:51:59.804762 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/tools/__init__.py
--rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/tools/input.py
--rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/tools/install.py
--rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/component.py
--rw-r--r--   0        0        0     1923 2024-05-18 13:59:37.528777 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/queue.py
--rw-r--r--   0        0        0     1812 2024-05-18 15:20:17.969376 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/run.py
--rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/tool.py
--rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1231 2024-05-19 13:47:54.020065 reasonify_headless-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     1971 2024-05-18 15:03:23.548088 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      242 2024-05-19 12:29:46.617624 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     1923 2024-05-18 13:59:37.528777 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1812 2024-05-18 15:20:17.969376 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a2/PKG-INFO
```

### Comparing `reasonify_headless-0.1.0a1/pyproject.toml` & `reasonify_headless-0.1.0a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "pyodide-py~=0.26.0a4 ; sys_platform != 'emscripten'",
     "promplate~=0.3.4.5",
     "python-box~=7.1.1",
     "promptools[validation]~=0.1.3.4",
     "promplate-recipes~=0.2.2.1",
     "pyyaml~=6.0.1",
 ]
-version = "0.1.0a1"
+version = "0.1.0a2"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -37,15 +37,14 @@
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=24.4.2",
     "isort>=5.13.2",
     "ruff>=0.4.4",
     "watchfiles>=0.21.0",
-    "promplate-pyodide~=0.0.3.2",
     "micropip~=0.6.0",
     "webtypy~=0.1.7",
 ]
 
 [tool.pdm.scripts.fmt]
 composite = [
     "ruff check --fix --exit-zero",
```

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/core/loop.py` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/core/loop.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/async.yaml` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/examples/async.yaml`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/models/shot.py` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/models/shot.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/__init__.py` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/main.j2` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/templates/main.j2`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/context.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/run.py` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/run.py`

 * *Files identical despite different names*

### Comparing `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/tool.py` & `reasonify_headless-0.1.0a2/reasonify-headless/reasonify/utils/tool.py`

 * *Files identical despite different names*

