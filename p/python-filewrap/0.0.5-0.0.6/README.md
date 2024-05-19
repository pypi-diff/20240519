# Comparing `tmp/python_filewrap-0.0.5.tar.gz` & `tmp/python_filewrap-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.5.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.6.tar", max compression
```

## Comparing `python_filewrap-0.0.5.tar` & `python_filewrap-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.5/LICENSE
--rwxr-xr-x   0        0        0    13683 2024-05-18 18:12:40.607694 python_filewrap-0.0.5/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.5/filewrap/py.typed
--rw-r--r--   0        0        0     1171 2024-05-18 18:14:25.280408 python_filewrap-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.5/readme.md
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.6/LICENSE
+-rwxr-xr-x   0        0        0    15223 2024-05-19 09:04:58.198764 python_filewrap-0.0.6/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.6/filewrap/py.typed
+-rw-r--r--   0        0        0     1171 2024-05-19 09:04:52.022518 python_filewrap-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.6/readme.md
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.6/PKG-INFO
```

### Comparing `python_filewrap-0.0.5/LICENSE` & `python_filewrap-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.5/filewrap/__init__.py` & `python_filewrap-0.0.6/filewrap/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 5)
+__version__ = (0, 0, 6)
 __all__ = [
     "SupportsRead", "SupportsWrite", 
     "bio_chunk_iter", "bio_chunk_async_iter", 
     "bio_skip_iter", "bio_skip_async_iter", 
     "bytes_iter_to_reader", "bytes_iter_to_async_reader", 
-    "bytes_to_chunk_iter", "bytes_to_chunk_async_iter"
+    "bytes_to_chunk_iter", "bytes_to_chunk_async_iter", 
+    "bytes_ensure_part_iter", "bytes_ensure_part_async_iter", 
 ]
 
 from asyncio import to_thread, Lock as AsyncLock
 from collections.abc import Awaitable, AsyncIterable, Iterable
 from functools import update_wrapper
 from inspect import isawaitable, iscoroutinefunction
 from collections.abc import AsyncIterator, Callable, Iterator
 from shutil import COPY_BUFSIZE # type: ignore
 from threading import Lock
 from typing import Any, Protocol, TypeVar
 
-from asynctools import ensure_async
+try:
+    from collections.abc import Buffer # type: ignore
+except ImportError:
+    Buffer = Any
+
+from asynctools import ensure_async, ensure_aiter
 
 
 _T_co = TypeVar("_T_co", covariant=True)
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 
 class SupportsRead(Protocol[_T_co]):
@@ -32,20 +38,20 @@
 
 
 class SupportsWrite(Protocol[_T_contra]):
     def write(self, __s: _T_contra) -> object: ...
 
 
 def bio_chunk_iter(
-    bio: SupportsRead[bytes] | Callable[[int], bytes], 
+    bio: SupportsRead[Buffer] | Callable[[int], Buffer], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
-) -> Iterator[bytes]:
+) -> Iterator[Buffer]:
     if callable(bio):
         read = bio
     else:
         read = bio.read
     if not callable(callback):
         callback = None
     if size > 0:
@@ -63,20 +69,20 @@
         while (chunk := read(chunksize)):
             if callback:
                 callback(len(chunk))
             yield chunk
 
 
 async def bio_chunk_async_iter(
-    bio: SupportsRead[bytes] | Callable[[int], bytes | Awaitable[bytes]], 
+    bio: SupportsRead[Buffer] | Callable[[int], Buffer | Awaitable[Buffer]], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
-) -> AsyncIterator[bytes]:
+) -> AsyncIterator[Buffer]:
     if callable(bio):
         read = ensure_async(bio)
     else:
         read = ensure_async(bio.read)
     callback = ensure_async(callback) if callable(callback) else None
     if size > 0:
         while size:
@@ -93,15 +99,15 @@
         while (chunk := (await read(chunksize))):
             if callback:
                 await callback(len(chunk))
             yield chunk
 
 
 def bio_skip_iter(
-    bio: SupportsRead[bytes] | Callable[[int], bytes], 
+    bio: SupportsRead[Buffer] | Callable[[int], Buffer], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> Iterator[int]:
     if size == 0:
         return
@@ -164,15 +170,15 @@
     else:
         if callback:
             callback(length)
         yield length
 
 
 async def bio_skip_async_iter(
-    bio: SupportsRead[bytes] | Callable[[int], bytes | Awaitable[bytes]], 
+    bio: SupportsRead[Buffer] | Callable[[int], Buffer | Awaitable[Buffer]], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> AsyncIterator[int]:
     if size == 0:
         return
@@ -233,15 +239,15 @@
     else:
         if callback:
             await callback(length)
         yield length
 
 
 def bytes_iter_to_reader(
-    it: Iterable[bytes | bytearray], 
+    it: Iterable[Buffer], 
     /, 
 ) -> SupportsRead[bytearray]:
     getnext = iter(it).__next__
     at_end = False
     unconsumed: bytearray = bytearray()
     lock = Lock()
     def read(n=-1, /) -> bytearray:
@@ -321,15 +327,15 @@
         "__iter__": lambda self, /: self, 
         "__next__": staticmethod(__next__), 
         "__repr__": staticmethod(lambda: reprs), 
     })()
 
 
 def bytes_iter_to_async_reader(
-    it: Iterable[bytes | bytearray] | AsyncIterable[bytes | bytearray], 
+    it: Iterable[Buffer] | AsyncIterable[Buffer], 
     /, 
     threaded: bool = True, 
 ) -> SupportsRead[bytearray]:
     if isinstance(it, AsyncIterable):
         getnext = aiter(it).__anext__
     else:
         getnext = ensure_async(iter(it).__next__, threaded=threaded)
@@ -413,25 +419,81 @@
         "__iter__": lambda self, /: self, 
         "__next__": staticmethod(__next__), 
         "__repr__": staticmethod(lambda: reprs), 
     })()
 
 
 def bytes_to_chunk_iter(
-    b, 
+    b: Buffer, 
     /, 
-    chunksize=1<<16, 
+    chunksize: int = COPY_BUFSIZE, 
 ) -> Iterator[memoryview]:
     m = memoryview(b)
     for i in range(0, len(m), chunksize):
         yield m[i:i+chunksize]
 
 
 async def bytes_to_chunk_async_iter(
-    b, 
+    b: Buffer, 
     /, 
-    chunksize=1<<16, 
+    chunksize: int = COPY_BUFSIZE, 
 ) -> AsyncIterator[memoryview]:
     m = memoryview(b)
     for i in range(0, len(m), chunksize):
         yield m[i:i+chunksize]
 
+
+def bytes_ensure_part_iter(
+    it: Iterable[Buffer], 
+    /, 
+    partsize: int = COPY_BUFSIZE, 
+) -> Iterator[Buffer | memoryview]:
+    n = partsize
+    for b in it:
+        m = memoryview(b)
+        l = len(m)
+        if l <= n:
+            yield b
+            if l == n:
+                n = partsize
+            else:
+                n -= l
+        else:
+            yield m[:n]
+            m = m[n:]
+            while len(m) >= partsize:
+                yield m[:partsize]
+                m = m[partsize:]
+            if m:
+                yield m
+                n = partsize - len(m)
+            else:
+                n = partsize
+
+
+async def bytes_ensure_part_async_iter(
+    it: Iterable[Buffer] | AsyncIterable[Buffer], 
+    /, 
+    partsize: int = COPY_BUFSIZE, 
+) -> AsyncIterator[Buffer | memoryview]:
+    n = partsize
+    async for b in ensure_aiter(it):
+        m = memoryview(b)
+        l = len(m)
+        if l <= n:
+            yield b
+            if l == n:
+                n = partsize
+            else:
+                n -= l
+        else:
+            yield m[:n]
+            m = m[n:]
+            while len(m) >= partsize:
+                yield m[:partsize]
+                m = m[partsize:]
+            if m:
+                yield m
+                n = partsize - len(m)
+            else:
+                n = partsize
+
```

### Comparing `python_filewrap-0.0.5/pyproject.toml` & `python_filewrap-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.5/PKG-INFO` & `python_filewrap-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

