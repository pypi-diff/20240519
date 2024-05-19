# Comparing `tmp/python_filewrap-0.0.4.1.tar.gz` & `tmp/python_filewrap-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.4.1.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.5.tar", max compression
```

## Comparing `python_filewrap-0.0.4.1.tar` & `python_filewrap-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.4.1/LICENSE
--rwxr-xr-x   0        0        0    13237 2024-05-17 11:20:06.097879 python_filewrap-0.0.4.1/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.4.1/filewrap/py.typed
--rw-r--r--   0        0        0     1173 2024-05-17 11:21:04.523756 python_filewrap-0.0.4.1/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.4.1/readme.md
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 python_filewrap-0.0.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0    13683 2024-05-18 18:12:40.607694 python_filewrap-0.0.5/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.5/filewrap/py.typed
+-rw-r--r--   0        0        0     1171 2024-05-18 18:14:25.280408 python_filewrap-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.5/readme.md
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.5/PKG-INFO
```

### Comparing `python_filewrap-0.0.4.1/LICENSE` & `python_filewrap-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.4.1/filewrap/__init__.py` & `python_filewrap-0.0.5/filewrap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 4)
+__version__ = (0, 0, 5)
 __all__ = [
     "SupportsRead", "SupportsWrite", 
     "bio_chunk_iter", "bio_chunk_async_iter", 
     "bio_skip_iter", "bio_skip_async_iter", 
     "bytes_iter_to_reader", "bytes_iter_to_async_reader", 
+    "bytes_to_chunk_iter", "bytes_to_chunk_async_iter"
 ]
 
 from asyncio import to_thread, Lock as AsyncLock
 from collections.abc import Awaitable, AsyncIterable, Iterable
 from functools import update_wrapper
 from inspect import isawaitable, iscoroutinefunction
 from collections.abc import AsyncIterator, Callable, Iterator
@@ -410,7 +411,27 @@
         "read": staticmethod(read), 
         "readinto": staticmethod(readinto), 
         "__iter__": lambda self, /: self, 
         "__next__": staticmethod(__next__), 
         "__repr__": staticmethod(lambda: reprs), 
     })()
 
+
+def bytes_to_chunk_iter(
+    b, 
+    /, 
+    chunksize=1<<16, 
+) -> Iterator[memoryview]:
+    m = memoryview(b)
+    for i in range(0, len(m), chunksize):
+        yield m[i:i+chunksize]
+
+
+async def bytes_to_chunk_async_iter(
+    b, 
+    /, 
+    chunksize=1<<16, 
+) -> AsyncIterator[memoryview]:
+    m = memoryview(b)
+    for i in range(0, len(m), chunksize):
+        yield m[i:i+chunksize]
+
```

### Comparing `python_filewrap-0.0.4.1/pyproject.toml` & `python_filewrap-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.4.1"
+version = "0.0.5"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.4.1/PKG-INFO` & `python_filewrap-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.4.1
+Version: 0.0.5
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

