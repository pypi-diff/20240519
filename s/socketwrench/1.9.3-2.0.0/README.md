# Comparing `tmp/socketwrench-1.9.3.tar.gz` & `tmp/socketwrench-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.9.3.tar", last modified: Fri May 17 21:43:21 2024, max compression
+gzip compressed data, was "socketwrench-2.0.0.tar", last modified: Sat May 18 22:54:23 2024, max compression
```

## Comparing `socketwrench-1.9.3.tar` & `socketwrench-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.925437 socketwrench-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-17 21:43:17.000000 socketwrench-1.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 21:43:17.000000 socketwrench-1.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-17 21:43:21.925437 socketwrench-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-17 21:43:17.000000 socketwrench-1.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-17 21:43:17.000000 socketwrench-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:43:21.925437 socketwrench-1.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.917437 socketwrench-1.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.921437 socketwrench-1.9.3/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    30750 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.921437 socketwrench-1.9.3/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.921437 socketwrench-1.9.3/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.921437 socketwrench-1.9.3/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    30762 2024-05-17 21:43:17.000000 socketwrench-1.9.3/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:43:21.921437 socketwrench-1.9.3/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-17 21:43:21.000000 socketwrench-1.9.3/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 21:43:21.000000 socketwrench-1.9.3/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:43:21.000000 socketwrench-1.9.3/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 21:43:21.000000 socketwrench-1.9.3/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.267316 socketwrench-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-18 22:54:18.000000 socketwrench-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-18 22:54:18.000000 socketwrench-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-05-18 22:54:23.267316 socketwrench-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-05-18 22:54:18.000000 socketwrench-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-18 22:54:18.000000 socketwrench-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:54:23.267316 socketwrench-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.259316 socketwrench-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.263316 socketwrench-2.0.0/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.263316 socketwrench-2.0.0/src/socketwrench/fake_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/fake_imports/fake_traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35334 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/public.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.263316 socketwrench-2.0.0/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.263316 socketwrench-2.0.0/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.267316 socketwrench-2.0.0/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/standardlib_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33772 2024-05-18 22:54:18.000000 socketwrench-2.0.0/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:54:23.267316 socketwrench-2.0.0/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15531 2024-05-18 22:54:23.000000 socketwrench-2.0.0/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-18 22:54:23.000000 socketwrench-2.0.0/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:54:23.000000 socketwrench-2.0.0/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-18 22:54:23.000000 socketwrench-2.0.0/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.9.3/LICENSE` & `socketwrench-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/PKG-INFO` & `socketwrench-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,9 @@
-Metadata-Version: 2.1
-Name: socketwrench
-Version: 1.9.3
-Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
-Author-email: Torin Halsted <modularizer@gmail.com>
-License: This is free and unencumbered software released into the public domain.
-        
-        Anyone is free to copy, modify, publish, use, compile, sell, or
-        distribute this software, either in source code form or as a compiled
-        binary, for any purpose, commercial or non-commercial, and by any
-        means.
-        
-        In jurisdictions that recognize copyright laws, the author or authors
-        of this software dedicate any and all copyright interest in the
-        software to the public domain. We make this dedication for the benefit
-        of the public at large and to the detriment of our heirs and
-        successors. We intend this dedication to be an overt act of
-        relinquishment in perpetuity of all present and future rights to this
-        software under copyright law.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-        IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-        OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-        ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-        OTHER DEALINGS IN THE SOFTWARE.
-        
-        For more information, please refer to <https://unlicense.org>
-Project-URL: Homepage, https://github.com/modularizer/socketwrench
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # socketwrench
-A webserver based on `socket.socket` with no dependencies other than the standard library.
+A webserver based on `socket.socket` with no dependencies whatsoever other **socket** (or a substitute you pass in ) and **optional** standard library dependencies which improve features. See [dependencies](#dependencies) for more info.
 Provides a lightweight quickstart to make an API which supports OpenAPI, Swagger, and more.
 
 ## NOTE:
 this is **not** a production-ready web server. It is a learning tool and a lightweight way to make a simple API. While I attempted to reduce overhead in calls, I haven't taken time to thoroughly optimize, and I have not implemented any complex features to deal with security, performance, or scalability.
 
 ## Project Goals
 Part of the goal of this project was to understand how web servers work and to make a simple web server that is easy to use and understand.
@@ -61,15 +25,15 @@
 class MyServer:
     src = StaticFileHandler(Path(__file__).parent.parent.parent)
     
     def hello(self):
         return "world"
   
 if __name__ == '__main__':
-    serve(MyServer)
+    serve(MyServer, thread=True)
     # OR
     # m = MyServer()
     # serve(m)
     # OR
     # serve("my_module.MyServer")
 ```
 * Go to http://localhost:8080/hello and see the response "world".
@@ -143,31 +107,83 @@
 
 ### favicon.ico
 No need to use our favicon! pass a `str | Path` `.ico` filepath to `favicon` argument to use your own favicon. Alternatively, tag `@route('/favicon.ico')` on a function returning the path.
 
 ### fallback handler
 Add a custom function to handle any requests that don't match any other routes.
 
+# Dependencies
+Default behavior is to use the standard library only. However, if you do not have the full standard library, socketwrench _should_ still work.
+This is a work in progress as I am attempting to support micropython, circuitpython, etc. but I have not tested on these environments yet.
+
+### How it works:
+* `socket.socket` is the only required dependency, BUT you can pass in a substitute socket object if you want.
+* The following standard library modules are used, BUT if import fails for any of them we fall back on dump fake versions I made in [src/socketwrench/fake_imports](.src/socketwrench/fake_imports) which attempt to approximate the same functionality
+```python
+import socket
+
+import builtins  # very niche case use for if a function is typehinted to accept a type, e.g. `def f(x: type):` and you pass in the type name via a string query e.g. `?x=int`
+import inspect  # used often for getting function signatures, autofilling parameters, etc., spoof version uses `__annotations__` and `__defaults__` of functions
+from sys import argv # only used in commandline mode
+from argparse import ArgumentParser # only used in commandline mode
+from tempfile import TemporaryFile # only used if you attempt to return a folder using a StaticFileHandler
+from zipfile import ZipFile # only used if you attempt to return a folder using a StaticFileHandler
+from functools import wraps, partial # used regularly but easily replaced
+import dataclasses # only used if your python function returns a dataclass which we try to coerce to json
+from datetime import datetime  # used for Last-Modified header of File responses
+from pathlib import Path # used for file responses and static file serving, spoof version works okay
+from json import dumps, loads # used for json responses, spoof version works okay
+import logging # used for logging, spoof version works okay
+from time import sleep # only used if pause_sleep > 0 or accept_sleep > 0, spoof version does not sleep at all
+from threading import Event, Thread # only used if you `thread=True` in `serve` function (defaults to False)
+from traceback import format_exception  # only used if error_mode="traceback"
+import importlib # only used if you pass a string into the serve module as the item to be served, e.g. in commandline mode
+from sys import modules # only used if you pass a string into the serve module as the item to be served, e.g. in commandline mode
+```
+
+### sample
+```python
+from socketwrench import serve
+import socket
+
+class Sample:
+    def hello(self):
+        return "world"
+
+if __name__ == '__main__':
+    serve(Sample, spoof_modules="all", thread=True, socket=socket, port=8123)
+```
+
 # Planned Features
-* [ ] Implement nesting / recursion to serve deeper routes and/or multiple classes
+* [x] Implement nesting / recursion to serve deeper routes and/or multiple classes
+* [x] support default navigation pages to help show links to available routes
 * [ ] Enforce OpenAPI spec with better error responses
 * [x] Serve static folders
 * [x] Make a better playground for testing endpoints
   * [ ] better preview of variadic routes
 * [ ] improve docs
   * [ ] document variadic routes
   * [ ] document autofilled parameters
   * [ ] document decorators
   * [ ] document error modes
   * [ ] document static file serving
   * [ ] document favicon
   * [ ] document fallback handler
   * [ ] document regexp / match routes
 * [ ] Make a client-side python proxy object to make API requests from python
+
+### Environment Support
+* [x] Remove `|` typehints to allow for older python versions :/ (this makes me sad)
+* [x] Remove standard library dependencies which microcontrollers may not have
+* [x] Allow passing in a socket object
+  * [ ] test and support different kinds of sockets and objects pretending to be sockets
 * [ ] Test on ESP32 and other microcontrollers
+* [ ] Test in browser-based python environments using pyodide
+
+### Other
 * [ ] Ideas? Let me know!
 
 # Other Usage Modes
 ### Serve a module
 Using commandline, just specify a filepath or file import path to a module.
 ```python
 # my_module.py
@@ -333,8 +349,8 @@
     from socketwrench import serve
     s = Sample()
     serve(s)
     # OR
     # serve(Sample)
     # OR
     # serve("socketwrench.samples.sample.Sample")
-```
+```
```

### Comparing `socketwrench-1.9.3/pyproject.toml` & `socketwrench-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.9.3"
+version = "2.0.0"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.9.3/src/socketwrench/__init__.py` & `socketwrench-2.0.0/src/socketwrench/public.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/__main__.py` & `socketwrench-2.0.0/src/socketwrench/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from socketwrench.server import Server
 
 
 def main():
-    import argparse
-    parser = argparse.ArgumentParser(description="Serve a module or class.")
+    from socketwrench.standardlib_dependencies import ArgumentParser
+    parser = ArgumentParser(description="Serve a module or class.")
     parser.add_argument("module_or_class", help="The module or class to serve.")
     # add help text for the other arguments
     parser.add_argument("--host", help="The host to bind to.", default="*", type=str)
     parser.add_argument("--port", help="The port to bind to.", default=8080, type=int)
     parser.add_argument("--errors", help="The error mode to use.", default="hide", type=str, choices=["hide", "short", "show", "tb","traceback"])
 
     args = parser.parse_args()
     Server.serve(args.module_or_class, host=args.host, port=args.port, error_mode=args.errors)
 
 
 if __name__ == '__main__':
-    import sys
-    if len(sys.argv) != 2:
+    from socketwrench.standardlib_dependencies import argv
+    if len(argv) != 2:
         print("Usage: python -m socketwrench <import.path.of.module.or.class>")
         print("Example: python -m socketwrench socketwrench.samples.sample.Sample")
         print(f"Sample Shortcut: python -m socketwrench sample")
-        sys.exit(1)
-    m = sys.argv[1]
+        exit(1)
+    m = argv[1]
     if m == "sample":
         m = "socketwrench.samples.sample.Sample"
     Server.serve(m)
```

### Comparing `socketwrench-1.9.3/src/socketwrench/connection.py` & `socketwrench-2.0.0/src/socketwrench/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import socket
-import logging
+from socketwrench.standardlib_dependencies import (
+    logging,
+    socket,
+)
 
 from socketwrench.types import Request, Response
 
 logger = logging.getLogger("socketwrench")
 
 
 class Connection:
@@ -11,34 +13,39 @@
     timeout = 5
 
     def __init__(self,
                  handler,
                  connection_socket: socket.socket,
                  client_address: tuple,
                  cleanup_event,
-                 chunk_size: int = default_chunk_size):
+                 chunk_size: int = default_chunk_size,
+                 origin: str = ""):
         self.socket = connection_socket
         self.client_addr = client_address
         self.chunk_size = chunk_size
         self.cleanup_event = cleanup_event
         self.handler = handler
+        self.origin = origin
 
         self._rep = None
 
     def handle(self):
         try:
             request = self.receive_request(self.socket)
             if self.check_cleanup():
                 return request, None, False
+            logger.debug(str(request))
             response = self.handler(request)
+            logger.log(9, f"\t\t{response}")
             if self.check_cleanup():
                 return request, response, False
             self.send_response(self.socket, response)
             return request, response, True
         except Exception as e:
+            logger.error(f"Error handling request: {e}")
             self.close()
             raise e
 
     def receive_request(self, connection_socket: socket.socket, chunk_size: int = None) -> Request:
         connection_socket.settimeout(self.timeout)
         if chunk_size is None:
             chunk_size = self.chunk_size
@@ -62,15 +69,15 @@
         if b'Content-Length:' in pre_body_bytes:
             length = int(pre_body_bytes.split(b'Content-Length: ')[1].split(new_line)[0])
             while len(body) < length and not self.cleanup_event or not self.cleanup_event.is_set():
                 body += connection_socket.recv(chunk_size)
         else:
             body = b''
 
-        r = Request.from_components(pre_body_bytes, body, self.client_addr, self.socket)
+        r = Request.from_components(pre_body_bytes, body, self.client_addr, self.socket, origin=self.origin)
         return r
 
     def send_response(self, connection_socket: socket.socket, response: Response):
         connection_socket.sendall(bytes(response))
         connection_socket.shutdown(socket.SHUT_WR) # seems to be needed for linux?
         connection_socket.close()
 
@@ -88,7 +95,8 @@
         if self._rep is None:
             r = ""
             if self.chunk_size != self.default_chunk_size:
                 r += f", chunk_size={self.chunk_size}"
 
             self._rep = f'<{self.__class__.__name__}({self.socket}, {self.client_addr}, {self.cleanup_event}{r})>'
         return self._rep
+
```

### Comparing `socketwrench-1.9.3/src/socketwrench/handlers.py` & `socketwrench-2.0.0/src/socketwrench/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import inspect
-import json
-import builtins
-import logging
-import traceback
-from contextlib import suppress
-from functools import wraps
-from pathlib import Path
-import socket
+from socketwrench.standardlib_dependencies import (
+    builtins,
+    inspect,
+    loads,
+    logging,
+    Path,
+    socket,
+    wraps
+)
 
 from socketwrench.tags import tag, get, gettag
 from socketwrench.types import Request, Response, Query, Body, Route, FullPath, Method, File, ClientAddr, \
-    HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, HTMLResponse, url_decode, StandardHTMLResponse
+    HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, url_decode, StandardHTMLResponse
 
 logger = logging.getLogger("socketwrench")
 
 
 class Autofill:
     def request(self, request: Request) -> Request:
         return request
@@ -84,74 +84,74 @@
             pass
     return False
 
 def _typehint_matches(typehint, others):
     return typehint in others or tryissubclass(typehint, others) or (hasattr(typehint, "__origin__") and typehint.__origin__ in others) or (hasattr(typehint, "__args__") and any(_typehint_matches(t, others) for t in typehint.__args__))
 
 
-def cast_to_typehint(value: str, typehint = inspect._empty):
+def cast_to_typehint(value: str, typehint = inspect.Parameter.empty):
 
     # unless specifically typed as a string, cast any numeric value to int or float
-    if _typehint_matches(typehint, [int, inspect._empty]):
+    if _typehint_matches(typehint, [int, inspect.Parameter.empty]):
         if value.isdigit() or (value.startswith("-") and value[1:].isdigit())  and not '.' in value:
             return int(value)
-    if _typehint_matches(typehint, [float, inspect._empty]):
+    if _typehint_matches(typehint, [float, inspect.Parameter.empty]):
         if value.isdigit() or (value.startswith("-") and value[1:].isdigit()):
             return float(value)
-    if _typehint_matches(typehint, [bool, inspect._empty]):
+    if _typehint_matches(typehint, [bool, inspect.Parameter.empty]):
         if value.lower() in ["false", "f", "no", "n"]:
             return False
         if value.lower() in ["true", "t", "yes", "y"]:
             return True
     if value.lower() in ["none", "null"] and (_typehint_matches(typehint, [None]) or not _typehint_matches(typehint, [str])):
         return None
     if _typehint_matches(typehint, [bool]):
         if value.lower() in ["0"]:
             return False
         if value.lower() in ["1", "ok"]:
             return True
-    if _typehint_matches(typehint, [list, inspect._empty]):
+    if _typehint_matches(typehint, [list, inspect.Parameter.empty]):
         if value.startswith("[") and value.endswith("]"):
             try:
-                return json.loads(value)
+                return loads(value)
             except:
                 pass
-    if _typehint_matches(typehint, [tuple, inspect._empty]):
+    if _typehint_matches(typehint, [tuple, inspect.Parameter.empty]):
         if value.startswith("(") and value.endswith(")"):
             try:
                 s = '[' + value[1:-1] + ']'
-                return tuple(json.loads(s))
+                return tuple(loads(s))
             except:
                 pass
-    if _typehint_matches(typehint, [dict, inspect._empty]):
+    if _typehint_matches(typehint, [dict, inspect.Parameter.empty]):
         if value.startswith("{") and value.endswith("}"):
             try:
-                return json.loads(value)
+                return loads(value)
             except:
                 pass
     if _typehint_matches(typehint, [frozenset]):
         if value.startswith("{") and value.endswith("}"):
             try:
-                return frozenset(json.loads('[' + value[1:-1] + ']'))
+                return frozenset(loads('[' + value[1:-1] + ']'))
             except:
                 pass
-    if _typehint_matches(typehint, [set, inspect._empty]):
+    if _typehint_matches(typehint, [set, inspect.Parameter.empty]):
         if value.startswith("{") and value.endswith("}"):
             try:
-                return set(json.loads('[' + value[1:-1] + ']'))
+                return set(loads('[' + value[1:-1] + ']'))
             except:
                 pass
     if typehint is bytes or tryissubclass(typehint, bytes):
         return value.encode()
     if typehint is bytearray or tryissubclass(typehint, bytearray):
         return bytearray(value.encode())
     if typehint is memoryview or tryissubclass(typehint, memoryview):
         return memoryview(value.encode())
     if typehint is type:
-        if hasattr(builtins, value):
+        if builtins and hasattr(builtins, value):
             return getattr(builtins, value)
         return globals().get(value, value)
     if hasattr(typehint, "__origin__"):
         if typehint.__origin__ in [list, tuple, set, frozenset]:
             return typehint([cast_to_typehint(v, typehint.__args__[0]) for v in value])
         return cast_to_typehint(value, typehint.__origin__)
     return value
@@ -165,15 +165,14 @@
                 query[param_name] = cast_to_typehint(param_value, typehint)
             except:
                 pass
     return query
 
 
 def preprocess_args(_handler):
-    import inspect
     sig = inspect.signature(_handler)
 
     # make sure the handler doesn't use "args" unless as *args
     if "args" in sig.parameters and sig.parameters["args"].kind != inspect.Parameter.VAR_POSITIONAL:
         raise ValueError("The handler cannot use 'args' as a parameter unless as *args.")
 
     # make sure the handler doesn't use "kwargs" unless as **kwargs
@@ -193,15 +192,15 @@
     for name, param in sig.parameters.items():
         ind += 1
 
         if param.annotation in available_type_values:
             i = available_type_values.index(param.annotation)
             key = available_type_keys[i]
             special_params[key].append(name)
-        elif param.annotation is inspect._empty and param.name in available_types:
+        elif param.annotation is inspect.Parameter.empty and param.name in available_types:
             special_params[param.name].append(name)
         elif param.name in available_types:
             a = param.annotation
             t = available_types[param.name]
             if isinstance(a, str):
                 if a != t.__name__ and a not in [_t.__name__ for _t in t.__subclasses()]:
                     raise ValueError(f"Parameter '{param.name}' of {_handler} must be typed as {available_types[param.name]}, not {param.annotation}.")
@@ -243,15 +242,15 @@
                 args.append(v)
             q = cast_to_types(q, sig.parameters)
             kwargs.update(q)
 
         b = request.body
         if b:
             try:
-                body = json.loads(b.decode())
+                body = loads(b.decode())
                 int_keys = sorted([int(k) for k in body if k.isdigit()])
                 if set(int_keys) != set(range(len(args), len(args) + len(int_keys))):
                     raise ValueError("Unable to parse args.")
                 for k in int_keys:
                     args.append(body.pop(str(k)))
                 kwargs.update(body)
             except:
@@ -284,14 +283,15 @@
         try:
             if parser is None:
                 r = _handler()
                 response = Response(r, version=request.version)
             else:
                 a, kw, return_annotation = parser(request, route_params=route_params)
                 r = _handler(*a, **kw)
+                print(f"{r=}, {type(r)}")
                 if isinstance(r, Response):
                     response = r
                 elif isinstance(r, HTTPStatusCode):
                     response = Response(r.phrase(), status_code=r, version=request.version)
                 else:
                     try:
                         if (not isinstance(return_annotation, str)) and issubclass(return_annotation, Response):
@@ -306,16 +306,22 @@
             if _error_mode == ErrorModes.HIDE:
                 msg = b'Internal Server Error'
             elif _error_mode == ErrorModes.TYPE:
                 msg = str(type(e)).encode()
             elif _error_mode == ErrorModes.SHORT:
                 msg = str(e).encode()
             elif _error_mode == ErrorModes.LONG:
-                msg = traceback.format_exc().encode()
-            response = ErrorResponse(msg, version=request.version)
+                from socketwrench.standardlib_dependencies import format_exception
+                tb = format_exception(type(e), e, e.__traceback__)
+                # trim the first part of the traceback which just shows socketwrench internals _handler(*a, **kw)
+                tb = ([tb[0]] if tb else [b"Internal Server Error"]) + tb[2:]
+                msg = "".join(tb)
+                if len(msg.splitlines()) == 2:
+                    msg = msg.splitlines()[1]
+            response = ErrorResponse(msg.encode(), version=request.version)
         return response
 
     tag(wrapper,
         is_wrapped=True,
         sig=getattr(parser, "sig", inspect.signature(_handler)),
         autofill=getattr(parser, "autofill", {}), **_handler.__dict__)
 
@@ -332,26 +338,25 @@
         raise NotImplementedError
 
 
 class StaticFileHandler(MatchableHandlerABC):
     is_wrapped = True
     allowed_methods = ["GET", "HEAD"]
 
-    def __init__(self, path: Path | str, route: str = None):
+    def __init__(self, path, route: str = None):
         self.path = path
         self.route = route or "/" + path.name
         self.allowed_methods = ["GET", "HEAD"]
 
     def match(self, route: str) -> bool:
         if not route.startswith(self.route):
             return False
         added = route[len(self.route):]
         p = (self.path / added.strip("/")) if added else self.path
         if not p.exists():
-            print("path doesn't exist", p, route, added)
             return False
         return True
 
     def __call__(self, request: Request) -> Response:
         route = request.path.route()
         if not route.startswith(self.route):
             return Response(b"Not Found", status_code=404, version=request.version)
@@ -363,15 +368,14 @@
         if not p.exists():
             return Response(b"Not Found", status_code=404, version=request.version)
         elif p.is_dir():
             folder_contents = list(p.iterdir())
             contents = "<!DOCTYPE html><html><body><ul>" + "\n".join([f"<li><a href='{route}/{f.name}'>{f.name}</a></li>" for f in folder_contents]) + "</ul></body></html>"
             return Response(contents.encode(), version=request.version)
         r = FileResponse(p, version=request.version)
-        print("content type", r.headers.get("Content-Type"))
         return r
 
 
 def matches_variadic_route(route: str, variadic_route: str) -> dict:
     try:
         if route.endswith("/") and not variadic_route.endswith("/"):
             route = route[:-1]
@@ -447,20 +451,21 @@
                             raise ValueError(f"Expected {section['value']} but got {nv}")
                         nonvariadic_start = nonvariadic_end
                 if sections[-1]["variadic"]:
                     variables[variadic_name] = r[nonvariadic_end:]
                 elif nonvariadic_end < len(r):
                     return False
                 found_matches.update(variables)
+
+
         return found_matches
     except Exception as e:
-        print("Error", e)
-        print(str(traceback.format_exc()))
         return False
 
+
 def sort_variadic_routes(patterns):
     q = []
     for pattern in patterns:
         parts = pattern.split("/")
         part_count = len(parts)
         variadic_part_count = len([p for p in parts if "{" in p and "}" in p])
         nonvariadic_part_count = part_count - variadic_part_count
@@ -499,20 +504,20 @@
 
 class RouteHandler:
     resources_folder = Path(__file__).parent / "resources"
     playground_folder = resources_folder / "playground"
     default_favicon = resources_folder / "favicon.ico"
 
     def __init__(self,
-                 routes: dict | None = None,
+                 routes: dict = None,
                  fallback_handler=None,
                  base_path: str = "/",
                  require_tag: bool = False,
-                 error_mode: str = ErrorModes.HIDE,
-                 favicon: str | None = default_favicon,
+                 error_mode: str = None,
+                 favicon: str = default_favicon,
                  nav_path = "/",
                  nav_recursion = True,
                  ):
         base_path = base_path.replace("//", "/")
         if not base_path.endswith("/"):
             base_path += "/"
         self.base_path = base_path
@@ -534,25 +539,26 @@
                 "error_mode": error_mode,
                 "require_tag": require_tag,
                 "nav_path": nav_path,
                 "nav_recursion": nav_recursion,
             }
             if isinstance(routes, dict):
                 for k, v in routes.items():
-                    sub = self.base_path + (k[1:] if k.startswith("/") else k) + ("/" if not k.endswith("/") else "")
+                    sub = self.base_path + (k[1:] if k.startswith("/") else k) + "/"
                     sub = sub.replace("//", "/")
 
                     if isinstance(v, type):
-                        self.sub_route_handlers[sub] = RouteHandler(v(), base_path=sub, **kw)
+                        self._add_subroute(sub, RouteHandler(v(), base_path=sub, **kw))
                     elif isinstance(v, RouteHandler):
-                        self.sub_route_handlers[sub] = v
+                        v.base_path = sub
+                        self._add_subroute(sub, v)
                     elif isinstance(v, dict):
-                        self.sub_route_handlers[sub] = RouteHandler(v, base_path=sub, **kw)
+                        self._add_subroute(sub, RouteHandler(v, base_path=sub, **kw))
                     elif is_object_instance(v):
-                        self.sub_route_handlers[sub] = RouteHandler(v, base_path=sub, **kw)
+                        self._add_subroute(sub, RouteHandler(v, base_path=sub, **kw))
                     else:
                         self[k] = v
             else:
                 self.parse_routes_from_object(routes)
         self.fallback_handler = wrap_handler(fallback_handler) if fallback_handler else None
 
         op = wrap_handler(self.openapi, error_mode=error_mode)
@@ -567,14 +573,25 @@
             "/api": wrap_handler(self.playground, error_mode=error_mode),
             "/api/playground.js": wrap_handler(self.playground_js, error_mode=error_mode),
             "/api/panels.js": wrap_handler(self.playground_panels_js, error_mode=error_mode),
         }
         if self.favicon_path:
             self.default_routes["/favicon.ico"] = wrap_handler(self.favicon, error_mode=error_mode)
 
+        default_route_keys = list(self.default_routes.keys())
+        for k in default_route_keys:
+            if k in self.routes:
+                del self.default_routes[k]
+
+
+    def _add_subroute(self, sub, handler):
+        if sub in self.sub_route_handlers:
+            raise NotImplementedError(f"Route {sub} already exists. Duplicate routes are not allowed.")
+        self.sub_route_handlers[sub] = handler
+
     def _all_routes(self, recursive=True):
         d = {
             **self.routes,
             **self.variadic_routes
         }
         if recursive:
             for k, v in self.sub_route_handlers.items():
@@ -593,15 +610,15 @@
             r = FileResponse(self.favicon_path, version=request.version)
         except Exception as e:
             r = Response(b"Not Found", status_code=404, version=request.version)
         return r
 
     @get
     def swagger(self) -> FileResponse:
-        return FileResponse(Path(__file__).parent / "resources" / "swagger.html")
+        return FileResponse(self.resources_folder / "swagger.html")
 
     @get
     def playground(self) -> Path:
         return self.playground_folder / "playground.html"
 
     @get
     def playground_js(self) -> Path:
@@ -618,103 +635,194 @@
                 if callable(v):
                     if self.require_tag and not hasattr(v, "allowed_methods"):
                         continue
                     if getattr(v, "do_not_serve", False):
                         continue
                     routes = getattr(v, "routes", [k])
                     for route in routes:
-                        with suppress(Exception):
+                        try:
                             self[route] = v
+                        except:
+                            pass
         if callable(obj):
             self[""] = obj
 
-    def get_nav(self):
+    def get_nav(self, start=""):
         routes = self._all_routes(self.nav_recursion)
         links = []
         for route in routes:
-            if route.startswith(self.base_path):
-                r = route[len(self.base_path):]
-                if not r.endswith("/"):
-                    r += "/"
-                n = r.count("/")
-                links.append(self.base_path + r)
+            if route.startswith(start):
+                r = route[len(start):]
+                if r.startswith("/"):
+                    r = r[1:]
+                links.append((f"./{r}", route))
         links = sorted(links)
-        nav = "<ul>\n" + "\n\t".join([f'<li><a href="{l}">{l}</a></li>' if '{' not in l else f'<li>{l}</li>'  for l in links]) + "\n</ul>"
+
+        # sort links into a nested order
+        nested = {}
+        for rel, full in links:
+            parts = full.strip("/").split("/")
+            n = nested
+            for part in parts[:-1]:
+                if part in n:
+                    if not isinstance(n[part], dict):
+                        n[part] = {}
+                    n = n[part]
+                else:
+                    n[part] = {}
+                    n = n[part]
+            n[parts[-1]] = (rel, full)
+
+        # now collapse back so if a parent has only one child, the keys are merged
+        def collapse(d, name=""):
+            if not d:
+                return d, name
+            if len(d) == 1:
+                k = list(d.keys())[0]
+                collapsed, new_name = collapse(d[k], name + "/" + k)
+                return collapsed, name + "/" + new_name
+            collapsed = {}
+            if isinstance(d, tuple):
+                return d, name
+            else:
+                for k, v in d.items():
+                    if isinstance(v, dict):
+                        new_v, new_k = collapse(v, k)
+                        collapsed[new_k] = new_v
+                    else:
+                        collapsed[k] = v
+            return collapsed, name
+
+        nested, name = collapse(nested)
+        def gen_nav(sub, p=""):
+            nav = ""
+            for k, v in sub.items():
+                if isinstance(v, dict):
+                    # make the list item contain a collapsible section
+                    nav += f'<li><details><summary>{p}/{k}</summary><ul>{gen_nav(v, p + "/" + k)}</ul></details></li>'
+
+                    # nav += f'<li>{k}<ul>{gen_nav(v)}</ul></li>'
+                elif isinstance(v, tuple):
+                    rel, full = v
+                    nav += f'<li><a href="{rel}">{full}</a></li>'
+            return nav
+
+        name = name.replace("//", "/")
+        nav = gen_nav(nested, name)
+
+        if name:
+            nav = f"<h1>{name}</h1>\n<ul>{nav}</ul>"
+        else:
+            nav = f"<ul>{nav}</ul>"
+
+
+        # nav = "<ul>\n" + "\n\t".join([f'<li><a href="{rel}">{full}</a></li>' if '{' not in full else f'<li>{full}</li>' for rel, full in links]) + "\n</ul>"
         return StandardHTMLResponse(nav, title=self.base_path)
 
     def __call__(self, request: Request) -> Response:
         route = request.path.route()
 
-        route_diff = route[len(self.base_path):]
-        if not route_diff.startswith("/"):
-            route_diff = "/" + route_diff
-        if self.nav_path and (route_diff == self.nav_path or route_diff == self.nav_path + "/"):
-            return self.get_nav()
-
         if not route.startswith(self.base_path):
             return Response(b'Not Found',
                             status_code=404,
                             headers={"Content-Type": "text/plain"},
                             version=request.version)
-        # search from longest to shortest subroute by length or string
-        subroute_keys = sorted(self.sub_route_handlers.keys(), key=lambda x: (len(x), x), reverse=True)
-        for k in subroute_keys:
-            if route.startswith(k):
-                return self.sub_route_handlers[k](request)
-
-        handler = self.routes.get(route, None)
 
         route_params = {}
-        if handler is None:
+        if route in self.default_routes:
+            handler = self.default_routes[route]
+        elif route in self.routes:
+            handler = self.routes[route]
+        else:
+            # search from longest to shortest subroute by length or string
+            subroute_keys = sorted(self.sub_route_handlers.keys(), key=lambda x: (len(x), x), reverse=True)
+            for k in subroute_keys:
+                if route.startswith(k):
+                    return self.sub_route_handlers[k](request)
+
             for k, v in self.matchable_routes.items():
                 if v.match(route):
                     handler = v
                     break
             else:
-                if route in self.default_routes:
-                    handler = self.default_routes[route]
-                elif "{" in (x:= url_decode(route)) and x in self.variadic_routes:
-                    raise ValueError(f"Route {route} is variadic , {{}} patterns should be filled in")
+                x = url_decode(route)
+                if "{" in x and x in self.variadic_routes:
+                    # raise ValueError(f"Route {route} is variadic, {{}} patterns should be filled in")
+                    return ErrorResponse(f"Route {x} is variadic, {{}} patterns should be filled in".encode(), version=request.version)
+                # check all variadic routes in the correct order, first by number of parts, then number of variadic parts, then length of nonvariadic parts
+                variadic_patterns = sort_variadic_routes(list(self.variadic_routes.keys()))
+
+                for k in variadic_patterns:
+                    # these are in format /a/{b}/c/{d}/e, convert to regexp groups
+                    route_params = matches_variadic_route(route, k)
+                    if route_params:
+                        handler = self.variadic_routes[k]
+                        for _k, _v in route_params.items():
+                            if hasattr(handler, "__dict__") and _k in handler.__dict__:
+                                options = handler.__dict__[_k]
+                                if _v == options:
+                                    # good! matches exactly
+                                    continue
+                                elif isinstance(options, (list, tuple, set, frozenset)):
+                                    for o in options:
+                                        if str(o) == _v:
+                                            # good! matches exactly one of the options
+                                            break
+                                        try:
+                                            if isinstance(o, type):
+                                                if isinstance(_v, o):
+                                                    # good! matches the type of one of the options
+                                                    break
+                                        except:
+                                            pass
+                                    else:
+                                        # oops! didn't match any of the options
+                                        break
+                                    continue
+                                elif isinstance(options, type):
+                                    try:
+                                        options(_v)
+                                        continue
+                                    except:
+                                        # oops! didn't match the type
+                                        break
+                                else:
+                                    # unable to interpret the options, maybe raise an error?
+                                    continue
+                        else:
+                            # this means the route_params matched all the options, which means we found the right handler
+                            break
                 else:
-                    # check all variadic routes in the correct order, first by number of parts, then number of variadic parts, then length of nonvariadic parts
-                    variadic_patterns = sort_variadic_routes(list(self.variadic_routes.keys()))
+                    handler = self.fallback_handler
 
-                    for k in variadic_patterns:
-                        # these are in format /a/{b}/c/{d}/e, convert to regexp groups
-                        route_params = matches_variadic_route(route, k)
-                        if route_params:
-                            handler = self.variadic_routes[k]
-                            break
-                    else:
-                        handler = self.fallback_handler
+        if handler is None and route.endswith(self.nav_path):
+            return self.get_nav(route[:-len(self.nav_path)])
 
         if handler is None:
             # send a response with 404
             return Response(b'Not Found',
                             status_code=404,
                             headers={"Content-Type": "text/plain"},
                             version=request.version)
         allowed_methods = gettag(handler, "allowed_methods", None)
-        # if allowed_methods is None:
-        #     print(handler, handler.__dict__)
         if request.method == "HEAD" and "GET" in allowed_methods:
             allowed_methods = list(allowed_methods) + ["HEAD"]
         if allowed_methods is None or request.method not in allowed_methods:
-            print("Method Not Allowed", route, request.method, allowed_methods, handler)
             return Response(b'Method Not Allowed',
                             status_code=405,
                             headers={"Content-Type": "text/plain"},
                             version=request.version)
         if route_params:
             r = handler(request, route_params)
         else:
             r = handler(request)
         return r
 
-    def route(self, handler, route: str | None = None, allowed_methods: tuple[str] | None = None):
+    # def route(self, handler, route: str | None = None, allowed_methods: tuple[str] | None = None):
+    def route(self, handler, route = None, allowed_methods = None):
         route = route.replace("//", "/")
         if isinstance(handler, Path):
             handler = StaticFileHandler(Path, route)
 
         if isinstance(handler, str):
             return lambda handler: self.route(handler, route, allowed_methods)
 
@@ -724,39 +832,39 @@
             allowed_methods = getattr(handler, "allowed_methods", ("GET",))
         em = getattr(handler, "error_mode", self.error_mode)
         h = wrap_handler(handler, error_mode=em)
         h.__dict__["allowed_methods"] = allowed_methods
         if self.base_path == "/" and route.startswith("/"):
             route = route[1:]
 
-        sub = self.base_path + route + ("/" if not route.endswith("/") else "")
+        sub = self.base_path + route
         sub = sub.replace("//", "/")
         if "{" in route and "}" in route:
             self.variadic_routes[sub] = h
         elif hasattr(h, "match") and callable(h.match):
             self.matchable_routes[sub] = h
         else:
             self.routes[sub] = h
 
-    def get(self, handler=None, route: str | None = None):
+    def get(self, handler=None, route: str = None):
         return self.route(handler, route, allowed_methods=("GET",))
 
-    def post(self, handler=None, route: str | None = None):
+    def post(self, handler=None, route: str = None):
         return self.route(handler, route, allowed_methods=("POST",))
 
-    def put(self, handler=None, route: str | None = None):
+    def put(self, handler=None, route: str = None):
         return self.route(handler, route, allowed_methods=("PUT",))
 
-    def patch(self, handler=None, route: str | None = None):
+    def patch(self, handler=None, route: str = None):
         return self.route(handler, route, allowed_methods=("PATCH",))
 
-    def delete(self, handler=None, route: str | None = None):
+    def delete(self, handler=None, route: str = None):
         return self.route(handler, route, allowed_methods=("DELETE",))
 
-    def head(self, handler=None, route: str | None = None):
+    def head(self, handler=None, route: str = None):
         route = route or handler.__name__
 
         def wrapper(request: Request) -> Response:
             response = handler(request)
             response.body = b""
             return response
 
@@ -767,11 +875,14 @@
 
     def __setitem__(self, key, value):
         self.route(value, key)
 
     def __getattr__(self, item):
         return self.__class__(self.fallback_handler, self.routes, self.base_path + item + "/")
 
+    def __repr__(self):
+        return f"<RouteHandler {self.base_path}>"
+
 
 if __name__ == "__main__":
     items = ["23", "3.14", "True", "False", "1", "0", "[1, 2, 3]", "(1, 2, 3)", "{1, 2, 3}", "{1: 2, 3: 4}", "hello", "world"]
     d = {v: (cast_to_typehint(v), type(cast_to_typehint(v))) for v in items}
```

### Comparing `socketwrench-1.9.3/src/socketwrench/openapi.py` & `socketwrench-2.0.0/src/socketwrench/openapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-import inspect
-from pathlib import Path
+from socketwrench.standardlib_dependencies import (
+    inspect,
+    Path,
+)
 
 from socketwrench import FileResponse, Response
 from socketwrench.tags import gettag
 
 
 def openapi_schema(routes_dict):
     openapi = {
@@ -37,15 +39,15 @@
                 }
                 parameters.append(param_info)
 
             route_info["parameters"] = parameters
         if "responses" not in route_info:
             sig = getattr(func, "sig", inspect.signature(func)) or inspect.signature(func)
             return_type = sig.return_annotation
-            if return_type is inspect._empty:
+            if return_type is inspect.Parameter.empty:
                 try:
                     last_line = inspect.getsourcelines(func)[0][-1].strip()
                     if "return" not in last_line:
                         return_type = None
                     else:
                         r = last_line.split("return ", 1)[1].strip()
                         if r in ["True", "False"]:
@@ -76,15 +78,15 @@
                             try:
                                 module = __import__("socketwrench.types", fromlist=[class_name])
                                 return_type = getattr(module, class_name)
                             except:
                                 return_type = Response
                 except:
                     pass
-            if return_type is not inspect._empty:
+            if return_type is not inspect.Parameter.empty:
                 if return_type is None:
                     route_info["responses"] = {
                         "200": {
                             "description": "Success",
                             "content": {
                                 "application/json": {
                                     "schema": {"type": "object"}
```

### Comparing `socketwrench-1.9.3/src/socketwrench/resources/favicon.ico` & `socketwrench-2.0.0/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/resources/playground/panels.js` & `socketwrench-2.0.0/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/resources/playground/playground.html` & `socketwrench-2.0.0/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/resources/playground/playground.js` & `socketwrench-2.0.0/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/resources/swagger.html` & `socketwrench-2.0.0/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/samples/file_sample.py` & `socketwrench-2.0.0/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.9.3/src/socketwrench/samples/sample.py` & `socketwrench-2.0.0/src/socketwrench/samples/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 import logging
 from pathlib import Path
 
 import cv2
 import numpy as np
 
 from socketwrench.handlers import StaticFileHandler
@@ -28,14 +29,15 @@
         return "this will not be served"
 
     @private
     def unserved(self):
         """This function will not be served."""
         return "this will not be served"
 
+
     @post
     def post(self, name):
         """This function will only be served by POST requests."""
         return f"hello {name}"
 
     @put
     def put(self, name):
@@ -119,16 +121,16 @@
             "headers": headers,
             "query": query,
             "body": body,
             "method": method,
             "route": route,
             "full_path": full_path,
         }
-        for k, v in d.items():
-            print(k, v)
+        # for k, v in d.items():
+        #     print(k, v)
         return d
 
     @route("/a/{c}", error_mode="traceback")
     def a(self, b, c=5):
         print(f"calling a with b={b}, c={c}")
         return f"captured b={b}, c={c}"
 
@@ -174,35 +176,43 @@
         return "world"
 
     def goodbye(self):
         return "cruel world"
 
 
 class Another:
+
+    @get("/add_small/{x}/{y}", x=[1,2,3,4], y=float)
+    def add_small(self, x, y):
+        return f"small: {x + y}"
+
+    @get("/add/{x}/{y}", x=int, y=float)
+    def add_big(self, x, y):
+        return f"big: {x + y}"
+
     @get("/add/{x}/{y}")
     def add(self, x, y):
         return x + y
 
     @get("/sub/{x}/{y}")
     def sub(self, x, y):
         return x - y
 
     def hello(self):
         return "world"
 
 
-
 if __name__ == '__main__':
     from socketwrench import serve
     s = Sample()
     serve({
         "sample": s,
         "a": Another(),
         "nest": {
             "a": Another,
             "o": Other
         }
-    }, nav_path="/nav")
+    })
     # OR
     # serve(Sample)
     # OR
     # serve("socketwrench.samples.sample.Sample")
```

### Comparing `socketwrench-1.9.3/src/socketwrench/server.py` & `socketwrench-2.0.0/src/socketwrench/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """A simple HTTP server built directly on top of socket.socket."""
-import socket
-import logging
-import time
-from pathlib import Path
+from socketwrench.standardlib_dependencies import (
+    logging,
+    Path,
+    socket,
+    sleep,
+    threading_available
+)
 
 from socketwrench.connection import Connection
 from socketwrench.handlers import RouteHandler, wrap_handler, is_object_instance
 
 logger = logging.getLogger("socketwrench")
 
 
@@ -23,26 +26,29 @@
         }
     }
     default_pause_sleep = 0.1
     default_accept_sleep = 0
     default_favicon = RouteHandler.default_favicon
 
     def __init__(self,
-                 routes: dict | None = None,
+                 routes: dict = None,
                  port: int = default_port,
                  host: str = default_host,
                  backlog: int = default_backlog,
                  chunk_size: int = default_chunk_size,
                  num_connection_threads: int = default_num_connection_threads,
-                 socket_options: dict[int, dict[int, int]] | None = default_socket_options,
+                 socket_options: dict = "default",
                  pause_sleep: float = default_pause_sleep,
                  accept_sleep: float = default_accept_sleep,
                  fallback_handler=None,
                  serve: bool = True,
-                 favicon: str | Path = default_favicon,
+                 favicon: str = default_favicon,
+                 protocol: str = "http",
+                 secured: bool = False,
+                 origin: str = None,
                  **kwargs
                  ):
         """A simple HTTP server built directly on top of socket.socket.
 
         Args:
             routes (dict[str, RequestHandler] | None, optional): A dictionary of routes to handlers.
             port (int, optional): The port to listen on. Defaults to 8080.
@@ -55,15 +61,21 @@
                 e.g. {socket.SOL_SOCKET: {socket.SO_REUSEADDR: 1}}
             pause_sleep (float, optional): The number of seconds to sleep between checking the threading.Event
                 when the server is paused. Could affect CPU and latency. Defaults to 0.1.
             accept_sleep (float, optional): The number of seconds to sleep between checking for new connections.
                 Could affect latency. Defaults to 0.1.
             fallback_handler (RequestHandler, optional): The function to use to handle requests that don't match any routes.
             serve (bool, optional): Whether to start serving immediately. Defaults to True.
+            favicon (str, optional): The path to the favicon to use. Defaults to None.
+            protocol (str, optional): The protocol to use for the server in logging statements. Defaults to "http".
+            secured (bool, optional): Whether the server is secured. Defaults to False. Only used for logging full url.
+            origin (str, optional): The full URL to use for the server in logging statements, otherwise we guess. Defaults to None.
         """
+        if socket_options == "default":
+            socket_options = self.default_socket_options
         if isinstance(routes, type):
             routes = routes()
 
         s = str(routes)
         s2 = s.split("\n")[0][:50]
         s = s2 + ("..." if len(s) > len(s2) else "")
         logger.info(f"Creating server with {s}")
@@ -80,14 +92,26 @@
                 base_path="/",
                 favicon=favicon,
                 **kwargs
             )
 
         self.host = host
         self.port = port
+
+        if origin is None:
+            if secured and protocol.lower() == "http":
+                protocol = "https"
+            else:
+                protocol = protocol.lower()
+            if (protocol == "http" and port == 80) or (protocol == "https" and port == 443):
+                p = ""
+            else:
+                p = f":{port}"
+            origin = f"{protocol}://{host or 'localhost'}{p}"
+        self.origin = origin
         self.backlog = backlog
         self.chunk_size = chunk_size
         self.num_connection_threads = num_connection_threads
         if self.num_connection_threads > 1:
             self.thread_pool_executor = None
         else:
             from concurrent.futures import ThreadPoolExecutor
@@ -123,113 +147,113 @@
             return
 
         # set socket options
         for level, options in socket_options.items():
             for option, value in options.items():
                 self.setsockopt(level, option, value)
 
-    def serve(self, thread: bool = False, cleanup_event = None, pause_event = None, nav_path="/", **kwargs) -> None | tuple:
+    def serve(self, thread: bool = False, cleanup_event = None, pause_event = None, nav_path="/", **kwargs) -> tuple:
         if not isinstance(self, Server):
             if isinstance(self, str) or "<module" in str(type(self)):
                 return Server.serve_module(self, thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, nav_path=nav_path, **kwargs)
             elif isinstance(self, type):
                 return Server.serve_class(self, thread=thread, cleanup_event=cleanup_event, pause_event=pause_event, nav_path=nav_path,**kwargs)
             # allows classmethod-like usage of Server.serve(my_server_instance)
             return Server(self, nav_path=nav_path, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
-        if thread:
-            import threading
+        if thread and threading_available:
+            from socketwrench.standardlib_dependencies import Event, Thread
 
-            self.cleanup_event = threading.Event()
-            self.pause_event = threading.Event()
+            self.cleanup_event = Event()
+            self.pause_event = Event()
 
-            t = threading.Thread(target=self.serve, args=(False, self.cleanup_event, self.pause_event), daemon=True)
+            t = Thread(target=self.serve, args=(False, self.cleanup_event, self.pause_event), daemon=True)
             t.start()
             self.server_thread = t
             return t, self.cleanup_event, self.pause_event
 
         self.bind((self.host, self.port))
         self.listen(self.backlog)
         logger.info("Serving HTTP on port " + str(self.port) + "...")
         logger.info(f"Press Ctrl+C to stop the server.")
-        logger.info(f"Go to http://{self.host or 'localhost'}:{self.port}/swagger to see documentation.")
-        logger.info(f"Go to http://{self.host or 'localhost'}:{self.port}/api for an api playground.")
+        logger.info(f"Go to {self.origin}/swagger to see documentation.")
+        logger.info(f"Go to {self.origin}/api for an api playground.")
 
         while cleanup_event is None or (not cleanup_event.is_set()):
             if self.pause_sleep and pause_event is not None:
                 while pause_event.is_set() and (cleanup_event is None or (not cleanup_event.is_set())):
-                    time.sleep(self.pause_sleep)
+                    sleep(self.pause_sleep)
             if self.accept_sleep:
-                time.sleep(self.accept_sleep)
+                sleep(self.accept_sleep)
             connection = self.accept_connection()
 
             # handle connection
             if self.thread_pool_executor:
                 self.thread_pool_executor.submit(connection.handle)
             else:
                 connection.handle()
 
     def accept_connection(self) -> Connection:
         """Accepts a connection and returns a Connection object."""
         client_connection, client_address = self.accept()
         connection = Connection(self.handler, client_connection, client_address,
                                 cleanup_event=self.cleanup_event,
-                                chunk_size=self.chunk_size)
+                                chunk_size=self.chunk_size,
+                                origin=self.origin)
         return connection
 
     def close(self) -> None:
         """Closes the server socket."""
         if self.server_thread:
             self.cleanup_event.set()
             self.server_thread.join()
         super().close()
 
     def __repr__(self) -> str:
         if self._rep is None:
             r = f"<{self.__class__.__name__}("
             if self.port != self.default_port:
-                r += f"{self.port=}, "
+                r += f"port={self.port}, "
             if self.host != self.default_host:
-                r += f"{self.host=}, "
+                r += f"host={self.host}, "
             if self.backlog != self.default_backlog:
-                r += f"{self.backlog=}, "
+                r += f"backlog={self.backlog}, "
             if self.chunk_size != self.default_chunk_size:
-                r += f"{self.chunk_size=}, "
+                r += f"chunk_size={self.chunk_size}, "
             if self.num_connection_threads != self.default_num_connection_threads:
-                r += f"{self.num_connection_threads=}, "
+                r += f"num_connection_threads={self.num_connection_threads}, "
             if self.init_socket_options != self.default_socket_options:
-                r += f"{self.init_socket_options=}, "
+                r += f"init_socket_options={self.init_socket_options}, "
             if self.pause_sleep != self.default_pause_sleep:
-                r += f"{self.pause_sleep=}, "
+                r += f"pause_sleep={self.pause_sleep}, "
             if self.accept_sleep != self.default_accept_sleep:
-                r += f"{self.accept_sleep=}, "
+                r += f"accept_sleep={self.accept_sleep}, "
             r = r.rstrip(", ")
             r += ")>"
             self._rep = r
         return self._rep
 
 
     @classmethod
     def serve_class(cls, c, thread: bool = False, cleanup_event = None, pause_event = None, **kwargs):
         inst = c()
         return cls(inst, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
 
     @classmethod
     def serve_module(cls, module, thread: bool = False, cleanup_event = None, pause_event = None, **kwargs):
         if isinstance(module, Path):
-            import importlib
-            import sys
+            from socketwrench.standardlib_dependencies import importlib, modules
             module = importlib.util.spec_from_file_location("module", module)
             module = importlib.util.module_from_spec(module)
             module.__file__ = module.__spec__.origin
             module.__package__ = module.__spec__.name
-            sys.modules[module.__spec__.name] = module
+            modules[module.__spec__.name] = module
             module.__spec__.loader.exec_module(module)
         elif isinstance(module, str):
             try:
-                import importlib
+                from socketwrench.standardlib_dependencies import importlib
                 module = importlib.import_module(module)
             except ImportError:
                 parts = module.split(".")
                 module = importlib.import_module(".".join(parts[:-1]))
                 module = getattr(module, parts[-1])
         return cls(module, **kwargs).serve(thread=thread, cleanup_event=cleanup_event, pause_event=pause_event)
```

### Comparing `socketwrench-1.9.3/src/socketwrench/tags.py` & `socketwrench-2.0.0/src/socketwrench/tags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from functools import partial
+from socketwrench.standardlib_dependencies import partial
 
 
 def tag(handler=None, **kwargs):
     if handler is None:
         return partial(tag, **kwargs)
 
     for key, value in kwargs.items():
@@ -22,27 +22,27 @@
 
 def private(handler):
     tag(handler, do_not_serve=True)
     return handler
 
 
 def allowed_methods(*methods: str):
-    def decorator(handler, route: str = None, error_mode: str = None, openapi: dict = None):
+    def decorator(handler, route: str = None, error_mode: str = None, openapi: dict = None, **kwargs):
         if isinstance(handler, str) and route is None:
-            return partial(get, route=handler, error_mode=error_mode, openapi=openapi)
+            return partial(get, route=handler, error_mode=error_mode, openapi=openapi, **kwargs)
         if route is not None:
             if "routes" not in handler.__dict__:
-                tag(handler, routes=[])
-            tag(handler, routes=list(set(handler.__dict__["routes"] + [route])))
+                tag(handler, routes=[], **kwargs)
+            tag(handler, routes=list(set(handler.__dict__["routes"] + [route])), **kwargs)
         if methods is not None:
             if "allowed_methods" not in handler.__dict__:
-                tag(handler, allowed_methods=[])
-            tag(handler, allowed_methods=list(set(handler.__dict__["allowed_methods"] + list(methods))))
+                tag(handler, allowed_methods=[], **kwargs)
+            tag(handler, allowed_methods=list(set(handler.__dict__["allowed_methods"] + list(methods))), **kwargs)
         if error_mode is not None:
-            tag(handler, error_mode=error_mode, openapi=openapi)
+            tag(handler, error_mode=error_mode, openapi=openapi, **kwargs)
         return handler
     return decorator
 
 
 get = allowed_methods("GET")
 post = allowed_methods("POST")
 put = allowed_methods("PUT")
```

### Comparing `socketwrench-1.9.3/src/socketwrench/types.py` & `socketwrench-2.0.0/src/socketwrench/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import dataclasses
-import datetime
-import json
-import socket
-from pathlib import Path
+from socketwrench.standardlib_dependencies import (
+    dataclasses,
+    datetime,
+    dumps,
+    socket,
+    Path,
+)
 
 
 class HTTPVersion(str):
     """Represents an HTTP version string."""
     HTTP_0_9 = "HTTP/0.9"
     HTTP_1_0 = "HTTP/1.0"
     HTTP_1_1 = "HTTP/1.1"
@@ -48,15 +50,16 @@
     def to_bytes(self) -> bytes:
         return self.to_string().encode()
 
 
 class HeaderBytes(bytes):
     EMPTY = b""
 
-    def __new__(cls, s: bytes | Headers | dict[str, str]):
+    def __new__(cls, s):
+    # def __new__(cls, s: bytes | Headers | dict[str, str]):
         if isinstance(s, Headers):
             s = s.to_bytes()
         elif isinstance(s, dict):
             s = Headers(s).to_bytes()
         return super().__new__(cls, s)
 
     def to_string(self):
@@ -77,96 +80,118 @@
     BASE = "/"
 
     def query(self) -> str:
         """Extracts the query string from the path."""
         if "?" not in self:
             return ""
         q = self.split("?", 1)[1]
-        return q
+        return "?" + q
 
     def route(self) -> str:
         """Extracts the path from the path and remove the query."""
         p = self.split("?", 1)[0]
-        if not p.endswith("/"):
-            p += "/"
         return p
 
     def query_args(self) -> dict[str, str]:
         """Extracts the query string from the path and parses into a dictionary."""
         q = self.query()
         if not q:
             return {}
+        q = q[1:]
         items = [v.split("=", 1) for v in q.split("&")]
         d = {url_decode(k): url_decode(v) for k, v in items}
         return d
 
 
 class ClientAddr(str):
-    def __new__(cls, host_port: str | tuple[str, int]):
+    def __new__(cls, host_port):
+    # def __new__(cls, host_port: str | tuple[str, int]):
         if isinstance(host_port, tuple):
             host = host_port[0]
             port = host_port[1]
         else:
             host = host_port
             port = None
         self = super().__new__(cls, host)
         self.host = host
         self.port = port
         return self
 
 
 class Request:
     @classmethod
-    def from_components(cls, pre_body_bytes: bytes, body: bytes, client_addr: str | tuple[str, int], connection_socket: socket.socket = None) -> "Request":
+    def from_components(cls, pre_body_bytes: bytes, body: bytes, client_addr: str, connection_socket: socket = None, origin: str = "") -> "Request":
+    # def from_components(cls, pre_body_bytes: bytes, body: bytes, client_addr: str | tuple[str, int], connection_socket: socket.socket = None) -> "Request":
         """Create a Request object from a header string and a body bytes object."""
         i = pre_body_bytes.index(b"\r\n")
         first_line = pre_body_bytes[:i].decode()
         method, path, version = first_line.split(" ")
         header_bytes = pre_body_bytes[i + 2:]
-        return cls(method, path, version, header_bytes, body, client_addr, connection_socket)
+        return cls(method, path, version, header_bytes, body, client_addr, connection_socket, origin=origin)
 
     def __init__(self,
-                 method: str | HTTPMethod = HTTPMethod.GET,
-                 path: str | RequestPath = RequestPath.BASE,
-                 version: str | HTTPVersion = HTTPVersion.HTTP_1_1,
-                 header: bytes | HeaderBytes | Headers | dict[str, str] = HeaderBytes.EMPTY,
-                 body: bytes | RequestBody = RequestBody.EMPTY,
-                 client_addr: str | tuple[str, int] | None = None,
-                 connection_socket: socket.socket | None = None
+                 method: str = HTTPMethod.GET,
+                 path: str = RequestPath.BASE,
+                 version: str = HTTPVersion.HTTP_1_1,
+                 header: bytes = HeaderBytes.EMPTY,
+                 body: bytes = RequestBody.EMPTY,
+                 client_addr: str = None,
+                 connection_socket: socket = None,
+                 origin: str = ""
                  ):
+        """Parsed HTML Request bytes broken down into its components.
+
+        Args:
+            method: str | HTTPMethod
+            path: str | RequestPath
+            version: str | HTTPVersion
+            header: bytes | HeaderBytes | Headers | dict[str, str]
+            body: bytes | RequestBody
+            client_addr: str | tuple[str, int] | None
+            connection_socket: socket.socket | None
+        """
         self.method = HTTPMethod(method)
         self.path = RequestPath(path)
         self.version = HTTPVersion(version)
         self.header_bytes = HeaderBytes(header)
         self._headers = None
         self.body = RequestBody(body)
         self.client_addr = ClientAddr(client_addr) if client_addr else None
         self.connection_socket = connection_socket
+        self.origin = origin
 
     @property
     def headers(self) -> Headers:
         if self._headers is None:
             self._headers = Headers(self.header_bytes.to_dict())
         return self._headers
 
     def to_string(self) -> str:
         return f'{self.method} {self.path} {self.version}\r\n{self.headers}\r\n\r\n{self.body}'
 
     def to_json(self) -> str:
-        return json.dumps({
+        return dumps({
             "method": self.method,
             "path": self.path,
             "version": self.version,
             "headers": self.headers,
             "body": str(self.body),
             "client_addr": self.client_addr
         })
 
+    def __str__(self):
+        return f"{self.method} {self.origin}{self.path} from {self.client_addr}"
+
     def __repr__(self):
-        return f"<Request {self.method} {self.path} client_addr={self.client_addr} ...>"
+        ca = f'"{self.client_addr}"' if isinstance(self.client_addr, str) else self.client_addr
+        r = f'<Request("{self.method}","{self.path}", "{self.version}", {bytes(self.header_bytes)}, {bytes(self.body)}, {ca}, {self.connection_socket}, "{self.origin}")>'
+        r = r.replace("\n", "\\n").replace("\r", "\\r").replace("\t", "\\t")
+        if len(r) > 100:
+            r = r[:100] + "..."
+        return r
 
 
 class ResponseBody(Body):
     pass
 
 
 class HTTPStatusCode(int):
@@ -238,15 +263,15 @@
     HTTP_VERSION_NOT_SUPPORTED = 505
     VARIANT_ALSO_NEGOTIATES = 506
     INSUFFICIENT_STORAGE = 507
     LOOP_DETECTED = 508
     NOT_EXTENDED = 510
     NETWORK_AUTHENTICATION_REQUIRED = 511
 
-    def __new__(cls, status_code: int, phrase: str | None = None):
+    def __new__(cls, status_code: int, phrase: str = None):
         self = super().__new__(cls, status_code)
         self._phrase = phrase
         return self
 
     def phrase(self) -> str:
         if self._phrase is None:
             for k, v in self.__class__.__dict__.items():
@@ -292,23 +317,27 @@
             default_content_type = item
         return TypedResponse
 
 
 class Response(metaclass=ResponseType):
     default_content_type = None
 
-    def __new__(cls, body: bytes | ResponseBody = ResponseBody.EMPTY,
-                status_code: int | HTTPStatusCode = HTTPStatusCode.OK,
-                headers: bytes | HeaderBytes | Headers | dict = HeaderBytes.EMPTY,
-                version: str | HTTPVersion = HTTPVersion.HTTP_1_1,
+    def __new__(cls, body: bytes = ResponseBody.EMPTY,
+                status_code: int = HTTPStatusCode.OK,
+                headers: dict = HeaderBytes.EMPTY,
+                version: str = HTTPVersion.HTTP_1_1,
+                raw: bool = False,
                 **headers_kwargs):
         # If the body is already a Response instance, return it
         if isinstance(body, Response):
             return body
 
+        if raw:
+            return super(RawResponse, cls).__new__(cls)
+
         # Create an instance of the appropriate subclass based on the body type
         if cls is Response:
             if isinstance(body, (bytes, memoryview)):
                 return super(Response, cls).__new__(cls)
             elif isinstance(body, str):
                 return super(Response, HTMLResponse).__new__(HTMLResponse)
             elif isinstance(body, Path):
@@ -317,44 +346,82 @@
                 return super(Response, ErrorResponse).__new__(ErrorResponse)
             else:
                 return super(Response, JSONResponse).__new__(JSONResponse)
         else:
             return super(Response, cls).__new__(cls)
 
     def __init__(self,
-                 body: bytes | ResponseBody = ResponseBody.EMPTY,
-                 status_code: int | HTTPStatusCode = HTTPStatusCode.OK,
-                 headers: bytes | HeaderBytes | Headers | dict = HeaderBytes.EMPTY,
-                 version: str | HTTPVersion = HTTPVersion.HTTP_1_1,
+                 body: bytes = ResponseBody.EMPTY,
+                 status_code: int = HTTPStatusCode.OK,
+                 headers: dict = HeaderBytes.EMPTY,
+                 version: str = HTTPVersion.HTTP_1_1,
+                 raw: bool = False,
                  **headers_kwargs
                  ):
         self.status_code = HTTPStatusCode(status_code)
         self.version = HTTPVersion(version)
         self.header_bytes = HeaderBytes(headers)
         self.headers = Headers(self.header_bytes.to_dict())
         for k, v in headers_kwargs.items():
             t = k.replace("_", " ").title().replace(" ", "-")
             if not isinstance(v, str):
-                v = json.dumps(v)
+                v = dumps(v)
             self.headers[t] = v
         self.body = ResponseBody(body)
+        self.raw = raw
 
     def pre_body_bytes(self) -> bytes:
         return f'{self.version} {self.status_code}\r\n{self.headers}\r\n'.encode()
 
     def __repr__(self):
-        return f"<Response {self.status_code} {self.body[:10]}>"
+        return f"<{self.__class__.__name__} {self.status_code} {self.body[:80]}>"
 
     def __bytes__(self):
         return self.pre_body_bytes() + self.body
 
     def __buffer__(self, flags):
         return memoryview(bytes(self))
 
 
+class RawResponse(Response):
+    def __init__(self, full_response_bytes: bytes, raw: bool = True, **kwargs):
+        if not raw:
+            raise ValueError("RawResponse must be raw.")
+        self.full_response_bytes = full_response_bytes
+        self.version, self.status_code, self.headers, self.body = self.parse(full_response_bytes)
+        self.raw = raw
+
+    @staticmethod
+    def parse(full_response_bytes: bytes):
+        try:
+            # get the first two lines
+            first_line_end = full_response_bytes.index(b"\r\n")
+            first_line = full_response_bytes[:first_line_end]
+            version, status_code, phrase = first_line.split(b" ", 2)
+            # get the headers
+            header_end = first_line_end + 2 + full_response_bytes[first_line_end + 2:].index(b"\r\n\r\n")
+            header_bytes = full_response_bytes[first_line_end + 2:header_end]
+
+            version = HTTPVersion(version)
+            status_code = HTTPStatusCode(int(status_code), phrase)
+            header_bytes = HeaderBytes(header_bytes)
+            headers = Headers(header_bytes.to_dict())
+            body = ResponseBody(full_response_bytes[header_end + 4:])
+            return version, status_code, headers, body
+        except:
+            return None, None, None, None
+
+    def __bytes__(self):
+        return bytes(self.full_response_bytes)
+
+    def __buffer__(self, flags):
+        return self.full_response_bytes if isinstance(self.full_response_bytes, memoryview) else memoryview(self.full_response_bytes)
+
+
+
 class FileResponse(Response):
     content_types = {
         "html": "text/html",
         "css": "text/css",
         "js": "application/javascript",
         "png": "image/png",
         "jpg": "image/jpeg",
@@ -428,22 +495,25 @@
 
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
 
     def __init__(self,
                  *a,
                  body: bytes = b"",
-                 path: str | Path = None,
-                 filename: str | None = None,
-                 extension: str | None = None,
+                 path: str = None,
+                 filename: str = None,
+                 extension: str = None,
                  status_code: int = 200,
                  headers: dict = None,
-                 content_type: str | None = None,
+                 content_type: str = None,
                  download: bool = False,
-                 version: str = "HTTP/1.1"):
+                 version: str = "HTTP/1.1",
+                 raw: bool = False):
+        if raw:
+            raise NotImplementedError
         if content_type is None and self.default_content_type is not None:
             content_type = self.default_content_type
         if content_type is None and extension is not None:
             content_type = self.get_content_type(extension.lstrip("."))
 
         if a:
             if len(a) == 1:
@@ -483,33 +553,32 @@
             elif hasattr(a[0], "tobytes"):
                 body = a[0].tobytes()
             elif hasattr(a[0], "to_bytes"):
                 body = a[0].to_bytes()
             elif hasattr(a[0], "dumps"):
                 body = (a[0]).dumps().encode()
             elif isinstance(a[0], dict):
-                body = json.dumps(a[0]).encode()
+                body = dumps(a[0]).encode()
             else:
                 raise ValueError(f"Invalid argument: {a[0]}")
 
         if headers is None:
             headers = {}
 
         if download and "Content-Disposition" not in headers:
             headers["Content-Disposition"] = f'attachment; filename="{filename}"'
 
         # add headers related to file stats
         if "Content-Length" not in headers:
             headers["Content-Length"] = str(path.stat().st_size) if path else str(len(body))
         if "Last-Modified" not in headers:
-            headers["Last-Modified"] = datetime.datetime.fromtimestamp(path.stat().st_mtime).isoformat() if path else datetime.datetime.now().isoformat()
+            headers["Last-Modified"] = datetime.fromtimestamp(path.stat().st_mtime).isoformat() if path else datetime.now().isoformat()
 
         if path and path.is_dir():
-            from tempfile import TemporaryFile
-            from zipfile import ZipFile
+            from socketwrench.standardlib_dependencies import TemporaryFile, ZipFile
             # zip the directory to a TemporaryFile
             with TemporaryFile() as f:
                 with ZipFile(f, "w") as z:
                     for p in path.iterdir():
                         z.write(p, p.name)
                 f.seek(0)
                 super().__init__(f.read(),
@@ -535,14 +604,18 @@
         else:
             super().__init__(body,
                              status_code=status_code,
                              headers=headers,
                              content_type=content_type,
                              version=version)
 
+    def __str__(self):
+        ct = self.headers.get("Content-Type", "application/octet-stream")
+        return f"{self.__class__.__name__}[{ct}] {self.status_code} {self.body[:80]}"
+
     def get_content_type(self, suffix: str):
         return self.content_types.get(suffix.lower(), self.content_types[self.default_content_type])
 
     def get_extension(self, content_type: str):
         for k, v in self.content_types.items():
             if v == content_type:
                 return "." + k
@@ -564,20 +637,20 @@
 
         class TypedFileResponse(FileResponse):
             default_content_type = content_type
 
             def __init__(self,
                          *a,
                          body: bytes = b"",
-                         path: str | Path = None,
-                         filename: str | None = None,
-                         extension: str | None = None,
+                         path: str = None,
+                         filename: str = None,
+                         extension: str = None,
                          status_code: int = 200,
                          headers: dict = None,
-                         content_type: str | None = None,
+                         content_type: str = None,
                          download: bool = False,
                          version: str = "HTTP/1.1"):
                 if write_function:
                     r = write_function(*a)
                     a = (r,)
                 super().__init__(*a,
                                     body=body,
@@ -603,24 +676,24 @@
 
 class FileTypeResponse(metaclass=FileTypeResponseMeta):
     def __new__(cls, *args, **kwargs):
         return FileTypeResponseMeta.get_class(*args, **kwargs)
 
 
 class HTMLResponse(Response):
-    def __init__(self, html: str, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+    def __init__(self, html: str, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
             headers["Content-Type"] = "text/html"
-        Response.__init__(self, html.encode(), status_code, headers, version)
+        Response.__init__(self, html.encode(), status_code, headers, version, raw=raw)
 
 
 class StandardHTMLResponse(HTMLResponse):
-    def __init__(self, body: str, title = "", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+    def __init__(self, body: str, title = "", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
         favicon = f'<link rel="icon" href="{favicon}">' if favicon else ""
         scripts = "\n".join([f'<script src="{i}"></script>' for i in scripts]) if scripts else ""
         stylesheets = "\n".join([f'<link rel="stylesheet" href="{i}">' for i in stylesheets]) if stylesheets else ""
         html = f"""<!DOCTYPE html>
 <html>
 <head>
     <title>{title}</title>
@@ -628,118 +701,119 @@
     {scripts}
     {stylesheets}
 </head>
 <body>
     {body}
 </body>
 </html>"""
-        super().__init__(html, status_code, headers, version)
+        super().__init__(html, status_code, headers, version, raw=raw)
 
 
 class HTMLTextResponse(StandardHTMLResponse): # this is easier to implement than escaping the text
-    def __init__(self, body: str, title="", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+    def __init__(self, body: str, title="", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
         super().__init__(f"<pre>{body}</pre>",
                             title=title,
                             favicon=favicon,
                             scripts=scripts,
                             stylesheets=stylesheets,
                             status_code=status_code,
                             headers=headers,
-                            version=version)
+                            version=version,
+                         raw=raw)
 
 
 class TBDBResponse(StandardHTMLResponse):
     """Displays tabular json data in a table using https://github.com/modularizer/teebydeeby"""
-    def __init__(self, data, title="", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+    def __init__(self, data, title="", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
         if not isinstance(data, str):
-            data = json.dumps(data, indent=4)
+            data = dumps(data, indent=4)
         super().__init__(f"<teeby-deeby>{data}</teeby-deeby>",
                             title=title,
                             favicon=favicon,
                             scripts=["https://cdnjs.cloudflare.com/ajax/libs/lz-string/1.4.4/lz-string.min.js", "https://modularizer.github.io/teebydeeby/tbdb.js"] + list(scripts or []),
                             stylesheets=stylesheets,
                             status_code=status_code,
                             headers=headers,
-                            version=version)
-
+                            version=version,
+                         raw=raw)
 
 
 class JSONResponse(Response):
-    def __init__(self, data: str | dict | list | tuple | int | float, status_code: int = 200, headers: dict = None,
-                 version: str = "HTTP/1.1"):
+    def __init__(self, data: dict, status_code: int = 200, headers: dict = None,
+                 version: str = "HTTP/1.1", raw: bool = False):
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
             headers["Content-Type"] = "application/json"
         if not isinstance(data, str):
             if isinstance(data, tuple):
                 data = list(data)
-            if dataclasses.is_dataclass(data):
+            if dataclasses and dataclasses.is_dataclass(data):
                 data = dataclasses.asdict(data)
 
             if hasattr(data, "to_json"):
                 try:
                     data = data.to_json()
                 except:
                     if hasattr(data, "to_dict"):
                         try:
-                            data = json.dumps(data.to_dict())
+                            data = dumps(data.to_dict())
                         except:
                             data = str(data)
                     else:
                         data = str(data)
             elif hasattr(data, "to_dict"):
                 try:
-                    data = json.dumps(data.to_dict())
+                    data = dumps(data.to_dict())
                 except:
                     data = str(data)
             else:
-                try:
-                    data = json.dumps(data)
-                except:
-                    data = str(data)
-        super().__init__(data.encode(), status_code, headers, version)
+                data = dumps(data)
+        super().__init__(data.encode(), status_code, headers, version, raw=raw)
 
 
 class ErrorResponse(Response):
     def __init__(self,
-                 error: str | bytes | Exception = b'Internal Server Error',
+                 error: Exception = b'Internal Server Error',
                  status_code: int = 500,
                  headers: dict = None,
-                 version: str = "HTTP/1.1"):
+                 version: str = "HTTP/1.1", raw: bool = False):
         if headers is None:
             headers = {}
         if isinstance(error, Exception):
             error = str(error).encode()
         elif isinstance(error, bytes):
             pass
         else:
             error = str(error).encode()
         if "Content-Type" not in headers:
             headers["Content-Type"] = "text/plain"
-        super().__init__(error, status_code, headers, version)
+        super().__init__(error, status_code, headers, version, raw=raw)
 
 
 class RedirectResponse(Response):
-    def __init__(self, location: str, status_code: int = 307, headers: dict = None, version: str = "HTTP/1.1"):
+    def __init__(self, location: str, status_code: int = 307, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
         if headers is None:
             headers = {}
         if "Location" not in headers:
             headers["Location"] = location
-        super().__init__(b"", status_code, headers, version)
+        super().__init__(b"", status_code, headers, version, raw=raw)
+
+    def __str__(self):
+        return f"{self.__class__.__name__}({self.headers['Location']})"
 
 
 class TemporaryRedirect(RedirectResponse):
-    def __init__(self, location: str, status_code: int = 307, headers: dict = None, version: str = "HTTP/1.1"):
-        super().__init__(location, status_code, headers, version)
+    def __init__(self, location: str, status_code: int = 307, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
+        super().__init__(location, status_code, headers, version, raw=raw)
 
 
 class PermanentRedirect(RedirectResponse):
-    def __init__(self, location: str, status_code: int = 308, headers: dict = None, version: str = "HTTP/1.1"):
-        super().__init__(location, status_code, headers, version)
+    def __init__(self, location: str, status_code: int = 308, headers: dict = None, version: str = "HTTP/1.1", raw: bool = False):
+        super().__init__(location, status_code, headers, version, raw=raw)
 
 
 url_encodings = {
     " ": "%20",
     "!": "%21",
     '"': "%22",
     "#": "%23",
@@ -1001,15 +1075,15 @@
 
 class ErrorModes:
     HIDE = "hide"
     TYPE = "type"
     SHORT = "short"
     TRACEBACK = TB = LONG = SHOW = "traceback"
 
-    DEFAULT = HIDE
+    DEFAULT = TRACEBACK
 
 
 def set_default_error_mode(mode: str):
     if mode not in [ErrorModes.HIDE, ErrorModes.TYPE, ErrorModes.SHORT, ErrorModes.TRACEBACK]:
         raise ValueError(f"Invalid error mode: {mode}. Options are 'hide', 'type', 'short', 'traceback'.")
     ErrorModes.DEFAULT = mode
```

### Comparing `socketwrench-1.9.3/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.9.3
+Version: 2.0.0
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -31,15 +31,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # socketwrench
-A webserver based on `socket.socket` with no dependencies other than the standard library.
+A webserver based on `socket.socket` with no dependencies whatsoever other **socket** (or a substitute you pass in ) and **optional** standard library dependencies which improve features. See [dependencies](#dependencies) for more info.
 Provides a lightweight quickstart to make an API which supports OpenAPI, Swagger, and more.
 
 ## NOTE:
 this is **not** a production-ready web server. It is a learning tool and a lightweight way to make a simple API. While I attempted to reduce overhead in calls, I haven't taken time to thoroughly optimize, and I have not implemented any complex features to deal with security, performance, or scalability.
 
 ## Project Goals
 Part of the goal of this project was to understand how web servers work and to make a simple web server that is easy to use and understand.
@@ -61,15 +61,15 @@
 class MyServer:
     src = StaticFileHandler(Path(__file__).parent.parent.parent)
     
     def hello(self):
         return "world"
   
 if __name__ == '__main__':
-    serve(MyServer)
+    serve(MyServer, thread=True)
     # OR
     # m = MyServer()
     # serve(m)
     # OR
     # serve("my_module.MyServer")
 ```
 * Go to http://localhost:8080/hello and see the response "world".
@@ -143,31 +143,83 @@
 
 ### favicon.ico
 No need to use our favicon! pass a `str | Path` `.ico` filepath to `favicon` argument to use your own favicon. Alternatively, tag `@route('/favicon.ico')` on a function returning the path.
 
 ### fallback handler
 Add a custom function to handle any requests that don't match any other routes.
 
+# Dependencies
+Default behavior is to use the standard library only. However, if you do not have the full standard library, socketwrench _should_ still work.
+This is a work in progress as I am attempting to support micropython, circuitpython, etc. but I have not tested on these environments yet.
+
+### How it works:
+* `socket.socket` is the only required dependency, BUT you can pass in a substitute socket object if you want.
+* The following standard library modules are used, BUT if import fails for any of them we fall back on dump fake versions I made in [src/socketwrench/fake_imports](.src/socketwrench/fake_imports) which attempt to approximate the same functionality
+```python
+import socket
+
+import builtins  # very niche case use for if a function is typehinted to accept a type, e.g. `def f(x: type):` and you pass in the type name via a string query e.g. `?x=int`
+import inspect  # used often for getting function signatures, autofilling parameters, etc., spoof version uses `__annotations__` and `__defaults__` of functions
+from sys import argv # only used in commandline mode
+from argparse import ArgumentParser # only used in commandline mode
+from tempfile import TemporaryFile # only used if you attempt to return a folder using a StaticFileHandler
+from zipfile import ZipFile # only used if you attempt to return a folder using a StaticFileHandler
+from functools import wraps, partial # used regularly but easily replaced
+import dataclasses # only used if your python function returns a dataclass which we try to coerce to json
+from datetime import datetime  # used for Last-Modified header of File responses
+from pathlib import Path # used for file responses and static file serving, spoof version works okay
+from json import dumps, loads # used for json responses, spoof version works okay
+import logging # used for logging, spoof version works okay
+from time import sleep # only used if pause_sleep > 0 or accept_sleep > 0, spoof version does not sleep at all
+from threading import Event, Thread # only used if you `thread=True` in `serve` function (defaults to False)
+from traceback import format_exception  # only used if error_mode="traceback"
+import importlib # only used if you pass a string into the serve module as the item to be served, e.g. in commandline mode
+from sys import modules # only used if you pass a string into the serve module as the item to be served, e.g. in commandline mode
+```
+
+### sample
+```python
+from socketwrench import serve
+import socket
+
+class Sample:
+    def hello(self):
+        return "world"
+
+if __name__ == '__main__':
+    serve(Sample, spoof_modules="all", thread=True, socket=socket, port=8123)
+```
+
 # Planned Features
-* [ ] Implement nesting / recursion to serve deeper routes and/or multiple classes
+* [x] Implement nesting / recursion to serve deeper routes and/or multiple classes
+* [x] support default navigation pages to help show links to available routes
 * [ ] Enforce OpenAPI spec with better error responses
 * [x] Serve static folders
 * [x] Make a better playground for testing endpoints
   * [ ] better preview of variadic routes
 * [ ] improve docs
   * [ ] document variadic routes
   * [ ] document autofilled parameters
   * [ ] document decorators
   * [ ] document error modes
   * [ ] document static file serving
   * [ ] document favicon
   * [ ] document fallback handler
   * [ ] document regexp / match routes
 * [ ] Make a client-side python proxy object to make API requests from python
+
+### Environment Support
+* [x] Remove `|` typehints to allow for older python versions :/ (this makes me sad)
+* [x] Remove standard library dependencies which microcontrollers may not have
+* [x] Allow passing in a socket object
+  * [ ] test and support different kinds of sockets and objects pretending to be sockets
 * [ ] Test on ESP32 and other microcontrollers
+* [ ] Test in browser-based python environments using pyodide
+
+### Other
 * [ ] Ideas? Let me know!
 
 # Other Usage Modes
 ### Serve a module
 Using commandline, just specify a filepath or file import path to a module.
 ```python
 # my_module.py
```

### Comparing `socketwrench-1.9.3/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-2.0.0/src/socketwrench.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -3,21 +3,35 @@
 README.md
 pyproject.toml
 src/socketwrench/__init__.py
 src/socketwrench/__main__.py
 src/socketwrench/connection.py
 src/socketwrench/handlers.py
 src/socketwrench/openapi.py
+src/socketwrench/public.py
 src/socketwrench/server.py
+src/socketwrench/settings.py
+src/socketwrench/standardlib_dependencies.py
 src/socketwrench/tags.py
 src/socketwrench/types.py
 src/socketwrench.egg-info/PKG-INFO
 src/socketwrench.egg-info/SOURCES.txt
 src/socketwrench.egg-info/dependency_links.txt
 src/socketwrench.egg-info/top_level.txt
+src/socketwrench/fake_imports/__init__.py
+src/socketwrench/fake_imports/fake_argparse.py
+src/socketwrench/fake_imports/fake_dataclasses.py
+src/socketwrench/fake_imports/fake_datetime.py
+src/socketwrench/fake_imports/fake_functools.py
+src/socketwrench/fake_imports/fake_inspect.py
+src/socketwrench/fake_imports/fake_json.py
+src/socketwrench/fake_imports/fake_logging.py
+src/socketwrench/fake_imports/fake_pathlib.py
+src/socketwrench/fake_imports/fake_tempfile.py
+src/socketwrench/fake_imports/fake_traceback.py
 src/socketwrench/resources/favicon.ico
 src/socketwrench/resources/swagger.html
 src/socketwrench/resources/playground/panels.js
 src/socketwrench/resources/playground/playground.html
 src/socketwrench/resources/playground/playground.js
 src/socketwrench/samples/__init__.py
 src/socketwrench/samples/file_sample.py
```

