# Comparing `tmp/tarina-0.4.4.tar.gz` & `tmp/tarina-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.4.4.tar", last modified: Mon Feb 26 03:03:55 2024, max compression
+gzip compressed data, was "tarina-0.5.0.tar", last modified: Sun May 19 07:28:30 2024, max compression
```

## Comparing `tarina-0.4.4.tar` & `tarina-0.5.0.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:03:55.002425 tarina-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-26 03:03:38.000000 tarina-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-26 03:03:38.000000 tarina-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-26 03:03:55.002425 tarina-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-26 03:03:38.000000 tarina-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-26 03:03:38.000000 tarina-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 03:03:55.002425 tarina-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-26 03:03:38.000000 tarina-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:03:54.994425 tarina-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:03:54.998425 tarina-0.4.4/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_op.h
--rw-r--r--   0 runner    (1001) docker     (127)   213169 2024-02-26 03:03:47.000000 tarina-0.4.4/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/guard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:03:55.002425 tarina-0.4.4/src/tarina/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/i18n/.config.json
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/i18n/en-US.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/i18n/zh-CN.json
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/lang.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-02-26 03:03:38.000000 tarina-0.4.4/src/tarina/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:03:55.002425 tarina-0.4.4/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-26 03:03:54.000000 tarina-0.4.4/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-26 03:03:54.000000 tarina-0.4.4/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 03:03:54.000000 tarina-0.4.4/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-26 03:03:54.000000 tarina-0.4.4/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-26 03:03:54.000000 tarina-0.4.4/src/tarina.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:03:55.002425 tarina-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-02-26 03:03:38.000000 tarina-0.4.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.807887 tarina-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 07:28:16.000000 tarina-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-19 07:28:16.000000 tarina-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 07:28:30.807887 tarina-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-19 07:28:16.000000 tarina-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-19 07:28:16.000000 tarina-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:28:30.807887 tarina-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 07:28:16.000000 tarina-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.803887 tarina-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.807887 tarina-0.5.0/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (127)   213169 2024-05-19 07:28:25.000000 tarina-0.5.0/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/guard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.807887 tarina-0.5.0/src/tarina/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/.config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/.lang.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/.template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/.template.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/en-US.json
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/i18n/zh-CN.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.807887 tarina-0.5.0/src/tarina/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/lang/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/lang/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/lang/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68734 2024-05-19 07:28:16.000000 tarina-0.5.0/src/tarina/trie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.807887 tarina-0.5.0/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 07:28:30.000000 tarina-0.5.0/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-19 07:28:30.000000 tarina-0.5.0/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:28:30.000000 tarina-0.5.0/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 07:28:30.000000 tarina-0.5.0/src/tarina.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 07:28:30.000000 tarina-0.5.0/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 07:28:30.000000 tarina-0.5.0/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:28:30.807887 tarina-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-19 07:28:16.000000 tarina-0.5.0/tests/test_main.py
```

### Comparing `tarina-0.4.4/LICENSE` & `tarina-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/PKG-INFO` & `tarina-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.4.4
+Version: 0.5.0
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions>=4.4.0
```

### Comparing `tarina-0.4.4/pyproject.toml` & `tarina-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 [project]
 name = "tarina"
-version = "0.4.4"
+version = "0.5.0"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 
+[project.scripts]
+tarina-lang = "tarina.lang.__main__:main"
+
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [tool.pdm]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest~=7.2.0",
     "coverage~=7.0.1",
     "cython>=3.0.0",
     "black>=24.2.0",
     "isort>=5.13.2",
+    "fix-future-annotations>=0.5.0",
 ]
 
 [tool.cibuildwheel]
 # don't build PyPy wheels, install from source instead
 skip = "pp*"
 
 [tool.black]
```

### Comparing `tarina-0.4.4/setup.py` & `tarina-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/__init__.py` & `tarina-0.5.0/src/tarina/__init__.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/_lru_c.c` & `tarina-0.5.0/src/tarina/_lru_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/_lru_c.pyi` & `tarina-0.5.0/src/tarina/_lru_c.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Any, Callable, Generic, Hashable, Iterable, TypeVar, overload
 
 _KT = TypeVar("_KT", bound=Hashable)
 _VT = TypeVar("_VT")
 _T = TypeVar("_T")
 
 class LRU(Generic[_KT, _VT]):
-    def __init__(self, size: int, callback: Callable[[_KT, _VT], Any] | None = ...) -> None: ...
+    @overload
+    def __init__(self, size: int, callback: None = None) -> None: ...
+    @overload
+    def __init__(self, size: int, callback: Callable[[_KT, _VT], Any]) -> None: ...
     def clear(self) -> None: ...
     @overload
     def get(self, key: _KT) -> _VT | None: ...
     @overload
     def get(self, key: _KT, instead: _VT | _T) -> _VT | _T: ...
     def get_size(self) -> int: ...
     def has_key(self, key: _KT) -> bool: ...
```

### Comparing `tarina-0.4.4/src/tarina/_lru_py.py` & `tarina-0.5.0/src/tarina/_lru_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     @overload
     def get(self, key: _KT) -> _VT | None: ...
 
     @overload
     def get(self, key: _KT, instead: _VT | _T) -> _VT | _T: ...
 
-    def get(self, key: _KT, instead: _VT | _T | None = None):
+    def get(self, key: _KT, instead: _VT | _T | None = None)-> _VT | _T | None:
         if key in self.__cache:
             self.__cache.move_to_end(key, last=False)
             return self.__cache[key]
         return instead
 
     def get_size(self) -> int:
         return self.__max
@@ -57,15 +57,15 @@
 
     @overload
     def pop(self, key: _KT) -> _VT | None: ...
 
     @overload
     def pop(self, key: _KT, default: _VT | _T) -> _VT | _T: ...
 
-    def pop(self, key: _KT, default: _VT | _T | None = None):
+    def pop(self, key: _KT, default: _VT | _T | None = None)-> _VT | _T:
         return self.__cache.pop(key, default)
 
     def popitem(self, least_recent: bool = True) -> tuple[_KT, _VT]:
         return self.__cache.popitem(last=least_recent)
 
     @overload
     def setdefault(self: LRU[_KT, _T | None], key: _KT) -> _T | None: ...
```

### Comparing `tarina-0.4.4/src/tarina/_op.h` & `tarina-0.5.0/src/tarina/_op.h`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/_string_c.c` & `tarina-0.5.0/src/tarina/_string_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/_string_c.pyi` & `tarina-0.5.0/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/_string_c.pyx` & `tarina-0.5.0/src/tarina/_string_c.pyx`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/_string_py.py` & `tarina-0.5.0/src/tarina/_string_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/context.py` & `tarina-0.5.0/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/date.py` & `tarina-0.5.0/src/tarina/date.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,23 @@
                 "s(?:ec(?:ond)?(?:s)?)?",
             ],
         )
     )
 )
 
 
+def get_total_seconds(delta: datetime):
+    offset = delta.utcoffset()
+    if not offset:
+        return 0
+    return offset.total_seconds() / 60
+
+
 class DateParser:
-    timezone_offset = datetime.now(timezone.utc).astimezone().utcoffset().total_seconds() / 60
+    timezone_offset = get_total_seconds(datetime.now(timezone.utc).astimezone())
 
     @classmethod
     def set_timezone_offset(cls, offset: float):
         cls.timezone_offset = offset
 
     @classmethod
     def get_timezone_offset(cls):
```

### Comparing `tarina-0.4.4/src/tarina/generic.py` & `tarina-0.5.0/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/guard.py` & `tarina-0.5.0/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/lang.py` & `tarina-0.5.0/src/tarina/lang/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import sys
 from pathlib import Path
 from typing import Final, TypedDict, cast, final
 
 from typing_extensions import Self
 
-root_dir: Final[Path] = Path(__file__).parent / "i18n"
+root_dir: Final[Path] = Path(__file__).parent.parent / "i18n"
 WINDOWS = sys.platform.startswith("win") or (sys.platform == "cli" and os.name == "nt")
 
 
 class _LangDict(TypedDict):
     default: str
     frozen: list[str]
     require: list[str]
@@ -46,31 +46,33 @@
         _get_win_locale = _get_win_locale_from_registry
 
 
 def get_locale() -> str | None:
     if WINDOWS:
         return _get_win_locale()
 
-    return locale.getlocale(locale.LC_MESSAGES)[0]
+    return locale.getlocale(locale.LC_MESSAGES)[0]  # type: ignore
 
 
 def _get_config(root: Path) -> _LangDict:
     if not (root / ".config.json").exists():
         raise FileNotFoundError(f"Config file not found in {root}")
     with (root / ".config.json").open("r", encoding="utf-8") as f:
         return cast(_LangDict, json.load(f))
 
 
 def _get_scopes(root: Path) -> list[str]:
-    return [i.stem for i in root.iterdir() if i.is_file() and not i.name.startswith(".")]
+    return [i.stem for i in root.iterdir() if i.is_file() and i.suffix == ".json" and not i.name.startswith(".")]
 
 
 def _get_lang(root: Path, _type: str) -> dict[str, dict[str, str]]:
     with (root / f"{_type}.json").open("r", encoding="utf-8") as f:
-        return json.load(f)
+        data: dict[str, dict[str, str]] = json.load(f)
+    data.pop("$schema", None)
+    return data
 
 
 def merge(source: dict, target: dict, ignore: list[str] | None = None) -> dict:
     ignore = ignore or []
     for key, value in source.items():
         if key in target and key in ignore:
             continue
@@ -83,111 +85,112 @@
     return target
 
 
 @final
 class _LangConfig:
     def __init__(self):
         __config = _get_config(root_dir)
-        self.__scope: str = __config["default"]
+        self.__locale: str = __config["default"]
         self.__frozen: list[str] = __config["frozen"]
         self.__require: list[str] = __config["require"]
         self.__langs = {t.replace("_", "-"): _get_lang(root_dir, t) for t in _get_scopes(root_dir)}
-        self.__scopes = set(self.__langs.keys())
+        self.__locales = set(self.__langs.keys())
         self.select_local()
 
     @property
-    def scopes(self):
-        return self.__scopes
+    def locales(self):
+        return self.__locales
 
     @property
     def current(self):
-        return self.__scope
+        return self.__locale
 
     def select_local(self):
         """
         依据系统语言尝试自动选择语言
         """
         if (lc := get_locale()) and lc.replace("_", "-") in self.__langs:
-            self.__scope = lc.replace("_", "-")
+            self.__locale = lc.replace("_", "-")
         return self
 
-    def select(self, item: str) -> Self:
-        item = item.replace("_", "-")
-        if item not in self.__langs:
-            raise ValueError(self.require("lang", "scope_error").format(target=item))
-        self.__scope = item
+    def select(self, locale: str) -> Self:
+        locale = locale.replace("_", "-")
+        if locale not in self.__langs:
+            raise ValueError(self.require("lang", "locale_error").format(target=locale))
+        self.__locale = locale
         return self
 
     def save(self, root: Path | None = None):
         _root = root or root_dir
         config = _get_config(_root)
-        config["default"] = self.__scope
+        config["default"] = self.__locale
         with (_root / ".config.json").open("w+", encoding="utf-8") as f:
             json.dump(config, f, ensure_ascii=False, indent=2)
 
-    def load_data(self, scope: str, data: dict[str, dict[str, str]]):
-        if scope in self.__langs:
-            self.__langs[scope] = merge(data, self.__langs[scope], self.__frozen)
+    def load_data(self, locale: str, data: dict[str, dict[str, str]]):
+        if locale in self.__langs:
+            self.__langs[locale] = merge(data, self.__langs[locale], self.__frozen)
         else:
-            self.__scopes.add(scope)
-            self.__langs[scope] = data
+            self.__locales.add(locale)
+            self.__langs[locale] = data
         for key in self.__require:
             parts = key.split(".", 1)
-            t = parts[0]
-            n = parts[1] if len(parts) > 1 else None
-            if t not in self.__langs[scope]:
-                raise KeyError(self.require("lang", "miss_require_type", scope).format(scope=scope, target=t))
-            if n and n not in self.__langs[scope][t]:
-                raise KeyError(self.require("lang", "miss_require_name", scope).format(scope=scope, type=t, target=n))
+            s = parts[0]
+            t = parts[1] if len(parts) > 1 else None
+            if s not in self.__langs[locale]:
+                raise KeyError(self.require("lang", "miss_require_scope", locale).format(locale=locale, target=s))
+            if t and t not in self.__langs[locale][s]:
+                raise KeyError(self.require("lang", "miss_require_type", locale).format(locale=locale, scope=s, target=t))
 
     def load_file(self, filepath: Path):
         return self.load_data(filepath.stem, _get_lang(filepath.parent, filepath.stem))
 
     def load_config(self, config: _LangDict):
-        self.__scope = config.get("default", self.__scope)
+        self.__locale = config.get("default", self.__locale)
         self.__frozen.extend(config.get("frozen", []))
         self.__require.extend(config.get("require", []))
         self.select_local()
 
-    def load(self, root: Path):
+    def load(self, root: Path) -> Self:
         self.load_config(_get_config(root))
         for i in root.iterdir():
             if not i.is_file() or i.name.startswith("."):
                 continue
             self.load_file(i)
+        return self
 
-    def require(self, _type: str, _name: str, scope: str | None = None) -> str:
-        scope = scope or self.__scope
-        if scope not in self.__langs:
-            raise ValueError(self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope))
-        if _type in self.__langs[scope]:
-            _types = self.__langs[scope][_type]
-        elif _type in self.__langs[self.__scope]:
-            _types = self.__langs[self.__scope][_type]
-        elif _type in self.__langs[(default := _get_config(root_dir)["default"])]:
-            _types = self.__langs[default][_type]
+    def require(self, scope: str, type: str, locale: str | None = None) -> str:
+        locale = locale or self.__locale
+        if locale not in self.__langs:
+            raise ValueError(self.__langs[self.__locale]["lang"]["locale_error"].format(target=locale))
+        if scope in self.__langs[locale]:
+            _types = self.__langs[locale][scope]
+        elif scope in self.__langs[self.__locale]:
+            _types = self.__langs[self.__locale][scope]
+        elif scope in self.__langs[(default := _get_config(root_dir)["default"])]:
+            _types = self.__langs[default][scope]
         else:
-            raise ValueError(self.__langs[scope]["lang"]["type_error"].format(target=_type, scope=scope))
-        if _name in _types:
-            return _types[_name]
-        elif _name in self.__langs[self.__scope][_type]:
-            return self.__langs[self.__scope][_type][_name]
-        elif _name in self.__langs[(default := _get_config(root_dir)["default"])][_type]:
-            return self.__langs[default][_type][_name]
+            raise ValueError(self.__langs[locale]["lang"]["scope_error"].format(target=scope, locale=locale))
+        if type in _types:
+            return _types[type]
+        elif type in self.__langs[self.__locale][scope]:
+            return self.__langs[self.__locale][scope][type]
+        elif type in self.__langs[(default := _get_config(root_dir)["default"])][scope]:
+            return self.__langs[default][scope][type]
         else:
-            raise ValueError(self.__langs[scope]["lang"]["name_error"].format(target=_name, scope=scope, type=_type))
+            raise ValueError(self.__langs[locale]["lang"]["type_error"].format(target=type, locale=locale, scope=scope))
 
-    def set(self, _type: str, _name: str, content: str, scope: str | None = None):
-        scope = scope or self.__scope
-        if scope not in self.__langs:
-            raise ValueError(self.__langs[self.__scope]["lang"]["scope_error"].format(target=scope))
-        if _type in self.__frozen:
-            raise ValueError(self.__langs[scope]["lang"]["type_error"].format(target=_type, scope=scope))
-        self.__langs[scope].setdefault(_type, {})[_name] = content
+    def set(self, scope: str, type: str, content: str, locale: str | None = None):
+        locale = locale or self.__locale
+        if locale not in self.__langs:
+            raise ValueError(self.__langs[self.__locale]["lang"]["locale_error"].format(target=locale))
+        if scope in self.__frozen:
+            raise ValueError(self.__langs[locale]["lang"]["scope_error"].format(target=scope, locale=locale))
+        self.__langs[locale].setdefault(scope, {})[type] = content
 
     def __repr__(self):
-        return f"<LangConfig: {self.__scope}>"
+        return f"<LangConfig: {self.__locale}>"
 
 
 lang: _LangConfig = _LangConfig()
 
 __all__ = ["lang"]
```

### Comparing `tarina-0.4.4/src/tarina/lru.pyi` & `tarina-0.5.0/src/tarina/lru.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Any, Callable, Generic, Hashable, Iterable, TypeVar, overload
 
 _KT = TypeVar("_KT", bound=Hashable)
 _VT = TypeVar("_VT")
 _T = TypeVar("_T")
 
 class LRU(Generic[_KT, _VT]):
-    def __init__(self, size: int, callback: Callable[[_KT, _VT], Any] | None = ...) -> None: ...
+    @overload
+    def __init__(self, size: int, callback: None = None) -> None: ...
+    @overload
+    def __init__(self, size: int, callback: Callable[[_KT, _VT], Any]) -> None: ...
     def clear(self) -> None: ...
     @overload
     def get(self, key: _KT) -> _VT: ...
     @overload
     def get(self, key: _KT, instead: _VT | _T) -> _VT | _T: ...
     def get_size(self) -> int: ...
     def has_key(self, key: _KT) -> bool: ...
```

### Comparing `tarina-0.4.4/src/tarina/signature.py` & `tarina-0.5.0/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/string.py` & `tarina-0.5.0/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.4.4/src/tarina/tools.py` & `tarina-0.5.0/src/tarina/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         temp.setdefault(k, []).append(i)
     return temp
 
 
 async def run_always_await(target: Callable[..., Any] | Callable[..., Awaitable[Any]], *args, **kwargs) -> Any:
     obj = target(*args, **kwargs)
     if is_async(target) or is_async(obj):
-        obj = await obj
+        obj = await obj  # type: ignore
     return obj
 
 
 def gen_subclass(cls: type[T]) -> Generator[type[T], None, None]:
     """生成某个类的所有子类 (包括其自身)
     Args:
         cls (Type[T]): 类
```

### Comparing `tarina-0.4.4/src/tarina.egg-info/PKG-INFO` & `tarina-0.5.0/src/tarina.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.4.4
+Version: 0.5.0
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions>=4.4.0
```

### Comparing `tarina-0.4.4/src/tarina.egg-info/SOURCES.txt` & `tarina-0.5.0/src/tarina.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,32 @@
 src/tarina/_string_c.pyx
 src/tarina/_string_py.py
 src/tarina/const.py
 src/tarina/context.py
 src/tarina/date.py
 src/tarina/generic.py
 src/tarina/guard.py
-src/tarina/lang.py
 src/tarina/lru.py
 src/tarina/lru.pyi
 src/tarina/signature.py
 src/tarina/string.py
 src/tarina/tools.py
+src/tarina/trie.py
 src/tarina.egg-info/PKG-INFO
 src/tarina.egg-info/SOURCES.txt
 src/tarina.egg-info/dependency_links.txt
+src/tarina.egg-info/entry_points.txt
 src/tarina.egg-info/requires.txt
 src/tarina.egg-info/top_level.txt
 src/tarina/i18n/.config.json
+src/tarina/i18n/.lang.schema.json
+src/tarina/i18n/.template.json
+src/tarina/i18n/.template.schema.json
+src/tarina/i18n/__init__.py
 src/tarina/i18n/en-US.json
+src/tarina/i18n/model.py
 src/tarina/i18n/zh-CN.json
+src/tarina/lang/__init__.py
+src/tarina/lang/__main__.py
+src/tarina/lang/model.py
+src/tarina/lang/schema.py
 tests/test_main.py
```

### Comparing `tarina-0.4.4/tests/test_main.py` & `tarina-0.5.0/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     """测试 LRU缓存"""
     from tarina import LRU
 
     cache: LRU[str, str] = LRU(3)
     cache["a"] = "a"
     cache["b"] = "b"
     cache["c"] = "c"
-    assert cache.peek_first_item()[1] == "c"
+    assert cache.peek_first_item()[1] == "c"  # type: ignore
     _ = cache.get("a", Ellipsis)
     print(f"\n{cache.items()}")
-    assert cache.peek_first_item()[1] == "a"
+    assert cache.peek_first_item()[1] == "a"  # type: ignore
     cache["d"] = "d"
     assert cache.get("b", Ellipsis) == Ellipsis
 
 
 def test_split_once():
     """测试单次分割函数, 能以引号扩起空格, 并允许保留引号"""
     from tarina import split_once
@@ -73,33 +73,33 @@
         assert str(e) == "Unterminated string: 'rrr \"bbb'"
 
 
 def test_lang():
     """测试 i18n"""
     from tarina import lang
 
-    assert lang.scopes == {"zh-CN", "en-US"}
+    assert lang.locales == {"zh-CN", "en-US"}
     lang.select("zh-CN")
     assert lang.current == "zh-CN"
-    assert lang.require("lang", "name_error") == "'{target}' 在 '{scope}:{type}' 不是合法的名称"
-    assert lang.require("lang", "name_error", "en-US") == "'{target}' is not a valid name in '{scope}:{type}'"
+    assert lang.require("lang", "type_error") == "'{target}' 在 '{locale}:{scope}' 不是合法的类型"
+    assert lang.require("lang", "type_error", "en-US") == "'{target}' is not a valid type in '{locale}:{scope}'"
     lang.select("en-US")
     assert lang.current == "en-US"
     try:
         lang.select("ru-RU")
     except ValueError as e:
-        assert str(e) == "'ru-RU' is not a valid language scope"
+        assert str(e) == "'ru-RU' is not a valid language locale"
     try:
         lang.load_data("test", {})
     except KeyError as e:
-        assert str(e) == "\"lang file 'test' missed require type 'lang'\""
-    lang.load_data("test", {"lang": {"name_error": "test"}})
+        assert str(e) == "\"lang file 'test' missed require scope 'lang'\""
+    lang.load_data("test", {"lang": {"type_error": "test"}})
     lang.select("test")
-    assert lang.require("lang", "name_error") == "test"
-    assert lang.require("lang", "scope_error") == "'{target}' 不是合法的语种"
+    assert lang.require("lang", "type_error") == "test"
+    assert lang.require("lang", "locale_error") == "'{target}' 不是合法的语种"
 
 
 def test_init_spec():
     from dataclasses import dataclass
 
     from tarina import init_spec
```

