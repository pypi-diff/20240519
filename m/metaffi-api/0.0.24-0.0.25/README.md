# Comparing `tmp/metaffi_api-0.0.24.tar.gz` & `tmp/metaffi_api-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.24.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.24.tar` & `metaffi_api-0.0.25.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.24/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.24/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.24/README.md
--rw-r--r--   0        0        0      428 2024-04-21 14:03:39.717766 metaffi_api-0.0.24/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.24/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      122 2024-01-01 14:18:03.539263 metaffi_api-0.0.24/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4988 2024-04-21 12:58:09.252965 metaffi_api-0.0.24/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      513 2024-01-01 16:45:39.723929 metaffi_api-0.0.24/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4619 2024-04-21 13:24:41.131761 metaffi_api-0.0.24/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:19:16.794164 metaffi_api-0.0.24/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     4719 2024-04-21 14:03:17.970853 metaffi_api-0.0.24/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      584 2024-04-21 10:05:04.530248 metaffi_api-0.0.24/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.24/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.24/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.25/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.25/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.25/README.md
+-rw-r--r--   0        0        0      538 2024-05-19 10:51:04.097565 metaffi_api-0.0.25/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.25/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      411 2024-05-19 08:34:56.915898 metaffi_api-0.0.25/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     4823 2024-05-19 07:36:05.188625 metaffi_api-0.0.25/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      484 2024-05-18 16:45:00.514372 metaffi_api-0.0.25/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4619 2024-05-19 03:25:53.676813 metaffi_api-0.0.25/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     2024 2024-05-18 16:43:11.504988 metaffi_api-0.0.25/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     5217 2024-05-19 06:50:11.445337 metaffi_api-0.0.25/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      584 2024-04-21 10:05:04.530248 metaffi_api-0.0.25/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.25/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.25/PKG-INFO
```

### Comparing `metaffi_api-0.0.24/LICENSE` & `metaffi_api-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.24/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.25/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.24/metaffi/metaffi_module.py` & `metaffi_api-0.0.25/metaffi/metaffi_module.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import ctypes.util
-import metaffi.xllr_wrapper
-from metaffi.metaffi_types import *
-import metaffi.metaffi_runtime
-
-XCallParamsRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint64))
-XCallNoParamsRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint64))
-XCallParamsNoRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint64))
-XCallNoParamsNoRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_uint64))
+from typing import Callable, Any, Tuple
+from . import metaffi_runtime, metaffi_types, xllr_wrapper
 
-create_lambda_python_code = ctypes.c_char_p.in_dll(metaffi.xllr_wrapper.xllr_python3, 'create_lambda_python_code').value.decode('utf-8')
-exec(create_lambda_python_code)
+XCallParamsRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p))
+XCallNoParamsRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p))
+XCallParamsNoRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p))
+XCallNoParamsNoRetType = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_void_p)
+
+create_lambda_python_code = ctypes.c_char_p.in_dll(xllr_wrapper.xllr_python3, 'create_lambda_python_code').value.decode('utf-8')
+exec(create_lambda_python_code)  # defines "create_lambda" function
 
 
 def make_metaffi_callable(f: Callable) -> Callable:
-	params_metaffi_types, retval_metaffi_types = metaffi.metaffi_types.get_callable_types(f)
+	params_metaffi_types, retval_metaffi_types = metaffi_types.get_callable_types(f)
 	
 	params_type = ctypes.c_uint64 * len(params_metaffi_types)
 	params_array = params_type(*params_metaffi_types)
 	
 	retvals_type = ctypes.c_uint64 * len(retval_metaffi_types)
 	retvals_array = retvals_type(*retval_metaffi_types)
 	
 	err = ctypes.c_char_p()
 	err_len = ctypes.c_uint32()
 	
 	xllr_python3_bytes = 'xllr.python311'.encode('utf-8')
 	
-	pxcall_and_context_array = metaffi.xllr_wrapper.xllr.make_callable(xllr_python3_bytes, len(xllr_python3_bytes), f, params_array, retvals_array, len(params_metaffi_types), len(retval_metaffi_types), ctypes.byref(err), ctypes.byref(err_len))
+	pxcall_and_context_array = xllr_wrapper.make_callable(xllr_python3_bytes, len(xllr_python3_bytes), f, params_array, retvals_array, len(params_metaffi_types), len(retval_metaffi_types), ctypes.byref(err), ctypes.byref(err_len))
 	
 	pxcall_and_context_array = ctypes.cast(pxcall_and_context_array, ctypes.POINTER(ctypes.c_void_p * 2))
 	
 	if len(params_metaffi_types) > 0 and len(retval_metaffi_types) > 0:
 		pxcall = XCallParamsRetType(pxcall_and_context_array.contents[0])
 	elif len(params_metaffi_types) > 0 and len(retval_metaffi_types) == 0:
 		pxcall = XCallParamsNoRetType(pxcall_and_context_array.contents[0])
@@ -44,56 +43,63 @@
 	res = create_lambda(pxcall, context, params_metaffi_types, retval_metaffi_types)
 	setattr(res, 'pxcall_and_context', ctypes.addressof(pxcall_and_context_array.contents))
 	setattr(res, 'params_metaffi_types', params_metaffi_types)
 	setattr(res, 'retval_metaffi_types', retval_metaffi_types)
 	return res
 
 
+class MetaFFIEntity:
+	def __init__(self, pxcall: ctypes.c_void_p, wrapping_lambda: Callable[..., Tuple[Any, ...]]):
+		self.calling_lambda = wrapping_lambda
+		self.pxcall = pxcall
+		
+	def __call__(self, *args):
+		result = self.calling_lambda(*args)
+		if result is not None and len(result) == 1:
+			return result[0]
+		else:
+			return result
+	
+	def __del__(self):
+		xllr_wrapper.free_xcall('xllr.python311', self.pxcall)
+		
+
 class MetaFFIModule:
-	def __init__(self, runtime: metaffi.metaffi_runtime.MetaFFIRuntime, xllr: metaffi.xllr_wrapper._XllrWrapper, module_path: str):
+	def __init__(self, runtime: metaffi_runtime.MetaFFIRuntime, module_path: str):
 		self.runtime = runtime
-		self.xllr = xllr
 		self.module_path = module_path
 	
-	def load(self, function_path: str, params_metaffi_types: Tuple[metaffi.metaffi_types.metaffi_type_info] | None,
-			retval_metaffi_types: Tuple[metaffi.metaffi_types.metaffi_type_info] | None) -> Callable[..., Tuple[Any, ...]]:
+	def load_entity(self, function_path: str, params_metaffi_types: Tuple[metaffi_types.metaffi_type_info] | None,
+			retval_metaffi_types: Tuple[metaffi_types.metaffi_type_info] | None) -> MetaFFIEntity:
 		
 		if params_metaffi_types is None:
 			params_metaffi_types = tuple()
 		
 		if retval_metaffi_types is None:
 			retval_metaffi_types = tuple()
 		
 		# Create ctypes arrays for params_metaffi_types and retval_metaffi_types
-		ParamsArray = metaffi.metaffi_types.metaffi_type_info * len(params_metaffi_types)
-		params_array = ParamsArray(*params_metaffi_types)
+		params_array_t = metaffi_types.metaffi_type_info * len(params_metaffi_types)
+		params_array = params_array_t(*params_metaffi_types)
+		
+		retval_array_t = metaffi_types.metaffi_type_info * len(retval_metaffi_types)
+		retval_array = retval_array_t(*retval_metaffi_types)
 		
-		RetvalArray = metaffi.metaffi_types.metaffi_type_info * len(retval_metaffi_types)
-		retval_array = RetvalArray(*retval_metaffi_types)
+		# if parameter is a list - convert it to tuple
+		if not isinstance(params_metaffi_types, tuple) and not isinstance(params_metaffi_types, list):
+			raise ValueError('params_metaffi_types must be a list or tuple')
+		
+		if not isinstance(retval_metaffi_types, tuple) and not isinstance(retval_metaffi_types, list):
+			raise ValueError('retval_metaffi_types must be a list or tuple')
 		
-		# capsule the metaffi_type_info objects to access them in call_xcall
 		if not isinstance(params_metaffi_types, tuple):
 			params_metaffi_types = tuple(params_metaffi_types)
 		
 		if not isinstance(retval_metaffi_types, tuple):
 			retval_metaffi_types = tuple(retval_metaffi_types)
 		
 		# Call xllr.load_function
-		pxcall_and_context = self.xllr.load_function('xllr.' + self.runtime.runtime_plugin, self.module_path, function_path, params_array, retval_array, len(params_metaffi_types), len(retval_metaffi_types))
-		
-		pxcall_and_context_array = ctypes.cast(pxcall_and_context, ctypes.POINTER(ctypes.c_void_p * 2))
-		
-		pxcall = None
-		if len(params_metaffi_types) > 0 and len(retval_metaffi_types) > 0:
-			pxcall = XCallParamsRetType(pxcall_and_context_array.contents[0])
-		elif len(params_metaffi_types) > 0 and len(retval_metaffi_types) == 0:
-			pxcall = XCallParamsNoRetType(pxcall_and_context_array.contents[0])
-		elif len(params_metaffi_types) == 0 and len(retval_metaffi_types) > 0:
-			pxcall = XCallNoParamsRetType(pxcall_and_context_array.contents[0])
-		else:
-			pxcall = XCallNoParamsNoRetType(pxcall_and_context_array.contents[0])
-		
-		context = pxcall_and_context_array.contents[1]
+		xcall = xllr_wrapper.load_entity('xllr.' + self.runtime.runtime_plugin, self.module_path, function_path, params_array, len(params_metaffi_types), retval_array, len(retval_metaffi_types))
 		
-		func_lambda: Callable[..., ...] = lambda *args: metaffi.xllr_wrapper.xllr_python3.call_xcall(pxcall, context, params_metaffi_types, retval_metaffi_types, None if not args else args)
+		func_lambda: Callable[..., ...] = lambda *args: xllr_wrapper.xllr_python3.call_xcall(xcall, params_metaffi_types, retval_metaffi_types, None if not args else args)
 		
-		return func_lambda
+		return MetaFFIEntity(xcall, func_lambda)
```

### Comparing `metaffi_api-0.0.24/metaffi/metaffi_types.py` & `metaffi_api-0.0.25/metaffi/metaffi_types.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.24/metaffi/pycdts_converter.py` & `metaffi_api-0.0.25/metaffi/pycdts_converter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 import ctypes
 from ctypes import py_object
-from typing import List
+from typing import List, Union, Tuple
 import os
 import platform
-import metaffi.xllr_wrapper
+from . import metaffi_types, xllr_wrapper
 
+if platform.system() == 'Windows':
+	os.add_dll_directory(os.environ['METAFFI_HOME'])
+	os.add_dll_directory(os.environ['METAFFI_HOME'] + '\\bin')
 
-class _PyCdtsConverter:
-	def __init__(self):
-		if platform.system() == 'Windows':
-			os.add_dll_directory(os.environ['METAFFI_HOME'])
-			os.add_dll_directory(os.environ['METAFFI_HOME'] + '\\bin')
-		
-		self.xllr_python3 = ctypes.cdll.LoadLibrary(metaffi.xllr_wrapper.get_dynamic_lib_path_from_metaffi_home('xllr.python311'))
-		
-		# Set argtypes and restype for convert_host_params_to_cdts
-		self.xllr_python3.convert_host_params_to_cdts.argtypes = [py_object, py_object, ctypes.c_uint64]
-		self.xllr_python3.convert_host_params_to_cdts.restype = ctypes.c_void_p
-		
-		# Set argtypes and restype for convert_host_return_values_from_cdts
-		self.xllr_python3.convert_host_return_values_from_cdts.argtypes = [ctypes.c_void_p, ctypes.c_uint64]
-		self.xllr_python3.convert_host_return_values_from_cdts.restype = py_object
+xllr_python3 = ctypes.cdll.LoadLibrary(xllr_wrapper.get_dynamic_lib_path_from_metaffi_home('xllr.python311'))
+
+# Set argtypes and restype for convert_host_params_to_cdts
+xllr_python3.convert_host_params_to_cdts.argtypes = [py_object, ctypes.POINTER(metaffi_types.metaffi_type_info), ctypes.c_uint64, ctypes.c_uint64]
+xllr_python3.convert_host_params_to_cdts.restype = ctypes.c_void_p
+
+# Set argtypes and restype for convert_host_return_values_from_cdts
+xllr_python3.convert_host_return_values_from_cdts.argtypes = [ctypes.c_void_p, ctypes.c_uint64]
+xllr_python3.convert_host_return_values_from_cdts.restype = py_object
+
+
+def convert_to_metaffi_type_info_ptr(input_types: Union[Tuple[metaffi_types.metaffi_type_info], List[metaffi_types.metaffi_type_info]]) -> ctypes.POINTER(metaffi_types.metaffi_type_info):
+	if not isinstance(input_types, (tuple, list)):
+		raise ValueError("Input must be a tuple or list of metaffi_type_info objects")
 	
-	def convert_host_params_to_cdts(self, params_names: py_object, params_types: py_object, return_values_size: int) -> ctypes.c_void_p:
-		res = self.xllr_python3.convert_host_params_to_cdts(params_names, params_types, return_values_size)
-		return res
+	metaffi_type_info_Array = metaffi_types.metaffi_type_info * len(input_types)
+	metaffi_type_info_array_instance = metaffi_type_info_Array(*input_types)
 	
-	def convert_host_return_values_from_cdts(self, pcdts: ctypes.c_void_p, index: int) -> py_object:
-		res = self.xllr_python3.convert_host_return_values_from_cdts(pcdts, index)
-		return res
+	return ctypes.pointer(metaffi_type_info_array_instance)
+
+
+def convert_host_params_to_cdts(params_names: py_object, params_types: tuple | list, params_size: ctypes.c_uint64, return_values_size: ctypes.c_uint64) -> ctypes.c_void_p:
+	pparams_types = convert_to_metaffi_type_info_ptr(params_types)
+	res = xllr_python3.convert_host_params_to_cdts(params_names, pparams_types, params_size, return_values_size)
+	return res
 
 
-py_cdts_converter: _PyCdtsConverter = _PyCdtsConverter()
+def convert_host_return_values_from_cdts(pcdts: ctypes.c_void_p, index: int) -> py_object:
+	res = xllr_python3.convert_host_return_values_from_cdts(pcdts, index)
+	return res
```

### Comparing `metaffi_api-0.0.24/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.25/metaffi/xllr_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ctypes
 from ctypes import *
-from metaffi.metaffi_types import *
+from .metaffi_types import *
 import platform
 import os
 
 
 def get_dynamic_lib_path_from_metaffi_home(fname: str):
 	osname = platform.system()
 	if os.getenv('METAFFI_HOME') is None:
@@ -17,81 +17,114 @@
 	elif osname == 'Darwin':
 		return os.getenv('METAFFI_HOME') + '/' + fname + '.dylib'
 	else:
 		return os.getenv('METAFFI_HOME') + '/' + fname + '.so'  # for everything that is not windows or mac, return .so
 
 
 if platform.system() == 'Windows':
-	os.add_dll_directory(os.getenv('METAFFI_HOME')+'\\bin\\')
+	os.add_dll_directory(os.getenv('METAFFI_HOME') + '\\bin\\')
 
 xllr_python3 = ctypes.cdll.LoadLibrary(get_dynamic_lib_path_from_metaffi_home('xllr.python311'))
-xllr_python3.call_xcall.argtypes = [ctypes.c_void_p, ctypes.c_void_p, ctypes.py_object, ctypes.py_object, ctypes.py_object]
+xllr_python3.call_xcall.argtypes = [ctypes.c_void_p, ctypes.py_object, ctypes.py_object, ctypes.py_object]
 xllr_python3.call_xcall.restype = ctypes.py_object
 
-xllr = cdll.LoadLibrary(get_dynamic_lib_path_from_metaffi_home('xllr'))
+_xllr = cdll.LoadLibrary(get_dynamic_lib_path_from_metaffi_home('xllr'))
 
 # Set argtypes and restype
-xllr.load_runtime_plugin.argtypes = [ctypes.c_char_p, ctypes.c_uint32, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint32)]
-xllr.load_runtime_plugin.restype = None
+_xllr.load_runtime_plugin.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p)]
+_xllr.load_runtime_plugin.restype = None
 
-xllr.free_runtime_plugin.argtypes = [ctypes.c_char_p, ctypes.c_uint32, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint32)]
-xllr.free_runtime_plugin.restype = None
+_xllr.free_runtime_plugin.argtypes = [ctypes.c_char_p, ctypes.POINTER(ctypes.c_char_p)]
+_xllr.free_runtime_plugin.restype = None
 
-xllr.load_function.argtypes = [ctypes.c_char_p, ctypes.c_uint32, ctypes.c_char_p, ctypes.c_uint32, ctypes.c_char_p, ctypes.c_uint32, ctypes.POINTER(metaffi_type_info), ctypes.POINTER(metaffi_type_info), ctypes.c_uint8, ctypes.c_uint8, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint32)]
-xllr.load_function.restype = ctypes.POINTER(ctypes.c_void_p)
+_xllr.load_entity.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.POINTER(metaffi_type_info), ctypes.c_int8, ctypes.POINTER(metaffi_type_info), ctypes.c_int8, ctypes.POINTER(ctypes.c_char_p)]
+_xllr.load_entity.restype = ctypes.c_void_p
 
-xllr.free_function.argtypes = [ctypes.c_char_p, ctypes.c_uint32, ctypes.POINTER(ctypes.c_void_p), ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint32)]
-xllr.free_function.restype = None
-
-xllr.alloc_cdts_buffer.argtypes = [ctypes.c_uint64, ctypes.c_uint64]
-xllr.alloc_cdts_buffer.restype = ctypes.c_void_p
-
-xllr.make_callable.argtypes = [ctypes.c_char_p, ctypes.c_uint32, ctypes.py_object, ctypes.POINTER(ctypes.c_uint64), ctypes.POINTER(ctypes.c_uint64), ctypes.c_uint8, ctypes.c_uint8, ctypes.POINTER(ctypes.c_char_p), ctypes.POINTER(ctypes.c_uint32)]
-xllr.make_callable.restype = ctypes.POINTER(ctypes.c_void_p)
-
-class _XllrWrapper:
-	def __init__(self):
-		global xllr
-		
-		if platform.system() == 'Windows':
-			os.add_dll_directory(os.environ['METAFFI_HOME'])
-			os.add_dll_directory(os.environ['METAFFI_HOME'] + '\\bin')
-	
-	def load_runtime_plugin(self, runtime_plugin: str) -> None:
-		err = ctypes.c_char_p()
-		err_len = ctypes.c_uint32()
-		xllr.load_runtime_plugin(runtime_plugin.encode('utf-8'), len(runtime_plugin), ctypes.byref(err), ctypes.byref(err_len))
-		if err_len.value > 0:
-			raise RuntimeError(err.value[:err_len.value].decode('utf-8'))
-	
-	def free_runtime_plugin(self, runtime_plugin: str) -> None:
-		err = ctypes.c_char_p()
-		err_len = ctypes.c_uint32()
-		xllr.free_runtime_plugin(runtime_plugin.encode('utf-8'), len(runtime_plugin), ctypes.byref(err), ctypes.byref(err_len))
-		if err_len.value > 0:
-			raise RuntimeError(err.value[:err_len.value].decode('utf-8'))
-	
-	def load_function(self, runtime_plugin_name: str, module_path: str, function_path: str,
-						params_types: ctypes.POINTER(metaffi_type_info),
-						retvals_types: ctypes.POINTER(metaffi_type_info), params_count: int,
-						retval_count: int) -> ctypes.c_void_p:
-		err = ctypes.c_char_p()
-		err_len = ctypes.c_uint32()
-		result = xllr.load_function(runtime_plugin_name.encode('utf-8'), len(runtime_plugin_name), module_path.encode('utf-8'), len(module_path),
-										function_path.encode('utf-8'), len(function_path), params_types, retvals_types, params_count,
-										retval_count, ctypes.byref(err), ctypes.byref(err_len))
-		if err_len.value > 0:
-			raise RuntimeError(err.value[:err_len.value].decode('utf-8'))
-		return result
-	
-	def free_function(self, runtime_plugin_name: str, pff: ctypes.POINTER(ctypes.c_void_p)) -> None:
-		err = ctypes.create_string_buffer(1000)
-		err_len = ctypes.c_uint32()
-		xllr.free_function(runtime_plugin_name, len(runtime_plugin_name), pff, ctypes.byref(err), ctypes.byref(err_len))
-		if err_len.value > 0:
-			raise RuntimeError(err.value[:err_len.value].decode('utf-8'))
+_xllr.free_xcall.argtypes = [ctypes.c_char_p, ctypes.c_void_p, ctypes.POINTER(ctypes.c_char_p)]
+_xllr.free_xcall.restype = None
+
+_xllr.make_callable.argtypes = [ctypes.c_char_p, ctypes.py_object, ctypes.POINTER(metaffi_type_info), ctypes.c_int8, ctypes.POINTER(metaffi_type_info), ctypes.c_int8, ctypes.POINTER(ctypes.c_char_p)]
+_xllr.make_callable.restype = ctypes.c_void_p
+
+_xllr.alloc_cdts_buffer.argtypes = [ctypes.c_uint64, ctypes.c_uint64]
+_xllr.alloc_cdts_buffer.restype = ctypes.c_void_p
+
+_xllr.free_cdts_buffer.argtypes = [ctypes.c_void_p]
+_xllr.free_cdts_buffer.restype = None
+
+_xllr.free_string.argtypes = [ctypes.c_char_p]
+_xllr.free_string.restype = None
+
+if platform.system() == 'Windows':
+	os.add_dll_directory(os.environ['METAFFI_HOME'])
+	os.add_dll_directory(os.environ['METAFFI_HOME'] + '\\bin')
+
+
+def load_runtime_plugin(runtime_plugin: str) -> None:
+	global _xllr
+	err = ctypes.c_char_p()
+	_xllr.load_runtime_plugin(runtime_plugin.encode('utf-8'), ctypes.byref(err))
+	
+	# check if err is not NULL
+	if err.value is not None:
+		msg = err.value.decode('utf-8')
+		_xllr.free_string(err)  # call xllr.free_string to free the memory allocated by xllr
+		raise RuntimeError(msg)
+
+
+def free_runtime_plugin(runtime_plugin: str) -> None:
+	err = ctypes.c_char_p()
+	_xllr.free_runtime_plugin(runtime_plugin.encode('utf-8'), ctypes.byref(err))
 	
-	def alloc_cdts_buffer(self, params_count: int, ret_count: int) -> ctypes.c_void_p:
-		return xllr.alloc_cdts_buffer(params_count, ret_count)
+	# check if err is not NULL
+	if err.value is not None:
+		msg = err.value.decode('utf-8')
+		_xllr.free_string(err)  # call xllr.free_string to free the memory allocated by xllr
+		raise RuntimeError(msg)
+
+
+def load_entity(runtime_plugin_name: str, module_path: str, function_path: str,
+		params_types: ctypes.POINTER(metaffi_type_info), params_count: int,
+		retvals_types: ctypes.POINTER(metaffi_type_info), retval_count: int) -> ctypes.c_void_p:
+	err = ctypes.c_char_p()
+	result = _xllr.load_entity(runtime_plugin_name.encode('utf-8'), module_path.encode('utf-8'),
+		function_path.encode('utf-8'), params_types, params_count, retvals_types,
+		retval_count, ctypes.byref(err))
+	
+	# check if err is not NULL
+	if err.value is not None:
+		msg = err.value.decode('utf-8')
+		_xllr.free_string(err)  # call xllr.free_string to free the memory allocated by xllr
+		raise RuntimeError(msg)
+	
+	return result
+
+
+def free_xcall(runtime_plugin_name: str, pxcall: ctypes.c_void_p) -> None:
+	err = ctypes.c_char_p()
+	_xllr.free_xcall(ctypes.c_char_p(runtime_plugin_name.encode('utf-8')), pxcall, ctypes.byref(err))
+	# check if err is not NULL
+	if err.value is not None:
+		msg = err.value.decode('utf-8')
+		_xllr.free_string(err)  # call xllr.free_string to free the memory allocated by xllr
+		raise RuntimeError(msg)
+
+
+def make_callable(runtime_plugin_name: str, f: callable, params_types: ctypes.POINTER(metaffi_type_info), params_count: int, retvals_types: ctypes.POINTER(metaffi_type_info), retval_count: int) -> ctypes.c_void_p:
+	err = ctypes.c_char_p()
+	result = _xllr.make_callable(runtime_plugin_name.encode('utf-8'), f, params_types, params_count, retvals_types, retval_count, ctypes.byref(err))
+	
+	# check if err is not NULL
+	if err.value is not None:
+		msg = err.value.decode('utf-8')
+		_xllr.free_string(err)  # call xllr.free_string to free the memory allocated by xllr
+		raise RuntimeError(msg)
+	
+	return result
+
+
+def alloc_cdts_buffer(params_count: int, ret_count: int) -> ctypes.c_void_p:
+	return _xllr.alloc_cdts_buffer(params_count, ret_count)
 
 
-xllr_wrapper: _XllrWrapper = _XllrWrapper()
+def free_cdts_buffer(buffer: ctypes.c_void_p) -> None:
+	_xllr.free_cdts_buffer(buffer)
```

### Comparing `metaffi_api-0.0.24/publish.ps1` & `metaffi_api-0.0.25/publish.ps1`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.24/pyproject.toml` & `metaffi_api-0.0.25/pyproject.toml`

 * *Files identical despite different names*

