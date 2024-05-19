# Comparing `tmp/itkwasm_compare_images-5.0.2.tar.gz` & `tmp/itkwasm_compare_images-5.1.1.tar.gz`

## Comparing `itkwasm_compare_images-5.0.2.tar` & `itkwasm_compare_images-5.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/Makefile
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/conf.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/index.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/make.bat
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/requirements.txt
--rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/_static/favicon.png
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/docs/_static/logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/_version.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images_async.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images_async.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude_async.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/.gitignore
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/README.md
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/pyproject.toml
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/Makefile
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/conf.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/make.bat
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0    13605 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/_static/favicon.png
+-rw-r--r--   0        0        0     4587 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/docs/_static/logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/_version.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_double_images.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_double_images_async.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_images.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_images_async.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/vector_magnitude.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/itkwasm_compare_images/vector_magnitude_async.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/.gitignore
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/README.md
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 itkwasm_compare_images-5.1.1/PKG-INFO
```

### Comparing `itkwasm_compare_images-5.0.2/docs/Makefile` & `itkwasm_compare_images-5.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/docs/conf.py` & `itkwasm_compare_images-5.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/docs/index.md` & `itkwasm_compare_images-5.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/docs/make.bat` & `itkwasm_compare_images-5.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/docs/_static/favicon.png` & `itkwasm_compare_images-5.1.1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images.py` & `itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_double_images.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_double_images_async.py` & `itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_double_images_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images.py` & `itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_images.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/itkwasm_compare_images/compare_images_async.py` & `itkwasm_compare_images-5.1.1/itkwasm_compare_images/compare_images_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude.py` & `itkwasm_compare_images-5.1.1/itkwasm_compare_images/vector_magnitude.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/itkwasm_compare_images/vector_magnitude_async.py` & `itkwasm_compare_images-5.1.1/itkwasm_compare_images/vector_magnitude_async.py`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/pyproject.toml` & `itkwasm_compare_images-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_compare_images-5.0.2/PKG-INFO` & `itkwasm_compare_images-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: itkwasm-compare-images
-Version: 5.0.2
+Version: 5.1.1
 Summary: Compare images with a tolerance for regression testing.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/itk-wasm
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/itk-wasm
 License-Expression: Apache-2.0
 Keywords: emscripten,itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

