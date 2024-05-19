# Comparing `tmp/reasonify_headless-0.0.2.2.tar.gz` & `tmp/reasonify_headless-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasonify_headless-0.0.2.2.tar", last modified: Fri May 10 04:05:53 2024, max compression
+gzip compressed data, was "reasonify_headless-0.1.0a1.tar", last modified: Sat May 18 15:58:53 2024, max compression
```

## Comparing `reasonify_headless-0.0.2.2.tar` & `reasonify_headless-0.1.0a1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1154 2024-05-10 04:05:53.939738 reasonify_headless-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0       48 2024-03-25 14:26:26.453867 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/__init__.py
--rw-r--r--   0        0        0      292 2024-04-01 15:41:30.934449 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/__init__.py
--rw-r--r--   0        0        0     1209 2024-04-01 15:39:10.607693 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step2.py
--rw-r--r--   0        0        0     1410 2024-05-10 03:39:16.452275 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step3.py
--rw-r--r--   0        0        0     1274 2024-03-26 05:15:49.768522 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/core/step4.py
--rw-r--r--   0        0        0      177 2024-05-10 03:28:17.853720 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/models/tool.py
--rw-r--r--   0        0        0      403 2024-03-25 11:32:08.766310 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/showTools.j2
--rw-r--r--   0        0        0     1677 2024-03-28 04:46:45.440890 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step2.j2
--rw-r--r--   0        0        0      177 2024-03-30 10:40:21.464187 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step2schema.ts
--rw-r--r--   0        0        0     1242 2024-03-28 04:50:40.795708 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step3.j2
--rw-r--r--   0        0        0      582 2024-03-30 10:40:21.464187 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step3schema.ts
--rw-r--r--   0        0        0     1137 2024-03-29 15:06:27.426080 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4a.j2
--rw-r--r--   0        0        0     1010 2024-03-29 14:51:23.953890 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4b.j2
--rw-r--r--   0        0        0      299 2024-03-30 10:40:21.464187 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/templates/step4bschema.ts
--rw-r--r--   0        0        0     1797 2024-05-10 03:24:31.466362 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/context.py
--rw-r--r--   0        0        0     1503 2024-03-30 11:05:27.898676 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/globals.py
--rw-r--r--   0        0        0       79 2024-03-16 05:46:45.084890 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/resolve.py
--rw-r--r--   0        0        0      204 2024-03-25 02:21:06.206815 reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/serialize.py
--rw-r--r--   0        0        0      317 1970-01-01 00:00:00.000000 reasonify_headless-0.0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1265 2024-05-18 15:58:53.462361 reasonify_headless-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-18 14:42:45.806006 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/__init__.py
+-rw-r--r--   0        0        0     1971 2024-05-18 15:03:23.548088 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/core/loop.py
+-rw-r--r--   0        0        0      348 2024-05-18 12:18:56.296399 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-18 12:16:09.253962 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/async.yaml
+-rw-r--r--   0        0        0      123 2024-05-18 12:16:03.993009 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/date.yaml
+-rw-r--r--   0        0        0      242 2024-05-18 15:05:10.422652 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/dir.yaml
+-rw-r--r--   0        0        0      147 2024-05-18 12:16:05.843406 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/examples/simple_ask.yaml
+-rw-r--r--   0        0        0     1055 2024-05-18 12:25:22.346392 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/models/shot.py
+-rw-r--r--   0        0        0      555 2024-05-16 15:55:14.788440 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-16 13:17:52.325349 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/chat.j2
+-rw-r--r--   0        0        0     1461 2024-05-18 14:49:28.418853 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/templates/main.j2
+-rw-r--r--   0        0        0      242 2024-05-18 14:51:59.804762 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/tools/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-18 13:26:25.492016 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/tools/input.py
+-rw-r--r--   0        0        0      355 2024-05-18 15:12:45.200378 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/tools/install.py
+-rw-r--r--   0        0        0      308 2024-05-18 13:47:58.916781 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/component.py
+-rw-r--r--   0        0        0     1923 2024-05-18 13:59:37.528777 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/context.py
+-rw-r--r--   0        0        0      486 2024-05-18 10:41:25.594160 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/queue.py
+-rw-r--r--   0        0        0     1812 2024-05-18 15:20:17.969376 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/run.py
+-rw-r--r--   0        0        0      303 2024-05-16 13:05:09.591515 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/serialize.py
+-rw-r--r--   0        0        0      827 2024-05-18 15:24:29.535157 reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/tool.py
+-rw-r--r--   0        0        0      454 1970-01-01 00:00:00.000000 reasonify_headless-0.1.0a1/PKG-INFO
```

### Comparing `reasonify_headless-0.0.2.2/pyproject.toml` & `reasonify_headless-0.1.0a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [project]
 name = "reasonify-headless"
 description = "headless implementation for the Reasonify Agent"
 dynamic = []
-requires-python = ">=3.10"
+requires-python = ">=3.12"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
-    "promplate~=0.3.4.4",
+    "pyodide-py~=0.26.0a4 ; sys_platform != 'emscripten'",
+    "promplate~=0.3.4.5",
     "python-box~=7.1.1",
-    "promptools[validation]~=0.1.3.2",
+    "promptools[validation]~=0.1.3.4",
+    "promplate-recipes~=0.2.2.1",
+    "pyyaml~=6.0.1",
 ]
-version = "0.0.2.2"
+version = "0.1.0a1"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
@@ -36,15 +39,14 @@
 dev = [
     "black>=24.4.2",
     "isort>=5.13.2",
     "ruff>=0.4.4",
     "watchfiles>=0.21.0",
     "promplate-pyodide~=0.0.3.2",
     "micropip~=0.6.0",
-    "pyodide-py~=0.25.1",
     "webtypy~=0.1.7",
 ]
 
 [tool.pdm.scripts.fmt]
 composite = [
     "ruff check --fix --exit-zero",
     "isort .",
@@ -55,11 +57,12 @@
 cmd = [
     "watchfiles",
     "pdm build --no-sdist -d static/whl",
     "reasonify-headless",
 ]
 
 [tool.black]
-line-length = 120
+line-length = 150
 
 [tool.pyright]
 reportMissingModuleSource = false
+pythonVersion = "3.12"
```

### Comparing `reasonify_headless-0.0.2.2/reasonify-headless/reasonify/utils/context.py` & `reasonify_headless-0.1.0a1/reasonify-headless/reasonify/utils/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,23 @@
         super().__init__(context)
 
     @property
     def snapshots(self) -> list[dict]:
         return self["snapshots"]
 
     def __setitem__(self, key, value):
-        self.snapshots[0][key] = value
+        with suppress(IndexError):
+            self.snapshots[0][key] = value
         super().__setitem__(key, value)
 
+    def __delitem__(self, key: str):
+        with suppress(IndexError):
+            del self.snapshots[0][key]
+        super().__delitem__(key)
+
     def __getitem__(self, key: str):
         if key != "snapshots":
             for snapshot in self.snapshots:
                 if key in snapshot:
                     return snapshot[key]
         return super().__getitem__(key)
 
@@ -42,14 +48,14 @@
             try:
                 return extract_json(self.result, fallback, expect, allow_partial)
             except NameError:  # pydantic v1
                 # NameError: Field name "schema" shadows a BaseModel attribute; use a different field name with "alias='schema'".
                 return extract_json(self.result, fallback, allow_partial=allow_partial)
 
 
-def new_checkpoint(context: ChainContext, *, name: str | None = None):
+def new_checkpoint(context: ChainContext):
     c = Context(context)
     with suppress(KeyError):
         # log the raw result to the snapshot
         c["result"] = c.result
 
-    c.snapshots.insert(0, {} if name is None else {"step": name})
+    c.snapshots.insert(0, {})
```

