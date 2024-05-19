# Comparing `tmp/itkwasm_downsample_wasi-1.2.0.tar.gz` & `tmp/itkwasm_downsample_wasi-1.3.0.tar.gz`

## Comparing `itkwasm_downsample_wasi-1.2.0.tar` & `itkwasm_downsample_wasi-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/_version.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample_bin_shrink.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample_label_image.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample_sigma.py
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/gaussian_kernel_radius.py
--rwxr-xr-x   0        0        0  3119465 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/wasm_modules/downsample-bin-shrink.wasi.wasm
--rwxr-xr-x   0        0        0  3682210 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/wasm_modules/downsample-label-image.wasi.wasm
--rwxr-xr-x   0        0        0   624847 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/wasm_modules/downsample-sigma.wasi.wasm
--rwxr-xr-x   0        0        0  4249689 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/wasm_modules/downsample.wasi.wasm
--rwxr-xr-x   0        0        0   641437 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/wasm_modules/gaussian-kernel-radius.wasi.wasm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/__init__.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/common.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/test_downsample.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/test_downsample_bin_shrink.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/test_downsample_label_image.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/test_downsample_sigma.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/test/test_gaussian_kernel_radius.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/common.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/test_downsample.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/test_downsample_bin_shrink.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/test_downsample_label_image.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/test_downsample_sigma.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/tests/test_gaussian_kernel_radius.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/.gitignore
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/README.md
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/_version.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample_bin_shrink.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample_label_image.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample_sigma.py
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/gaussian_kernel_radius.py
+-rwxr-xr-x   0        0        0  5413307 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/wasm_modules/downsample-bin-shrink.wasi.wasm
+-rwxr-xr-x   0        0        0  5988505 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/wasm_modules/downsample-label-image.wasi.wasm
+-rwxr-xr-x   0        0        0  2937786 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/wasm_modules/downsample-sigma.wasi.wasm
+-rwxr-xr-x   0        0        0  6556932 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/wasm_modules/downsample.wasi.wasm
+-rwxr-xr-x   0        0        0  2953872 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/wasm_modules/gaussian-kernel-radius.wasi.wasm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/__init__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/common.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/test_downsample.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/test_downsample_bin_shrink.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/test_downsample_label_image.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/test_downsample_sigma.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/test/test_gaussian_kernel_radius.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/common.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/test_downsample.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/test_downsample_bin_shrink.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/test_downsample_label_image.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/test_downsample_sigma.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/tests/test_gaussian_kernel_radius.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/.gitignore
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/README.md
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 itkwasm_downsample_wasi-1.3.0/PKG-INFO
```

### Comparing `itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample.py` & `itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample_bin_shrink.py` & `itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample_bin_shrink.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample_label_image.py` & `itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample_label_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/downsample_sigma.py` & `itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/downsample_sigma.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/itkwasm_downsample_wasi/gaussian_kernel_radius.py` & `itkwasm_downsample_wasi-1.3.0/itkwasm_downsample_wasi/gaussian_kernel_radius.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/test/test_downsample.py` & `itkwasm_downsample_wasi-1.3.0/test/test_downsample.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/test/test_downsample_bin_shrink.py` & `itkwasm_downsample_wasi-1.3.0/test/test_downsample_bin_shrink.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/test/test_downsample_label_image.py` & `itkwasm_downsample_wasi-1.3.0/test/test_downsample_label_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/README.md` & `itkwasm_downsample_wasi-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/pyproject.toml` & `itkwasm_downsample_wasi-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample_wasi-1.2.0/PKG-INFO` & `itkwasm_downsample_wasi-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-downsample-wasi
-Version: 1.2.0
+Version: 1.3.0
 Summary: Pipelines for downsampling images.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

