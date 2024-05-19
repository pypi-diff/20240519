# Comparing `tmp/specialist-0.6.0.tar.gz` & `tmp/specialist-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialist-0.6.0.tar", last modified: Sun Aug  6 00:34:58 2023, max compression
+gzip compressed data, was "specialist-0.7.0.tar", last modified: Sun May 19 04:55:34 2024, max compression
```

## Comparing `specialist-0.6.0.tar` & `specialist-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:34:58.179149 specialist-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-06 00:34:49.000000 specialist-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-06 00:34:58.179149 specialist-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-08-06 00:34:49.000000 specialist-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 00:34:58.179149 specialist-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-06 00:34:49.000000 specialist-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 00:34:58.175150 specialist-0.6.0/specialist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-06 00:34:58.000000 specialist-0.6.0/specialist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22645 2023-08-06 00:34:49.000000 specialist-0.6.0/specialist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:55:34.379435 specialist-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-19 04:55:31.000000 specialist-0.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-19 04:55:34.379435 specialist-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-19 04:55:31.000000 specialist-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:55:34.379435 specialist-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-19 04:55:31.000000 specialist-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:55:34.379435 specialist-0.7.0/specialist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8521 2024-05-19 04:55:34.000000 specialist-0.7.0/specialist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 04:55:34.000000 specialist-0.7.0/specialist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:55:34.000000 specialist-0.7.0/specialist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 04:55:34.000000 specialist-0.7.0/specialist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 04:55:34.000000 specialist-0.7.0/specialist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    28627 2024-05-19 04:55:31.000000 specialist-0.7.0/specialist.py
```

### Comparing `specialist-0.6.0/LICENSE.md` & `specialist-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specialist-0.6.0/PKG-INFO` & `specialist-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.6.0
-Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
+Version: 0.7.0
+Summary: Visualize CPython's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -21,16 +21,16 @@
 <br>
 
 </div>
 
 <div align=justify>
 
 Specialist uses [fine-grained location](https://peps.python.org/pep-0657/)
-information to create visual representations of exactly *where* and *how* CPython
-3.11's new
+information to create visual representations of exactly *where* and *how*
+CPython's new
 [specializing, adaptive interpreter](https://peps.python.org/pep-0659/)
 optimizes your code.
 
 <div align=center>
 
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-0.png)
 
@@ -59,20 +59,20 @@
 and fill it with browsable HTML visualizations for each module in the current
 directory tree.
 
 
 Background
 ----------
 
-While CPython 3.11 is running your code, it identifies "hot" regions that are
-being run often enough to spend time optimizing. It occasionally "quickens"
-these regions, which `specialist` represents using color. **Dark, rich colors
-indicate code with many quickened instructions (and, therefore, high
-specialization potential), while light, pale colors indicate code with
-relatively few specialization opportunities.**
+While CPython is running your code, it identifies "hot" regions that are being
+run often enough to spend time optimizing. It occasionally "quickens" these
+regions, which `specialist` represents using color. **Dark, rich colors indicate
+code with many quickened instructions (and, therefore, high specialization
+potential), while light, pale colors indicate code with relatively few
+specialization opportunities.**
 
 Most of the time, quickening involves three phases:
 
 - Replacing individual bytecode instructions with "adaptive" forms. These are
 actually a bit slower than normal instructions, because they attempt to
 "specialize" themselves periodically. If they are unable to specialize, they
 will remain in their adaptive form. **`specialist` uses red to indicate the
@@ -126,15 +126,15 @@
     # Round-trip Celsius through Fahrenheit:
     assert math.isclose(t, c_to_f(f_to_c(t))), f"{t} C -> F -> C failed!"
 
 if __name__ == "__main__":
     test_conversions()
 ```
 
-We can run this file with CPython 3.11 from the command-line using `specialist`:
+We can run this file with CPython from the command-line using `specialist`:
 
 ```sh
 $ specialist conversions.py
 ```
 
 After the script has finished running, `specialist` will open a web browser and
 display the annotated program source:
```

### Comparing `specialist-0.6.0/README.md` & `specialist-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 <br>
 
 </div>
 
 <div align=justify>
 
 Specialist uses [fine-grained location](https://peps.python.org/pep-0657/)
-information to create visual representations of exactly *where* and *how* CPython
-3.11's new
+information to create visual representations of exactly *where* and *how*
+CPython's new
 [specializing, adaptive interpreter](https://peps.python.org/pep-0659/)
 optimizes your code.
 
 <div align=center>
 
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-0.png)
 
@@ -47,20 +47,20 @@
 and fill it with browsable HTML visualizations for each module in the current
 directory tree.
 
 
 Background
 ----------
 
-While CPython 3.11 is running your code, it identifies "hot" regions that are
-being run often enough to spend time optimizing. It occasionally "quickens"
-these regions, which `specialist` represents using color. **Dark, rich colors
-indicate code with many quickened instructions (and, therefore, high
-specialization potential), while light, pale colors indicate code with
-relatively few specialization opportunities.**
+While CPython is running your code, it identifies "hot" regions that are being
+run often enough to spend time optimizing. It occasionally "quickens" these
+regions, which `specialist` represents using color. **Dark, rich colors indicate
+code with many quickened instructions (and, therefore, high specialization
+potential), while light, pale colors indicate code with relatively few
+specialization opportunities.**
 
 Most of the time, quickening involves three phases:
 
 - Replacing individual bytecode instructions with "adaptive" forms. These are
 actually a bit slower than normal instructions, because they attempt to
 "specialize" themselves periodically. If they are unable to specialize, they
 will remain in their adaptive form. **`specialist` uses red to indicate the
@@ -114,15 +114,15 @@
     # Round-trip Celsius through Fahrenheit:
     assert math.isclose(t, c_to_f(f_to_c(t))), f"{t} C -> F -> C failed!"
 
 if __name__ == "__main__":
     test_conversions()
 ```
 
-We can run this file with CPython 3.11 from the command-line using `specialist`:
+We can run this file with CPython from the command-line using `specialist`:
 
 ```sh
 $ specialist conversions.py
 ```
 
 After the script has finished running, `specialist` will open a web browser and
 display the annotated program source:
```

### Comparing `specialist-0.6.0/setup.py` & `specialist-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import pathlib
 import setuptools  # type: ignore
 
 README = pathlib.Path(__file__).parent / "README.md"
 setuptools.setup(
     author="Brandt Bucher",
     author_email="brandt@python.org",
-    description="Visualize CPython 3.11's specializing, adaptive interpreter.",
+    description="Visualize CPython's specializing, adaptive interpreter.",
     entry_points={"console_scripts": ["specialist=specialist:main"]},
     license="MIT",
     long_description=README.read_text(),
     long_description_content_type="text/markdown",
     name="specialist",
     py_modules=["specialist"],
     python_requires=">=3.11",
     url="https://github.com/brandtbucher/specialist",
-    version="0.6.0",
+    version="0.7.0",
 )
```

### Comparing `specialist-0.6.0/specialist.egg-info/PKG-INFO` & `specialist-0.7.0/specialist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.6.0
-Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
+Version: 0.7.0
+Summary: Visualize CPython's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -21,16 +21,16 @@
 <br>
 
 </div>
 
 <div align=justify>
 
 Specialist uses [fine-grained location](https://peps.python.org/pep-0657/)
-information to create visual representations of exactly *where* and *how* CPython
-3.11's new
+information to create visual representations of exactly *where* and *how*
+CPython's new
 [specializing, adaptive interpreter](https://peps.python.org/pep-0659/)
 optimizes your code.
 
 <div align=center>
 
 ![](https://raw.githubusercontent.com/brandtbucher/specialist/main/examples/output-0.png)
 
@@ -59,20 +59,20 @@
 and fill it with browsable HTML visualizations for each module in the current
 directory tree.
 
 
 Background
 ----------
 
-While CPython 3.11 is running your code, it identifies "hot" regions that are
-being run often enough to spend time optimizing. It occasionally "quickens"
-these regions, which `specialist` represents using color. **Dark, rich colors
-indicate code with many quickened instructions (and, therefore, high
-specialization potential), while light, pale colors indicate code with
-relatively few specialization opportunities.**
+While CPython is running your code, it identifies "hot" regions that are being
+run often enough to spend time optimizing. It occasionally "quickens" these
+regions, which `specialist` represents using color. **Dark, rich colors indicate
+code with many quickened instructions (and, therefore, high specialization
+potential), while light, pale colors indicate code with relatively few
+specialization opportunities.**
 
 Most of the time, quickening involves three phases:
 
 - Replacing individual bytecode instructions with "adaptive" forms. These are
 actually a bit slower than normal instructions, because they attempt to
 "specialize" themselves periodically. If they are unable to specialize, they
 will remain in their adaptive form. **`specialist` uses red to indicate the
@@ -126,15 +126,15 @@
     # Round-trip Celsius through Fahrenheit:
     assert math.isclose(t, c_to_f(f_to_c(t))), f"{t} C -> F -> C failed!"
 
 if __name__ == "__main__":
     test_conversions()
 ```
 
-We can run this file with CPython 3.11 from the command-line using `specialist`:
+We can run this file with CPython from the command-line using `specialist`:
 
 ```sh
 $ specialist conversions.py
 ```
 
 After the script has finished running, `specialist` will open a web browser and
 display the annotated program source:
```

### Comparing `specialist-0.6.0/specialist.py` & `specialist-0.7.0/specialist.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Visualize CPython 3.11's specializing, adaptive interpreter."""
+"""Visualize CPython's specializing, adaptive interpreter."""
+
 import pathlib
 import sys
 import types
 
 if sys.version_info < (3, 11) or sys.implementation.name != "cpython":
     raise RuntimeError("Specialist only supports CPython 3.11+!")  # pragma: no cover
 
@@ -20,20 +21,23 @@
             _code[pathlib.Path(code.co_filename).resolve()] = code
 
 
 _audit_imports.__cantrace__ = True  # type: ignore [attr-defined]
 sys.addaudithook(_audit_imports)
 
 # pylint: disable = wrong-import-order, wrong-import-position
+import _opcode  # type: ignore [import-not-found]
 import argparse
 import collections
 import colorsys
 import contextlib
+import ctypes
 import dataclasses
 import dis
+import gc
 import html
 import http.server
 import importlib.util
 import itertools
 import opcode
 import os
 import re
@@ -44,57 +48,71 @@
 import threading
 import typing
 import webbrowser
 
 _RE_WHITESPACE = re.compile(r"(\s*\n\s*)")
 _FIRST_POSTION = (1, 0)
 _LAST_POSITION = (sys.maxsize, 0)
-_CACHE_FORMAT = frozenset(opcode._cache_format)  # type: ignore [attr-defined] # pylint: disable = protected-access
-_SPECIALIZED_INSTRUCTIONS = frozenset(opcode._specialized_instructions)  # type: ignore [attr-defined] # pylint: disable = protected-access
+if sys.version_info < (3, 13):  # pragma: no cover
+    _CACHE_FORMAT = frozenset(opcode._cache_format)  # type: ignore [attr-defined] # pylint: disable = protected-access
+else:  # pragma: no cover
+    _CACHE_FORMAT = frozenset(opcode._cache_format) - {  # type: ignore [attr-defined] # pylint: disable = protected-access
+        "JUMP_BACKWARD",
+        "POP_JUMP_IF_FALSE",
+        "POP_JUMP_IF_NONE",
+        "POP_JUMP_IF_NOT_NONE",
+        "POP_JUMP_IF_TRUE",
+    }
+if sys.version_info < (3, 13):  # pragma: no cover
+    _SPECIALIZED_INSTRUCTIONS = frozenset(opcode._specialized_instructions)  # type: ignore [attr-defined] # pylint: disable = no-member, protected-access
+else:  # pragma: no cover
+    _SPECIALIZED_INSTRUCTIONS = frozenset(opcode._specialized_opmap) - {"RESUME_CHECK"}  # type: ignore [attr-defined] # pylint: disable = no-member, protected-access
 if sys.version_info < (3, 12):  # pragma: no cover
     _SUPERDUPERINSTRUCTIONS = frozenset({"PRECALL_NO_KW_LIST_APPEND"})
-    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | frozenset(
-        {
-            "BINARY_OP_INPLACE_ADD_UNICODE",
-            "COMPARE_OP_FLOAT_JUMP",
-            "COMPARE_OP_INT_JUMP",
-            "COMPARE_OP_STR_JUMP",
-            "LOAD_CONST__LOAD_FAST",
-            "LOAD_FAST__LOAD_CONST",
-            "LOAD_FAST__LOAD_FAST",
-            "PRECALL_BUILTIN_CLASS",
-            "PRECALL_BUILTIN_FAST_WITH_KEYWORDS",
-            "PRECALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS",
-            "PRECALL_NO_KW_BUILTIN_FAST",
-            "PRECALL_NO_KW_BUILTIN_O",
-            "PRECALL_NO_KW_ISINSTANCE",
-            "PRECALL_NO_KW_LEN",
-            "PRECALL_NO_KW_METHOD_DESCRIPTOR_FAST",
-            "PRECALL_NO_KW_METHOD_DESCRIPTOR_NOARGS",
-            "PRECALL_NO_KW_METHOD_DESCRIPTOR_O",
-            "PRECALL_NO_KW_STR_1",
-            "PRECALL_NO_KW_TUPLE_1",
-            "PRECALL_NO_KW_TYPE_1",
-            "STORE_FAST__LOAD_FAST",
-            "STORE_FAST__STORE_FAST",
-        }
-    )
+    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | {
+        "BINARY_OP_INPLACE_ADD_UNICODE",
+        "COMPARE_OP_FLOAT_JUMP",
+        "COMPARE_OP_INT_JUMP",
+        "COMPARE_OP_STR_JUMP",
+        "LOAD_CONST__LOAD_FAST",
+        "LOAD_FAST__LOAD_CONST",
+        "LOAD_FAST__LOAD_FAST",
+        "PRECALL_BUILTIN_CLASS",
+        "PRECALL_BUILTIN_FAST_WITH_KEYWORDS",
+        "PRECALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS",
+        "PRECALL_NO_KW_BUILTIN_FAST",
+        "PRECALL_NO_KW_BUILTIN_O",
+        "PRECALL_NO_KW_ISINSTANCE",
+        "PRECALL_NO_KW_LEN",
+        "PRECALL_NO_KW_METHOD_DESCRIPTOR_FAST",
+        "PRECALL_NO_KW_METHOD_DESCRIPTOR_NOARGS",
+        "PRECALL_NO_KW_METHOD_DESCRIPTOR_O",
+        "PRECALL_NO_KW_STR_1",
+        "PRECALL_NO_KW_TUPLE_1",
+        "PRECALL_NO_KW_TYPE_1",
+        "STORE_FAST__LOAD_FAST",
+        "STORE_FAST__STORE_FAST",
+    }
+elif sys.version_info < (3, 13):  # pragma: no cover
+    _SUPERDUPERINSTRUCTIONS: frozenset[str] = frozenset()
+    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | {
+        "BINARY_OP_INPLACE_ADD_UNICODE",
+        "CALL_NO_KW_LIST_APPEND",
+        "LOAD_CONST__LOAD_FAST",
+        "LOAD_FAST__LOAD_CONST",
+        "LOAD_FAST__LOAD_FAST",
+        "STORE_FAST__LOAD_FAST",
+        "STORE_FAST__STORE_FAST",
+    }
 else:  # pragma: no cover
     _SUPERDUPERINSTRUCTIONS: frozenset[str] = frozenset()
-    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | frozenset(
-        {
-            "BINARY_OP_INPLACE_ADD_UNICODE",
-            "CALL_NO_KW_LIST_APPEND",
-            "LOAD_CONST__LOAD_FAST",
-            "LOAD_FAST__LOAD_CONST",
-            "LOAD_FAST__LOAD_FAST",
-            "STORE_FAST__LOAD_FAST",
-            "STORE_FAST__STORE_FAST",
-        }
-    )
+    _SUPERINSTRUCTIONS = _SUPERDUPERINSTRUCTIONS | {
+        "BINARY_OP_INPLACE_ADD_UNICODE",
+        "CALL_LIST_APPEND",
+    }
 _PURELIB = pathlib.Path(sysconfig.get_path("purelib")).resolve()
 assert _PURELIB.is_dir(), _PURELIB
 _STDLIB = pathlib.Path(sysconfig.get_path("stdlib")).resolve()
 assert _STDLIB.is_dir(), _STDLIB
 _TMP = pathlib.Path(tempfile.gettempdir()).resolve()
 assert _TMP.is_dir(), _TMP
 
@@ -295,36 +313,45 @@
 def _parse(code: types.CodeType) -> typing.Generator[_SourceChunk, None, None]:
     """Parse a code object's source code into SourceChunks."""
     events: collections.defaultdict[tuple[int, int], _Stats] = collections.defaultdict(
         _Stats
     )
     events[_FIRST_POSTION] = _Stats()
     events[_LAST_POSITION] = _Stats()
-    previous_previous = previous = None
+    previous_two: tuple[None, None] | tuple[dis.Instruction, dis.Instruction | None] = (
+        None,
+        None,
+    )
+    jit_code = _find_jit_code()
+    have_jit_code = any(jit_code.values())
     for child in _walk_code(code):
-        raw_bytecode = child._co_code_adaptive  # type: ignore [attr-defined]  # pylint: disable = protected-access
         for instruction in dis.get_instructions(child, adaptive=True):
             if instruction.is_jump_target:
-                previous_previous = previous = None
+                previous_two = None, None
             if instruction.positions is None or None in instruction.positions:
-                previous_previous = previous
-                previous = instruction
+                previous_two = instruction, previous_two[0]
                 continue
             lineno, end_lineno, col_offset, end_col_offset = instruction.positions
             assert lineno is not None
             assert end_lineno is not None
             assert col_offset is not None
             assert end_col_offset is not None
             stats = _score_instruction(
-                instruction, previous, previous_previous, raw_bytecode
+                instruction, previous_two[0], previous_two[1], child._co_code_adaptive  # type: ignore [attr-defined]  # pylint: disable = protected-access
             )
+            if have_jit_code:  # pragma: no cover
+                if stats.specialized and instruction.offset // 2 not in jit_code[child]:
+                    stats = _Stats(unquickened=True)
+                elif (
+                    stats.adaptive or stats.unquickened
+                ) and instruction.offset // 2 in jit_code[child]:
+                    stats = _Stats(specialized=True)
             events[lineno, col_offset] += stats
             events[end_lineno, end_col_offset] -= stats
-            previous_previous = previous
-            previous = instruction
+            previous_two = instruction, previous_two[0]
     stats = _Stats()
     for (start, event), (stop, _) in itertools.pairwise(sorted(events.items())):
         stats += event
         yield _SourceChunk(start, stop, stats)
 
 
 def _source_and_stats(
@@ -366,14 +393,121 @@
 
 def _is_quickened(code: types.CodeType) -> bool:
     return any(  # pragma: no cover
         chunk.stats.specialized or chunk.stats.adaptive for chunk in _parse(code)
     )
 
 
+def _find_executors() -> (
+    typing.Generator[
+        tuple[types.CodeType, typing.Sequence[tuple[str, int, int, int]]], None, None
+    ]
+):  # pragma: no cover
+    for code in _code.values():
+        for child in _walk_code(code):
+            for i in range(0, len(child._co_code_adaptive), 2):  # type: ignore [attr-defined] # pylint: disable = protected-access
+                if child._co_code_adaptive[i] == opcode.opmap["ENTER_EXECUTOR"]:  # type: ignore [attr-defined] # pylint: disable = protected-access
+                    try:
+                        executor = _opcode.get_executor(  # pylint: disable = no-member
+                            child, i
+                        )
+                    except (RuntimeError, ValueError):
+                        continue
+                    yield (child, executor)
+
+
+def _callee_from_operand(operand: int) -> types.CodeType | None:  # pragma: no cover
+    if operand & 1:
+        return typing.cast(
+            types.CodeType, ctypes.cast(operand - 1, ctypes.py_object).value
+        )
+    if operand:
+        return typing.cast(
+            types.CodeType, ctypes.cast(operand, ctypes.py_object).value.__code__
+        )
+    return None
+
+
+def _handle_inlining(
+    stack: list[types.CodeType | None], opname: str, operand: int
+) -> None:  # pragma: no cover
+    if opname == "_PUSH_FRAME":
+        stack.append(_callee_from_operand(operand))
+    elif opname == "_POP_FRAME":
+        assert stack[-1] is not None
+        del stack[-1]
+
+
+def _find_jit_code() -> (
+    collections.defaultdict[types.CodeType, set[int]]
+):  # pragma: no cover
+    if "ENTER_EXECUTOR" not in opcode.opmap:
+        return collections.defaultdict(set)
+    todo: set[
+        tuple[types.CodeType | None, typing.Sequence[tuple[str, int, int, int]]]
+    ] = set(_find_executors())
+    jit_code: collections.defaultdict[types.CodeType, set[int]] = (
+        collections.defaultdict(set)
+    )
+    done: set[
+        tuple[types.CodeType | None, typing.Sequence[tuple[str, int, int, int]]]
+    ] = set()
+    while todo - done:
+        for code, executor in todo - done:
+            done.add((code, executor))
+            stack: list[types.CodeType | None] = [code]
+            side_exits = gc.get_referents(executor)
+            assert all(type(side_exit) is type(executor) for side_exit in side_exits)
+            for opname, _, target, operand in executor:
+                if opname in {"_DEOPT", "_ERROR_POP_N", "_EXIT_TRACE", "_DYNAMIC_EXIT"}:
+                    continue
+                jump_target = target & 0xFFFF
+                error_target = target >> 16
+                valid_jump = jump_target < len(executor) and (
+                    (jump_target == 0)
+                    or executor[jump_target][0]
+                    in {"_DEOPT", "_EXIT_TRACE", "_DYNAMIC_EXIT"}
+                )
+                valid_error = error_target < len(executor) and (
+                    (error_target == 0) or executor[error_target][0] in {"_ERROR_POP_N"}
+                )
+                if (
+                    valid_jump
+                    and valid_error
+                    and jump_target
+                    and executor[jump_target][0]
+                    in {
+                        "_EXIT_TRACE",
+                        "_DYNAMIC_EXIT",
+                    }
+                ):
+                    side_exit = side_exits[executor[jump_target][2] & 0xFFFF]
+                    todo.add((stack[-1], side_exit))
+                elif valid_jump and valid_error and jump_target:
+                    assert executor[jump_target][0] == "_DEOPT"
+                    target = executor[jump_target][2]
+                    assert (
+                        stack[-1] is None or target < len(stack[-1]._co_code_adaptive) // 2  # type: ignore [attr-defined] # pylint: disable = protected-access
+                    )
+                    if stack[-1] is not None:
+                        jit_code[stack[-1]].add(target)
+                if valid_jump and valid_error and error_target:
+                    assert executor[jump_target][0] == "_ERROR_POP_N"
+                    target = executor[error_target][3]
+                    assert stack[-1] is None or target < len(stack[-1]._co_code_adaptive) // 2  # type: ignore [attr-defined] # pylint: disable = protected-access
+                    if stack[-1] is not None:
+                        jit_code[stack[-1]].add(target)
+                else:
+                    assert stack[-1] is None or target < len(stack[-1]._co_code_adaptive) // 2  # type: ignore [attr-defined] # pylint: disable = protected-access
+                    if stack[-1] is not None:
+                        jit_code[stack[-1]].add(target)
+                _handle_inlining(stack, opname, operand)
+    return jit_code
+
+
 def _view(
     path: pathlib.Path,
     *,
     blue: bool = False,
     dark: bool = False,
     out: pathlib.Path | None = None,
     name: str | None = None,
```

