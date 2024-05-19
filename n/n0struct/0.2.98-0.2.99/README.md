# Comparing `tmp/n0struct-0.2.98.tar.gz` & `tmp/n0struct-0.2.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\n0struct-0.2.98.tar", last modified: Sat May 27 10:01:32 2023, max compression
+gzip compressed data, was "dist\n0struct-0.2.99.tar", last modified: Thu Oct 19 08:14:34 2023, max compression
```

## Comparing `n0struct-0.2.98.tar` & `n0struct-0.2.99.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.347421 n0struct-0.2.98/
--rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.98/LICENSE
--rw-rw-rw-   0        0        0     1060 2023-05-27 10:01:32.347421 n0struct-0.2.98/PKG-INFO
--rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.98/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.316165 n0struct-0.2.98/n0struct/
--rw-rw-rw-   0        0        0      988 2023-05-13 11:12:54.000000 n0struct-0.2.98/n0struct/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-05-12 12:43:36.000000 n0struct-0.2.98/n0struct/n0struct_arrays.py
--rw-rw-rw-   0        0        0     2104 2023-05-13 11:27:25.000000 n0struct-0.2.98/n0struct/n0struct_comprehensions.py
--rw-rw-rw-   0        0        0    13176 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_date.py
--rw-rw-rw-   0        0        0     3389 2023-05-13 05:52:52.000000 n0struct-0.2.98/n0struct/n0struct_files.py
--rw-rw-rw-   0        0        0    29723 2023-05-27 09:55:21.000000 n0struct-0.2.98/n0struct/n0struct_files_csv.py
--rw-rw-rw-   0        0        0     7117 2023-05-13 11:56:28.000000 n0struct-0.2.98/n0struct/n0struct_files_fwf.py
--rw-rw-rw-   0        0        0    15648 2023-05-13 11:36:31.000000 n0struct-0.2.98/n0struct/n0struct_findall.py
--rw-rw-rw-   0        0        0     4070 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_git.py
--rw-rw-rw-   0        0        0    20514 2023-05-27 10:00:27.000000 n0struct-0.2.98/n0struct/n0struct_logging.py
--rw-rw-rw-   0        0        0     2287 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_mask.py
--rw-rw-rw-   0        0        0    10093 2023-05-26 08:59:17.000000 n0struct-0.2.98/n0struct/n0struct_n0dict_.py
--rw-rw-rw-   0        0        0    17116 2023-05-13 12:19:09.000000 n0struct-0.2.98/n0struct/n0struct_n0dict__.py
--rw-rw-rw-   0        0        0     8568 2023-05-22 16:31:02.000000 n0struct-0.2.98/n0struct/n0struct_n0list_.py
--rw-rw-rw-   0        0        0    75645 2023-05-13 12:22:04.000000 n0struct-0.2.98/n0struct/n0struct_n0list_n0dict.py
--rw-rw-rw-   0        0        0      917 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_random.py
--rw-rw-rw-   0        0        0     3852 2023-04-25 08:08:57.000000 n0struct-0.2.98/n0struct/n0struct_references.py
--rw-rw-rw-   0        0        0     3235 2023-05-12 12:49:17.000000 n0struct-0.2.98/n0struct/n0struct_transform_structure.py
--rw-rw-rw-   0        0        0    18218 2023-05-14 15:31:16.000000 n0struct-0.2.98/n0struct/n0struct_utils.py
--rw-rw-rw-   0        0        0     6659 2023-05-12 12:42:29.000000 n0struct-0.2.98/n0struct/n0struct_utils_compare.py
--rw-rw-rw-   0        0        0     4120 2023-05-12 12:42:54.000000 n0struct-0.2.98/n0struct/n0struct_utils_find.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.347421 n0struct-0.2.98/n0struct/test/
--rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.98/n0struct/test/__init__.py
--rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.98/n0struct/test/__main__.py
--rw-rw-rw-   0        0        0    33051 2023-05-13 12:06:10.000000 n0struct-0.2.98/n0struct/test/test_n0struct.py
--rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.98/n0struct/test/test_n0struct2.py
--rw-rw-rw-   0        0        0      890 2023-05-13 12:07:38.000000 n0struct-0.2.98/n0struct/test/test_n0struct3.py
--rw-rw-rw-   0        0        0     1490 2023-05-13 12:23:25.000000 n0struct-0.2.98/n0struct/test/test_n0struct4.py
-drwxrwxrwx   0        0        0        0 2023-05-27 10:01:32.347421 n0struct-0.2.98/n0struct.egg-info/
--rw-rw-rw-   0        0        0     1060 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 10:01:32.000000 n0struct-0.2.98/n0struct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 10:01:32.363011 n0struct-0.2.98/setup.cfg
--rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.98/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-19 08:14:34.870366 n0struct-0.2.99/
+-rw-rw-rw-   0        0        0    11558 2022-09-04 19:16:09.000000 n0struct-0.2.99/LICENSE
+-rw-rw-rw-   0        0        0     1060 2023-10-19 08:14:34.870366 n0struct-0.2.99/PKG-INFO
+-rw-rw-rw-   0        0        0      590 2022-09-04 19:16:09.000000 n0struct-0.2.99/README.md
+drwxrwxrwx   0        0        0        0 2023-10-19 08:14:34.839124 n0struct-0.2.99/n0struct/
+-rw-rw-rw-   0        0        0      988 2023-05-13 11:12:54.000000 n0struct-0.2.99/n0struct/__init__.py
+-rw-rw-rw-   0        0        0     3778 2023-10-19 08:04:10.000000 n0struct-0.2.99/n0struct/n0struct_arrays.py
+-rw-rw-rw-   0        0        0     2613 2023-10-19 08:04:10.000000 n0struct-0.2.99/n0struct/n0struct_comprehensions.py
+-rw-rw-rw-   0        0        0    13176 2023-04-25 08:08:57.000000 n0struct-0.2.99/n0struct/n0struct_date.py
+-rw-rw-rw-   0        0        0     3832 2023-10-19 08:04:10.000000 n0struct-0.2.99/n0struct/n0struct_files.py
+-rw-rw-rw-   0        0        0    29723 2023-05-27 09:55:21.000000 n0struct-0.2.99/n0struct/n0struct_files_csv.py
+-rw-rw-rw-   0        0        0     7117 2023-05-13 11:56:28.000000 n0struct-0.2.99/n0struct/n0struct_files_fwf.py
+-rw-rw-rw-   0        0        0    15648 2023-05-13 11:36:31.000000 n0struct-0.2.99/n0struct/n0struct_findall.py
+-rw-rw-rw-   0        0        0     4070 2023-04-25 08:08:57.000000 n0struct-0.2.99/n0struct/n0struct_git.py
+-rw-rw-rw-   0        0        0    20514 2023-05-27 10:00:27.000000 n0struct-0.2.99/n0struct/n0struct_logging.py
+-rw-rw-rw-   0        0        0     2287 2023-04-25 08:08:57.000000 n0struct-0.2.99/n0struct/n0struct_mask.py
+-rw-rw-rw-   0        0        0    10093 2023-05-26 08:59:17.000000 n0struct-0.2.99/n0struct/n0struct_n0dict_.py
+-rw-rw-rw-   0        0        0    17116 2023-05-13 12:19:09.000000 n0struct-0.2.99/n0struct/n0struct_n0dict__.py
+-rw-rw-rw-   0        0        0     9002 2023-10-19 07:36:08.000000 n0struct-0.2.99/n0struct/n0struct_n0list_.py
+-rw-rw-rw-   0        0        0    75645 2023-05-13 12:22:04.000000 n0struct-0.2.99/n0struct/n0struct_n0list_n0dict.py
+-rw-rw-rw-   0        0        0      917 2023-04-25 08:08:57.000000 n0struct-0.2.99/n0struct/n0struct_random.py
+-rw-rw-rw-   0        0        0     3852 2023-04-25 08:08:57.000000 n0struct-0.2.99/n0struct/n0struct_references.py
+-rw-rw-rw-   0        0        0     3235 2023-05-12 12:49:17.000000 n0struct-0.2.99/n0struct/n0struct_transform_structure.py
+-rw-rw-rw-   0        0        0    27151 2023-10-19 08:13:41.000000 n0struct-0.2.99/n0struct/n0struct_utils.py
+-rw-rw-rw-   0        0        0     6659 2023-05-12 12:42:29.000000 n0struct-0.2.99/n0struct/n0struct_utils_compare.py
+-rw-rw-rw-   0        0        0     4120 2023-05-12 12:42:54.000000 n0struct-0.2.99/n0struct/n0struct_utils_find.py
+drwxrwxrwx   0        0        0        0 2023-10-19 08:14:34.870366 n0struct-0.2.99/n0struct/test/
+-rw-rw-rw-   0        0        0        0 2022-09-04 19:16:09.000000 n0struct-0.2.99/n0struct/test/__init__.py
+-rw-rw-rw-   0        0        0      136 2022-09-04 19:16:09.000000 n0struct-0.2.99/n0struct/test/__main__.py
+-rw-rw-rw-   0        0        0    33051 2023-05-13 12:06:10.000000 n0struct-0.2.99/n0struct/test/test_n0struct.py
+-rw-rw-rw-   0        0        0     2572 2023-03-06 04:48:48.000000 n0struct-0.2.99/n0struct/test/test_n0struct2.py
+-rw-rw-rw-   0        0        0      890 2023-05-13 12:07:38.000000 n0struct-0.2.99/n0struct/test/test_n0struct3.py
+-rw-rw-rw-   0        0        0     1490 2023-05-13 12:23:25.000000 n0struct-0.2.99/n0struct/test/test_n0struct4.py
+-rw-rw-rw-   0        0        0     1492 2023-10-19 07:36:09.000000 n0struct-0.2.99/n0struct/test/test_n0struct6.py
+-rw-rw-rw-   0        0        0     1520 2023-10-19 07:36:09.000000 n0struct-0.2.99/n0struct/test/test_n0struct7.py
+drwxrwxrwx   0        0        0        0 2023-10-19 08:14:34.870366 n0struct-0.2.99/n0struct.egg-info/
+-rw-rw-rw-   0        0        0     1060 2023-10-19 08:14:34.000000 n0struct-0.2.99/n0struct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1096 2023-10-19 08:14:34.000000 n0struct-0.2.99/n0struct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-19 08:14:34.000000 n0struct-0.2.99/n0struct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-19 08:14:34.000000 n0struct-0.2.99/n0struct.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-10-19 08:14:34.000000 n0struct-0.2.99/n0struct.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-10-19 08:14:34.000000 n0struct-0.2.99/n0struct.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-19 08:14:34.870366 n0struct-0.2.99/setup.cfg
+-rw-rw-rw-   0        0        0     2476 2023-04-02 07:28:40.000000 n0struct-0.2.99/setup.py
```

### Comparing `n0struct-0.2.98/LICENSE` & `n0struct-0.2.99/LICENSE`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/PKG-INFO` & `n0struct-0.2.99/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.98
+Version: 0.2.99
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.98/README.md` & `n0struct-0.2.99/README.md`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/__init__.py` & `n0struct-0.2.99/n0struct/__init__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_arrays.py` & `n0struct-0.2.99/n0struct/n0struct_arrays.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing
+from .n0struct_utils import iterable
 # ******************************************************************************
 # ******************************************************************************
 def split_pair(
                 in_str: str,
-                delimiter: str,
+                delimiter: typing.Union[str, typing.Iterable],
                 transform_left: callable = lambda x: x,
                 transform_right: callable = lambda x: x,
                 default_element: int = 1,
                 default_left: typing.Any = None,
                 default_right: typing.Any = None,
 ) -> tuple:
     """
@@ -18,24 +19,25 @@
         'www.aaa.com' by '://'                          => (default_left, 'www.aaa.com')
         'https://www.aaa.com' by '://'                  => ('http', 'www.aaa.com')
         'www.aaa.com',default_element = 0 by '/'        => ('www.aaa.com')
         'www.aaa.com/path',default_element = 0 by '/'   => ('www.aaa.com', 'path')
     """
     if not in_str:
         return transform_left(default_left), transform_right(default_right)
-
-    str_parts = in_str.split(delimiter, 1)
-    if len(str_parts) == 1:
-        if default_element:
-            # second (right) element is default
-            return transform_left(default_left), transform_right(str_parts[0])
-        else:
-            # first (left) element is default
-            return transform_left(str_parts[0]), transform_right(default_right)
-    return transform_left(str_parts[0]), transform_right(str_parts[1])
+        
+    for _delimiter in iterable(delimiter):
+        if _delimiter in in_str:
+            str_parts = in_str.split(_delimiter, 1)
+            return transform_left(str_parts[0]), transform_right(str_parts[1])
+    if default_element:
+        # second (right) element is default
+        return transform_left(default_left), transform_right(in_str)
+    else:
+        # first (left) element is default
+        return transform_left(in_str), transform_right(default_right)
 # ******************************************************************************
 def join_triplets(
                     in_list: typing.Union[None, str, tuple, list],
                     level: int = 0
 ) -> str:
     """
     join_triplets(in_list: typing.Union[None, str, tuple, list], level = 0) -> str:
```

### Comparing `n0struct-0.2.98/n0struct/n0struct_comprehensions.py` & `n0struct-0.2.99/n0struct/n0struct_comprehensions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Python 3.8+ is required. := (walrus operator) is used in comprehension inside load_ini(...)
 import typing
 from .n0struct_utils import isnumber
+from .n0struct_utils import iterable
 from .n0struct_files import load_lines
+from .n0struct_arrays import split_pair
 # ******************************************************************************
 def default_parse_value(key_value, default_value):
     stripped_value = key_value[1].strip()
     if isnumber(stripped_value):
         if '.' in stripped_value:
             return round(float(stripped_value), 7)
         else:
@@ -18,16 +20,16 @@
             return stripped_value[1:-1]
         else:
             return stripped_value
 
 def load_ini(
                 file_path: str,
                 default_value = None,
-                equal_tag: str = '=',
-                comment_tags: typing.Union[tuple, list] = ("#", "//"),
+                equal_tag: typing.Union[str, typing.Iterable] = '=',
+                comment_tags: typing.Union[str, typing.Iterable] = ("#", "//"),
                 parse_key: typing.Callable = lambda key_value, default_key: key_value[0].strip().upper(),
                 parse_value: typing.Callable = default_parse_value,
 ) -> dict:
     """
         load ini file as:
             // Ini file
             KEY1 =VALUE1
@@ -36,19 +38,27 @@
         to dict:
             {
                 'KEY1': "VALUE1",
                 'KEY2': "VALUE2",
             }
 
     """
-    return {
-        parse_key((key_value:=stripped_line.split(equal_tag, 1)), None): (
-            parse_value(key_value, default_value)
-            if len(key_value) > 1
-            else default_value
-        )
-        for line in load_lines(file_path)
-        if  (stripped_line:=line.strip())
-            and not any(stripped_line.startswith(comment_tag) for comment_tag in comment_tags)
-    }
+    result_dict = {}
+    for line in load_lines(file_path):
+        if (stripped_line:=line.strip()) \
+        and not any(stripped_line.startswith(comment_tag) for comment_tag in iterable(comment_tags)):
+            key, value = split_pair(
+                stripped_line,
+                delimiter = equal_tag,
+                transform_left = lambda x: parse_key((x, None), None),
+                transform_right = lambda x: parse_value((None, x), default_value),
+                default_element = 0,
+                default_right = default_value
+            )
+            if key.endswith('+'):
+                key = key[:-1]
+                if key in result_dict:
+                    value = result_dict[key] + value
+            result_dict[key] = value
+    return result_dict
 # ******************************************************************************
 # ******************************************************************************
```

### Comparing `n0struct-0.2.98/n0struct/n0struct_date.py` & `n0struct-0.2.99/n0struct/n0struct_date.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_files.py` & `n0struct-0.2.99/n0struct/n0struct_files.py`

 * *Files 12% similar despite different names*

```diff
@@ -68,8 +68,20 @@
         if isinstance(output_buffer, str):
             output_buffer = output_buffer.encode(encoding)
         encoding = None
 
     with open(file_path, 'w'+mode, encoding=encoding) as out_filehandler:
         out_filehandler.write(output_buffer)
 # ******************************************************************************
+
+
+def unique_file_path(file_path: str, purpose: str = "") -> Path:
+    for i in range(1000):
+        unique_file_path = Path(str(file_path) + (f".{i:03}" if i else ""))
+        if not unique_file_path.exists():
+            return unique_file_path
+    else:
+        raise FileExistsError("Impossible to find unique name for {purpose}'{file_path}'")
+# ******************************************************************************
 # ******************************************************************************
+
+
```

### Comparing `n0struct-0.2.98/n0struct/n0struct_files_csv.py` & `n0struct-0.2.99/n0struct/n0struct_files_csv.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_files_fwf.py` & `n0struct-0.2.99/n0struct/n0struct_files_fwf.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_findall.py` & `n0struct-0.2.99/n0struct/n0struct_findall.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_git.py` & `n0struct-0.2.99/n0struct/n0struct_git.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_logging.py` & `n0struct-0.2.99/n0struct/n0struct_logging.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_mask.py` & `n0struct-0.2.99/n0struct/n0struct_mask.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_n0dict_.py` & `n0struct-0.2.99/n0struct/n0struct_n0dict_.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_n0dict__.py` & `n0struct-0.2.99/n0struct/n0struct_n0dict__.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_n0list_.py` & `n0struct-0.2.99/n0struct/n0struct_n0list_.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing
 from .n0struct_utils import n0eval
 from .n0struct_findall import findall as n0struct_findall__findall
 from .n0struct_findall import findfirst as n0struct_findall__findfirst
 from .n0struct_logging import n0pretty
+## from .n0struct_logging import n0debug, n0debug_calc
 # ******************************************************************************
 # ******************************************************************************
 class n0list_(list):
     def findall(self, xpath: str, raise_exception: bool = True):
         return n0struct_findall__findall(self, xpath, raise_exception)
     def findfirst(self, xpath: str, raise_exception: bool = True):
         return n0struct_findall__findfirst(self, xpath, raise_exception)
@@ -48,14 +49,24 @@
             try:
                 return super(n0list_, self).__getitem__(n0eval(xpath))
             except IndexError as ex:
                 if raise_exception:
                     raise ex
                 else:
                     return if_not_found
+            except TypeError as ex:
+                ## n0debug("self")
+                ## n0debug("xpath")
+                ## n0debug_calc(n0eval(xpath), "n0eval(xpath)")
+                print("*"*50)
+                print(f"{self=}")
+                print(f"{xpath=}")
+                print(f"{n0eval(xpath)=}")
+                print("*"*50)
+                raise ex
     # **************************************************************************
     # n0list_. get()
     # **************************************************************************
     def get(self, xpath: typing.Union[str, int], if_not_found = None):
         """
         Public function:
         return self[where1/where2/.../whereN]
```

### Comparing `n0struct-0.2.98/n0struct/n0struct_n0list_n0dict.py` & `n0struct-0.2.99/n0struct/n0struct_n0list_n0dict.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_random.py` & `n0struct-0.2.99/n0struct/n0struct_random.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_references.py` & `n0struct-0.2.99/n0struct/n0struct_references.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_transform_structure.py` & `n0struct-0.2.99/n0struct/n0struct_transform_structure.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_utils_compare.py` & `n0struct-0.2.99/n0struct/n0struct_utils_compare.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/n0struct_utils_find.py` & `n0struct-0.2.99/n0struct/n0struct_utils_find.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/test/test_n0struct.py` & `n0struct-0.2.99/n0struct/test/test_n0struct.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/test/test_n0struct2.py` & `n0struct-0.2.99/n0struct/test/test_n0struct2.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/test/test_n0struct3.py` & `n0struct-0.2.99/n0struct/test/test_n0struct3.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct/test/test_n0struct4.py` & `n0struct-0.2.99/n0struct/test/test_n0struct4.py`

 * *Files identical despite different names*

### Comparing `n0struct-0.2.98/n0struct.egg-info/PKG-INFO` & `n0struct-0.2.99/n0struct.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n0struct
-Version: 0.2.98
+Version: 0.2.99
 Summary: list/dict extensions allow to load/save/serialize/deserialize xml/json/csv/dsv/fwf files into python/from structures, compare them and work with them using xpath approach
 Home-page: https://github.com/pythonist552/n0struct/
 Author: pythonist552
 Author-email: pythonist552@gmail.com
 License: ASL
 Platform: any
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `n0struct-0.2.98/setup.py` & `n0struct-0.2.99/setup.py`

 * *Files identical despite different names*

