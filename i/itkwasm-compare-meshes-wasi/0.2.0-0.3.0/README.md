# Comparing `tmp/itkwasm_compare_meshes_wasi-0.2.0.tar.gz` & `tmp/itkwasm_compare_meshes_wasi-0.3.0.tar.gz`

## Comparing `itkwasm_compare_meshes_wasi-0.2.0.tar` & `itkwasm_compare_meshes_wasi-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/_version.py
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/compare_meshes.py
--rwxr-xr-x   0        0        0  1183927 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/wasm_modules/compare-meshes.wasi.wasm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/tests/common.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/tests/test_compare_meshes.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/.gitignore
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/README.md
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/itkwasm_compare_meshes_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/itkwasm_compare_meshes_wasi/_version.py
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/itkwasm_compare_meshes_wasi/compare_meshes.py
+-rwxr-xr-x   0        0        0  3475077 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/itkwasm_compare_meshes_wasi/wasm_modules/compare-meshes.wasi.wasm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/tests/common.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/tests/test_compare_meshes.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/.gitignore
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/README.md
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 itkwasm_compare_meshes_wasi-0.3.0/PKG-INFO
```

### Comparing `itkwasm_compare_meshes_wasi-0.2.0/itkwasm_compare_meshes_wasi/compare_meshes.py` & `itkwasm_compare_meshes_wasi-0.3.0/itkwasm_compare_meshes_wasi/compare_meshes.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_meshes_wasi-0.2.0/README.md` & `itkwasm_compare_meshes_wasi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_meshes_wasi-0.2.0/pyproject.toml` & `itkwasm_compare_meshes_wasi-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
   "itkwasm",
   "webassembly",
   "wasi",
 ]
 
 requires-python = ">=3.8"
 dependencies = [
-    "itkwasm >= 1.0.b145",
+    "itkwasm >= 1.0.b171",
     "importlib_resources",
 
 ]
 
 [tool.hatch.version]
 path = "itkwasm_compare_meshes_wasi/_version.py"
```

### Comparing `itkwasm_compare_meshes_wasi-0.2.0/PKG-INFO` & `itkwasm_compare_meshes_wasi-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-compare-meshes-wasi
-Version: 0.2.0
+Version: 0.3.0
 Summary: Compare meshes and polydata for regression testing.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources
-Requires-Dist: itkwasm>=1.0.b145
+Requires-Dist: itkwasm>=1.0.b171
 Description-Content-Type: text/markdown
 
 # itkwasm-compare-meshes-wasi
 
 [![PyPI version](https://badge.fury.io/py/itkwasm-compare-meshes-wasi.svg)](https://badge.fury.io/py/itkwasm-compare-meshes-wasi)
 
 Compare meshes and polydata for regression testing. WASI implementation.
```

