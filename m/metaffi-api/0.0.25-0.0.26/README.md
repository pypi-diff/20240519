# Comparing `tmp/metaffi_api-0.0.25.tar.gz` & `tmp/metaffi_api-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaffi_api-0.0.25.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "metaffi_api-0.0.26.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `metaffi_api-0.0.25.tar` & `metaffi_api-0.0.26.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.25/CMakeLists.txt
--rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.25/LICENSE
--rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.25/README.md
--rw-r--r--   0        0        0      538 2024-05-19 10:51:04.097565 metaffi_api-0.0.25/metaffi/__init__.py
--rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.25/metaffi/classes_metaffi.puml
--rw-r--r--   0        0        0      411 2024-05-19 08:34:56.915898 metaffi_api-0.0.25/metaffi/metaffi_handle.py
--rw-r--r--   0        0        0     4823 2024-05-19 07:36:05.188625 metaffi_api-0.0.25/metaffi/metaffi_module.py
--rw-r--r--   0        0        0      484 2024-05-18 16:45:00.514372 metaffi_api-0.0.25/metaffi/metaffi_runtime.py
--rw-r--r--   0        0        0     4619 2024-05-19 03:25:53.676813 metaffi_api-0.0.25/metaffi/metaffi_types.py
--rw-r--r--   0        0        0     2024 2024-05-18 16:43:11.504988 metaffi_api-0.0.25/metaffi/pycdts_converter.py
--rw-r--r--   0        0        0     5217 2024-05-19 06:50:11.445337 metaffi_api-0.0.25/metaffi/xllr_wrapper.py
--rw-r--r--   0        0        0      584 2024-04-21 10:05:04.530248 metaffi_api-0.0.25/publish.ps1
--rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.25/pyproject.toml
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0      205 2024-04-15 06:15:13.341334 metaffi_api-0.0.26/CMakeLists.txt
+-rw-r--r--   0        0        0     1096 2022-05-28 09:56:58.251104 metaffi_api-0.0.26/LICENSE
+-rw-r--r--   0        0        0       57 2024-01-18 12:19:08.787247 metaffi_api-0.0.26/README.md
+-rw-r--r--   0        0        0      538 2024-05-19 11:11:13.569556 metaffi_api-0.0.26/metaffi/__init__.py
+-rw-r--r--   0        0        0     1270 2024-02-04 18:44:32.014120 metaffi_api-0.0.26/metaffi/classes_metaffi.puml
+-rw-r--r--   0        0        0      350 2024-05-19 11:08:01.944504 metaffi_api-0.0.26/metaffi/metaffi_handle.py
+-rw-r--r--   0        0        0     4823 2024-05-19 07:36:05.188625 metaffi_api-0.0.26/metaffi/metaffi_module.py
+-rw-r--r--   0        0        0      484 2024-05-18 16:45:00.514372 metaffi_api-0.0.26/metaffi/metaffi_runtime.py
+-rw-r--r--   0        0        0     4619 2024-05-19 03:25:53.676813 metaffi_api-0.0.26/metaffi/metaffi_types.py
+-rw-r--r--   0        0        0     2024 2024-05-18 16:43:11.504988 metaffi_api-0.0.26/metaffi/pycdts_converter.py
+-rw-r--r--   0        0        0     5217 2024-05-19 06:50:11.445337 metaffi_api-0.0.26/metaffi/xllr_wrapper.py
+-rw-r--r--   0        0        0      660 2024-05-19 11:10:59.459848 metaffi_api-0.0.26/publish.ps1
+-rw-r--r--   0        0        0      535 2024-03-08 20:55:47.528284 metaffi_api-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 metaffi_api-0.0.26/PKG-INFO
```

### Comparing `metaffi_api-0.0.25/LICENSE` & `metaffi_api-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.25/metaffi/__init__.py` & `metaffi_api-0.0.26/metaffi/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Python MetaFFI API"""
 
-__version__ = "0.0.25"
+__version__ = "0.0.26"
 
 __all__ = ['metaffi', 'metaffi_types', 'metaffi_runtime', 'metaffi_module', 'metaffi_handle', 'metaffi_types', 'xllr_wrapper', 'pycdts_converter', 'metaffi_type_info', 'MetaFFITypes']
 
 import metaffi
 from . import metaffi_types
 from . import metaffi_runtime
 from . import metaffi_module
```

### Comparing `metaffi_api-0.0.25/metaffi/classes_metaffi.puml` & `metaffi_api-0.0.26/metaffi/classes_metaffi.puml`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.25/metaffi/metaffi_module.py` & `metaffi_api-0.0.26/metaffi/metaffi_module.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.25/metaffi/metaffi_types.py` & `metaffi_api-0.0.26/metaffi/metaffi_types.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.25/metaffi/pycdts_converter.py` & `metaffi_api-0.0.26/metaffi/pycdts_converter.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.25/metaffi/xllr_wrapper.py` & `metaffi_api-0.0.26/metaffi/xllr_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaffi_api-0.0.25/pyproject.toml` & `metaffi_api-0.0.26/pyproject.toml`

 * *Files identical despite different names*

