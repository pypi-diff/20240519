# Comparing `tmp/itkwasm_mesh_to_poly_data_wasi-1.0.0.tar.gz` & `tmp/itkwasm_mesh_to_poly_data_wasi-1.1.0.tar.gz`

## Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0.tar` & `itkwasm_mesh_to_poly_data_wasi-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/_version.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/mesh_to_poly_data.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/poly_data_to_mesh.py
--rwxr-xr-x   0        0        0  2209388 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/wasm_modules/mesh-to-poly-data.wasi.wasm
--rwxr-xr-x   0        0        0  1319166 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/wasm_modules/poly-data-to-mesh.wasi.wasm
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/tests/test_mesh_to_poly_data.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/.gitignore
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/README.md
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/_version.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/mesh_to_poly_data.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/poly_data_to_mesh.py
+-rwxr-xr-x   0        0        0  4529812 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/wasm_modules/mesh-to-poly-data.wasi.wasm
+-rwxr-xr-x   0        0        0  3632190 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/wasm_modules/poly-data-to-mesh.wasi.wasm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/tests/common.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/tests/test_mesh_to_poly_data.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/tests/test_poly_data_to_mesh.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/.gitignore
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/README.md
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 itkwasm_mesh_to_poly_data_wasi-1.1.0/PKG-INFO
```

### Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/mesh_to_poly_data.py` & `itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/mesh_to_poly_data.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0/itkwasm_mesh_to_poly_data_wasi/poly_data_to_mesh.py` & `itkwasm_mesh_to_poly_data_wasi-1.1.0/itkwasm_mesh_to_poly_data_wasi/poly_data_to_mesh.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0/tests/test_mesh_to_poly_data.py` & `itkwasm_mesh_to_poly_data_wasi-1.1.0/tests/test_mesh_to_poly_data.py`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0/README.md` & `itkwasm_mesh_to_poly_data_wasi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0/pyproject.toml` & `itkwasm_mesh_to_poly_data_wasi-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkwasm_mesh_to_poly_data_wasi-1.0.0/PKG-INFO` & `itkwasm_mesh_to_poly_data_wasi-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: itkwasm-mesh-to-poly-data-wasi
-Version: 1.0.0
+Version: 1.1.0
 Summary: Convert an ITK Mesh to a simple data structure compatible with vtkPolyData.
 Project-URL: Home, https://github.com/InsightSoftwareConsortium/ITKMeshToPolyData
 Project-URL: Source, https://github.com/InsightSoftwareConsortium/ITKMeshToPolyData
 License-Expression: Apache-2.0
 Keywords: itkwasm,wasi,webassembly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: WebAssembly
```

