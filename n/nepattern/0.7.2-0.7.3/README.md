# Comparing `tmp/nepattern-0.7.2.tar.gz` & `tmp/nepattern-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.7.2.tar", last modified: Thu Apr 25 09:56:26 2024, max compression
+gzip compressed data, was "nepattern-0.7.3.tar", last modified: Sun May 19 08:35:10 2024, max compression
```

## Comparing `nepattern-0.7.2.tar` & `nepattern-0.7.3.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.2/LICENSE
--rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.2/README.md
--rw-r--r--   0        0        0     3058 2024-04-25 09:22:34.763668 nepattern-0.7.2/nepattern/__init__.py
--rw-r--r--   0        0        0    29346 2024-04-25 09:49:34.487307 nepattern-0.7.2/nepattern/base.py
--rw-r--r--   0        0        0     4148 2024-04-25 09:22:34.747677 nepattern-0.7.2/nepattern/context.py
--rw-r--r--   0        0        0     1525 2024-04-25 09:22:43.597720 nepattern-0.7.2/nepattern/context.pyi
--rw-r--r--   0        0        0    30111 2024-04-25 09:28:25.729185 nepattern-0.7.2/nepattern/core.py
--rw-r--r--   0        0        0    34323 2024-04-25 09:28:38.979141 nepattern-0.7.2/nepattern/core.pyi
--rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/exception.py
--rw-r--r--   0        0        0     6761 2024-04-25 09:31:42.239930 nepattern-0.7.2/nepattern/func.py
--rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.7.2/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0     5611 2024-04-23 09:38:29.355325 nepattern-0.7.2/nepattern/main.py
--rw-r--r--   0        0        0     2237 2024-04-25 09:22:43.626718 nepattern-0.7.2/nepattern/main.pyi
--rw-r--r--   0        0        0     1071 2024-04-25 09:22:43.620721 nepattern-0.7.2/nepattern/util.py
--rw-r--r--   0        0        0     2065 2024-04-25 09:56:26.393732 nepattern-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.3/LICENSE
+-rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.3/README.md
+-rw-r--r--   0        0        0     3058 2024-04-25 09:22:34.763668 nepattern-0.7.3/nepattern/__init__.py
+-rw-r--r--   0        0        0    29342 2024-05-07 16:07:56.796778 nepattern-0.7.3/nepattern/base.py
+-rw-r--r--   0        0        0     4148 2024-05-07 16:07:56.460570 nepattern-0.7.3/nepattern/context.py
+-rw-r--r--   0        0        0     1525 2024-05-07 16:07:56.436566 nepattern-0.7.3/nepattern/context.pyi
+-rw-r--r--   0        0        0    30111 2024-05-07 16:08:23.332857 nepattern-0.7.3/nepattern/core.py
+-rw-r--r--   0        0        0    34505 2024-05-19 08:30:30.186320 nepattern-0.7.3/nepattern/core.pyi
+-rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.3/nepattern/exception.py
+-rw-r--r--   0        0        0     6761 2024-05-07 16:07:56.756733 nepattern-0.7.3/nepattern/func.py
+-rw-r--r--   0        0        0       61 2024-05-19 07:40:29.008976 nepattern-0.7.3/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0     1471 2024-05-19 07:42:18.054639 nepattern-0.7.3/nepattern/i18n/.lang.schema.json
+-rw-r--r--   0        0        0      313 2024-05-19 07:42:10.249725 nepattern-0.7.3/nepattern/i18n/.template.json
+-rw-r--r--   0        0        0      863 2024-05-19 07:40:18.353881 nepattern-0.7.3/nepattern/i18n/.template.schema.json
+-rw-r--r--   0        0        0      193 2024-05-19 07:40:18.353881 nepattern-0.7.3/nepattern/i18n/__init__.py
+-rw-r--r--   0        0        0      518 2024-05-19 07:42:40.465771 nepattern-0.7.3/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      507 2024-05-19 07:42:43.510322 nepattern-0.7.3/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0     5611 2024-04-23 09:38:29.355325 nepattern-0.7.3/nepattern/main.py
+-rw-r--r--   0        0        0     2237 2024-05-07 16:07:56.708713 nepattern-0.7.3/nepattern/main.pyi
+-rw-r--r--   0        0        0     1000 2024-05-19 08:04:12.972632 nepattern-0.7.3/nepattern/util.py
+-rw-r--r--   0        0        0     2065 2024-05-19 08:35:10.200728 nepattern-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.3/PKG-INFO
```

### Comparing `nepattern-0.7.2/LICENSE` & `nepattern-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/README.md` & `nepattern-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/__init__.py` & `nepattern-0.7.3/nepattern/__init__.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/base.py` & `nepattern-0.7.3/nepattern/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         except MatchFailed as e:
             if default is Empty:
                 return ValidateResult(error=e, flag=ResultFlag.ERROR)
             return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
 
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, DirectPattern) and self.target == other.target
-    
+
     def copy(self):
         return DirectPattern(self.target, self.alias)
 
 
 class DirectTypePattern(BasePattern[TOrigin, TOrigin, Literal[MatchMode.KEEP]]):
     """直接类型判断"""
```

### Comparing `nepattern-0.7.2/nepattern/context.py` & `nepattern-0.7.3/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/context.pyi` & `nepattern-0.7.3/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/core.py` & `nepattern-0.7.3/nepattern/core.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/core.pyi` & `nepattern-0.7.3/nepattern/core.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -135,23 +135,23 @@
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[T], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TInput, TInput, Literal[MatchMode.KEEP]],
+        self: BasePattern[TInput1, TInput1, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
-        accepts: type[TInput],
+        accepts: type[TInput1],
         origin: Any = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TInput], bool]] | None = None,
+        validators: list[Callable[[TInput1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput1, TInput1, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         addition_accepts: BasePattern[Any, TInput1, Any],
@@ -246,571 +246,571 @@
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
         validators: list[Callable[[str], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]],
+        self: BasePattern[TOrigin1, str | TOrigin1, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         converter: (
             Callable[
-                [BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]],
-                TOrigin | None,
+                [BasePattern[TOrigin1, str | TOrigin1, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         previous: None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, str | TOrigin | TInput1, Literal[MatchMode.REGEX_CONVERT]],
+        self: BasePattern[TOrigin1, str | TOrigin1 | TInput1, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         previous: (
-            BasePattern[str | TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]]
+            BasePattern[str | TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]]
             | BasePattern[str, TInput1, Literal[MatchMode.TYPE_CONVERT]]
-            | BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]]
+            | BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]]
         ),
         converter: (
             Callable[
                 [
-                    BasePattern[TOrigin, str | TOrigin | TInput1, Literal[MatchMode.REGEX_CONVERT]],
+                    BasePattern[TOrigin1, str | TOrigin1 | TInput1, Literal[MatchMode.REGEX_CONVERT]],
                     re.Match[str],
                 ],
-                TOrigin | None,
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]],
+        self: BasePattern[TOrigin1, str | TOrigin1, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         previous: (
-            BasePattern[str | TOrigin, str | TOrigin, Literal[MatchMode.VALUE_OPERATE]]
+            BasePattern[str | TOrigin1, str | TOrigin1, Literal[MatchMode.VALUE_OPERATE]]
             | BasePattern[str, str, Literal[MatchMode.VALUE_OPERATE]]
-            | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]]
         ),
         converter: (
             Callable[
-                [BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]],
-                TOrigin | None,
+                [BasePattern[TOrigin1, str | TOrigin1, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         converter: Callable[
-            [BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None
+            [BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin1 | None
         ],
         origin: None = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
         ],
         origin: None = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         addition_accepts: BasePattern[Any, TInput1, Any],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
         ],
         origin: None = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         addition_accepts: BasePattern[Any, TInput2, Any],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2],
-            TOrigin | None,
+            [BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2],
+            TOrigin1 | None,
         ],
         origin: None = None,
         alias: str | None = None,
         previous: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         converter: (
-            Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None] | None
+            Callable[[BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin1 | None] | None
         ) = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         accepts: type[TInput1],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+                [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
             ]
             | None
         ) = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         addition_accepts: BasePattern[Any, TInput1, Any],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+                [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
             ]
             | None
         ) = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         accepts: type[TInput1],
         addition_accepts: BasePattern[Any, TInput2, Any],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2],
-                TOrigin | None,
+                [BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         previous: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         previous: BasePattern[TInput1, Any, Literal[MatchMode.TYPE_CONVERT]],
         converter: Callable[
-            [BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None
+            [BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin1 | None
         ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         previous: BasePattern[TInput1, Any, Literal[MatchMode.TYPE_CONVERT]],
         converter: (
             Callable[
-                [BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None
+                [BasePattern[TOrigin1, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin1 | None
             ]
             | None
         ) = None,
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
         ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TOrigin1 | TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         previous: (
-            BasePattern[TOrigin | TInput1, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]]
-            | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]]
+            BasePattern[TOrigin1 | TInput1, TOrigin1 | TInput1, Literal[MatchMode.VALUE_OPERATE]]
+            | BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]]
             | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]]
         ),
         converter: (
             Callable[
-                [BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1],
-                TOrigin | None,
+                [BasePattern[TOrigin1, TOrigin1 | TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
-            TOrigin | None,
+            [BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+            TOrigin1 | None,
         ],
         alias: str | None = None,
         origin: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         accepts: type[TInput1],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
-                TOrigin | None,
+                [BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
         ],
         alias: str | None = None,
         origin: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         accepts: type[TInput1],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+                [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
             ]
             | None
         ) = None,
         alias: str | None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
-            TOrigin | None,
+            [BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+            TOrigin1 | None,
         ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
-                TOrigin | None,
+                [BasePattern[TOrigin1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
         accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+            [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
         ],
         alias: str | None = None,
         origin: None = None,
         accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None
+                [BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin1 | None
             ]
             | None
         ) = None,
         alias: str | None = None,
         accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         previous: (
             BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
             | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]]
             | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
         ),
         addition_accepts: BasePattern[Any, TInput3, Any],
         converter: Callable[
             [
-                BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+                BasePattern[TOrigin1, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
                 TInput1 | TInput3,
             ],
-            TOrigin | None,
+            TOrigin1 | None,
         ],
         alias: str | None = None,
         origin: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         accepts: type[TInput1],
         previous: (
             BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
             | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]]
             | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]]
         ),
         addition_accepts: BasePattern[Any, TInput3, Any],
         converter: (
             Callable[
                 [
-                    BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+                    BasePattern[TOrigin1, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
                     TInput1 | TInput3,
                 ],
-                TOrigin | None,
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         accepts: type[TInput1],
         previous: (
             BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]]
             | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]]
             | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]]
         ),
         addition_accepts: BasePattern[Any, TInput3, Any],
         converter: Callable[
-            [BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3],
-            TOrigin | None,
+            [BasePattern[TOrigin1, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3],
+            TOrigin1 | None,
         ],
         origin: None = None,
         alias: str | None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin1, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         accepts: type[TInput1],
         previous: (
             BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]]
             | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]]
             | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]]
         ),
         addition_accepts: BasePattern[Any, TInput3, Any],
         converter: (
             Callable[
-                [BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3],
-                TOrigin | None,
+                [BasePattern[TOrigin1, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3],
+                TOrigin1 | None,
             ]
             | None
         ) = None,
         alias: str | None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
+        self: BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
-        origin: type[TOrigin],
+        origin: type[TOrigin1],
         converter: Callable[
-            [BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None
+            [BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]], TOrigin1], TOrigin1 | None
         ],
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        self: BasePattern[TOrigin1, TOrigin1 | TInput1, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
-        origin: type[TOrigin],
-        previous: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        origin: type[TOrigin1],
+        previous: BasePattern[TOrigin1, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         converter: Callable[
-            [BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]], TOrigin],
-            TOrigin | None,
+            [BasePattern[TOrigin1, TOrigin1 | TInput1, Literal[MatchMode.VALUE_OPERATE]], TOrigin1],
+            TOrigin1 | None,
         ],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TOrigin | TInput2, Literal[MatchMode.VALUE_OPERATE]],
+        self: BasePattern[TOrigin1, TOrigin1 | TInput2, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
-        origin: type[TOrigin],
-        previous: BasePattern[TOrigin, TOrigin | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        origin: type[TOrigin1],
+        previous: BasePattern[TOrigin1, TOrigin1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         converter: Callable[
-            [BasePattern[TOrigin, TOrigin | TInput2, Literal[MatchMode.VALUE_OPERATE]], TOrigin],
-            TOrigin | None,
+            [BasePattern[TOrigin1, TOrigin1 | TInput2, Literal[MatchMode.VALUE_OPERATE]], TOrigin1],
+            TOrigin1 | None,
         ],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
+        self: BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
-        origin: type[TOrigin],
-        previous: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
+        origin: type[TOrigin1],
+        previous: BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]],
         converter: Callable[
-            [BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None
+            [BasePattern[TOrigin1, TOrigin1, Literal[MatchMode.VALUE_OPERATE]], TOrigin1], TOrigin1 | None
         ],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
-        validators: list[Callable[[TOrigin], bool]] | None = None,
+        validators: list[Callable[[TOrigin1], bool]] | None = None,
     ): ...
     def refresh(self): ...
     def __calc_hash__(self): ...
     def __calc_repr__(self): ...
     def __calc_eq__(self, other): ...
     def __repr__(self): ...
     def __str__(self): ...
```

### Comparing `nepattern-0.7.2/nepattern/func.py` & `nepattern-0.7.3/nepattern/func.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/main.py` & `nepattern-0.7.3/nepattern/main.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/main.pyi` & `nepattern-0.7.3/nepattern/main.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.2/nepattern/util.py` & `nepattern-0.7.3/nepattern/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import dataclasses
-from pathlib import Path
 import sys
 from typing import TYPE_CHECKING, List, Pattern, Union
 
-from tarina.lang import lang
+from .i18n import lang as lang
 
 if sys.version_info >= (3, 9):  # pragma: no cover
     from types import GenericAlias as CGenericAlias  # noqa
 else:  # pragma: no cover
     CGenericAlias: type = type(List[int])  # noqa
 
 if sys.version_info >= (3, 10):  # pragma: no cover
@@ -29,10 +28,7 @@
 GenericAlias: type = type(List[int])
 UnionType: type = type(Union[int, str])
 
 
 @dataclasses.dataclass
 class RawStr:
     value: str
-
-
-lang.load(Path(__file__).parent / "i18n")
```

### Comparing `nepattern-0.7.2/pyproject.toml` & `nepattern-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "nepattern"
-version = "0.7.2"
+version = "0.7.3"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
-    "tarina>=0.4.1",
+    "tarina>=0.5.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "typing",
     "pattern",
     "converter",
```

### Comparing `nepattern-0.7.2/PKG-INFO` & `nepattern-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.7.2
+Version: 0.7.3
 Summary: a complex pattern, support typing
 Keywords: typing,pattern,converter,validator
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Project-URL: Repository, https://github.com/ArcletProject/NEPattern
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions>=4.5.0
-Requires-Dist: tarina>=0.4.1
+Requires-Dist: tarina>=0.5.1
 Description-Content-Type: text/markdown
 
 # NEPattern
 
 [![Licence](https://img.shields.io/github/license/ArcletProject/NEPattern)](https://github.com/ArcletProject/NEPattern/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/nepattern)](https://pypi.org/project/nepattern)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nepattern)](https://www.python.org/)
```

