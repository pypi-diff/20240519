# Comparing `tmp/types-fpdf2-2.7.8.20240423.tar.gz` & `tmp/types-fpdf2-2.7.9.20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-fpdf2-2.7.8.20240423.tar", last modified: Tue Apr 23 02:19:52 2024, max compression
+gzip compressed data, was "types-fpdf2-2.7.9.20240519.tar", last modified: Sun May 19 02:24:58 2024, max compression
```

## Comparing `types-fpdf2-2.7.8.20240423.tar` & `types-fpdf2-2.7.9.20240519.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/fpdf-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/_fonttools_shims.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/actions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/annotations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/bidi.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/deprecation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15139 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/encryption.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/fpdf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/graphics_state.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/html.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/image_datastructures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/image_parsing.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/line_break.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/linearization.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/outline.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/output.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/prefs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/recorder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/sign.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/structure_tree.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/svg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/syntax.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/table.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/template.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/text_region.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/transitions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-23 02:18:48.000000 types-fpdf2-2.7.8.20240423/fpdf-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:52.936497 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 02:19:52.000000 types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:58.707858 types-fpdf2-2.7.9.20240519/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 02:24:58.707858 types-fpdf2-2.7.9.20240519/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:58.707858 types-fpdf2-2.7.9.20240519/fpdf-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/_fonttools_shims.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/actions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/annotations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/bidi.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/deprecation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/encryption.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21492 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/fpdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/graphics_state.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/html.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/image_datastructures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/image_parsing.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/line_break.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/linearization.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/outline.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/output.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/prefs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/recorder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/sign.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/structure_tree.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/svg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/syntax.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/template.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/text_region.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/transitions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-19 02:23:25.000000 types-fpdf2-2.7.9.20240519/fpdf-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:24:58.707858 types-fpdf2-2.7.9.20240519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:58.707858 types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 02:24:58.000000 types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/top_level.txt
```

### Comparing `types-fpdf2-2.7.8.20240423/CHANGELOG.md` & `types-fpdf2-2.7.9.20240519/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.7.9.20240519 (2024-05-19)
+
+Use assignment instead of annotation in third party enums (#11957)
+
+[fpdf2] Update to 2.7.9 (#11953)
+
 ## 2.7.8.20240423 (2024-04-23)
 
 Add precise values for enum members where possible (#11299)
 
 Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
 Co-authored-by: Alex Waygood <alex.waygood@gmail.com>
```

### Comparing `types-fpdf2-2.7.8.20240423/PKG-INFO` & `types-fpdf2-2.7.9.20240519/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.7.8.20240423
+Version: 2.7.9.20240519
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`.
 
 This version of `types-fpdf2` aims to provide accurate annotations
-for `fpdf2==2.7.8`.
+for `fpdf2==2.7.9`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/__init__.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/_fonttools_shims.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/_fonttools_shims.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/actions.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/actions.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/annotations.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/annotations.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/bidi.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/bidi.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from _typeshed import Incomplete
 from collections.abc import Sequence
 from dataclasses import dataclass
 from typing import Final, Literal, TypedDict, type_check_only
 
+from .enums import TextDirection
+
 MAX_DEPTH: Final = 125
 
 @type_check_only
 class _BracketInfo(TypedDict):
     pair: str
     type: Literal["o", "c"]
 
@@ -36,25 +38,25 @@
     next_direction: str
     def __init__(self, characters: list[BidiCharacter], sos: str, eos: str) -> None: ...
     def resolve_weak_types(self) -> None: ...
     def pair_brackets(self) -> list[tuple[int, int]]: ...
     def resolve_neutral_types(self) -> None: ...
     def resolve_implicit_levels(self) -> None: ...
 
-def auto_detect_base_direction(string: str, stop_at_pdi: bool = False, debug: bool = False) -> Literal["L", "R"]: ...
+def auto_detect_base_direction(string: str, stop_at_pdi: bool = False, debug: bool = False) -> TextDirection: ...
 def calculate_isolate_runs(paragraph: Sequence[BidiCharacter]) -> list[IsolatingRun]: ...
 
 class BidiParagraph:
     text: str
-    base_direction: Literal["L", "R"]
+    base_direction: TextDirection
     debug: bool
     base_embedding_level: int
     characters: list[BidiCharacter]
 
-    def __init__(self, text: str, base_direction: Literal["L", "R"] | None = None, debug: bool = False) -> None: ...
+    def __init__(self, text: str, base_direction: TextDirection | None = None, debug: bool = False) -> None: ...
     def get_characters(self) -> list[BidiCharacter]: ...
     def get_characters_with_embedding_level(self) -> list[BidiCharacter]: ...
     def get_reordered_characters(self) -> list[BidiCharacter]: ...
     def get_all(self) -> tuple[list[BidiCharacter], tuple[BidiCharacter, ...]]: ...
     def get_reordered_string(self) -> str: ...
     def get_bidi_fragments(self) -> tuple[tuple[str, Literal["L", "R"]], ...]: ...
     def get_bidi_characters(self) -> None: ...
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/drawing.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/drawing.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,25 +37,29 @@
     a: Number | None
 
 class DeviceRGB(_DeviceRGBBase):
     OPERATOR: ClassVar[str]
     def __new__(cls, r: Number, g: Number, b: Number, a: Number | None = None) -> Self: ...
     @property
     def colors(self) -> tuple[Number, Number, Number]: ...
+    @property
+    def colors255(self) -> tuple[Number, Number, Number]: ...
     def serialize(self) -> str: ...
 
 class _DeviceGrayBase(NamedTuple):
     g: Number
     a: Number | None
 
 class DeviceGray(_DeviceGrayBase):
     OPERATOR: ClassVar[str]
     def __new__(cls, g: Number, a: Number | None = None) -> Self: ...
     @property
-    def colors(self) -> tuple[Number]: ...
+    def colors(self) -> tuple[Number, Number, Number]: ...
+    @property
+    def colors255(self) -> tuple[Number, Number, Number]: ...
     def serialize(self) -> str: ...
 
 class _DeviceCMYKBase(NamedTuple):
     c: Number
     m: Number
     y: Number
     k: Number
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/encryption.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/encryption.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/enums.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/enums.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 class VAlign(CoerciveEnum):
     M = "MIDDLE"
     T = "TOP"
     B = "BOTTOM"
 
 class TextEmphasis(CoerciveIntFlag):
+    NONE = 0
     B = 1
     I = 2
     U = 4
 
     @property
     def style(self) -> str: ...
 
@@ -66,20 +67,26 @@
     SINGLE_TOP_LINE = "SINGLE_TOP_LINE"
 
 class TableCellFillMode(CoerciveEnum):
     NONE = "NONE"
     ALL = "ALL"
     ROWS = "ROWS"
     COLUMNS = "COLUMNS"
+    EVEN_ROWS = "EVEN_ROWS"
+    EVEN_COLUMNS = "EVEN_COLUMNS"
 
     def should_fill_cell(self, i: int, j: int) -> bool: ...
 
 class TableSpan(CoerciveEnum):
-    ROW: Literal["ROW"]
-    COL: Literal["COL"]
+    ROW = "ROW"
+    COL = "COL"
+
+class TableHeadingsDisplay(CoerciveIntEnum):
+    NONE = 0
+    ON_TOP_OF_EVERY_PAGE = 1
 
 class RenderStyle(CoerciveEnum):
     D = "DRAW"
     F = "FILL"
     DF = "DRAW_FILL"
     @property
     def operator(self) -> str: ...
@@ -255,7 +262,13 @@
     def none(cls) -> Literal[0]: ...
 
 class EncryptionMethod(Enum):
     NO_ENCRYPTION = 0
     RC4 = 1
     AES_128 = 2
     AES_256 = 3
+
+class TextDirection(CoerciveEnum):
+    LTR = "LTR"
+    RTL = "RTL"
+    TTB = "TTB"
+    BTT = "BTT"
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/fonts.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/fonts.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/fpdf.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/fpdf.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     FileAttachmentAnnotationName,
     MethodReturnValue,
     PageLayout,
     PathPaintRule,
     RenderStyle,
     TableBordersLayout,
     TableCellFillMode,
+    TextDirection,
     TextMarkupType,
     TextMode as TextMode,
     WrapMode as WrapMode,
     XPos as XPos,
     YPos as YPos,
 )
 from .errors import FPDFException as FPDFException
@@ -203,15 +204,15 @@
         zoom: Literal["fullpage", "fullwidth", "real", "default"] | float,
         layout: Literal["single", "continuous", "two", "default"] = "continuous",
     ) -> None: ...
     def set_text_shaping(
         self,
         use_shaping_engine: bool = True,
         features: dict[str, bool] | None = None,
-        direction: Literal["ltr", "rtl"] | None = None,
+        direction: Literal["ltr", "rtl"] | TextDirection | None = None,
         script: str | None = None,
         language: str | None = None,
     ) -> None: ...
     def set_compression(self, compress: bool) -> None: ...
     title: str
     def set_title(self, title: str) -> None: ...
     lang: str
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/graphics_state.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/graphics_state.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/image_datastructures.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/image_datastructures.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/image_parsing.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/image_parsing.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/line_break.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/line_break.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from _typeshed import Incomplete
 from collections.abc import Callable, Sequence
-from typing import Final, Literal, NamedTuple
+from typing import Final, NamedTuple
 
-from .enums import Align, WrapMode
+from .enums import Align, TextDirection, WrapMode
 
 SOFT_HYPHEN: Final[str]
 HYPHEN: Final[str]
 SPACE: Final[str]
 NBSP: Final[str]
 NEWLINE: Final[str]
 FORM_FEED: Final[str]
@@ -56,17 +56,17 @@
     @property
     def string(self) -> str: ...
     @property
     def width(self) -> float: ...
     @property
     def text_shaping_parameters(self): ...
     @property
-    def paragraph_direction(self) -> Literal["L", "R"]: ...
+    def paragraph_direction(self) -> TextDirection: ...
     @property
-    def fragment_direction(self) -> Literal["L", "R"]: ...
+    def fragment_direction(self) -> TextDirection: ...
     def trim(self, index: int) -> None: ...
     def __eq__(self, other: Fragment) -> bool: ...  # type: ignore[override]
     def get_width(self, start: int = 0, end: int | None = None, chars: str | None = None, initial_cs: bool = True) -> float: ...
     def get_character_width(self, character: str, print_sh: bool = False, initial_cs: bool = True): ...
     def render_pdf_text(self, frag_ws, current_ws, word_spacing, adjust_x, adjust_y, h): ...
     def render_pdf_text_ttf(self, frag_ws, word_spacing): ...
     def render_with_text_shaping(self, pos_x: float, pos_y: float, h: float, word_spacing: float) -> str: ...
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/linearization.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/linearization.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/outline.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/outline.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import NamedTuple
 
 from .structure_tree import StructElem
 from .syntax import Destination, PDFObject, PDFString
 
 class OutlineSection(NamedTuple):
     name: str
-    level: str
+    level: int
     page_number: int
     dest: Destination
     struct_elem: StructElem | None = ...
 
 class OutlineItemDictionary(PDFObject):
     title: PDFString
     parent: Incomplete | None
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/output.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/output.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/prefs.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/prefs.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/sign.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/sign.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/structure_tree.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/structure_tree.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/svg.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/svg.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 def convert_miterlimit(incoming): ...
 def clamp_float(min_val, max_val): ...
 def inheritable(value, converter=...): ...
 def optional(value, converter=...): ...
 
 svg_attr_map: dict[str, Callable[[Incomplete], tuple[str, Incomplete]]]
 
-def parse_style(svg_element) -> None: ...
 def apply_styles(stylable, svg_element) -> None: ...
 
 class ShapeBuilder:
     @overload
     @staticmethod
     def new_path(tag, clipping_path: Literal[True]) -> ClippingPath: ...
     @overload
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/syntax.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/syntax.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/table.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/table.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Literal, overload
 
 from PIL import Image
 
 from .drawing import DeviceGray, DeviceRGB
-from .enums import Align, TableBordersLayout, TableCellFillMode, TableSpan, VAlign, WrapMode
+from .enums import Align, TableBordersLayout, TableCellFillMode, TableHeadingsDisplay, TableSpan, VAlign, WrapMode
 from .fonts import FontFace
 from .fpdf import FPDF
 from .util import Padding
 
 DEFAULT_HEADINGS_STYLE: FontFace
 
 class Table:
@@ -36,14 +36,15 @@
         markdown: bool = False,
         text_align: str | Align = "JUSTIFY",
         width: int | None = None,
         wrapmode: WrapMode = ...,
         padding: float | Padding | None = None,
         outer_border_width: float | None = None,
         num_heading_rows: int = 1,
+        repeat_headings: TableHeadingsDisplay | int = 1,
     ) -> None: ...
     def row(self, cells: Iterable[str] = (), style: FontFace | None = None) -> Row: ...
     def render(self) -> None: ...
     def get_cell_border(self, i: int, j: int, cell: Cell) -> str | Literal[0, 1]: ...
 
 class Row:
     cells: list[Cell]
```

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/template.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/template.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/text_region.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/text_region.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/transitions.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/transitions.pyi`

 * *Files identical despite different names*

### Comparing `types-fpdf2-2.7.8.20240423/fpdf-stubs/util.pyi` & `types-fpdf2-2.7.9.20240519/fpdf-stubs/util.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 def get_scale_factor(unit: _Unit | float) -> float: ...
 def convert_unit(
     # to_convert has a recursive type
     to_convert: float | Iterable[float | Iterable[Any]],
     old_unit: str | float,
     new_unit: str | float,
 ) -> float | tuple[float, ...]: ...
+
+ROMAN_NUMERAL_MAP: Final[tuple[tuple[str, int], ...]]
+
+def int2roman(n: int) -> str: ...
 def print_mem_usage(prefix: str) -> None: ...
 def get_mem_usage(prefix: str) -> str: ...
 def get_process_rss() -> str: ...
 def get_process_rss_as_mib() -> float | None: ...
 def get_process_heap_and_stack_sizes() -> tuple[str, str]: ...
 def get_pymalloc_allocated_over_total_size() -> str: ...
 def get_gc_managed_objs_total_size() -> str: ...
```

### Comparing `types-fpdf2-2.7.8.20240423/setup.py` & `types-fpdf2-2.7.9.20240519/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`.
 
 This version of `types-fpdf2` aims to provide accurate annotations
-for `fpdf2==2.7.8`.
+for `fpdf2==2.7.9`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.7.8.20240423",
+      version="2.7.9.20240519",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md",
```

### Comparing `types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/PKG-INFO` & `types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-fpdf2
-Version: 2.7.8.20240423
+Version: 2.7.9.20240519
 Summary: Typing stubs for fpdf2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/fpdf2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `fpdf2`.
 
 This version of `types-fpdf2` aims to provide accurate annotations
-for `fpdf2==2.7.8`.
+for `fpdf2==2.7.9`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/fpdf2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7858e6058b51733f526c6c54035b96a370a12ffc` and was tested
-with mypy 1.9.0, pyright 1.1.358, and
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-fpdf2-2.7.8.20240423/types_fpdf2.egg-info/SOURCES.txt` & `types-fpdf2-2.7.9.20240519/types_fpdf2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

