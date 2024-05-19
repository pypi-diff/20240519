# Comparing `tmp/trengine-1.2.tar.gz` & `tmp/trengine-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trengine-1.2.tar", last modified: Thu May 16 23:26:59 2024, max compression
+gzip compressed data, was "trengine-1.3.tar", last modified: Sat May 18 17:18:51 2024, max compression
```

## Comparing `trengine-1.2.tar` & `trengine-1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 23:26:59.352201 trengine-1.2/
--rw-rw-rw-   0        0        0     1080 2024-05-16 22:50:59.000000 trengine-1.2/LICENSE
--rw-rw-rw-   0        0        0     1961 2024-05-16 23:26:59.339235 trengine-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2024-05-16 23:25:50.000000 trengine-1.2/README.md
--rw-rw-rw-   0        0        0      587 2024-05-16 23:21:24.000000 trengine-1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 23:26:59.352201 trengine-1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 23:26:59.144755 trengine-1.2/trengine/
--rw-rw-rw-   0        0        0     1284 2024-05-16 23:18:11.000000 trengine-1.2/trengine/__init__.py
--rw-rw-rw-   0        0        0     3191 2024-05-16 22:50:59.000000 trengine-1.2/trengine/ajax.py
--rw-rw-rw-   0        0        0       42 2024-05-16 22:50:59.000000 trengine-1.2/trengine/exceptions.py
--rw-rw-rw-   0        0        0     1425 2024-05-16 22:50:59.000000 trengine-1.2/trengine/google.py
--rw-rw-rw-   0        0        0     1783 2024-05-16 22:50:59.000000 trengine-1.2/trengine/hozory.py
--rw-rw-rw-   0        0        0     3013 2024-05-16 23:20:58.000000 trengine-1.2/trengine/ocr.py
--rw-rw-rw-   0        0        0      968 2024-05-16 22:50:59.000000 trengine-1.2/trengine/tdict.py
--rw-rw-rw-   0        0        0     1776 2024-05-16 22:50:59.000000 trengine-1.2/trengine/types.py
-drwxrwxrwx   0        0        0        0 2024-05-16 23:26:59.338237 trengine-1.2/trengine.egg-info/
--rw-rw-rw-   0        0        0     1961 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-16 23:26:59.000000 trengine-1.2/trengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 23:26:58.000000 trengine-1.2/trengine.egg-info/top_level.txt
+drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-18 17:18:51.870627 trengine-1.3/
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1060 2024-05-18 16:59:11.000000 trengine-1.3/LICENSE
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1865 2024-05-18 17:18:51.869627 trengine-1.3/PKG-INFO
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1283 2024-05-18 16:59:11.000000 trengine-1.3/README.md
+-rw-r--r--   0 zaid      (1000) zaid      (1000)      551 2024-05-18 17:15:32.000000 trengine-1.3/pyproject.toml
+-rw-r--r--   0 zaid      (1000) zaid      (1000)       38 2024-05-18 17:18:51.870627 trengine-1.3/setup.cfg
+drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-18 17:18:51.865627 trengine-1.3/trengine/
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1231 2024-05-18 16:59:11.000000 trengine-1.3/trengine/__init__.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     3092 2024-05-18 16:59:11.000000 trengine-1.3/trengine/ajax.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)       40 2024-05-18 16:59:11.000000 trengine-1.3/trengine/exceptions.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1375 2024-05-18 16:59:11.000000 trengine-1.3/trengine/google.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1722 2024-05-18 16:59:11.000000 trengine-1.3/trengine/hozory.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     2862 2024-05-18 17:15:12.000000 trengine-1.3/trengine/ocr.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)      930 2024-05-18 16:59:11.000000 trengine-1.3/trengine/tdict.py
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1712 2024-05-18 16:59:11.000000 trengine-1.3/trengine/types.py
+drwxr-xr-x   0 zaid      (1000) zaid      (1000)        0 2024-05-18 17:18:51.868627 trengine-1.3/trengine.egg-info/
+-rw-r--r--   0 zaid      (1000) zaid      (1000)     1865 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/PKG-INFO
+-rw-r--r--   0 zaid      (1000) zaid      (1000)      342 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/SOURCES.txt
+-rw-r--r--   0 zaid      (1000) zaid      (1000)        1 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/dependency_links.txt
+-rw-r--r--   0 zaid      (1000) zaid      (1000)       25 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/requires.txt
+-rw-r--r--   0 zaid      (1000) zaid      (1000)        9 2024-05-18 17:18:51.000000 trengine-1.3/trengine.egg-info/top_level.txt
```

### Comparing `trengine-1.2/LICENSE` & `trengine-1.3/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 ZAID
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 ZAID
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `trengine-1.2/PKG-INFO` & `trengine-1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-Metadata-Version: 2.1
-Name: trengine
-Version: 1.2
-Summary: TREngine is python library based on 4 translators engines
-Author-email: ZAID <y8838@hotmail.com>
-Project-URL: Homepage, https://github.com/zaid5o5/trengine
-Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: asyncio
-Requires-Dist: requests
-Requires-Dist: aiofiles
-
-# Install:
-```commandline
-pip install trengine
-```
-
-# About this project:
-- TREngine is python library based on 4 translators engines with OCR:
-- Ajax ( [translate.com](https://www.translate.com/translator) )
-- Google ( [translate.google.com](https://translate.google.com/) )
-- Hozory ( [hozory.com](https://hozory.com/FA) )
-- Translatedict ( [translatedict.com](https://www.translatedict.com/) )
-- OCR ( [ocr.space](https://ocr.space/) )
-
-- Supporting Sync & Async.
-
-# How to use?
-- Here an example to use it:
-```python
-from trengine import Engine
-
-eng = Engine()
-text = "Hola, mi amor"
-
-print(
-    eng.google.translate(text, "en"), "\n",
-    eng.ajax.translate(text, "en"), "\n",
-    eng.hozory.translate(text, "en"), "\n",
-    eng.tdict.translate(text, "en"), "\n",
-)
-
-# OCR
-print(eng.ocr.from_image("./test.png"))
-```
-- Here an async example:
-```python
-import asyncio
-from trengine import AsyncEngine
-
-eng = AsyncEngine()
-text = "Hola, mi amor"
-
-async def main():
-    print(
-        await eng.google.translate(text, "en"), "\n",
-        await eng.ajax.translate(text, "en"), "\n",
-        await eng.hozory.translate(text, "en"), "\n",
-        await eng.tdict.translate(text, "en"), "\n",
-    )
-
-    # OCR
-    print(await eng.ocr.from_image("./test.png"))
-
-asyncio.run(main())
-```
+Metadata-Version: 2.1
+Name: trengine
+Version: 1.3
+Summary: TREngine is python library based on 4 translators engines
+Author-email: ZAID <y8838@hotmail.com>
+Project-URL: Homepage, https://github.com/zaid5o5/trengine
+Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: asyncio
+Requires-Dist: requests
+
+# Install:
+```commandline
+pip install trengine
+```
+
+# About this project:
+- TREngine is python library based on 4 translators engines with OCR:
+- Ajax ( [translate.com](https://www.translate.com/translator) )
+- Google ( [translate.google.com](https://translate.google.com/) )
+- Hozory ( [hozory.com](https://hozory.com/FA) )
+- Translatedict ( [translatedict.com](https://www.translatedict.com/) )
+- OCR ( [ocr.space](https://ocr.space/) )
+
+- Supporting Sync & Async.
+
+# How to use?
+- Here an example to use it:
+```python
+from trengine import Engine
+
+eng = Engine()
+text = "Hola, mi amor"
+
+print(
+    eng.google.translate(text, "en"), "\n",
+    eng.ajax.translate(text, "en"), "\n",
+    eng.hozory.translate(text, "en"), "\n",
+    eng.tdict.translate(text, "en"), "\n",
+)
+
+# OCR
+print(eng.ocr.from_image("./test.png"))
+```
+- Here an async example:
+```python
+import asyncio
+from trengine import AsyncEngine
+
+eng = AsyncEngine()
+text = "Hola, mi amor"
+
+async def main():
+    print(
+        await eng.google.translate(text, "en"), "\n",
+        await eng.ajax.translate(text, "en"), "\n",
+        await eng.hozory.translate(text, "en"), "\n",
+        await eng.tdict.translate(text, "en"), "\n",
+    )
+
+    # OCR
+    print(await eng.ocr.from_image("./test.png"))
+
+asyncio.run(main())
+```
```

### Comparing `trengine-1.2/README.md` & `trengine-1.3/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# Install:
-```commandline
-pip install trengine
-```
-
-# About this project:
-- TREngine is python library based on 4 translators engines with OCR:
-- Ajax ( [translate.com](https://www.translate.com/translator) )
-- Google ( [translate.google.com](https://translate.google.com/) )
-- Hozory ( [hozory.com](https://hozory.com/FA) )
-- Translatedict ( [translatedict.com](https://www.translatedict.com/) )
-- OCR ( [ocr.space](https://ocr.space/) )
-
-- Supporting Sync & Async.
-
-# How to use?
-- Here an example to use it:
-```python
-from trengine import Engine
-
-eng = Engine()
-text = "Hola, mi amor"
-
-print(
-    eng.google.translate(text, "en"), "\n",
-    eng.ajax.translate(text, "en"), "\n",
-    eng.hozory.translate(text, "en"), "\n",
-    eng.tdict.translate(text, "en"), "\n",
-)
-
-# OCR
-print(eng.ocr.from_image("./test.png"))
-```
-- Here an async example:
-```python
-import asyncio
-from trengine import AsyncEngine
-
-eng = AsyncEngine()
-text = "Hola, mi amor"
-
-async def main():
-    print(
-        await eng.google.translate(text, "en"), "\n",
-        await eng.ajax.translate(text, "en"), "\n",
-        await eng.hozory.translate(text, "en"), "\n",
-        await eng.tdict.translate(text, "en"), "\n",
-    )
-
-    # OCR
-    print(await eng.ocr.from_image("./test.png"))
-
-asyncio.run(main())
+# Install:
+```commandline
+pip install trengine
+```
+
+# About this project:
+- TREngine is python library based on 4 translators engines with OCR:
+- Ajax ( [translate.com](https://www.translate.com/translator) )
+- Google ( [translate.google.com](https://translate.google.com/) )
+- Hozory ( [hozory.com](https://hozory.com/FA) )
+- Translatedict ( [translatedict.com](https://www.translatedict.com/) )
+- OCR ( [ocr.space](https://ocr.space/) )
+
+- Supporting Sync & Async.
+
+# How to use?
+- Here an example to use it:
+```python
+from trengine import Engine
+
+eng = Engine()
+text = "Hola, mi amor"
+
+print(
+    eng.google.translate(text, "en"), "\n",
+    eng.ajax.translate(text, "en"), "\n",
+    eng.hozory.translate(text, "en"), "\n",
+    eng.tdict.translate(text, "en"), "\n",
+)
+
+# OCR
+print(eng.ocr.from_image("./test.png"))
+```
+- Here an async example:
+```python
+import asyncio
+from trengine import AsyncEngine
+
+eng = AsyncEngine()
+text = "Hola, mi amor"
+
+async def main():
+    print(
+        await eng.google.translate(text, "en"), "\n",
+        await eng.ajax.translate(text, "en"), "\n",
+        await eng.hozory.translate(text, "en"), "\n",
+        await eng.tdict.translate(text, "en"), "\n",
+    )
+
+    # OCR
+    print(await eng.ocr.from_image("./test.png"))
+
+asyncio.run(main())
 ```
```

### Comparing `trengine-1.2/trengine/google.py` & `trengine-1.3/trengine/google.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from aiohttp import ClientSession
-
-from .types import GoogleTranslateResult
-
-import requests
-
-
-class GoogleTranslator:
-    def __init__(self) -> None:
-        pass
-
-    def translate(self, text: str, dest: str = "en") -> "GoogleTranslateResult":
-        response = requests.get(
-            f"https://clients5.google.com/translate_a/t?client=at&sl=auto&tl={dest}&q={text}"
-        )
-        try:
-            result = response.json()
-        except Exception as e:
-            raise BaseException(str(e))
-
-        return GoogleTranslateResult.parse(result[0], dest)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *args):
-        return self
-
-
-class AsyncGoogleTranslator:
-    def __init__(self) -> None:
-        pass
-
-    async def translate(self, text: str, dest: str = "en") -> "GoogleTranslateResult":
-        async with ClientSession() as session:
-            async with session.get(
-                f"https://clients5.google.com/translate_a/t?client=at&sl=auto&tl={dest}&q={text}"
-            ) as response:
-                try:
-                    result = await response.json()
-                except Exception as e:
-                    raise BaseException(str(e))
-
-                return GoogleTranslateResult.parse(result[0], dest)
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, *args):
-        return self
+from aiohttp import ClientSession
+
+from .types import GoogleTranslateResult
+
+import requests
+
+
+class GoogleTranslator:
+    def __init__(self) -> None:
+        pass
+
+    def translate(self, text: str, dest: str = "en") -> "GoogleTranslateResult":
+        response = requests.get(
+            f"https://clients5.google.com/translate_a/t?client=at&sl=auto&tl={dest}&q={text}"
+        )
+        try:
+            result = response.json()
+        except Exception as e:
+            raise BaseException(str(e))
+
+        return GoogleTranslateResult.parse(result[0], dest)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args):
+        return self
+
+
+class AsyncGoogleTranslator:
+    def __init__(self) -> None:
+        pass
+
+    async def translate(self, text: str, dest: str = "en") -> "GoogleTranslateResult":
+        async with ClientSession() as session:
+            async with session.get(
+                f"https://clients5.google.com/translate_a/t?client=at&sl=auto&tl={dest}&q={text}"
+            ) as response:
+                try:
+                    result = await response.json()
+                except Exception as e:
+                    raise BaseException(str(e))
+
+                return GoogleTranslateResult.parse(result[0], dest)
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        return self
```

### Comparing `trengine-1.2/trengine/hozory.py` & `trengine-1.3/trengine/hozory.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from aiohttp import ClientSession
-
-from .types import HozoryTranslateResult
-from .exceptions import ApiException
-
-from json import dumps
-
-import requests
-
-
-class HozoryTranslator:
-    def __init__(self) -> None:
-        pass
-
-    def translate(self, text: str, dest: str = "en") -> "HozoryTranslateResult":
-        response = requests.get(
-            f"https://hozory.com/translate/?target={dest}&text={text}"
-        )
-        try:
-            result = response.json()
-        except Exception as e:
-            raise BaseException(str(e))
-
-        if not result["status"] == "ok":
-            raise ApiException(dumps(result["result"], indent=2, ensure_ascii=False))
-
-        return HozoryTranslateResult.parse(result["result"], dest)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *args):
-        return self
-
-
-class AsyncHozoryTranslator:
-    def __init__(self) -> None:
-        pass
-
-    async def translate(self, text: str, dest: str = "en") -> "HozoryTranslateResult":
-        async with ClientSession() as session:
-            async with session.get(
-                f"https://hozory.com/translate/?target={dest}&text={text}"
-            ) as response:
-                try:
-                    result = await response.json()
-                except Exception as e:
-                    raise BaseException(str(e))
-
-                if not result["status"] == "ok":
-                    raise ApiException(
-                        dumps(result["result"], indent=2, ensure_ascii=False)
-                    )
-
-                return HozoryTranslateResult.parse(result["result"], dest)
-
-    async def __aenter__(self):
-        return self
-
-    async def __aexit__(self, *args):
-        return self
+from aiohttp import ClientSession
+
+from .types import HozoryTranslateResult
+from .exceptions import ApiException
+
+from json import dumps
+
+import requests
+
+
+class HozoryTranslator:
+    def __init__(self) -> None:
+        pass
+
+    def translate(self, text: str, dest: str = "en") -> "HozoryTranslateResult":
+        response = requests.get(
+            f"https://hozory.com/translate/?target={dest}&text={text}"
+        )
+        try:
+            result = response.json()
+        except Exception as e:
+            raise BaseException(str(e))
+
+        if not result["status"] == "ok":
+            raise ApiException(dumps(result["result"], indent=2, ensure_ascii=False))
+
+        return HozoryTranslateResult.parse(result["result"], dest)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *args):
+        return self
+
+
+class AsyncHozoryTranslator:
+    def __init__(self) -> None:
+        pass
+
+    async def translate(self, text: str, dest: str = "en") -> "HozoryTranslateResult":
+        async with ClientSession() as session:
+            async with session.get(
+                f"https://hozory.com/translate/?target={dest}&text={text}"
+            ) as response:
+                try:
+                    result = await response.json()
+                except Exception as e:
+                    raise BaseException(str(e))
+
+                if not result["status"] == "ok":
+                    raise ApiException(
+                        dumps(result["result"], indent=2, ensure_ascii=False)
+                    )
+
+                return HozoryTranslateResult.parse(result["result"], dest)
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, *args):
+        return self
```

### Comparing `trengine-1.2/trengine/ocr.py` & `trengine-1.3/trengine/ocr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,89 @@
-import requests
-import aiohttp
-import json
-import os
-
-from aiofiles import open as AsyncOpen
-
-from .exceptions import ApiException
-
-
-class OCR:
-    def __init__(self) -> None:
-        pass
-
-    def from_image(self, path: str, language: str = "eng") -> str:
-        with open(path, "rb") as f:
-            response = requests.post(
-                "https://api8.ocr.space/parse/image",
-                data={
-                    "language": language,
-                    "isOverlayRequired": True,
-                    "OCREngine": 1,
-                    "detectCheckbox": False,
-                    "IsCreateSearchablePDF": False,
-                    "isSearchablePdfHideTextLayer": True,
-                    "FileType": ".AUTO",
-                },
-                headers={
-                    "Apikey": "donotstealthiskey_ip1",
-                },
-                files={"file": f},
-            )
-            try:
-                result = response.json()
-            except Exception as e:
-                raise BaseException(str(e))
-
-            if isinstance(result, str):
-                raise ApiException(result)
-            if not result.get("ParsedResults"):
-                raise ApiException(json.dumps(result, indent=4, ensure_ascii=False))
-
-            return result["ParsedResults"][0]["ParsedText"]
-
-
-class AsyncOCR:
-    def __init__(self) -> None:
-        pass
-
-    async def from_image(self, path: str, language: str = "eng") -> str:
-        async with AsyncOpen(path, "rb") as f:
-            async with aiohttp.ClientSession(
-                headers={"Apikey": "donotstealthiskey_ip1"}
-            ) as session:
-                payload = {
-                    "language": language,
-                    "isOverlayRequired": True,
-                    "OCREngine": 1,
-                    "detectCheckbox": False,
-                    "IsCreateSearchablePDF": False,
-                    "isSearchablePdfHideTextLayer": True,
-                    "FileType": ".AUTO",
-                }
-                data = aiohttp.formdata.FormData(quote_fields=False)
-                for k, v in payload.items():
-                    data.add_field(k, str(v))
-                data.add_field("file", await f.read(), filename=os.path.basename(path))
-                async with session.post(
-                    "https://api8.ocr.space/parse/image", data=data
-                ) as response:
-                    try:
-                        result = await response.json()
-                    except Exception as e:
-                        raise BaseException(str(e))
-
-                    if isinstance(result, str):
-                        raise ApiException(result)
-                    if not result.get("ParsedResults"):
-                        raise ApiException(
-                            json.dumps(result, indent=4, ensure_ascii=False)
-                        )
-
-                    return result["ParsedResults"][0]["ParsedText"]
+import requests
+import aiohttp
+import json
+import os
+
+
+from .exceptions import ApiException
+from typing import Union
+
+
+class OCR:
+    def __init__(self) -> None:
+        pass
+
+    def from_image(self, path: Union[str, bytes], language: str = "eng") -> str:
+        if isinstance(path, bytes):
+            b = path
+        else:
+            with open(path, "rb") as f:
+                b = f.read()
+        response = requests.post(
+            "https://api8.ocr.space/parse/image",
+            data={
+                "language": language,
+                "isOverlayRequired": True,
+                "OCREngine": 1,
+                "detectCheckbox": False,
+                "IsCreateSearchablePDF": False,
+                "isSearchablePdfHideTextLayer": True,
+                "FileType": ".AUTO",
+            },
+            headers={
+                "Apikey": "donotstealthiskey_ip1",
+            },
+            files={"file": b},
+        )
+        try:
+            result = response.json()
+        except Exception as e:
+            raise BaseException(str(e))
+
+        if isinstance(result, str):
+            raise ApiException(result)
+        if not result.get("ParsedResults"):
+            raise ApiException(json.dumps(result, indent=4, ensure_ascii=False))
+
+        return result["ParsedResults"][0]["ParsedText"]
+
+
+class AsyncOCR:
+    def __init__(self) -> None:
+        pass
+
+    async def from_image(self, path: Union[str, bytes], language: str = "eng") -> str:
+        if isinstance(path, bytes):
+            b = path
+        else:
+            with open(path, "rb") as f:
+                b = f.read()
+        async with aiohttp.ClientSession(
+            headers={"Apikey": "donotstealthiskey_ip1"}
+        ) as session:
+            payload = {
+                "language": language,
+                "isOverlayRequired": True,
+                "OCREngine": 1,
+                "detectCheckbox": False,
+                "IsCreateSearchablePDF": False,
+                "isSearchablePdfHideTextLayer": True,
+                "FileType": ".AUTO",
+            }
+            data = aiohttp.formdata.FormData(quote_fields=False)
+            for k, v in payload.items():
+                data.add_field(k, str(v))
+            data.add_field("file", b, filename=os.path.basename(path))
+            async with session.post(
+                "https://api8.ocr.space/parse/image", data=data
+            ) as response:
+                try:
+                    result = await response.json()
+                except Exception as e:
+                    raise BaseException(str(e))
+
+                if isinstance(result, str):
+                    raise ApiException(result)
+                if not result.get("ParsedResults"):
+                    raise ApiException(json.dumps(result, indent=4, ensure_ascii=False))
+
+                return result["ParsedResults"][0]["ParsedText"]
```

### Comparing `trengine-1.2/trengine.egg-info/PKG-INFO` & `trengine-1.3/trengine.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-Metadata-Version: 2.1
-Name: trengine
-Version: 1.2
-Summary: TREngine is python library based on 4 translators engines
-Author-email: ZAID <y8838@hotmail.com>
-Project-URL: Homepage, https://github.com/zaid5o5/trengine
-Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: asyncio
-Requires-Dist: requests
-Requires-Dist: aiofiles
-
-# Install:
-```commandline
-pip install trengine
-```
-
-# About this project:
-- TREngine is python library based on 4 translators engines with OCR:
-- Ajax ( [translate.com](https://www.translate.com/translator) )
-- Google ( [translate.google.com](https://translate.google.com/) )
-- Hozory ( [hozory.com](https://hozory.com/FA) )
-- Translatedict ( [translatedict.com](https://www.translatedict.com/) )
-- OCR ( [ocr.space](https://ocr.space/) )
-
-- Supporting Sync & Async.
-
-# How to use?
-- Here an example to use it:
-```python
-from trengine import Engine
-
-eng = Engine()
-text = "Hola, mi amor"
-
-print(
-    eng.google.translate(text, "en"), "\n",
-    eng.ajax.translate(text, "en"), "\n",
-    eng.hozory.translate(text, "en"), "\n",
-    eng.tdict.translate(text, "en"), "\n",
-)
-
-# OCR
-print(eng.ocr.from_image("./test.png"))
-```
-- Here an async example:
-```python
-import asyncio
-from trengine import AsyncEngine
-
-eng = AsyncEngine()
-text = "Hola, mi amor"
-
-async def main():
-    print(
-        await eng.google.translate(text, "en"), "\n",
-        await eng.ajax.translate(text, "en"), "\n",
-        await eng.hozory.translate(text, "en"), "\n",
-        await eng.tdict.translate(text, "en"), "\n",
-    )
-
-    # OCR
-    print(await eng.ocr.from_image("./test.png"))
-
-asyncio.run(main())
-```
+Metadata-Version: 2.1
+Name: trengine
+Version: 1.3
+Summary: TREngine is python library based on 4 translators engines
+Author-email: ZAID <y8838@hotmail.com>
+Project-URL: Homepage, https://github.com/zaid5o5/trengine
+Project-URL: Issues, https://github.com/zaid5o5/trengine/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: asyncio
+Requires-Dist: requests
+
+# Install:
+```commandline
+pip install trengine
+```
+
+# About this project:
+- TREngine is python library based on 4 translators engines with OCR:
+- Ajax ( [translate.com](https://www.translate.com/translator) )
+- Google ( [translate.google.com](https://translate.google.com/) )
+- Hozory ( [hozory.com](https://hozory.com/FA) )
+- Translatedict ( [translatedict.com](https://www.translatedict.com/) )
+- OCR ( [ocr.space](https://ocr.space/) )
+
+- Supporting Sync & Async.
+
+# How to use?
+- Here an example to use it:
+```python
+from trengine import Engine
+
+eng = Engine()
+text = "Hola, mi amor"
+
+print(
+    eng.google.translate(text, "en"), "\n",
+    eng.ajax.translate(text, "en"), "\n",
+    eng.hozory.translate(text, "en"), "\n",
+    eng.tdict.translate(text, "en"), "\n",
+)
+
+# OCR
+print(eng.ocr.from_image("./test.png"))
+```
+- Here an async example:
+```python
+import asyncio
+from trengine import AsyncEngine
+
+eng = AsyncEngine()
+text = "Hola, mi amor"
+
+async def main():
+    print(
+        await eng.google.translate(text, "en"), "\n",
+        await eng.ajax.translate(text, "en"), "\n",
+        await eng.hozory.translate(text, "en"), "\n",
+        await eng.tdict.translate(text, "en"), "\n",
+    )
+
+    # OCR
+    print(await eng.ocr.from_image("./test.png"))
+
+asyncio.run(main())
+```
```

