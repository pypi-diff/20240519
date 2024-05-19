# Comparing `tmp/itkwasm_compress_stringify-3.0.0.tar.gz` & `tmp/itkwasm_compress_stringify-3.2.0.tar.gz`

## Comparing `itkwasm_compress_stringify-3.0.0.tar` & `itkwasm_compress_stringify-3.2.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/Makefile
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/conf.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/_version.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/compress_stringify.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/compress_stringify_async.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/parse_string_decompress.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/parse_string_decompress_async.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/test/test_compress_stringify_emscripten.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/test/test_compress_stringify_wasi.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/.gitignore
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/README.md
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/Makefile
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/conf.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/_version.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/compress_stringify.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/compress_stringify_async.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/interface_type_json.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/parse_string_decompress.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/parse_string_decompress_async.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/test/test_compress_stringify_emscripten.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/test/test_compress_stringify_wasi.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/test/test_interface_type_json.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/.gitignore
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/README.md
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 itkwasm_compress_stringify-3.2.0/PKG-INFO
```

### Comparing `itkwasm_compress_stringify-3.0.0/docs/Makefile` & `itkwasm_compress_stringify-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/docs/conf.py` & `itkwasm_compress_stringify-3.2.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 from datetime import date
+import os
 
 project = 'itkwasm-compress-stringify'
 copyright = f'{date.today().year}, NumFOCUS'
 author = 'Insight Software Consortium'
 
 extensions = [
     'sphinx.ext.autosummary',
@@ -41,15 +42,16 @@
 }
 
 html_theme = 'furo'
 html_static_path = ['_static']
 html_logo = "_static/logo.svg"
 html_favicon = "_static/favicon.png"
 html_title = f"{project}"
+html_baseurl = os.environ.get("SPHINX_BASE_URL", "")
 
 # Furo options
 html_theme_options = {
     "top_of_page_button": "edit",
     "source_repository": "https://github.com/InsightSoftwareConsortium/itk-wasm",
     "source_branch": "main",
-    "source_directory": "docs",
+    "source_directory": "packages/compress-stringify/python/itkwasm-compress-stringify/docs",
 }
```

### Comparing `itkwasm_compress_stringify-3.0.0/docs/index.md` & `itkwasm_compress_stringify-3.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/docs/make.bat` & `itkwasm_compress_stringify-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/docs/_static/favicon.png` & `itkwasm_compress_stringify-3.2.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/compress_stringify.py` & `itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/compress_stringify_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from typing import Dict, Tuple, Optional, List, Any
 
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
-def compress_stringify(
+async def compress_stringify_async(
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
-    data_url_prefix: str = "data:base64,",
+    data_url_prefix: str = "data:application/zstd;base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
     :param input: Input binary
     :type  input: bytes
 
     :param stringify: Stringify the output
@@ -27,10 +27,10 @@
 
     :param data_url_prefix: dataURL prefix
     :type  data_url_prefix: str
 
     :return: Output compressed binary
     :rtype:  bytes
     """
-    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify")
-    output = func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
+    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify_async")
+    output = await func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
     return output
```

### Comparing `itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/compress_stringify_async.py` & `itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/compress_stringify.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from typing import Dict, Tuple, Optional, List, Any
 
 from itkwasm import (
     environment_dispatch,
     BinaryStream,
 )
 
-async def compress_stringify_async(
+def compress_stringify(
     input: bytes,
     stringify: bool = False,
     compression_level: int = 3,
-    data_url_prefix: str = "data:base64,",
+    data_url_prefix: str = "data:application/zstd;base64,",
 ) -> bytes:
     """Given a binary, compress and optionally base64 encode.
 
     :param input: Input binary
     :type  input: bytes
 
     :param stringify: Stringify the output
@@ -27,10 +27,10 @@
 
     :param data_url_prefix: dataURL prefix
     :type  data_url_prefix: str
 
     :return: Output compressed binary
     :rtype:  bytes
     """
-    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify_async")
-    output = await func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
+    func = environment_dispatch("itkwasm_compress_stringify", "compress_stringify")
+    output = func(input, stringify=stringify, compression_level=compression_level, data_url_prefix=data_url_prefix)
     return output
```

### Comparing `itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/parse_string_decompress.py` & `itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/parse_string_decompress.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/itkwasm_compress_stringify/parse_string_decompress_async.py` & `itkwasm_compress_stringify-3.2.0/itkwasm_compress_stringify/parse_string_decompress_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/test/test_compress_stringify_emscripten.py` & `itkwasm_compress_stringify-3.2.0/test/test_compress_stringify_emscripten.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify-3.0.0/test/test_compress_stringify_wasi.py` & `itkwasm_compress_stringify-3.2.0/test/test_compress_stringify_wasi.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     assert decompressed_data[1] == 173
     assert decompressed_data[2] == 190
     assert decompressed_data[3] == 239
 
 def test_we_can_stringify_during_compression():
     data = bytes([222, 173, 190, 239])
     compressed_data = compress_stringify(data, compression_level=8, stringify=True)
-    assert compressed_data.decode() == 'data:base64,KLUv/SAEIQAA3q2+7w=='
+    assert compressed_data.decode() == 'data:application/zstd,KLUv/SAEIQAA3q2+7w=='
     decompressed_data = parse_string_decompress(compressed_data, parse_string=True)
 
     assert decompressed_data[0] == 222
     assert decompressed_data[1] == 173
     assert decompressed_data[2] == 190
     assert decompressed_data[3] == 239
```

### Comparing `itkwasm_compress_stringify-3.0.0/pyproject.toml` & `itkwasm_compress_stringify-3.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "webassembly",
   "wasi",
   "emscripten",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
-    "itkwasm >= 1.0.b145",
+    "itkwasm >= 1.0.b171",
     "itkwasm-compress-stringify-wasi; sys_platform != \"emscripten\"",
     "itkwasm-compress-stringify-emscripten; sys_platform == \"emscripten\"",
 ]
 
 [project.urls]
 Home = "https://itk-wasm-compress-stringify-python-docs.on.fleek.co"
 Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
@@ -47,24 +47,30 @@
 [tool.hatch.version]
 path = "itkwasm_compress_stringify/_version.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-pyodide",
+  "itkwasm-compare-images",
+  "itkwasm-image-io",
+  "itkwasm-compare-meshes",
+  "itkwasm-mesh-io",
+  "itkwasm-mesh-to-poly-data",
 ]
 
 
 [tool.hatch.envs.default.scripts]
 test = [
   "hatch build -t wheel ./dist/pyodide/",
   "pytest --dist-dir=./dist/pyodide --rt=chrome",
 ]
 download-pyodide = [
-  "curl -L https://github.com/pyodide/pyodide/releases/download/0.24.1/pyodide-0.24.1.tar.bz2 -o pyodide.tar.bz2",
+  "curl -L https://github.com/pyodide/pyodide/releases/download/0.25.0/pyodide-0.25.0.tar.bz2 -o pyodide.tar.bz2",
+  "tar xjf pyodide.tar.bz2",
   "rm -rf dist/pyodide pyodide.tar.bz2",
   "mkdir -p dist",
   "mv pyodide dist",
 ]
 serve = [
   "hatch build -t wheel ./dist/pyodide/",
   'echo "\nVisit http://localhost:8877/console.html\n"',
```

### Comparing `itkwasm_compress_stringify-3.0.0/PKG-INFO` & `itkwasm_compress_stringify-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itkwasm-compress-stringify
-Version: 3.0.0
+Version: 3.2.0
 Summary: Zstandard compression and decompression and base64 encoding and decoding in WebAssembly.
 Project-URL: Home, https://itk-wasm-compress-stringify-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: itkwasm-compress-stringify-emscripten; sys_platform == 'emscripten'
 Requires-Dist: itkwasm-compress-stringify-wasi; sys_platform != 'emscripten'
-Requires-Dist: itkwasm>=1.0.b145
+Requires-Dist: itkwasm>=1.0.b171
 Description-Content-Type: text/markdown
 
 # itkwasm-compress-stringify
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-compress-stringify.svg)](https://badge.fury.io/py/itkwasm-compress-stringify)
 
 Zstandard compression and decompression and base64 encoding and decoding in WebAssembly.
```

