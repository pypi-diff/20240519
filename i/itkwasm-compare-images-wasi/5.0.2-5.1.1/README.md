# Comparing `tmp/itkwasm_compare_images_wasi-5.0.2.tar.gz` & `tmp/itkwasm_compare_images_wasi-5.1.1.tar.gz`

## Comparing `itkwasm_compare_images_wasi-5.0.2.tar` & `itkwasm_compare_images_wasi-5.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/_version.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/compare_double_images.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/compare_images.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/vector_magnitude.py
--rwxr-xr-x   0        0        0  1592397 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/wasm_modules/compare-double-images.wasi.wasm
--rwxr-xr-x   0        0        0  1442526 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/wasm_modules/vector-magnitude.wasi.wasm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/tests/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/tests/common.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/tests/test_compare_double_images.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/tests/test_vector_magnitude.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/.gitignore
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/README.md
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/_version.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/compare_double_images.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/compare_images.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/vector_magnitude.py
+-rwxr-xr-x   0        0        0  3896498 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/wasm_modules/compare-double-images.wasi.wasm
+-rwxr-xr-x   0        0        0  3744217 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/wasm_modules/vector-magnitude.wasi.wasm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/tests/common.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/tests/test_compare_double_images.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/tests/test_vector_magnitude.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/.gitignore
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/README.md
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 itkwasm_compare_images_wasi-5.1.1/PKG-INFO
```

### Comparing `itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/compare_double_images.py` & `itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/compare_double_images.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/compare_images.py` & `itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/compare_images.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images_wasi-5.0.2/itkwasm_compare_images_wasi/vector_magnitude.py` & `itkwasm_compare_images_wasi-5.1.1/itkwasm_compare_images_wasi/vector_magnitude.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images_wasi-5.0.2/README.md` & `itkwasm_compare_images_wasi-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images_wasi-5.0.2/pyproject.toml` & `itkwasm_compare_images_wasi-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images_wasi-5.0.2/PKG-INFO` & `itkwasm_compare_images_wasi-5.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-compare-images-wasi
-Version: 5.0.2
+Version: 5.1.1
 Dynamic: Summary
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

