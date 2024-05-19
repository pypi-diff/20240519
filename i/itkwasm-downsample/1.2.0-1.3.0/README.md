# Comparing `tmp/itkwasm_downsample-1.2.0.tar.gz` & `tmp/itkwasm_downsample-1.3.0.tar.gz`

## Comparing `itkwasm_downsample-1.2.0.tar` & `itkwasm_downsample-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/conf.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/_version.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_async.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_bin_shrink.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_bin_shrink_async.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_label_image.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_label_image_async.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_sigma.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_sigma_async.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/gaussian_kernel_radius.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/itkwasm_downsample/gaussian_kernel_radius_async.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/README.md
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 itkwasm_downsample-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/Makefile
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/conf.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/_static/favicon.png
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/_version.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_async.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_bin_shrink.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_bin_shrink_async.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_label_image.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_label_image_async.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_sigma.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_sigma_async.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/gaussian_kernel_radius.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/itkwasm_downsample/gaussian_kernel_radius_async.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/README.md
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 itkwasm_downsample-1.3.0/PKG-INFO
```

### Comparing `itkwasm_downsample-1.2.0/docs/Makefile` & `itkwasm_downsample-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/docs/conf.py` & `itkwasm_downsample-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/docs/index.md` & `itkwasm_downsample-1.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/docs/make.bat` & `itkwasm_downsample-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/docs/_static/favicon.png` & `itkwasm_downsample-1.3.0/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/__init__.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/__init__.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_async.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_bin_shrink.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_bin_shrink.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_bin_shrink_async.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_bin_shrink_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_label_image.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_label_image.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_label_image_async.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_label_image_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_sigma.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_sigma.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/downsample_sigma_async.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/downsample_sigma_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/gaussian_kernel_radius.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/gaussian_kernel_radius.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/itkwasm_downsample/gaussian_kernel_radius_async.py` & `itkwasm_downsample-1.3.0/itkwasm_downsample/gaussian_kernel_radius_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/pyproject.toml` & `itkwasm_downsample-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_downsample-1.2.0/PKG-INFO` & `itkwasm_downsample-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-downsample
-Version: 1.2.0
+Version: 1.3.0
 Summary: Pipelines for downsampling images.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

