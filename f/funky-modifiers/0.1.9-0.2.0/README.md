# Comparing `tmp/funky_modifiers-0.1.9.tar.gz` & `tmp/funky_modifiers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funky_modifiers-0.1.9.tar", last modified: Thu May  9 23:49:34 2024, max compression
+gzip compressed data, was "funky_modifiers-0.2.0.tar", last modified: Sun May 19 19:50:40 2024, max compression
```

## Comparing `funky_modifiers-0.1.9.tar` & `funky_modifiers-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.138435 funky_modifiers-0.1.9/
--rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-05-09 23:49:34.137939 funky_modifiers-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.1.9/README.md
--rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.1.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 23:49:34.138435 funky_modifiers-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      711 2024-05-09 23:48:59.000000 funky_modifiers-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.103715 funky_modifiers-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.108179 funky_modifiers-0.1.9/src/funk_py/
--rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.1.9/src/funk_py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.112146 funky_modifiers-0.1.9/src/funk_py/modularity/
--rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.1.9/src/funk_py/modularity/__init__.py
--rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.1.9/src/funk_py/modularity/basic_structures.py
--rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.1.9/src/funk_py/modularity/bespoke_properties.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.115122 funky_modifiers-0.1.9/src/funk_py/modularity/decoration/
--rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.1.9/src/funk_py/modularity/decoration/__init__.py
--rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.1.9/src/funk_py/modularity/decoration/enum_modifiers.py
--rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.1.9/src/funk_py/modularity/decoration/init_modifiers.py
--rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.1.9/src/funk_py/modularity/decoration/transforming_list.py
--rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.1.9/src/funk_py/modularity/logging.py
--rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.1.9/src/funk_py/modularity/type_matching.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.118124 funky_modifiers-0.1.9/src/funk_py/sorting/
--rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.1.9/src/funk_py/sorting/__init__.py
--rw-rw-rw-   0        0        0    20021 2024-05-05 16:10:17.000000 funky_modifiers-0.1.9/src/funk_py/sorting/converters.py
--rw-rw-rw-   0        0        0    19628 2024-05-07 11:15:54.000000 funky_modifiers-0.1.9/src/funk_py/sorting/dict_manip.py
--rw-rw-rw-   0        0        0    18887 2024-05-09 23:48:08.000000 funky_modifiers-0.1.9/src/funk_py/sorting/pieces.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.123059 funky_modifiers-0.1.9/src/funk_py/super_dicts/
--rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.1.9/src/funk_py/super_dicts/__init__.py
--rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.1.9/src/funk_py/super_dicts/drop_none_dict.py
--rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.1.9/src/funk_py/super_dicts/list_dict.py
--rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.1.9/src/funk_py/super_dicts/windowed_list.py
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.137443 funky_modifiers-0.1.9/src/funky_modifiers.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-09 23:49:34.000000 funky_modifiers-0.1.9/src/funky_modifiers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-05-09 23:49:34.000000 funky_modifiers-0.1.9/src/funky_modifiers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 23:49:34.000000 funky_modifiers-0.1.9/src/funky_modifiers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-09 23:49:34.000000 funky_modifiers-0.1.9/src/funky_modifiers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-09 23:49:34.000000 funky_modifiers-0.1.9/src/funky_modifiers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 23:49:34.136451 funky_modifiers-0.1.9/test/
--rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.1.9/test/test_check_dict_equality.py
--rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.1.9/test/test_check_list_equality.py
--rw-rw-rw-   0        0        0    21911 2024-04-27 15:34:29.000000 funky_modifiers-0.1.9/test/test_convert_tuplish_dict.py
--rw-rw-rw-   0        0        0    15212 2024-05-05 16:22:23.000000 funky_modifiers-0.1.9/test/test_converters.py
--rw-rw-rw-   0        0        0     3127 2024-04-24 10:25:16.000000 funky_modifiers-0.1.9/test/test_converts_enums.py
--rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.1.9/test/test_drop_none_dict.py
--rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.1.9/test/test_function_hash_and_equality.py
--rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.1.9/test/test_logs_vars.py
--rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.1.9/test/test_obj.py
--rw-rw-rw-   0        0        0    68867 2024-05-05 18:36:38.000000 funky_modifiers-0.1.9/test/test_pick.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.080443 funky_modifiers-0.2.0/
+-rw-rw-rw-   0        0        0     1525 2024-02-25 05:24:52.000000 funky_modifiers-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       37 2024-05-05 20:43:12.000000 funky_modifiers-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-05-19 19:50:40.079945 funky_modifiers-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2024-05-05 19:24:08.000000 funky_modifiers-0.2.0/README.md
+-rw-rw-rw-   0        0        0       13 2024-05-05 21:32:06.000000 funky_modifiers-0.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 19:50:40.080443 funky_modifiers-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      711 2024-05-19 19:48:14.000000 funky_modifiers-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.043739 funky_modifiers-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.049193 funky_modifiers-0.2.0/src/funk_py/
+-rw-rw-rw-   0        0        0       50 2023-12-27 12:08:10.000000 funky_modifiers-0.2.0/src/funk_py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.053659 funky_modifiers-0.2.0/src/funk_py/modularity/
+-rw-rw-rw-   0        0        0        0 2023-12-26 12:23:31.000000 funky_modifiers-0.2.0/src/funk_py/modularity/__init__.py
+-rw-rw-rw-   0        0        0    39190 2024-05-05 15:25:24.000000 funky_modifiers-0.2.0/src/funk_py/modularity/basic_structures.py
+-rw-rw-rw-   0        0        0     4500 2024-05-03 11:21:07.000000 funky_modifiers-0.2.0/src/funk_py/modularity/bespoke_properties.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.057131 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/
+-rw-rw-rw-   0        0        0      496 2024-02-24 19:47:42.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/__init__.py
+-rw-rw-rw-   0        0        0     1260 2024-04-24 10:42:19.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/enum_modifiers.py
+-rw-rw-rw-   0        0        0     9073 2024-02-25 05:13:05.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/init_modifiers.py
+-rw-rw-rw-   0        0        0     2749 2023-12-26 12:23:31.000000 funky_modifiers-0.2.0/src/funk_py/modularity/decoration/transforming_list.py
+-rw-rw-rw-   0        0        0     6475 2024-02-25 05:13:05.000000 funky_modifiers-0.2.0/src/funk_py/modularity/logging.py
+-rw-rw-rw-   0        0        0    34949 2024-05-02 10:31:37.000000 funky_modifiers-0.2.0/src/funk_py/modularity/type_matching.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.060602 funky_modifiers-0.2.0/src/funk_py/sorting/
+-rw-rw-rw-   0        0        0        0 2024-04-07 16:23:56.000000 funky_modifiers-0.2.0/src/funk_py/sorting/__init__.py
+-rw-rw-rw-   0        0        0    20021 2024-05-05 16:10:17.000000 funky_modifiers-0.2.0/src/funk_py/sorting/converters.py
+-rw-rw-rw-   0        0        0    32960 2024-05-19 13:15:49.000000 funky_modifiers-0.2.0/src/funk_py/sorting/dict_manip.py
+-rw-rw-rw-   0        0        0    18891 2024-05-10 22:45:39.000000 funky_modifiers-0.2.0/src/funk_py/sorting/pieces.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.063578 funky_modifiers-0.2.0/src/funk_py/super_dicts/
+-rw-rw-rw-   0        0        0     2139 2024-05-05 18:39:34.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/__init__.py
+-rw-rw-rw-   0        0        0     8330 2024-03-03 18:51:02.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/drop_none_dict.py
+-rw-rw-rw-   0        0        0     8942 2024-03-03 17:19:44.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/list_dict.py
+-rw-rw-rw-   0        0        0     3583 2023-12-30 12:27:19.000000 funky_modifiers-0.2.0/src/funk_py/super_dicts/windowed_list.py
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.078954 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1285 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 19:50:40.000000 funky_modifiers-0.2.0/src/funky_modifiers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 19:50:40.078461 funky_modifiers-0.2.0/test/
+-rw-rw-rw-   0        0        0    21040 2024-05-03 11:33:03.000000 funky_modifiers-0.2.0/test/test_check_dict_equality.py
+-rw-rw-rw-   0        0        0    27490 2024-05-03 11:33:03.000000 funky_modifiers-0.2.0/test/test_check_list_equality.py
+-rw-rw-rw-   0        0        0    22476 2024-05-19 13:46:24.000000 funky_modifiers-0.2.0/test/test_convert_tuplish_dict.py
+-rw-rw-rw-   0        0        0    15212 2024-05-19 13:46:24.000000 funky_modifiers-0.2.0/test/test_converters.py
+-rw-rw-rw-   0        0        0     3672 2024-05-19 12:53:09.000000 funky_modifiers-0.2.0/test/test_converts_enums.py
+-rw-rw-rw-   0        0        0    10746 2024-05-19 13:19:52.000000 funky_modifiers-0.2.0/test/test_dict_builder.py
+-rw-rw-rw-   0        0        0    12426 2024-03-03 19:25:27.000000 funky_modifiers-0.2.0/test/test_drop_none_dict.py
+-rw-rw-rw-   0        0        0    26544 2024-03-03 19:25:27.000000 funky_modifiers-0.2.0/test/test_function_hash_and_equality.py
+-rw-rw-rw-   0        0        0    12013 2024-04-12 20:31:58.000000 funky_modifiers-0.2.0/test/test_logs_vars.py
+-rw-rw-rw-   0        0        0    35329 2024-05-02 11:24:45.000000 funky_modifiers-0.2.0/test/test_obj.py
+-rw-rw-rw-   0        0        0    68867 2024-05-19 13:46:24.000000 funky_modifiers-0.2.0/test/test_pick.py
```

### Comparing `funky_modifiers-0.1.9/LICENSE` & `funky_modifiers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/setup.py` & `funky_modifiers-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as fh:
     install_requires = fh.read()
 
 setup(
     name='funky_modifiers',
-    version='0.1.9',
+    version='0.2.0',
     description='A package containing tiny bits and bobs to remove boilerplate or just make things simpler.',
     url='https://github.com/Sparqzi/funk_py',
     author='Erich Kopp',
     license='BSD 3-Clause',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/basic_structures.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/basic_structures.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/bespoke_properties.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/bespoke_properties.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/decoration/enum_modifiers.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/decoration/enum_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/decoration/init_modifiers.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/decoration/init_modifiers.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/decoration/transforming_list.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/decoration/transforming_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/logging.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/logging.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/modularity/type_matching.py` & `funky_modifiers-0.2.0/src/funk_py/modularity/type_matching.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/sorting/converters.py` & `funky_modifiers-0.2.0/src/funk_py/sorting/converters.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/sorting/dict_manip.py` & `funky_modifiers-0.2.0/src/funk_py/sorting/dict_manip.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Generator, Optional, Union, Any, Callable, Dict
-
-from funk_py.modularity.logging import make_logger
+from copy import deepcopy
+from typing import Generator, Optional, Union, Any, Callable, Dict, Tuple, Iterable, Mapping, Type
 
+from funk_py.modularity.basic_structures import pass_
+from funk_py.modularity.logging import make_logger, logs_vars
 
 main_logger = make_logger('dict_manip', env_var='DICT_MANIP_LOG_LEVEL', default_level='warning')
 
 
 _skip_message = 'Skipped a key-val pair in convert_tuplish_dict '
 
 
@@ -156,49 +157,58 @@
 
 def _ctd_pair_search(data: Union[dict, list], pair_name, func: Callable, builder, *args):
     """_convert_tuplish_dict_pair_search"""
     for potential_pair in dive_to_dicts(data, pair_name):
         func(potential_pair[pair_name], *args, builder)
 
 
-def merge_tuplish_pair(pair: list, builder: dict):
+def merge_tuplish_pair(pair: list, builder: dict, unsafe: bool = False):
     """
     Merges a list representing a key-value pair into a dictionary builder.
 
     This function iterates over the elements of the input pair list, representing a key-value pair,
     and merges it into the given dictionary builder. The builder is progressively updated to
     construct a nested dictionary structure based on the keys in the pair list. It will construct
     paths that are missing on its own.
 
     :param pair: A list representing a key-value pair, where all items except the last represent a
         *path* of keys under which the last item is to be stored.
     :type pair: list
     :param builder: The dictionary to merge ``pair`` into.
     :type builder: dict
+    :param unsafe: Whether a failure to merge should actually raise an error. Defaults to ``False``.
+    :type unsafe: bool
 
     .. warning::
 
-        If the function encounters a key in the pair list that already exists in the builder and the
-        corresponding value is not a dictionary, but there are more keys involved in the path to the
-        value, it will not attempt to update the value or build the dictionary any deeper, but
-        instead will do nothing to ``builder``. It logs a message under the ``dict_manip`` logger at
-        the info level when this occurs. You can turn on this logger by setting the
-        ``DICT_MANIP_LOG_LEVEL`` environment variable to ``'info'``.
+        Default behavior is if the function encounters a key in the pair list that already exists in
+        the builder and the corresponding value is not a dictionary, but there are more keys
+        involved in the path to the value, it will not attempt to update the value or build the
+        dictionary any deeper, but instead will do nothing to ``builder``. It logs a message under
+        the ``dict_manip`` logger at the info level when this occurs. You can turn on this logger by
+        setting the ``DICT_MANIP_LOG_LEVEL`` environment variable to ``'info'``.
     """
     # Given this function is frequently called at the deepest point on a stack of calls, it is built
     # to NOT be recursive. This helps ensure stack limit is not exceeded.
     worker = builder
     for i in range(len(pair) - 1):
         if (t := pair[i]) in worker:
             if isinstance(worker[t], dict) and i < len(pair) - 2:
                 worker = worker[t]
 
+            elif i == len(pair) - 2:
+                worker[t] = pair[-1]
+                break
+
             else:
-                main_logger.info(f'Can\'t merge into dict correctly. Attempted to merge '
-                                 f'{repr(pair[i + 1:])} into {repr(worker[t])}.')
+                msg = (f'Can\'t merge into dict correctly. Attempted to merge '
+                       f'{repr(pair[i + 1:])} into {repr(worker[t])}.')
+                main_logger.info(msg)
+                if unsafe:
+                    raise ValueError(msg)
 
         else:
             if i < len(pair) - 2:
                 # Do not change to worker = worker[t] = {}, makes infinitely-nested list
                 # This is because the bytecode is compiled left-to-right for the objects assigned
                 # to.
                 worker[t] = worker = {}
@@ -433,11 +443,353 @@
     exist will simply be omitted.
     """
     return {key: data[key] for key in keys if key in data}
 
 
 def get_subset_values(data: dict, *keys) -> tuple:
     """
-    Retireves a subset values (based on ``keys``) from a dictionary in the format of a tuple. Any
+    Retrieves a subset values (based on ``keys``) from a dictionary in the format of a tuple. Any
     keys that do not exist will have ``None`` as their value.
     """
     return tuple(data.get(key, None) for key in keys)
+
+
+def tuples_to_dict(*pairs: Tuple[Any, Any], all_pairs: Iterable[Tuple[Any, Any]] = None) -> dict:
+    """Constructs a dictionary from provided tuples."""
+    builder = {}
+    if all_pairs is not None:
+        builder.update({k: v for k, v in all_pairs})
+
+    builder.update({k: v for k, v in pairs})
+    return builder
+
+
+def get_val_from_path(source: dict, *path: Any, default: Any = None, unsafe: bool = False) -> Any:
+    """
+    Follow a path through a dictionary to find the value at the end.
+
+    :param source: The dictionary to get a value from.
+    :param path: The paht of keys to follow to get to the desired value inside ``source``.
+    :param default: A default value to return if the path ends prematurely. Will be ignored if
+        unsafe is ``True``.
+    :param unsafe: Whether to raise an exception if the path ends early. Overrides ``default``.
+    :return: The value at the end of the desired path in ``source``, if it exists. Otherwise,
+        ``default``.
+    """
+    for key in path:
+        if key in source:
+            source = source[key]
+
+        elif unsafe:
+            raise KeyError(f'Path failed at {key}.')
+
+        else:
+            return default
+
+    return source
+
+
+@logs_vars(main_logger)
+def get_one_of_keys(source: dict, *keys: Union[Any, list], default: Any = None) -> Any:
+    """
+    Get the value at one of the keys (or key paths) specified in ``keys`` from ``source``. Will
+    return default if none of the keys/key paths exist in ``source``.
+
+    :param source: The source ``dict`` to get the value from.
+    :type source: dict
+    :param keys: The possible keys or key paths the sought value could be located at.
+    :type keys: Union[Any, list]
+    :param default: The default value to return if the target value cannot be found.
+    :type default: Any
+    :return: The target value, if it is found. Otherwise, ``default``.
+    """
+    for key in keys:
+        if isinstance(key, list):
+            diver = source
+            found = True
+            for k in key:
+                if k in diver:
+                    diver = diver[k]
+
+                else:
+                    found = False
+                    break
+
+            if found:
+                return diver
+
+        elif key in source:
+            return source[key]
+
+    return default
+
+
+class DictBuilder:
+    def __new__(cls, *args, clazz: Type = dict, **kwargs):
+        inst = super().__new__(cls)
+        inst.__class = clazz
+        return inst
+
+    def __init__(self, _map: Mapping = ..., *, clazz: Type = dict, **kwargs):
+        """
+        A builder for dictionaries that has a few helpful methods for merging in data from other
+        dictionaries.
+
+        :param _map: The ``Mapping`` to start the builder out with. Works like it does for ``dict``.
+        :type _map: Mapping
+        :param clazz: A ``dictionary class to inherit from. Used to make sure the builder is the
+            desired type of dictionary.
+        :type clazz: Type
+        :param kwargs: The ``kwargs`` to construct the starting builder with. Works like it does for
+            ``dict``.
+        """
+        if 'clazz' in kwargs:
+            del kwargs['clazz']
+
+        if _map is ...:
+            self.__builder = self.__class(**kwargs)
+
+        else:
+            self.__builder = self.__class(_map, **kwargs)
+
+    @staticmethod
+    def _check_dict(other: dict):
+        if not isinstance(other, dict):
+            raise TypeError('Invalid type for other.')
+
+    @staticmethod
+    def _pathify_as(_as: Union[Any, list], val: Any):
+        if isinstance(_as, list):
+            (path := list(_as)).append(val)
+
+        else:
+            path = _as, val
+
+        return path
+
+    @logs_vars(main_logger, start_message='Getting a value from another dictionary...',
+               start_message_level='info',
+               end_message='Finished attempt to get a value from another dictionary.',
+               end_message_level='info')
+    def pull_from_other(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
+                        transformer: Callable = pass_) -> 'DictBuilder':
+        """
+        Get a value from another dictionary at a given key, and insert it at the key specified in
+        ``_as``. Using this will raise an error if the key doesn't exist in ``other`` or if it
+        cannot safely be added to the ``DictBuilder``.
+
+        :param other: The dictionary to grab the key from.
+        :type other: dict
+        :param key: The key at which to find a value in ``other``.
+        :type key: Union[Any, list]
+        :param _as: The key at which to place the found value from ``other``.
+        :type _as: Union[Any, list]
+        :param transformer: A transformer that should be called on a value if found.
+        :type transformer: Callable
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_dict(other)
+
+        # Get the value.
+        if isinstance(key, list):
+            val = transformer(get_val_from_path(other, *key, unsafe=True))
+
+        else:
+            val = transformer(other[key])
+
+        path = self._pathify_as(_as, val)
+        merge_tuplish_pair(path, self.__builder, unsafe=True)
+
+        return self
+
+    @logs_vars(main_logger, start_message='Getting a value from another dictionary...',
+               start_message_level='info',
+               end_message='Finished attempt to get a value from another dictionary.',
+               end_message_level='info')
+    def get_from_other(self, other: dict, key: Union[Any, list], _as: Union[Any, list],
+                       transformer: Callable = pass_, default: Any = ...) -> 'DictBuilder':
+        """
+        Get a value from another dictionary at a given key, and insert it at the key specified in
+        ``_as``. If ``key`` cannot be found in other or ``the value cannot be added to this
+        ``DictBuilder``, then the value simply won't be added.
+
+        :param other: The dictionary to grab the key from.
+        :type other: dict
+        :param key: The key at which to find a value in ``other``.
+        :type key: Union[Any, list]
+        :param _as: The key at which to place the found value from ``other``.
+        :type _as: Union[Any, list]
+        :param transformer: A transformer that should be called on a value if found.
+        :type transformer: Callable
+        :param default: The default value to use if a value cannot be found. If omitted, and the
+            value is not found, then the value simply won't be added.
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_dict(other)
+
+        # Get the value.
+        if isinstance(key, list):
+            val = get_val_from_path(other, *key, default=...)
+
+        else:
+            val = other.get(key, ...)
+
+        if val is ...:
+            if default is ...:
+                return self
+
+            val = default
+
+        else:
+            val = transformer(val)
+
+        path = self._pathify_as(_as, val)
+        merge_tuplish_pair(path, self.__builder)
+
+        return self
+
+    @logs_vars(main_logger, start_message='Updating from another dictionary...',
+               start_message_level='info',
+               end_message='Finished attempt to update from another dictionary.',
+               end_message_level='info')
+    def update_from_other(self, other: dict, key: Union[Any, None, list] = None,
+                          _as: Union[Any, None, list] = None, transformer: Callable = pass_,
+                          unsafe: bool = False) -> 'DictBuilder':
+        """
+        Update this ``DictBuilder`` from another dict.
+
+        :param other: The dictionary to update with.
+        :type other: dict
+        :param key: The key at which the source dictionary should be in ``other``. If not specified
+            ``other`` will be used as-is.
+        :type key: Union[Any, None, list]
+        :param _as: The key at which to place update with the found value from ``other``. If not
+            specified, will simply update the entire ``DictBuilder``.
+        :type _as: Union[Any, None, list]
+        :param transformer: A transformer that should be called on the value being used to update
+            the ``DictBuilder``.
+        :type transformer: Callable
+        :param unsafe: Whether an error should be raised if the desired operation cannot be
+            completed.
+        :type unsafe: bool
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        self._check_dict(other)
+        # Get the value.
+        if key is not None:
+            if isinstance(key, list):
+                val = get_val_from_path(other, *key, unsafe=unsafe, default=...)
+
+            elif unsafe:
+                val = other[key]
+
+            else:
+                val = other.get(key, ...)
+
+        else:
+            val = other
+
+        if val is ...:
+            return self
+
+        if not isinstance(val, dict):
+            if unsafe:
+                msg = 'Cannot merge a dict to a value.'
+                main_logger.error(msg)
+                raise ValueError(msg)
+
+            return self
+
+        worker = self.__builder
+        worker = self._update_seek(_as, worker, unsafe)
+        worker.update(transformer(val))
+
+        return self
+
+    def _update_seek(self, _as: Any, worker: dict, unsafe: bool):
+        if _as is not None:
+            if isinstance(_as, list):
+                for val in _as:
+                    worker = self._update_seek_next(val, worker, unsafe)
+
+            else:
+                worker = self._update_seek_next(_as, worker, unsafe)
+
+        return worker
+
+    def _update_seek_next(self, val: Any, worker: dict, unsafe: bool):
+        if val in worker:
+            if isinstance(worker[val], dict):
+                worker = worker[val]
+
+            elif unsafe:
+                msg = 'An invalid path was encountered'
+                main_logger.error(msg + ' while updating from another dictionary.')
+                raise ValueError(msg + '.')
+
+            else:
+                worker[val] = worker = self.clazz()
+
+        else:
+            worker[val] = worker = self.clazz()
+
+        return worker
+
+    @logs_vars(main_logger, start_message='Getting one of the keys from another dictionary...',
+               start_message_level='info',
+               end_message='Finished attempt to get one of the keys from another dictionary.',
+               end_message_level='info')
+    def get_one_of_keys_from_other(self, other: dict, _as: Union[Any, list],
+                                   *keys: Union[Any, list], transformer: Callable = pass_,
+                                   default: Any = ...) -> 'DictBuilder':
+        """
+        Gets the value at one of the keys (or key paths) specified in ``keys`` from ``other`` and
+        adds it at ``_as`` within the ``DictBuilder``.
+
+        :param other: The source ``dict`` to get the value from.
+        :type other: dict
+        :param _as: The key or key path to add a found value at.
+        :type _as: Union[Any, list]
+        :param keys: The possible keys or key paths the sought value could be located at.
+        :type keys: Union[Any, list]
+        :param default: The default value to return if the target value cannot be found. If this is
+            not specified, then should no value be found, a value simply won't be added.
+        :type default: Any
+        :return: The current ``DictBuilder`` for chaining.
+        """
+        val = get_one_of_keys(other, *keys, ...)
+        if val is ...:
+            if default is ...:
+                return self
+
+            val = default
+
+        else:
+            val = transformer(val)
+
+        path = self._pathify_as(_as, val)
+        merge_tuplish_pair(path, self.__builder)
+
+        return self
+
+    @logs_vars(main_logger, start_message='Updating dictionary...', start_message_level='info',
+               end_message='Finished updating.', end_message_level='info')
+    def update(self, _map: Mapping = ..., **kwargs) -> 'DictBuilder':
+        self.__builder.update(_map, **kwargs)
+        return self
+
+    def __delitem__(self, key) -> 'DictBuilder':
+        del self.__builder[key]
+        return self
+
+    def __getitem__(self, key):
+        return self.__builder[key]
+
+    def get(self, key: Any, default: Any = None):
+        return self.__builder.get(key, default)
+
+    def __setitem__(self, key, value) -> 'DictBuilder':
+        self.__builder[key] = value
+        return self
+
+    def build(self) -> dict:
+        return deepcopy(self.__builder)
```

### Comparing `funky_modifiers-0.1.9/src/funk_py/sorting/pieces.py` & `funky_modifiers-0.2.0/src/funk_py/sorting/pieces.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         PickInstruction.TUPLE_DICT: _parse_and_execute_tuplish,
     }
 
     if _type in switch:
         return switch[_type](data)
 
     elif _type in arg_switch:
-        return switch[_type](data, args)
+        return arg_switch[_type](data, args)
 
     raise ValueError('Invalid type specified.')
 
 
 def _parse_and_execute_tuplish(data: Union[dict, list], args: list) -> dict:
     if len(args):
         args = args[0]
```

### Comparing `funky_modifiers-0.1.9/src/funk_py/super_dicts/__init__.py` & `funky_modifiers-0.2.0/src/funk_py/super_dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/super_dicts/drop_none_dict.py` & `funky_modifiers-0.2.0/src/funk_py/super_dicts/drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/super_dicts/list_dict.py` & `funky_modifiers-0.2.0/src/funk_py/super_dicts/list_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funk_py/super_dicts/windowed_list.py` & `funky_modifiers-0.2.0/src/funk_py/super_dicts/windowed_list.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/src/funky_modifiers.egg-info/SOURCES.txt` & `funky_modifiers-0.2.0/src/funky_modifiers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,13 @@
 src/funky_modifiers.egg-info/requires.txt
 src/funky_modifiers.egg-info/top_level.txt
 test/test_check_dict_equality.py
 test/test_check_list_equality.py
 test/test_convert_tuplish_dict.py
 test/test_converters.py
 test/test_converts_enums.py
+test/test_dict_builder.py
 test/test_drop_none_dict.py
 test/test_function_hash_and_equality.py
 test/test_logs_vars.py
 test/test_obj.py
 test/test_pick.py
```

### Comparing `funky_modifiers-0.1.9/test/test_check_dict_equality.py` & `funky_modifiers-0.2.0/test/test_check_dict_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/test/test_check_list_equality.py` & `funky_modifiers-0.2.0/test/test_check_list_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/test/test_convert_tuplish_dict.py` & `funky_modifiers-0.2.0/test/test_convert_tuplish_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 from dataclasses import dataclass
 from typing import Union
 
 import pytest
 
+from t_support import cov, cov_counter
 from funk_py.modularity.basic_structures import pass_
 from funk_py.sorting.pieces import convert_tuplish_dict
 
 
+# The following manages whether the generated coverage instance from t_support should report. This
+# method of coverage is used so that coverage can be turned off to not interfere in timed tests.
+@pytest.fixture(scope='session', autouse=True)
+def c():
+    cov_counter.value += 1
+
+    yield cov
+
+    cov_counter.value -= 1
+
+    # We don't want to report till all test modules are completed...
+    if not cov_counter.value:
+        cov.stop()
+        cov.save()
+        cov.html_report()
+
+
+NEWLINE = '\n'
+
+
 @dataclass
 class TuplishDictDef:
     data: Union[dict, list]
     result: dict
     pair_name: str = None
     key_name: str = None
     val_name: str = None
```

### Comparing `funky_modifiers-0.1.9/test/test_converters.py` & `funky_modifiers-0.2.0/test/test_converters.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 from xml.etree import ElementTree as ET
 
 import pytest
 
-from funk_py.modularity.basic_structures import Speed
 from t_support import too_slow_func_two_arg_updated, too_slow_func_one_arg, cov, cov_counter
+from funk_py.modularity.basic_structures import Speed
 from funk_py.sorting.converters import csv_to_json, xml_to_json, wonky_json_to_json, jsonl_to_json
 
 
 # The following manages whether the generated coverage instance from t_support should report. This
 # method of coverage is used so that coverage can be turned off to not interfere in timed tests.
 @pytest.fixture(scope='session', autouse=True)
 def c():
```

### Comparing `funky_modifiers-0.1.9/test/test_converts_enums.py` & `funky_modifiers-0.2.0/test/test_converts_enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 from enum import Enum, IntEnum
 
 import pytest
 
+from t_support import cov, cov_counter
 from funk_py.modularity.decoration.enum_modifiers import converts_enums
 
 
+# The following manages whether the generated coverage instance from t_support should report. This
+# method of coverage is used so that coverage can be turned off to not interfere in timed tests.
+@pytest.fixture(scope='session', autouse=True)
+def c():
+    cov_counter.value += 1
+
+    yield cov
+
+    cov_counter.value -= 1
+
+    # We don't want to report till all test modules are completed...
+    if not cov_counter.value:
+        cov.stop()
+        cov.save()
+        cov.html_report()
+
+
 LOREM = 'lorem'
 
 
 class TestEnum:
     class TEnum(Enum):
         HORSE = 1
         LLAMA = 'llama'
```

### Comparing `funky_modifiers-0.1.9/test/test_drop_none_dict.py` & `funky_modifiers-0.2.0/test/test_drop_none_dict.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/test/test_function_hash_and_equality.py` & `funky_modifiers-0.2.0/test/test_function_hash_and_equality.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/test/test_logs_vars.py` & `funky_modifiers-0.2.0/test/test_logs_vars.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/test/test_obj.py` & `funky_modifiers-0.2.0/test/test_obj.py`

 * *Files identical despite different names*

### Comparing `funky_modifiers-0.1.9/test/test_pick.py` & `funky_modifiers-0.2.0/test/test_pick.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import io
 import json
 from typing import List, Any, Union, Tuple, Dict, Optional, Callable
 import yaml
 
 import pytest
 
+from t_support import too_slow_func_one_arg, cov, cov_counter
 from funk_py.modularity.basic_structures import pass_, Speed
 from funk_py.sorting.dict_manip import align_to_list, nest_under_keys
-from t_support import too_slow_func_one_arg, cov, cov_counter
 from funk_py.sorting.pieces import pick, PickType
 from funk_py.sorting.converters import json_to_xml, json_to_csv, json_to_jsonl, xml_to_json
 
 
 # The following manages whether the generated coverage instance from t_support should report. This
 # method of coverage is used so that coverage can be turned off to not interfere in timed tests.
 @pytest.fixture(scope='session', autouse=True)
```

