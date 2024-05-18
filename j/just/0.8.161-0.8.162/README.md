# Comparing `tmp/just-0.8.161.tar.gz` & `tmp/just-0.8.162.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just-0.8.161.tar", last modified: Sun Jun 18 19:52:09 2023, max compression
+gzip compressed data, was "just-0.8.162.tar", last modified: Sat May 18 23:24:43 2024, max compression
```

## Comparing `just-0.8.161.tar` & `just-0.8.162.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 19:52:09.963469 just-0.8.161/
--rw-r--r--   0 pascal    (1000) pascal    (1000)      148 2019-10-30 12:22:05.000000 just-0.8.161/.coveragerc
--rw-r--r--   0 pascal    (1000) pascal    (1000)      189 2019-10-30 12:22:05.000000 just-0.8.161/.gitignore
--rw-r--r--   0 pascal    (1000) pascal    (1000)      195 2019-10-30 12:22:05.000000 just-0.8.161/.travis.yml
--rw-r--r--   0 pascal    (1000) pascal    (1000)    34519 2019-10-30 12:22:05.000000 just-0.8.161/LICENSE
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2023-06-18 19:52:09.963469 just-0.8.161/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2791 2021-02-24 22:23:55.000000 just-0.8.161/README.md
--rw-r--r--   0 pascal    (1000) pascal    (1000)       60 2019-10-30 12:22:05.000000 just-0.8.161/README.rst
--rw-r--r--   0 pascal    (1000) pascal    (1000)      192 2019-10-30 12:22:05.000000 just-0.8.161/conftest.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      973 2022-12-11 15:47:37.000000 just-0.8.161/deploy.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 19:52:09.963469 just-0.8.161/just/
--rw-r--r--   0 pascal    (1000) pascal    (1000)      802 2023-06-18 19:52:09.000000 just-0.8.161/just/__init__.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      510 2019-10-31 14:56:25.000000 just-0.8.161/just/bytes.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      323 2020-05-07 22:19:36.000000 just-0.8.161/just/dir.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      240 2022-10-12 23:24:09.000000 just-0.8.161/just/dt.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     6707 2022-10-11 01:42:38.000000 just-0.8.161/just/forcedip.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      422 2020-09-14 22:28:41.000000 just-0.8.161/just/jpath.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2860 2023-06-18 19:41:09.000000 just-0.8.161/just/json_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      631 2019-10-30 12:22:05.000000 just-0.8.161/just/log.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      313 2019-10-30 12:22:05.000000 just-0.8.161/just/newl.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     4247 2023-03-19 11:38:12.000000 just-0.8.161/just/path_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2565 2023-01-24 21:15:23.000000 just-0.8.161/just/pattern.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      183 2019-10-30 12:22:05.000000 just-0.8.161/just/pickle_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     6591 2023-06-18 16:50:00.000000 just-0.8.161/just/read_write.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)    11536 2023-06-14 23:33:21.000000 just-0.8.161/just/requests_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2617 2022-10-11 02:05:39.000000 just-0.8.161/just/source_ip.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      177 2022-10-31 11:24:28.000000 just-0.8.161/just/toml_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      706 2020-01-15 22:53:45.000000 just-0.8.161/just/txt.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      198 2021-02-06 15:54:20.000000 just-0.8.161/just/yaml_.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      693 2021-04-17 11:52:08.000000 just-0.8.161/just/zstd_.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 19:52:09.963469 just-0.8.161/just.egg-info/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2023-06-18 19:52:09.000000 just-0.8.161/just.egg-info/PKG-INFO
--rw-r--r--   0 pascal    (1000) pascal    (1000)      651 2023-06-18 19:52:09.000000 just-0.8.161/just.egg-info/SOURCES.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2023-06-18 19:52:09.000000 just-0.8.161/just.egg-info/dependency_links.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)       45 2023-06-18 19:52:09.000000 just-0.8.161/just.egg-info/entry_points.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2019-10-30 12:22:52.000000 just-0.8.161/just.egg-info/not-zip-safe
--rw-r--r--   0 pascal    (1000) pascal    (1000)       59 2023-06-18 19:52:09.000000 just-0.8.161/just.egg-info/requires.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)        5 2023-06-18 19:52:09.000000 just-0.8.161/just.egg-info/top_level.txt
--rw-r--r--   0 pascal    (1000) pascal    (1000)       97 2023-06-18 19:52:09.963469 just-0.8.161/setup.cfg
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1683 2023-06-18 19:52:09.000000 just-0.8.161/setup.py
-drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2023-06-18 19:52:09.963469 just-0.8.161/tests/
--rw-r--r--   0 pascal    (1000) pascal    (1000)     2748 2021-03-18 22:21:23.000000 just-0.8.161/tests/test_files.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      196 2019-10-30 12:22:05.000000 just-0.8.161/tests/test_jpath.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)     1041 2021-03-18 22:22:11.000000 just-0.8.161/tests/test_requests.py
--rw-r--r--   0 pascal    (1000) pascal    (1000)      358 2021-02-06 15:52:11.000000 just-0.8.161/tox.ini
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2024-05-18 23:24:43.473531 just-0.8.162/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      148 2019-10-30 12:22:05.000000 just-0.8.162/.coveragerc
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      189 2019-10-30 12:22:05.000000 just-0.8.162/.gitignore
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      195 2019-10-30 12:22:05.000000 just-0.8.162/.travis.yml
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    34519 2019-10-30 12:22:05.000000 just-0.8.162/LICENSE
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2024-05-18 23:24:43.473531 just-0.8.162/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2791 2021-02-24 22:23:55.000000 just-0.8.162/README.md
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       60 2019-10-30 12:22:05.000000 just-0.8.162/README.rst
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      192 2019-10-30 12:22:05.000000 just-0.8.162/conftest.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      973 2022-12-11 15:47:37.000000 just-0.8.162/deploy.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2024-05-18 23:24:43.470198 just-0.8.162/just/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      834 2024-05-18 23:24:41.000000 just-0.8.162/just/__init__.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      510 2019-10-31 14:56:25.000000 just-0.8.162/just/bytes.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      131 2023-11-09 11:16:16.000000 just-0.8.162/just/date.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      323 2020-05-07 22:19:36.000000 just-0.8.162/just/dir.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      240 2022-10-12 23:24:09.000000 just-0.8.162/just/dt.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     6707 2022-10-11 01:42:38.000000 just-0.8.162/just/forcedip.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      422 2020-09-14 22:28:41.000000 just-0.8.162/just/jpath.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2860 2023-06-18 19:41:09.000000 just-0.8.162/just/json_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      631 2019-10-30 12:22:05.000000 just-0.8.162/just/log.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      313 2019-10-30 12:22:05.000000 just-0.8.162/just/newl.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     4389 2024-05-01 22:29:15.000000 just-0.8.162/just/path_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2740 2024-04-11 15:47:27.000000 just-0.8.162/just/pattern.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      183 2019-10-30 12:22:05.000000 just-0.8.162/just/pickle_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     6591 2023-06-18 16:50:00.000000 just-0.8.162/just/read_write.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)    11715 2024-05-18 23:23:54.000000 just-0.8.162/just/requests_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2617 2022-10-11 02:05:39.000000 just-0.8.162/just/source_ip.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      177 2022-10-31 11:24:28.000000 just-0.8.162/just/toml_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      706 2020-01-15 22:53:45.000000 just-0.8.162/just/txt.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      198 2021-02-06 15:54:20.000000 just-0.8.162/just/yaml_.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      693 2021-04-17 11:52:08.000000 just-0.8.162/just/zstd_.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2024-05-18 23:24:43.470198 just-0.8.162/just.egg-info/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1134 2024-05-18 23:24:43.000000 just-0.8.162/just.egg-info/PKG-INFO
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      664 2024-05-18 23:24:43.000000 just-0.8.162/just.egg-info/SOURCES.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2024-05-18 23:24:43.000000 just-0.8.162/just.egg-info/dependency_links.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       45 2024-05-18 23:24:43.000000 just-0.8.162/just.egg-info/entry_points.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        1 2019-10-30 12:22:52.000000 just-0.8.162/just.egg-info/not-zip-safe
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       59 2024-05-18 23:24:43.000000 just-0.8.162/just.egg-info/requires.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)        5 2024-05-18 23:24:43.000000 just-0.8.162/just.egg-info/top_level.txt
+-rw-r--r--   0 pascal    (1000) pascal    (1000)       97 2024-05-18 23:24:43.473531 just-0.8.162/setup.cfg
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1683 2024-05-18 23:24:41.000000 just-0.8.162/setup.py
+drwxr-xr-x   0 pascal    (1000) pascal    (1000)        0 2024-05-18 23:24:43.473531 just-0.8.162/tests/
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     2748 2021-03-18 22:21:23.000000 just-0.8.162/tests/test_files.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      196 2019-10-30 12:22:05.000000 just-0.8.162/tests/test_jpath.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)     1041 2021-03-18 22:22:11.000000 just-0.8.162/tests/test_requests.py
+-rw-r--r--   0 pascal    (1000) pascal    (1000)      358 2021-02-06 15:52:11.000000 just-0.8.162/tox.ini
```

### Comparing `just-0.8.161/LICENSE` & `just-0.8.162/LICENSE`

 * *Files identical despite different names*

### Comparing `just-0.8.161/PKG-INFO` & `just-0.8.162/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: just
-Version: 0.8.161
+Version: 0.8.162
 Summary: Automatically just read and write files based on extension.
 Home-page: https://github.com/kootenpv/just
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: any
```

### Comparing `just-0.8.161/README.md` & `just-0.8.162/README.md`

 * *Files identical despite different names*

### Comparing `just-0.8.161/deploy.py` & `just-0.8.162/deploy.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/__init__.py` & `just-0.8.162/just/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     glob,
     remove,
     mkdir,
     most_recent,
 )
 from just.read_write import *
 from just.requests_ import request, request_tree, get, get_tree, post, post_tree, save_session
+from just.date import yesterday
 from just.dir import mkdir
 from just.log import log
 from just.jpath import json_extract, jpath
 from just.pattern import Pattern
 
 # In [19]: with open("fuck.xz", "wb") as f: f.write(lzma.compress(html.encode()))
 
 # In [20]: with lzma.open("fuck.xz") as f: hh=f.read()
 
 __project__ = "just"
-__version__ = "0.8.161"
+__version__ = "0.8.162"
```

### Comparing `just-0.8.161/just/forcedip.py` & `just-0.8.162/just/forcedip.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/json_.py` & `just-0.8.162/just/json_.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/log.py` & `just-0.8.162/just/log.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/path_.py` & `just-0.8.162/just/path_.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
+import errno
+import functools
 import inspect
 import os
 import re
+
 import glob2
-import errno
-import functools
 
 __cached_just_path = None
 
 
 def glob(path, sort_reverse=False):
     res = re.findall("([$][A-Z_]+)", path)
     for x in res:
         path = path.replace(x, os.environ[x[1:]])
     path = make_path(path)
-    return sorted(glob2.glob(path), reverse=sort_reverse)
+    output = glob2.glob(path)
+    if sort_reverse is not None:
+        output = sorted(output, reverse=sort_reverse)
+    return output
 
 
 def get_just_env_path():
     return os.environ.get("JUST_PATH")
 
 
 def find_just_path(base=None, max_depth=5):
@@ -51,28 +55,28 @@
     __cached_just_path = just_path
     return just_path
 
 
 @functools.lru_cache(maxsize=1_000_000)
 def make_path(filename):
     just_path = get_just_path()
-    if not isinstance(filename, (str, bytes)):
+    if not isinstance(filename, str | bytes):
         filename = filename.name.encode("utf8").decode()
     filename = filename.replace("file://", "")
     path = os.path.join(just_path, os.path.expanduser(filename))
     if path.endswith("."):
         path = path[:-1]
     return path
 
 
 def exists(fname):
     return os.path.isfile(make_path(fname))
 
 
-def rename(src, dest, no_exist=None):
+def rename(src, dest, no_exist=None) -> bool:
     src = make_path(src)
     dest = make_path(dest)
     if not dest.endswith("/"):
         *dest_folder_parts, filename = dest.split("/")
         dest_folder = "/".join(dest_folder_parts)
         if not os.path.exists(dest_folder) and "." in filename:
             os.makedirs(dest_folder)
@@ -80,15 +84,15 @@
         return False
     os.rename(src, dest)
     return True
 
 
 def _as_glob(dir_name, recursive):
     dir_name = make_path(dir_name)
-    if not "*" in dir_name:
+    if "*" not in dir_name:
         if dir_name.endswith("/"):
             dir_name += "*"
         else:
             dir_name += "/*"
         if recursive:
             dir_name += "*"
     return dir_name
@@ -98,47 +102,50 @@
     dir_name = _as_glob(dir_name, recursive)
     if no_dirs:
         return [x for x in glob(dir_name) if not os.path.isdir(x)]
     else:
         return glob(dir_name)
 
 
-def mkdir(path, mode=0o777):
+def mkdir(path, mode=0o777) -> None:
     path = make_path(path)
     try:
         os.makedirs(path, mode)
     # Python >2.5
     except OSError as exc:  # pragma: no cover
         if exc.errno == errno.EEXIST and os.path.isdir(path):
             pass
         else:
             raise
 
 
 def remove(file_path, no_exist=False, allow_recursive=False):
-    if isinstance(file_path, (tuple, list)):
+    if isinstance(file_path, tuple | list):
         file_path = os.path.join(*file_path)
     if "*" in file_path:
         if not allow_recursive:
-            raise IOError("Cannot remove wildcard unless allow_recursive=True")
+            msg = "Cannot remove wildcard unless allow_recursive=True"
+            raise OSError(msg)
         paths = glob(file_path)
         for fn in sorted(paths, key=lambda x: -len(x)):
             os.remove(fn)
         return bool(paths)
     file_path = make_path(file_path)
     if os.path.isfile(file_path):
         os.remove(file_path)
         return True
     if os.path.isdir(file_path):
         if allow_recursive:
             shutil.rmtree(file_path)
             return True
         else:
-            raise IOError("Cannot remove directory unless allow_recursive=True")
+            msg = "Cannot remove directory unless allow_recursive=True"
+            raise OSError(msg)
     # if there is a default value, return that if no file/dir found when attempting to remove
     if no_exist is not None:
         return no_exist
-    raise IOError("File '{}' does not exist.".format(file_path))
+    msg = f"File '{file_path}' does not exist."
+    raise OSError(msg)
 
 
 def most_recent(file_path):
     return max(glob(file_path), key=os.path.getctime)
```

### Comparing `just-0.8.161/just/pattern.py` & `just-0.8.162/just/pattern.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from ciso8601 import parse_datetime as isoparse
 from datetime import datetime
-from just import iread
+
+from just import glob, iread
 
 
 def parse_specials(special_str):  # -> name, cast
     if not special_str:
         return "", "str"
     if "@" not in special_str:
         return special_str, ""
@@ -13,21 +13,20 @@
 
 
 def iso(x):
     return datetime.fromisoformat(x.replace(",", ".").replace("Z", "+00:00"))
 
 
 def convert_str(format_str):
-    r = ""
+    format_str = re.sub(" +", " ", format_str)
+    rr = ""
     on = False
-    specials = []
     types = []
     tmp = ""
     lenm = len(format_str)
-    last = -1
     captured_names = []
     for i, x in enumerate(format_str):
         if x == "}":
             on = False
             # fw = False
             name, cast = parse_specials(tmp)
             capture = bool(name)
@@ -38,32 +37,32 @@
                 pat = ".+"
             else:
                 pat = f"[^{format_str[i+1]}]+"
             if capture:
                 pat = f"({pat})"
                 captured_names.append(name)
                 types.append(tp)
-            r += pat
+            rr += pat
             tmp = ""
-            last = len(r)
+            len(rr)
         elif x == "{":
             on = True
+        elif not on:
+            rr += re.escape(x)
         else:
-            if not on:
-                r += re.escape(x)
-            else:
-                tmp += x
-    return r, types, captured_names
+            tmp += x
+    rr = rr.replace("\\ ", "\\ *")
+    return rr, types, captured_names
 
 
 NUMERIC = {int, float}
 
 
 class Pattern:
-    def __init__(self, format_str):
+    def __init__(self, format_str) -> None:
         self.format_str = format_str
         self.pattern, self.types, self.names = convert_str(format_str)
         if len(self.types) == 1:
             self.type = self.types[0]
             self.find = self.finder_one
         else:
             self.find = self.finder_multi
@@ -76,17 +75,21 @@
             return None
         return self.type(res.groups()[0].strip())
 
     def finder_multi(self, line):
         res = self.r.search(line)
         if not res:
             return [None] * self.num_captures_vars
-        return [tp(x.strip()) for name, tp, x in zip(self.names, self.types, res.groups()) if name]
+        return [tp(x.strip()) for name, tp, x in zip(self.names, self.types, res.groups(), strict=False) if name]
 
     def find_dict(self, line):
         res = self.finder_multi(line)
         if res[0] is None:
             return None
-        return {k: v for k, v in zip(self.names, res) if isinstance(k, int) or not k.startswith("_") and k}
+        return {
+            k: v for k, v in zip(self.names, res, strict=False) if isinstance(k, int) or not k.startswith("_") and k
+        }
 
     def stream(self, fname):
+        if "*" in fname:
+            return sum([[res for x in iread(fname) if (res := self.find_dict(x))] for fname in glob(fname)], [])
         return [res for x in iread(fname) if (res := self.find_dict(x))]
```

### Comparing `just-0.8.161/just/read_write.py` & `just-0.8.162/just/read_write.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/requests_.py` & `just-0.8.162/just/requests_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
+import hashlib
 import os
 import time
 import warnings
-import hashlib
 from collections import defaultdict
 from urllib.parse import urlparse
 
-from just.dir import mkdir
-from just.path_ import exists, glob, make_path, remove, rename
-from just.read_write import write, read
-
+from just.path_ import exists, glob, make_path, remove
+from just.read_write import read, write
 
 session = None
 PER_FOLDER = 3000
-BINARY_EXTENSIONS = {"jpg", "png", "jpeg", "png"}
+BINARY_EXTENSIONS = {"jpg", "png", "jpeg"}
 
 caches = {}
 timers = {}
 sessions = {}
 last_cache_fname = {}
 
 obj_counts = defaultdict(int)
@@ -54,15 +52,15 @@
                 count = 0
         except FileNotFoundError:
             count = 0
         obj_counts[(domain, obj_type)] = count
     return obj_counts[(domain, obj_type)]
 
 
-def get_cache_file_name(domain, request_info, compression=".gz"):
+def get_cache_file_name(domain, request_info, compression=".gz") -> str:
     from preconvert.output import json
 
     key = json.dumps(request_info)
     m = hashlib.md5()
     m.update(key.encode("utf8"))
     md5 = m.hexdigest()
     dir_name, fname = md5[:3], md5[3:]
@@ -80,15 +78,15 @@
         else:
             obj_type, fname = "", cache_key
         if obj_type:
             obj_type = "/" + obj_type
     return obj_type, fname
 
 
-def get_cache_file_name_str(domain, cache_key, compression=".gz"):
+def get_cache_file_name_str(domain, cache_key, compression=".gz") -> str:
     obj_type, fname = get_obj_type(cache_key)
     initial_part = f"~/.just_requests/{domain}{obj_type}"
     partition = update_obj_count(domain, initial_part, obj_type) // PER_FOLDER
     if not compression:
         compression = ""
     return f"{initial_part}/{partition}/{fname}.json{compression}"
 
@@ -146,35 +144,35 @@
 def _retry(
     method,
     max_retries,
     delay_base,
     raw,
     caching,
     cache_compression,
+    cache_ttl,
     sleep_time,
     reuse_session,
     local_address,
     remote_ip,
     refresh_session_on_error,
     kwargs,
 ):
-    import requests
-    from requests import RequestException, Session
+    from requests import RequestException
     from requests.utils import cookiejar_from_dict
 
     tries = 0
     url = kwargs["url"]
     domain_name = get_domain(url)
 
     use_cache, *request_info = caching
 
-    cache_file_name = get_cache_file_name(domain_name, request_info, cache_compression)
+    cache_file_name = os.path.expanduser(get_cache_file_name(domain_name, request_info, cache_compression))
 
     if exists(cache_file_name):
-        if use_cache:
+        if use_cache and (not cache_ttl or time.time() < cache_ttl + os.path.getmtime(cache_file_name)):
             last_cache_fname[domain_name] = cache_file_name
             return read(cache_file_name)["resp"]
         if use_cache is None:
             use_cache = True
         remove(cache_file_name)
 
     if "timeout" not in kwargs:
@@ -210,23 +208,22 @@
             break
         except RequestException as e:
             print("just.requests_", kwargs["url"], "attempt", tries, str(e))
             if tries == max_retries:
                 err = ""
                 r = None
                 break
-            else:
-                if refresh_session_on_error:
-                    request_fn = get_session_method(reuse_session, session_key, remote_ip, method, kwargs["url"])
+            elif refresh_session_on_error:
+                request_fn = get_session_method(reuse_session, session_key, remote_ip, method, kwargs["url"])
             tries += 1
             time.sleep(delay_base**tries)
 
     timers[session_key] = time.time()
 
-    file_extension = url.split(".")[-1]
+    url.split(".")[-1]
     # result handling
     if err is None or err == "":
         text = r.text[:500] if r is not None else ""
         if len(text) == 500:
             text += "..."
         code = r.status_code if r is not None else None
         print("ERR", code, url, text)
@@ -264,14 +261,15 @@
     url,
     params=None,
     max_retries=2,
     delay_base=3,
     raw=False,
     use_cache=False,
     cache_compression=".gz",
+    cache_ttl=0,
     sleep_time=None,
     fname=None,
     reuse_session=True,
     local_address=None,
     remote_ip=None,
     refresh_session_on_error=False,
     user_agent=USER_AGENT,
@@ -291,14 +289,15 @@
     result = _retry(
         "get",
         max_retries,
         delay_base,
         raw,
         caching,
         cache_compression,
+        cache_ttl,
         sleep_time,
         reuse_session,
         local_address,
         remote_ip,
         refresh_session_on_error,
         kwargs,
     )
@@ -308,15 +307,15 @@
 
     return result
 
 
 get.from_cache = from_cache
 
 
-def warn_cache():
+def warn_cache() -> None:
     warnings.warn(
         "This attribute is deprecated as boolean, it still works but advised to make a str key",
         DeprecationWarning,
         stacklevel=2,
     )
 
 
@@ -326,14 +325,15 @@
     data=None,
     max_retries=5,
     raw=False,
     json=None,
     delay_base=3,
     use_cache=False,
     cache_compression=".gz",
+    cache_ttl=0,
     sleep_time=None,
     fname=None,
     reuse_session=True,
     local_address=None,
     remote_ip=None,
     refresh_session_on_error=False,
     user_agent=USER_AGENT,
@@ -359,14 +359,15 @@
     result = _retry(
         "post",
         max_retries,
         delay_base,
         raw,
         caching,
         cache_compression,
+        cache_ttl,
         sleep_time,
         reuse_session,
         local_address,
         remote_ip,
         refresh_session_on_error,
         kwargs,
     )
@@ -380,39 +381,46 @@
 def request(data, **kwargs):
     data = data.copy()
     return {"get": get, "post": post}[data.pop("method")](**data, **kwargs)
 
 
 def request_tree(*args, **kwargs):
     import lxml.html
-    import requests_viewer  # to extend trees with `view`
+    import requests_viewer
 
-    return lxml.html.fromstring(request(*args, **kwargs))
+    assert requests_viewer is not None
+
+    html = request(*args, **kwargs)
+    if html is None:
+        return None
+    return lxml.html.fromstring(html)
 
 
 post.from_cache = from_cache
 
 
 def get_tree(*args, **kwargs):
     import lxml.html
-    import requests_viewer  # to extend trees with `view`
+    import requests_viewer
+
+    assert requests_viewer is not None
 
     return lxml.html.fromstring(get(*args, **kwargs))
 
 
 def post_tree(*args, **kwargs):
     import lxml.html
 
     return lxml.html.fromstring(post(*args, **kwargs))
 
 
-def save_session(name, session):
+def save_session(name, session) -> None:
     from requests.utils import dict_from_cookiejar
 
-    if any(["Session" in x.__name__ for x in session.__class__.__mro__]):
+    if any("Session" in x.__name__ for x in session.__class__.__mro__):
         try:
             print("trf")
             session.transfer_driver_cookies_to_session()
         except Exception as e:
             print("ERR", e)
         session = {"headers": session.headers, "cookies": dict_from_cookiejar(session.cookies)}
-    write(session, f"~/.just_sessions/" + name + ".json")
+    write(session, "~/.just_sessions/" + name + ".json")
```

### Comparing `just-0.8.161/just/source_ip.py` & `just-0.8.162/just/source_ip.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/txt.py` & `just-0.8.162/just/txt.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just/zstd_.py` & `just-0.8.162/just/zstd_.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/just.egg-info/PKG-INFO` & `just-0.8.162/just.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: just
-Version: 0.8.161
+Version: 0.8.162
 Summary: Automatically just read and write files based on extension.
 Home-page: https://github.com/kootenpv/just
 Author: Pascal van Kooten
 Author-email: kootenpv@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: any
```

### Comparing `just-0.8.161/just.egg-info/SOURCES.txt` & `just-0.8.162/just.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 conftest.py
 deploy.py
 setup.cfg
 setup.py
 tox.ini
 just/__init__.py
 just/bytes.py
+just/date.py
 just/dir.py
 just/dt.py
 just/forcedip.py
 just/jpath.py
 just/json_.py
 just/log.py
 just/newl.py
```

### Comparing `just-0.8.161/setup.py` & `just-0.8.162/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 MAJOR_VERSION = "0"
 MINOR_VERSION = "8"
-MICRO_VERSION = "161"
+MICRO_VERSION = "162"
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 setup(
     name="just",
     version=VERSION,
     description="Automatically just read and write files based on extension.",
     author="Pascal van Kooten",
```

### Comparing `just-0.8.161/tests/test_files.py` & `just-0.8.162/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `just-0.8.161/tests/test_requests.py` & `just-0.8.162/tests/test_requests.py`

 * *Files identical despite different names*

