# Comparing `tmp/thymus_ast-0.1.7.tar.gz` & `tmp/thymus_ast-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thymus_ast-0.1.7.tar", max compression
+gzip compressed data, was "thymus_ast-0.1.8.tar", max compression
```

## Comparing `thymus_ast-0.1.7.tar` & `thymus_ast-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1093 2023-09-19 16:12:05.290498 thymus_ast-0.1.7/LICENSE
--rw-r--r--   0        0        0      492 2024-04-12 09:04:25.834401 thymus_ast-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      544 2023-12-09 12:09:08.370980 thymus_ast-0.1.7/README.md
--rw-r--r--   0        0        0        2 2023-09-19 21:16:45.075801 thymus_ast-0.1.7/thymus_ast/__init__.py
--rw-r--r--   0        0        0      342 2023-06-17 13:40:41.547409 thymus_ast-0.1.7/thymus_ast/ios/__init__.py
--rw-r--r--   0        0        0    14638 2024-04-18 19:36:07.707768 thymus_ast-0.1.7/thymus_ast/ios/ios.py
--rw-r--r--   0        0        0      702 2024-04-18 19:38:59.977723 thymus_ast-0.1.7/thymus_ast/junos/__init__.py
--rw-r--r--   0        0        0    15718 2024-04-18 19:39:06.920916 thymus_ast-0.1.7/thymus_ast/junos/junos.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 thymus_ast-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-09-19 16:12:05.290498 thymus_ast-0.1.8/LICENSE
+-rw-r--r--   0        0        0      490 2024-04-25 16:39:46.257428 thymus_ast-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      544 2023-12-09 12:09:08.370980 thymus_ast-0.1.8/README.md
+-rw-r--r--   0        0        0        2 2023-09-19 21:16:45.075801 thymus_ast-0.1.8/thymus_ast/__init__.py
+-rw-r--r--   0        0        0      572 2024-05-17 14:25:09.835234 thymus_ast-0.1.8/thymus_ast/ios/__init__.py
+-rw-r--r--   0        0        0    26755 2024-05-18 11:57:21.181590 thymus_ast-0.1.8/thymus_ast/ios/ios.py
+-rw-r--r--   0        0        0      702 2024-04-18 19:38:59.977723 thymus_ast-0.1.8/thymus_ast/junos/__init__.py
+-rw-r--r--   0        0        0    15894 2024-05-17 07:47:29.109539 thymus_ast-0.1.8/thymus_ast/junos/junos.py
+-rw-r--r--   0        0        0      897 2024-04-26 10:08:26.706295 thymus_ast-0.1.8/thymus_ast/junos_ng/__init__.py
+-rw-r--r--   0        0        0    21611 2024-05-17 07:57:02.830830 thymus_ast-0.1.8/thymus_ast/junos_ng/junos_ng.py
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 thymus_ast-0.1.8/PKG-INFO
```

### Comparing `thymus_ast-0.1.7/LICENSE` & `thymus_ast-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.7/README.md` & `thymus_ast-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.7/thymus_ast/junos/__init__.py` & `thymus_ast-0.1.8/thymus_ast/junos/__init__.py`

 * *Files identical despite different names*

### Comparing `thymus_ast-0.1.7/thymus_ast/junos/junos.py` & `thymus_ast-0.1.8/thymus_ast/junos/junos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+DEPRECATION ALERT!!!
+
+This set of functions is obsolete. I will leave this module here solely for backward compatibility purposes.
+It is not going to be supported any further.
+"""
+
 from __future__ import annotations
 
 import sys
 import re
 
 from typing import TypedDict, Optional
 from collections import deque
@@ -38,15 +45,15 @@
     For every list element, an extra argument is accounted for to cover cases
         when these elements are inactive and/or protected.
     """
     if len(left) != len(right):
         return False
     dleft = deque(left)
     dright = deque(right)
-    extra_pattern = r'(?:inactive: |protect: ){1,2}'
+    extra_pattern = r'(?:inactive: |protect: ){0,2}'
     while True:
         lml = dleft.popleft()
         lmr = dright.popleft()
         if lml == lmr or re.match(extra_pattern + lml, lmr) or re.match(extra_pattern + lmr, lml):
             if dleft or dright:
                 continue
             return True
@@ -105,17 +112,17 @@
 
 
 def wc_parser(
     data: list[str], path: str, pattern: str, delimiter='^'
 ) -> tuple[dict[str, list[str]], dict[str, list[str]]]:
     if pattern.startswith('^'):
         pattern = pattern[1:]
-        if not pattern:
-            return {}, {}
-    pattern = r'^(?:inactive: |protect: ){1,2}' + pattern
+    if not pattern:
+        return {}, {}
+    pattern = r'^(?:inactive: |protect: ){0,2}' + pattern
     sections: list[str] = []
     container: dict[str, list[str]] = {}
     params: dict[str, list[str]] = {}
     parts = path.split(delimiter) if path else []
     plen = len(parts)
     for line in data:
         stripped = line.strip()
@@ -147,17 +154,17 @@
                 container[sections[plen][:-2]].append(stripped)
     return container, params
 
 
 def lazy_wc_parser(data: Iterable[str], path: str, pattern: str, delimiter='^') -> Generator[str, None, None]:
     if pattern.startswith('^'):
         pattern = pattern[1:]
-        if not pattern:
-            return
-    pattern = r'^(?:inactive: |protect: ){1,2}' + pattern
+    if not pattern:
+        return
+    pattern = r'^(?:inactive: |protect: ){0,2}' + pattern
     sections: list[str] = []
     parts: list[str] = path.split(delimiter) if path else []
     plen = len(parts)
     for line in data:
         stripped = line.strip()
         if '{' in stripped and '}' not in stripped and ';' not in stripped:
             sections.append(stripped)
```

### Comparing `thymus_ast-0.1.7/PKG-INFO` & `thymus_ast-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: thymus-ast
-Version: 0.1.7
+Version: 0.1.8
 Summary: A set of tools to build ASTs for different NOS
 Author: Igor Malyushkin
 Author-email: gmalyushkin@gmail.com
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
```

