# Comparing `tmp/itkwasm_compress_stringify_wasi-3.0.0.tar.gz` & `tmp/itkwasm_compress_stringify_wasi-3.2.0.tar.gz`

## Comparing `itkwasm_compress_stringify_wasi-3.0.0.tar` & `itkwasm_compress_stringify_wasi-3.2.0.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/_version.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/compress_stringify.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/parse_string_decompress.py
--rwxr-xr-x   0        0        0  1026360 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasi.wasm
--rwxr-xr-x   0        0        0   754637 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasi.wasm
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/test/test_compress_stringify.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/.gitignore
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/_version.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/compress_stringify.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/parse_string_decompress.py
+-rwxr-xr-x   0        0        0  3316463 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/wasm_modules/compress-stringify.wasi.wasm
+-rwxr-xr-x   0        0        0  3066337 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/wasm_modules/parse-string-decompress.wasi.wasm
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/test/test_compress_stringify.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/tests/common.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/tests/test_compress_stringify.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/tests/test_parse_string_decompress.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/.gitignore
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/README.md
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_compress_stringify_wasi-3.2.0/PKG-INFO
```

### Comparing `itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/compress_stringify.py` & `itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/compress_stringify.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     BinaryStream,
 )
 
 def compress_stringify(
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
```

### Comparing `itkwasm_compress_stringify_wasi-3.0.0/itkwasm_compress_stringify_wasi/parse_string_decompress.py` & `itkwasm_compress_stringify_wasi-3.2.0/itkwasm_compress_stringify_wasi/parse_string_decompress.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-3.0.0/test/test_compress_stringify.py` & `itkwasm_compress_stringify_wasi-3.2.0/test/test_compress_stringify.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     assert decompressed_data[1] == 173
     assert decompressed_data[2] == 190
     assert decompressed_data[3] == 239
 
 def test_we_can_stringify_during_compression():
     data = bytes([222, 173, 190, 239])
     compressed_data = compress_stringify(data, compression_level=8, stringify=True)
-    assert compressed_data.decode() == 'data:base64,KLUv/SAEIQAA3q2+7w=='
+    assert compressed_data.decode() == 'data:application/zstd;base64,KLUv/SAEIQAA3q2+7w=='
     decompressed_data = parse_string_decompress(compressed_data, parse_string=True)
 
     assert decompressed_data[0] == 222
     assert decompressed_data[1] == 173
     assert decompressed_data[2] == 190
     assert decompressed_data[3] == 239
```

### Comparing `itkwasm_compress_stringify_wasi-3.0.0/README.md` & `itkwasm_compress_stringify_wasi-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compress_stringify_wasi-3.0.0/pyproject.toml` & `itkwasm_compress_stringify_wasi-3.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,24 +18,25 @@
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 keywords = [
   "itkwasm",
   "webassembly",
   "wasi",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
-    "itkwasm >= 1.0.b131",
+    "itkwasm >= 1.0.b171",
     "importlib_resources",
 
 ]
 
 [project.urls]
 Home = "https://itk-wasm-compress-stringify-python-docs.on.fleek.co"
 Source = "https://github.com/InsightSoftwareConsortium/itk-wasm"
```

### Comparing `itkwasm_compress_stringify_wasi-3.0.0/PKG-INFO` & `itkwasm_compress_stringify_wasi-3.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itkwasm-compress-stringify-wasi
-Version: 3.0.0
+Version: 3.2.0
+Dynamic: Summary
 Project-URL: Home, https://itk-wasm-compress-stringify-python-docs.on.fleek.co
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Issues, https://github.com/InsightSoftwareConsortium/itk-wasm/issues
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
@@ -16,17 +17,18 @@
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources
-Requires-Dist: itkwasm>=1.0.b131
+Requires-Dist: itkwasm>=1.0.b171
 Description-Content-Type: text/markdown
 
 # itkwasm-compress-stringify-wasi
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-compress-stringify-wasi.svg)](https://badge.fury.io/py/itkwasm-compress-stringify-wasi)
 
 Zstandard compression and decompression and base64 encoding and decoding in WebAssembly. WASI implementation.
```

