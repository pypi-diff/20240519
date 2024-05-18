# Comparing `tmp/uwebserver-0.1.3.tar.gz` & `tmp/uwebserver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwebserver-0.1.3.tar", last modified: Mon May 13 20:51:21 2024, max compression
+gzip compressed data, was "uwebserver-0.2.0.tar", last modified: Sat May 18 22:24:10 2024, max compression
```

## Comparing `uwebserver-0.1.3.tar` & `uwebserver-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 20:51:21.551142 uwebserver-0.1.3/
--rw-rw-rw-   0        0        0     1062 2024-05-12 16:25:08.000000 uwebserver-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2352 2024-05-13 20:51:21.540155 uwebserver-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-05-13 16:19:18.000000 uwebserver-0.1.3/README.md
--rw-rw-rw-   0        0        0     1015 2024-05-13 20:50:29.000000 uwebserver-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 20:51:21.551142 uwebserver-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 20:51:21.516143 uwebserver-0.1.3/uwebserver/
--rw-rw-rw-   0        0        0    10280 2024-05-13 20:44:04.000000 uwebserver-0.1.3/uwebserver/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-13 20:43:42.000000 uwebserver-0.1.3/uwebserver/py.typed
-drwxrwxrwx   0        0        0        0 2024-05-13 20:51:21.537143 uwebserver-0.1.3/uwebserver.egg-info/
--rw-rw-rw-   0        0        0     2352 2024-05-13 20:51:21.000000 uwebserver-0.1.3/uwebserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-05-13 20:51:21.000000 uwebserver-0.1.3/uwebserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 20:51:21.000000 uwebserver-0.1.3/uwebserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 20:51:21.000000 uwebserver-0.1.3/uwebserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 20:51:21.000000 uwebserver-0.1.3/uwebserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:24:10.250913 uwebserver-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-18 22:24:06.000000 uwebserver-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-18 22:24:10.250913 uwebserver-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-18 22:24:06.000000 uwebserver-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-18 22:24:06.000000 uwebserver-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:24:10.250913 uwebserver-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:24:10.250913 uwebserver-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-18 22:24:06.000000 uwebserver-0.2.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-18 22:24:06.000000 uwebserver-0.2.0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-18 22:24:06.000000 uwebserver-0.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-18 22:24:06.000000 uwebserver-0.2.0/tests/test_webserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:24:10.250913 uwebserver-0.2.0/uwebserver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2024-05-18 22:24:06.000000 uwebserver-0.2.0/uwebserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:24:06.000000 uwebserver-0.2.0/uwebserver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:24:10.250913 uwebserver-0.2.0/uwebserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-18 22:24:10.000000 uwebserver-0.2.0/uwebserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-18 22:24:10.000000 uwebserver-0.2.0/uwebserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:24:10.000000 uwebserver-0.2.0/uwebserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 22:24:10.000000 uwebserver-0.2.0/uwebserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-18 22:24:10.000000 uwebserver-0.2.0/uwebserver.egg-info/top_level.txt
```

### Comparing `uwebserver-0.1.3/LICENSE` & `uwebserver-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uwebserver-0.1.3/PKG-INFO` & `uwebserver-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-Metadata-Version: 2.1
-Name: uwebserver
-Version: 0.1.3
-Summary: Simple web server for micropython
-Author: 0x4aK
-License: MIT License
-        
-        Copyright (c) 2024 0x4aK
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/0x4aK/uWebServer
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: AsyncIO
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: ruff>=0.4.4; extra == "dev"
-Requires-Dist: pyright>=1.1.362; extra == "dev"
-
-# uWebServer
-
-TODO: simple slogan
-
-## Features
-
-- Simple interface
-
-## Examples
-
-```python
-import asyncio
-
-from uwebserver import Request, Response, WebServer
-
-app = WebServer()
-
-
-@app.route("/")
-async def hello(req: Request, resp: Response):
-    resp.set_content_type("text/html")
-    return "<h1>Hello World</h1>"
-
-
-asyncio.run(app.run())
-```
+Metadata-Version: 2.1
+Name: uwebserver
+Version: 0.2.0
+Summary: Simple web server for micropython
+Author: 0x4aK
+License: MIT License
+        
+        Copyright (c) 2024 0x4aK
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/0x4aK/uWebServer
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: ruff>=0.4.4; extra == "dev"
+Requires-Dist: pyright>=1.1.362; extra == "dev"
+
+# uWebServer
+
+Simple, fast and memory efficient web server for MicroPython.
+
+## ✅ Features
+
+- Compatible with CPython.
+- Type hints.
+- Static files with GZip compression.
+
+## ✏️ Examples
+
+```python
+import asyncio
+
+# Importing `Request` and `Response` optional, used for typehinting
+from uwebserver import Request, Response, WebServer
+
+app = WebServer()
+
+
+@app.route("/")
+async def hello(req: Request, resp: Response):
+    return "Hello world!"
+
+
+asyncio.run(app.run())
+```
+
+**Check out [📁examples](https://github.com/0x4aK/uWebServer/blob/master/examples) for more**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `uwebserver-0.1.3/pyproject.toml` & `uwebserver-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-[project]
-name = "uwebserver"
-version = "0.1.3"
-authors = [{ name = "0x4aK" }]
-description = "Simple web server for micropython"
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-    "Development Status :: 4 - Beta",
-    "Framework :: AsyncIO",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.10",
-]
-license = { file = "LICENSE" }
-urls = { repository = "https://github.com/0x4aK/uWebServer" }
-
-[project.optional-dependencies]
-dev = ["ruff >= 0.4.4", "pyright >= 1.1.362"]
-
-[build-system]
-requires = ["setuptools >= 69.5.1", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.setuptools]
-packages = ["uwebserver"]
-package-data = { "uwebserver" = ["py.typed"] }
-
-[tool.pyright]
-reportMissingImports = false
-
-[tool.ruff]
-line-length = 100
-lint = { select = ["E", "F", "I", "UP", "SIM"] }
+[project]
+name = "uwebserver"
+version = "0.2.0"
+authors = [{ name = "0x4aK" }]
+description = "Simple web server for micropython"
+readme = "README.md"
+requires-python = ">=3.10"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Framework :: AsyncIO",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+]
+license = { file = "LICENSE" }
+urls = { repository = "https://github.com/0x4aK/uWebServer" }
+
+[project.optional-dependencies]
+dev = ["ruff >= 0.4.4", "pyright >= 1.1.362"]
+
+[build-system]
+requires = ["setuptools >= 69.5.1", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools]
+packages = ["uwebserver"]
+package-data = { "uwebserver" = ["py.typed"] }
+
+[tool.pyright]
+reportMissingImports = false
+
+[tool.ruff]
+line-length = 100
+lint = { select = ["E", "F", "I", "UP", "SIM"] }
```

### Comparing `uwebserver-0.1.3/uwebserver/__init__.py` & `uwebserver-0.2.0/uwebserver/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,341 +1,359 @@
-import asyncio
-import gc
-import os
-from collections import namedtuple
-
-try:
-    from collections.abc import Callable, Coroutine, Iterable
-    from typing import TYPE_CHECKING, Literal, TypeAlias, TypeGuard
-except ImportError:
-    TYPE_CHECKING = False
-
-
-if TYPE_CHECKING:
-    BytesIter: TypeAlias = "Iterable[bytes]"
-    Body: TypeAlias = "bytes|BytesIter|None"
-    Results: TypeAlias = "Coroutine[None,None,Body|str]"
-    Handler: TypeAlias = "Callable[[Request,Response],Results]"
-    ErrorHanlder: TypeAlias = "Callable[[Request,Response,Exception],Results]"
-    Methods: TypeAlias = "Iterable[Literal['GET','POST','DELETE','PUT','HEAD','OPTIONS']]"
-    StrDict: TypeAlias = "dict[str,str]"
-
-try:
-    import micropython
-except ImportError:
-    from types import SimpleNamespace
-
-    micropython = SimpleNamespace(const=lambda i: i)
-
-_READ_SIZE = micropython.const(128)
-_WRITE_BUFFER_SIZE = micropython.const(128)
-_FILE_INDICATOR = micropython.const(1 << 16)
-MIME_TYPES = {
-    "css": "text/css",
-    "png": "image/png",
-    "html": "text/html",
-    "jpg": "image/jpeg",
-    "jpeg": "image/jpeg",
-    "ico": "image/x-icon",
-    "svg": "image/svg+xml",
-    "json": "application/json",
-    "js": "application/javascript",
-}
-
-
-_FileInfo = namedtuple("_FileInfo", "path size encoding")
-
-
-def _iterable(o: object) -> "TypeGuard[BytesIter]":
-    return hasattr(o, "__next__") or hasattr(o, "__iter__")
-
-
-def _raise(e: Exception):
-    raise e
-
-
-def _gc_after(f):
-    async def w(*args):
-        try:
-            return await f(*args)
-        except:
-            raise
-        finally:
-            gc.collect()
-
-    return w
-
-
-def _parse_request(raw: str) -> tuple[str, str, str]:
-    m, p, v = r if len(r := raw.split(" ", 2)) == 3 else _raise(ValueError("Invalid request line"))
-    return m, p, v
-
-
-def _parse_header(header: str) -> tuple[str, str]:
-    n, _, v = header.partition(":")
-    return n.lower(), v.strip()
-
-
-def _parse_headers(raw: str) -> "StrDict":
-    return dict(map(_parse_header, raw.split("\r\n")))
-
-
-def _parse_qsv(qkv: str) -> tuple[str, str]:
-    k, _, v = qkv.partition("=")
-    return k, v
-
-
-def _parse_qs(raw: str) -> "StrDict":
-    return dict(map(_parse_qsv, raw.split("&")))
-
-
-def _parse_path(raw: str) -> "tuple[str, StrDict | None]":
-    p, rqs = raw.split("?", 1) if "?" in raw else (raw, None)
-    return p, _parse_qs(rqs) if rqs is not None else None
-
-
-def _get_file_size(path: str) -> int | None:
-    try:
-        stat = os.stat(path)
-    except OSError:
-        return None
-    if stat[0] & _FILE_INDICATOR != 0:
-        return None
-    return stat[6]
-
-
-class _Reader:
-    def __init__(self, stream: asyncio.StreamReader):
-        self.b = b""
-        self.s = stream
-
-    async def readuntil(self, sep=b"\n"):
-        b, sr = self.b, self.s.read
-        while (i := b.find(sep)) < 0 and (d := await sr(_READ_SIZE)):
-            b += d
-
-        r, self.b = b[:i], b[i + len(sep) :]
-        return r.decode()
-
-    async def readexactly(self, n: int):
-        b, sr = self.b, self.s.read
-        while len(b) < n and (d := await sr(_READ_SIZE)):
-            b += d
-
-        r, self.b = b[:n], b[n:]
-        return r.decode()
-
-
-class Response:
-    def __init__(self):
-        self.headers = {"connection": "close", "content-type": "text/plain"}
-        self.body: "Body" = None
-        self.status = b"200 OK"
-
-    def set_header(self, header: str, value: str):
-        self.headers[header] = value
-
-    def set_status(self, status: bytes | str):
-        self.status = status.encode() if isinstance(status, str) else status
-
-    def set_body(self, body: "Body | str"):
-        self.body = body.encode() if isinstance(body, str) else body
-
-    def set_content_type(self, ct: str):
-        self.headers["content-type"] = ct
-
-
-class Request:
-    def __init__(
-        self,
-        method: str,
-        path: str,
-        version: str,
-        headers: "StrDict",
-        qs: "StrDict | None",
-        body: str | None,
-    ) -> None:
-        self.method = method
-        self.path = path
-        self.version = version
-        self.headers = headers
-        self.qs = qs
-        self.body = body
-
-    @classmethod
-    @_gc_after
-    async def from_stream(cls, s: asyncio.StreamReader) -> "Request":
-        r = _Reader(s)
-
-        m, rp, v = _parse_request(await r.readuntil(b"\r\n"))
-        p, qs = _parse_path(rp)
-        h = _parse_headers(await r.readuntil(b"\r\n\r\n"))
-        b = await r.readexactly(int(bl)) if (bl := h.get("content-length")) else None
-        return cls(m, p, v, h, qs, b)
-
-
-class WebServer:
-    def __init__(
-        self,
-        *,
-        host: str = "0.0.0.0",
-        port: int = 80,
-        static_folder: str = "static",
-    ) -> None:
-        self.host = host
-        self.port = port
-        self.r: dict[tuple[str, str], Handler] = {}
-        self.static = static_folder
-        self._cah: "Handler" = self._dch  # Catch-all handler
-        self._eh: "ErrorHanlder" = self._deh  # Error handler
-        self.s: asyncio.Server | None = None
-
-    def route(self, path: str, methods: "Methods" = ("GET",)):
-        def w(handler: "Handler"):
-            self.add_route(path, handler, methods)
-            return handler
-
-        return w
-
-    def add_route(self, path: str, handler: "Handler", methods: "Methods" = ("GET",)):
-        for method in methods:
-            self.r[(method.upper(), path)] = handler
-
-    @staticmethod
-    async def _dch(req: Request, resp: Response):
-        "Default catch-all handler"
-        resp.set_status(b"404 Not Found")
-        return "Not Found"
-
-    def catchall(self, h: "Handler"):
-        self.set_catchall(h)
-        return h
-
-    def set_catchall(self, h: "Handler"):
-        self._cah = h
-
-    @staticmethod
-    async def _deh(req: Request, resp: Response, e: Exception):
-        "Default error handler"
-        print("Error while handling:", repr(e))
-        resp.set_status(b"500 Internal Server Error")
-        resp.set_content_type("text/plain")
-        return f"Error: {str(e)}"
-
-    def error_handler(self, h: "ErrorHanlder"):
-        self.set_error_handler(h)
-        return h
-
-    def set_error_handler(self, h: "ErrorHanlder"):
-        self._eh = h
-
-    @staticmethod
-    async def _write_status(w, s: bytes):
-        w.write(b"HTTP/1.1 %s\r\n" % s)
-        await w.drain()
-
-    @staticmethod
-    async def _write_headers(w, h: "StrDict"):
-        for v in map(lambda v: tuple(map(str.encode, v)), h.items()):
-            w.write(b"%s: %s\r\n" % v)
-        w.write(b"\r\n")
-        await w.drain()
-
-    async def _respond(self, w, s: bytes, h: "StrDict", b: bytes | None):
-        await self._write_status(w, s)
-
-        if b is None:
-            await self._write_headers(w, h)
-            return
-
-        h["content-length"] = str(len(b))
-        await self._write_headers(w, h)
-        w.write(b)
-        await w.drain()
-
-    async def _respond_file(self, w, s: bytes, h: "StrDict", p: str):
-        ext = (e := p.rsplit(".", 2))[-2 if e[-1] == "gz" else -1]
-        if ct := MIME_TYPES.get(ext):
-            h["content-type"] = ct
-
-        await self._write_status(w, s)
-        await self._write_headers(w, h)
-
-        wb, ww, wd = bytearray(_WRITE_BUFFER_SIZE), w.write, w.drain
-        with open(p, "rb") as f:
-            while f.readinto(wb):
-                ww(wb)
-                await wd()
-
-    async def _respond_chunks(self, w, s: bytes, h: "StrDict", i: "BytesIter"):
-        h["transfer-encoding"] = "chunked"
-        await self._write_status(w, s)
-        await self._write_headers(w, h)
-
-        ww, wd = w.write, w.drain
-        for d in i:
-            ww(b"%x\r\n%s\r\n" % (len(d), d))
-            await wd()
-        ww(b"0\r\n\r\n")
-        await wd()
-
-    def _get_static(self, req: Request):
-        path = "./" + self.static + req.path + ("index.html" if req.path.endswith("/") else "")
-
-        if "gzip" in req.headers.get("accept-encoding", "") and (
-            fsize := _get_file_size(path + ".gz")
-        ):
-            return _FileInfo(path + ".gz", fsize, "gzip")
-
-        elif fsize := _get_file_size(path):
-            return _FileInfo(path, fsize, None)
-
-    async def _handle_static(self, w, resp: Response, fi: _FileInfo):
-        resp.set_header("content-length", str(fi.size))
-        if fi.encoding:
-            resp.set_header("content-encoding", fi.encoding)
-        await self._respond_file(w, resp.status, resp.headers, fi.path)
-
-    async def _handle_request(self, w, req: Request, resp: Response):
-        try:
-            if handler := self.r.get((req.method, req.path)):
-                r = await handler(req, resp)
-            elif req.method == "GET" and (fi := self._get_static(req)):
-                await self._handle_static(w, resp, fi)
-                return
-            else:
-                r = await self._cah(req, resp)
-
-        except Exception as e:
-            r = await self._eh(req, resp, e)
-
-        if r is not None:
-            resp.set_body(r)
-
-        if isinstance(resp.body, bytes):
-            await self._respond(w, resp.status, resp.headers, resp.body)
-        elif _iterable(resp.body):
-            await self._respond_chunks(w, resp.status, resp.headers, resp.body)
-        else:
-            await self._respond(w, resp.status, resp.headers, str(resp.body).encode())
-
-    @_gc_after
-    async def _handle(self, r, w):
-        print("Got request from", w.get_extra_info("peername"))
-        resp = Response()
-
-        try:
-            req = await Request.from_stream(r)
-        except Exception as e:
-            print("Error while parsing:", repr(e))
-            await self._respond(w, b"400 Bad Request", resp.headers, b"Bad Request")
-        else:
-            await self._handle_request(w, req, resp)
-        finally:
-            w.close()
-
-    def close(self):
-        return self.s and self.s.close()
-
-    async def run(self):
-        self.s = await asyncio.start_server(self._handle, self.host, self.port)
-        await self.s.wait_closed()
+import asyncio
+import gc
+import os
+
+try:
+    from collections.abc import Callable, Coroutine, Iterable
+    from typing import TYPE_CHECKING, Literal, TypeAlias, TypeGuard
+except ImportError:
+    TYPE_CHECKING = False
+
+
+if TYPE_CHECKING:
+    StrDict: TypeAlias = "dict[str,str]"
+    BytesIter: TypeAlias = "Iterable[bytes]"
+    Body: TypeAlias = "bytes|BytesIter|File|None"
+    Results: TypeAlias = "Coroutine[None,None,Body|str]"
+    Handler: TypeAlias = "Callable[[Request,Response],Results]"
+    ErrorHanlder: TypeAlias = "Callable[[Request,Response,Exception],Results]"
+    Methods: TypeAlias = "Iterable[Literal['GET','POST','DELETE','PUT','HEAD','OPTIONS']]"
+    Encodings: TypeAlias = "Literal['gzip']"
+
+try:
+    import micropython
+except ImportError:
+    from types import SimpleNamespace
+
+    micropython = SimpleNamespace(const=lambda i: i)
+
+_READ_SIZE = micropython.const(128)
+_WRITE_BUFFER_SIZE = micropython.const(128)
+_FILE_INDICATOR = micropython.const(1 << 16)
+MIME_TYPES = {
+    "css": "text/css",
+    "png": "image/png",
+    "html": "text/html",
+    "jpg": "image/jpeg",
+    "jpeg": "image/jpeg",
+    "ico": "image/x-icon",
+    "svg": "image/svg+xml",
+    "json": "application/json",
+    "js": "application/javascript",
+}
+
+
+def _iterable(o: object) -> "TypeGuard[BytesIter]":
+    return hasattr(o, "__next__") or hasattr(o, "__iter__")
+
+
+def _raise(e: Exception):
+    raise e
+
+
+def _gc_after(f):
+    async def w(*args):
+        try:
+            return await f(*args)
+        except:
+            raise
+        finally:
+            gc.collect()
+
+    return w
+
+
+def _parse_request(raw: str) -> tuple[str, str, str]:
+    m, p, v = r if len(r := raw.split(" ")) == 3 else _raise(ValueError("Invalid request line"))
+    return m, p, v
+
+
+def _parse_header(header: str) -> tuple[str, str]:
+    n, _, v = header.partition(":")
+    return n.lower(), v.strip()
+
+
+def _parse_headers(raw: str) -> "StrDict":
+    return dict(map(_parse_header, raw.split("\r\n")))
+
+
+def _parse_qsv(qkv: str) -> tuple[str, str]:
+    k, _, v = qkv.partition("=")
+    return k, v
+
+
+def _parse_qs(raw: str) -> "StrDict":
+    return dict(map(_parse_qsv, raw.split("&")))
+
+
+def _parse_path(raw: str) -> "tuple[str, StrDict | None]":
+    p, rqs = raw.split("?", 1) if "?" in raw else (raw, None)
+    return p, _parse_qs(rqs) if rqs is not None else None
+
+
+def _get_file_size(path: str) -> int | None:
+    try:
+        stat = os.stat(path)
+    except OSError:
+        return None
+    if stat[0] & _FILE_INDICATOR:
+        return None
+    return stat[6]
+
+
+class _Reader:
+    def __init__(self, stream: asyncio.StreamReader):
+        self.b = b""
+        self.s = stream
+
+    async def readuntil(self, sep=b"\n"):
+        b, sr = self.b, self.s.read
+        while (i := b.find(sep)) < 0 and (d := await sr(_READ_SIZE)):
+            b += d
+
+        r, self.b = b[:i], b[i + len(sep) :]
+        return r.decode()
+
+    async def readexactly(self, n: int):
+        b, sr = self.b, self.s.read
+        while len(b) < n and (d := await sr(_READ_SIZE)):
+            b += d
+
+        r, self.b = b[:n], b[n:]
+        return r.decode()
+
+
+class File:
+    def __init__(
+        self,
+        path: str,
+        size: int | None = None,
+        encoding: "Encodings | None" = None,
+    ) -> None:
+        self.s = size or _get_file_size(path) or _raise(OSError("Invalid file"))
+        self.e = encoding
+        self.p = path
+
+    @classmethod
+    def from_path(cls, path: str, encoding: "Encodings | None" = None):
+        if s := _get_file_size(path):
+            return cls(path, s, encoding)
+
+
+class Request:
+    def __init__(
+        self,
+        method: str,
+        path: str,
+        version: str,
+        headers: "StrDict",
+        qs: "StrDict | None",
+        body: str | None,
+    ) -> None:
+        self.method = method
+        self.path = path
+        self.version = version
+        self.headers = headers
+        self.qs = qs
+        self.body = body
+
+    @classmethod
+    @_gc_after
+    async def from_stream(cls, s: asyncio.StreamReader) -> "Request":
+        r = _Reader(s)
+
+        m, rp, v = _parse_request(await r.readuntil(b"\r\n"))
+        p, qs = _parse_path(rp)
+        h = _parse_headers(await r.readuntil(b"\r\n\r\n"))
+        b = await r.readexactly(int(bl)) if (bl := h.get("content-length")) else None
+        return cls(m, p, v, h, qs, b)
+
+
+class Response:
+    def __init__(self):
+        self.headers = {"connection": "close", "content-type": "text/plain"}
+        self.body: "Body" = None
+        self.status = b"200 OK"
+
+    def set_header(self, header: str, value: str):
+        self.headers[header] = value
+
+    def set_status(self, status: bytes | str):
+        self.status = status.encode() if isinstance(status, str) else status
+
+    def set_body(self, body: "Body | str"):
+        self.body = body.encode() if isinstance(body, str) else body
+
+    def set_content_type(self, ct: str):
+        self.headers["content-type"] = ct
+
+
+class WebServer:
+    def __init__(
+        self,
+        *,
+        host: str = "0.0.0.0",
+        port: int = 80,
+        static_folder: str | None = "static",
+        request_timeout: float = 5,
+    ) -> None:
+        self.host = host
+        self.port = port
+        self.r: dict[tuple[str, str], Handler] = {}
+        self.static = static_folder
+        self.timeout = request_timeout
+        self._cah: "Handler" = self._dch  # Catch-all handler
+        self._eh: "ErrorHanlder" = self._deh  # Error handler
+        self.s: asyncio.Server | None = None
+        self._r = asyncio.Event()
+
+    def route(self, path: str, methods: "Methods" = ("GET",)):
+        def w(handler: "Handler"):
+            self.add_route(path, handler, methods)
+            return handler
+
+        return w
+
+    def add_route(self, path: str, handler: "Handler", methods: "Methods" = ("GET",)):
+        for method in methods:
+            self.r[(method.upper(), path)] = handler
+
+    @staticmethod
+    async def _dch(req: Request, resp: Response):
+        "Default catch-all handler"
+        resp.set_status(b"404 Not Found")
+        return "Not Found"
+
+    def catchall(self, h: "Handler"):
+        self._cah = h
+        return h
+
+    @staticmethod
+    async def _deh(req: Request, resp: Response, e: Exception):
+        "Default error handler"
+        print("Error while handling:", repr(e))
+        resp.set_status(b"500 Internal Server Error")
+        resp.set_content_type("text/plain")
+        return f"Error: {str(e)}"
+
+    def error_handler(self, h: "ErrorHanlder"):
+        self._eh = h
+        return h
+
+    @staticmethod
+    async def _write_status(w, s: bytes):
+        w.write(b"HTTP/1.1 %s\r\n" % s)
+        await w.drain()
+
+    @staticmethod
+    async def _write_headers(w, h: "StrDict"):
+        for v in map(lambda v: tuple(map(str.encode, v)), h.items()):
+            w.write(b"%s: %s\r\n" % v)
+        w.write(b"\r\n")
+        await w.drain()
+
+    async def _respond(self, w, s: bytes, h: "StrDict", b: bytes | None):
+        await self._write_status(w, s)
+
+        if b is None:
+            await self._write_headers(w, h)
+            return
+
+        h["content-length"] = str(len(b))
+        await self._write_headers(w, h)
+        w.write(b)
+        await w.drain()
+
+    async def _respond_file(self, w, s: bytes, h: "StrDict", fi: File):
+        h["content-length"] = str(fi.s)
+
+        if fi.e is not None:
+            h["content-encoding"] = fi.e
+
+        ext = (fi.p.rsplit(".", 2))[-2 if fi.e else -1]
+        if ct := MIME_TYPES.get(ext):
+            h["content-type"] = ct
+
+        await self._write_status(w, s)
+        await self._write_headers(w, h)
+
+        wb, ww, wd = memoryview(bytearray(_WRITE_BUFFER_SIZE)), w.write, w.drain
+        with open(fi.p, "rb") as f:
+            while r := f.readinto(wb):
+                ww(wb[:r])
+                await wd()
+
+    async def _respond_chunks(self, w, s: bytes, h: "StrDict", i: "BytesIter"):
+        h["transfer-encoding"] = "chunked"
+        await self._write_status(w, s)
+        await self._write_headers(w, h)
+
+        ww, wd = w.write, w.drain
+        for d in i:
+            ww(b"%x\r\n%s\r\n" % (len(d), d))
+            await wd()
+        ww(b"0\r\n\r\n")
+        await wd()
+
+    def _get_static(self, req: Request):
+        if self.static is None:
+            return
+
+        p = "./" + self.static + req.path + ("index.html" if req.path.endswith("/") else "")
+
+        if (
+            "gzip" in req.headers.get("accept-encoding", "")
+            and (fi := File.from_path(p + ".gz", "gzip"))
+            or (fi := File.from_path(p))
+        ):
+            return fi
+
+    async def _handle_request(self, w, req: Request, resp: Response):
+        try:
+            if h := self.r.get((req.method, req.path)):
+                r = await h(req, resp)
+            elif req.method == "GET" and (fi := self._get_static(req)):
+                r = fi
+            else:
+                r = await self._cah(req, resp)
+
+        except Exception as e:
+            r = await self._eh(req, resp, e)
+
+        if r is not None:
+            resp.set_body(r)
+
+        if isinstance(resp.body, bytes) or resp.body is None:
+            await self._respond(w, resp.status, resp.headers, resp.body)
+        elif isinstance(resp.body, File):
+            await self._respond_file(w, resp.status, resp.headers, resp.body)
+        elif _iterable(resp.body):
+            await self._respond_chunks(w, resp.status, resp.headers, resp.body)
+        else:
+            await self._respond(w, resp.status, resp.headers, str(resp.body).encode())
+
+    @_gc_after
+    async def _handle(self, r, w):
+        resp = Response()
+
+        try:
+            req = await asyncio.wait_for(Request.from_stream(r), self.timeout)
+        except asyncio.TimeoutError:
+            await self._respond(w, b"408 Request timeout", resp.headers, b"Timeout")
+        except Exception:
+            await self._respond(w, b"400 Bad Request", resp.headers, b"Bad Request")
+        else:
+            await self._handle_request(w, req, resp)
+        finally:
+            w.close()
+            await w.wait_closed()
+
+    def close(self):
+        return self.s and self.s.close()
+
+    async def wait_ready(self):
+        await self._r.wait()
+
+    async def run(self):
+        self.s = await asyncio.start_server(self._handle, self.host, self.port)
+        self._r.set()
+        await self.s.wait_closed()
```

### Comparing `uwebserver-0.1.3/uwebserver.egg-info/PKG-INFO` & `uwebserver-0.2.0/uwebserver.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-Metadata-Version: 2.1
-Name: uwebserver
-Version: 0.1.3
-Summary: Simple web server for micropython
-Author: 0x4aK
-License: MIT License
-        
-        Copyright (c) 2024 0x4aK
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: repository, https://github.com/0x4aK/uWebServer
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: AsyncIO
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: dev
-Requires-Dist: ruff>=0.4.4; extra == "dev"
-Requires-Dist: pyright>=1.1.362; extra == "dev"
-
-# uWebServer
-
-TODO: simple slogan
-
-## Features
-
-- Simple interface
-
-## Examples
-
-```python
-import asyncio
-
-from uwebserver import Request, Response, WebServer
-
-app = WebServer()
-
-
-@app.route("/")
-async def hello(req: Request, resp: Response):
-    resp.set_content_type("text/html")
-    return "<h1>Hello World</h1>"
-
-
-asyncio.run(app.run())
-```
+Metadata-Version: 2.1
+Name: uwebserver
+Version: 0.2.0
+Summary: Simple web server for micropython
+Author: 0x4aK
+License: MIT License
+        
+        Copyright (c) 2024 0x4aK
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/0x4aK/uWebServer
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: AsyncIO
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: ruff>=0.4.4; extra == "dev"
+Requires-Dist: pyright>=1.1.362; extra == "dev"
+
+# uWebServer
+
+Simple, fast and memory efficient web server for MicroPython.
+
+## ✅ Features
+
+- Compatible with CPython.
+- Type hints.
+- Static files with GZip compression.
+
+## ✏️ Examples
+
+```python
+import asyncio
+
+# Importing `Request` and `Response` optional, used for typehinting
+from uwebserver import Request, Response, WebServer
+
+app = WebServer()
+
+
+@app.route("/")
+async def hello(req: Request, resp: Response):
+    return "Hello world!"
+
+
+asyncio.run(app.run())
+```
+
+**Check out [📁examples](https://github.com/0x4aK/uWebServer/blob/master/examples) for more**
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

