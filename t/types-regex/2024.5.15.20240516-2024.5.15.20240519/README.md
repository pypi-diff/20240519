# Comparing `tmp/types-regex-2024.5.15.20240516.tar.gz` & `tmp/types-regex-2024.5.15.20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2024.5.15.20240516.tar", last modified: Thu May 16 02:21:13 2024, max compression
+gzip compressed data, was "types-regex-2024.5.15.20240519.tar", last modified: Sun May 19 02:23:41 2024, max compression
```

## Comparing `types-regex-2024.5.15.20240516.tar` & `types-regex-2024.5.15.20240519.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:13.399429 types-regex-2024.5.15.20240516/
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-16 02:21:12.000000 types-regex-2024.5.15.20240516/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 02:21:12.000000 types-regex-2024.5.15.20240516/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-16 02:21:13.399429 types-regex-2024.5.15.20240516/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:13.399429 types-regex-2024.5.15.20240516/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 02:21:12.000000 types-regex-2024.5.15.20240516/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 02:20:58.000000 types-regex-2024.5.15.20240516/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 02:20:58.000000 types-regex-2024.5.15.20240516/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-16 02:20:58.000000 types-regex-2024.5.15.20240516/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:12.000000 types-regex-2024.5.15.20240516/regex-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-05-16 02:20:58.000000 types-regex-2024.5.15.20240516/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 02:21:13.399429 types-regex-2024.5.15.20240516/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-16 02:21:12.000000 types-regex-2024.5.15.20240516/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 02:21:13.399429 types-regex-2024.5.15.20240516/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-16 02:21:13.000000 types-regex-2024.5.15.20240516/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 02:21:13.000000 types-regex-2024.5.15.20240516/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 02:21:13.000000 types-regex-2024.5.15.20240516/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 02:21:13.000000 types-regex-2024.5.15.20240516/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:41.978855 types-regex-2024.5.15.20240519/
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 02:23:41.978855 types-regex-2024.5.15.20240519/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:41.978855 types-regex-2024.5.15.20240519/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 02:23:25.000000 types-regex-2024.5.15.20240519/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 02:23:25.000000 types-regex-2024.5.15.20240519/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-19 02:23:25.000000 types-regex-2024.5.15.20240519/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/regex-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19518 2024-05-19 02:23:25.000000 types-regex-2024.5.15.20240519/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:23:41.978855 types-regex-2024.5.15.20240519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:41.978855 types-regex-2024.5.15.20240519/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 02:23:41.000000 types-regex-2024.5.15.20240519/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2024.5.15.20240516/CHANGELOG.md` & `types-regex-2024.5.15.20240519/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2024.5.15.20240519 (2024-05-19)
+
+Mark pos-only __class_getitem__ args (#11970)
+
+Use assignment instead of annotation in third party enums (#11957)
+
 ## 2024.5.15.20240516 (2024-05-16)
 
 [stubsabot] Bump regex to 2024.5.15 (#11918)
 
 Co-authored-by: stubsabot <>
 
 ## 2024.5.10.20240512 (2024-05-12)
```

### Comparing `types-regex-2024.5.15.20240516/PKG-INFO` & `types-regex-2024.5.15.20240519/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.5.15.20240516
+Version: 2024.5.15.20240519
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.5.15`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `77d6947479a7ba2cddc6b50d5600a941a84ca4d4` and was tested
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
 with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-regex-2024.5.15.20240516/regex-stubs/_regex.pyi` & `types-regex-2024.5.15.20240519/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.5.15.20240516/regex-stubs/regex.pyi` & `types-regex-2024.5.15.20240519/regex-stubs/regex.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
         concurrent: bool | None = None,
         partial: bool = False,
         timeout: float | None = None,
     ) -> _regex.Scanner[bytes]: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self) -> Self: ...
     if sys.version_info >= (3, 9):
-        def __class_getitem__(cls, item: Any) -> GenericAlias: ...
+        def __class_getitem__(cls, item: Any, /) -> GenericAlias: ...
 
 @final
 class Match(Generic[AnyStr]):
     @property
     def pos(self) -> int: ...
     @property
     def endpos(self) -> int: ...
@@ -645,8 +645,8 @@
     @overload
     def __getitem__(self, key: Literal[0], /) -> AnyStr: ...
     @overload
     def __getitem__(self, key: int | str, /) -> AnyStr | Any: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self) -> Self: ...
     if sys.version_info >= (3, 9):
-        def __class_getitem__(cls, item: Any) -> GenericAlias: ...
+        def __class_getitem__(cls, item: Any, /) -> GenericAlias: ...
```

### Comparing `types-regex-2024.5.15.20240516/setup.py` & `types-regex-2024.5.15.20240519/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.5.15`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `77d6947479a7ba2cddc6b50d5600a941a84ca4d4` and was tested
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
 with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2024.5.15.20240516",
+      version="2024.5.15.20240519",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2024.5.15.20240516/types_regex.egg-info/PKG-INFO` & `types-regex-2024.5.15.20240519/types_regex.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.5.15.20240516
+Version: 2024.5.15.20240519
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.5.15`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `77d6947479a7ba2cddc6b50d5600a941a84ca4d4` and was tested
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
 with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

