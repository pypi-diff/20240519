# Comparing `tmp/thymus_ast-0.1.8.tar.gz` & `tmp/thymus_ast-0.1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thymus_ast-0.1.8.tar", max compression
+gzip compressed data, was "thymus_ast-0.1.8.1.tar", max compression
```

## Comparing `thymus_ast-0.1.8.tar` & `thymus_ast-0.1.8.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1093 2023-09-19 16:12:05.290498 thymus_ast-0.1.8/LICENSE
--rw-r--r--   0        0        0      490 2024-04-25 16:39:46.257428 thymus_ast-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      544 2023-12-09 12:09:08.370980 thymus_ast-0.1.8/README.md
--rw-r--r--   0        0        0        2 2023-09-19 21:16:45.075801 thymus_ast-0.1.8/thymus_ast/__init__.py
--rw-r--r--   0        0        0      572 2024-05-17 14:25:09.835234 thymus_ast-0.1.8/thymus_ast/ios/__init__.py
--rw-r--r--   0        0        0    26755 2024-05-18 11:57:21.181590 thymus_ast-0.1.8/thymus_ast/ios/ios.py
--rw-r--r--   0        0        0      702 2024-04-18 19:38:59.977723 thymus_ast-0.1.8/thymus_ast/junos/__init__.py
--rw-r--r--   0        0        0    15894 2024-05-17 07:47:29.109539 thymus_ast-0.1.8/thymus_ast/junos/junos.py
--rw-r--r--   0        0        0      897 2024-04-26 10:08:26.706295 thymus_ast-0.1.8/thymus_ast/junos_ng/__init__.py
--rw-r--r--   0        0        0    21611 2024-05-17 07:57:02.830830 thymus_ast-0.1.8/thymus_ast/junos_ng/junos_ng.py
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 thymus_ast-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-09-19 16:12:05.290498 thymus_ast-0.1.8.1/LICENSE
+-rw-r--r--   0        0        0      492 2024-05-19 09:08:16.921708 thymus_ast-0.1.8.1/pyproject.toml
+-rw-r--r--   0        0        0      544 2023-12-09 12:09:08.370980 thymus_ast-0.1.8.1/README.md
+-rw-r--r--   0        0        0        2 2023-09-19 21:16:45.075801 thymus_ast-0.1.8.1/thymus_ast/__init__.py
+-rw-r--r--   0        0        0      572 2024-05-17 14:25:09.835234 thymus_ast-0.1.8.1/thymus_ast/ios/__init__.py
+-rw-r--r--   0        0        0    26712 2024-05-19 09:07:51.284183 thymus_ast-0.1.8.1/thymus_ast/ios/ios.py
+-rw-r--r--   0        0        0      702 2024-04-18 19:38:59.977723 thymus_ast-0.1.8.1/thymus_ast/junos/__init__.py
+-rw-r--r--   0        0        0    15894 2024-05-17 07:47:29.109539 thymus_ast-0.1.8.1/thymus_ast/junos/junos.py
+-rw-r--r--   0        0        0      897 2024-04-26 10:08:26.706295 thymus_ast-0.1.8.1/thymus_ast/junos_ng/__init__.py
+-rw-r--r--   0        0        0    21611 2024-05-17 07:57:02.830830 thymus_ast-0.1.8.1/thymus_ast/junos_ng/junos_ng.py
+-rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 thymus_ast-0.1.8.1/PKG-INFO
```

### Comparing `thymus_ast-0.1.8/LICENSE` & `thymus_ast-0.1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/README.md` & `thymus_ast-0.1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/thymus_ast/ios/__init__.py` & `thymus_ast-0.1.8.1/thymus_ast/ios/__init__.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/thymus_ast/ios/ios.py` & `thymus_ast-0.1.8.1/thymus_ast/ios/ios.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,22 +633,20 @@
 
 
 def validate_config(data: list[str]) -> bool:
     version_found = False
     end_found = False
 
     for line in data:
-        stripped = line.strip()
-
-        if stripped.startswith('version '):
+        if line.startswith('version '):
             if end_found:
                 # version cannot be present after the end statement
                 return False
             version_found = True
-        elif stripped == 'end':
+        elif line == 'end':
             end_found = True
 
     return version_found and end_found
 
 
 def find_head(data: list[str]) -> int:
     for line_no, line in enumerate(data):
```

### Comparing `thymus_ast-0.1.8/thymus_ast/junos/__init__.py` & `thymus_ast-0.1.8.1/thymus_ast/junos/__init__.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/thymus_ast/junos/junos.py` & `thymus_ast-0.1.8.1/thymus_ast/junos/junos.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/thymus_ast/junos_ng/__init__.py` & `thymus_ast-0.1.8.1/thymus_ast/junos_ng/__init__.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/thymus_ast/junos_ng/junos_ng.py` & `thymus_ast-0.1.8.1/thymus_ast/junos_ng/junos_ng.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.8/PKG-INFO` & `thymus_ast-0.1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thymus-ast
-Version: 0.1.8
+Version: 0.1.8.1
 Summary: A set of tools to build ASTs for different NOS
 Author: Igor Malyushkin
 Author-email: gmalyushkin@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

