# Comparing `tmp/arclet_alconna_tools-0.7.3.tar.gz` & `tmp/arclet_alconna_tools-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_alconna_tools-0.7.3.tar", last modified: Sun Apr 21 15:03:44 2024, max compression
+gzip compressed data, was "arclet_alconna_tools-0.7.4.tar", last modified: Sun May 19 09:08:40 2024, max compression
```

## Comparing `arclet_alconna_tools-0.7.3.tar` & `arclet_alconna_tools-0.7.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1091 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.3/LICENSE
--rw-r--r--   0        0        0      749 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.3/README.md
--rw-r--r--   0        0        0     1033 2024-04-21 15:03:44.041103 arclet_alconna_tools-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      991 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    35652 2024-03-15 14:38:48.571519 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     4703 2024-04-05 06:49:19.105061 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    16954 2024-03-15 13:45:46.463804 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      822 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      783 2024-02-28 05:17:30.449506 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4405 2024-04-21 15:02:08.020498 arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 arclet_alconna_tools-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.4/LICENSE
+-rw-r--r--   0        0        0      749 2024-02-28 05:17:30.447506 arclet_alconna_tools-0.7.4/README.md
+-rw-r--r--   0        0        0     1033 2024-05-19 09:08:40.974018 arclet_alconna_tools-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      988 2024-05-19 09:06:37.437865 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2024-02-28 05:17:30.448506 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0    35652 2024-03-15 14:38:48.571519 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     4703 2024-04-05 06:49:19.105061 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    16954 2024-03-15 13:45:46.463804 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       61 2024-05-19 09:04:48.692299 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0     3376 2024-05-19 09:04:58.777547 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/.lang.schema.json
+-rw-r--r--   0        0        0      626 2024-05-19 09:04:48.688781 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/.template.json
+-rw-r--r--   0        0        0      863 2024-05-19 09:03:38.665146 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/.template.schema.json
+-rw-r--r--   0        0        0      193 2024-05-19 09:03:38.664167 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-19 09:06:37.439866 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      820 2024-05-19 09:06:37.430872 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4405 2024-04-21 15:02:08.020498 arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 arclet_alconna_tools-0.7.4/PKG-INFO
```

### Comparing `arclet_alconna_tools-0.7.3/LICENSE` & `arclet_alconna_tools-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/README.md` & `arclet_alconna_tools-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/pyproject.toml` & `arclet_alconna_tools-0.7.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.7.3"
+version = "0.7.4"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "nepattern<1.0.0,>=0.7.0",
-    "arclet-alconna>=1.8.10",
+    "nepattern<1.0.0,>=0.7.3",
+    "arclet-alconna>=1.8.12",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/__init__.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .config import lang as _lang  # noqa
+from .i18n import lang as lang  # noqa
 from .construct import AlconnaDecorate as AlconnaDecorate
 from .construct import AlconnaFire as AlconnaFire
 from .construct import AlconnaFormat as AlconnaFormat
 from .construct import AlconnaString as AlconnaString
 from .construct import Argument as Argument
 from .construct import Executor as Executor
 from .construct import alconna_from_format
```

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/actions.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/checker.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/construct.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/construct.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/debug.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/formatter.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/en-US.json` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'./.lang.schema.json'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "./.lang.schema.json",
     "tools": {
         "actions.cooldown": "Your action is too frequent",
         "actions.exclusion": "{left} and {right} cannot be both matched",
         "actions.inclusion": "{target} must be matched",
         "construct.decorate_error": "This action must behind a @xxx.command()",
         "construct.format_error": "Unidentified segment: {target}",
         "construct.func_name_error": "function name can not start with '_'",
```

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'$schema'": "'./.lang.schema.json'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "$schema": "./.lang.schema.json",
     "tools": {
         "actions.cooldown": "\u64cd\u4f5c\u8fc7\u4e8e\u9891\u7e41",
         "actions.exclusion": "{left} \u4e0e {right} \u4e0d\u80fd\u540c\u65f6\u5b58\u5728",
         "actions.inclusion": "{target} \u5fc5\u987b\u5b58\u5728",
         "construct.decorate_error": "\u8be5\u884c\u4e3a\u5fc5\u987b\u5728 @xxx.command() \u4e4b\u540e",
         "construct.format_error": "\u4e0d\u660e\u5b57\u6bb5: {target}",
         "construct.func_name_error": "\u51fd\u6570\u540d\u4e0d\u80fd\u4ee5 '_' \u5f00\u5934",
```

### Comparing `arclet_alconna_tools-0.7.3/src/arclet/alconna/tools/pattern.py` & `arclet_alconna_tools-0.7.4/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_tools-0.7.3/PKG-INFO` & `arclet_alconna_tools-0.7.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-tools
-Version: 0.7.3
+Version: 0.7.4
 Summary: Builtin Tools for Alconna
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
-Requires-Dist: nepattern<1.0.0,>=0.7.0
-Requires-Dist: arclet-alconna>=1.8.10
+Requires-Dist: nepattern<1.0.0,>=0.7.3
+Requires-Dist: arclet-alconna>=1.8.12
 Description-Content-Type: text/markdown
 
 # Alconna Tools
 
 Provider various tools for Alconna
 
 Extensions:
```

