# Comparing `tmp/types-flake8-7.0.0.20240511.tar.gz` & `tmp/types-flake8-7.0.0.20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-7.0.0.20240511.tar", last modified: Sat May 11 02:18:07 2024, max compression
+gzip compressed data, was "types-flake8-7.0.0.20240519.tar", last modified: Sun May 19 02:24:55 2024, max compression
```

## Comparing `types-flake8-7.0.0.20240511.tar` & `types-flake8-7.0.0.20240519.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.430169 types-flake8-7.0.0.20240511/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-11 02:18:06.000000 types-flake8-7.0.0.20240511/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:18:06.000000 types-flake8-7.0.0.20240511/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/flake8-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-11 02:18:06.000000 types-flake8-7.0.0.20240511/flake8-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/_compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/flake8-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/api/legacy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/checker.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/defaults.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/discover_files.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/flake8-stubs/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/formatting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/formatting/_windows_color.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/formatting/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/formatting/default.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/flake8-stubs/main/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/main/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/main/application.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/main/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/main/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/main/options.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/flake8-stubs/options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/options/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/options/aggregator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/options/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/options/manager.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/options/parse_args.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/flake8-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/plugins/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/plugins/finder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/plugins/pycodestyle.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/plugins/pyflakes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/plugins/reporter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/processor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:06.000000 types-flake8-7.0.0.20240511/flake8-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/statistics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/style_guide.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 02:17:34.000000 types-flake8-7.0.0.20240511/flake8-stubs/violation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:18:07.430169 types-flake8-7.0.0.20240511/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-11 02:18:06.000000 types-flake8-7.0.0.20240511/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:07.426169 types-flake8-7.0.0.20240511/types_flake8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-11 02:18:07.000000 types-flake8-7.0.0.20240511/types_flake8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-11 02:18:07.000000 types-flake8-7.0.0.20240511/types_flake8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:18:07.000000 types-flake8-7.0.0.20240511/types_flake8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 02:18:07.000000 types-flake8-7.0.0.20240511/types_flake8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 02:18:07.000000 types-flake8-7.0.0.20240511/types_flake8.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.011810 types-flake8-7.0.0.20240519/flake8-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/flake8-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/_compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.011810 types-flake8-7.0.0.20240519/flake8-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/api/legacy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/checker.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/defaults.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/discover_files.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.011810 types-flake8-7.0.0.20240519/flake8-stubs/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/formatting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/formatting/_windows_color.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/formatting/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/formatting/default.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/flake8-stubs/main/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/main/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/main/application.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/main/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/main/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/main/options.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/flake8-stubs/options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/options/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/options/aggregator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/options/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/options/manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/options/parse_args.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/flake8-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/plugins/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/plugins/finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/plugins/pycodestyle.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/plugins/pyflakes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/plugins/reporter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/processor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/flake8-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/statistics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/style_guide.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 02:23:25.000000 types-flake8-7.0.0.20240519/flake8-stubs/violation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:24:55.015810 types-flake8-7.0.0.20240519/types_flake8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/types_flake8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/types_flake8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/types_flake8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/types_flake8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 02:24:54.000000 types-flake8-7.0.0.20240519/types_flake8.egg-info/top_level.txt
```

### Comparing `types-flake8-7.0.0.20240511/PKG-INFO` & `types-flake8-7.0.0.20240519/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8
-Version: 7.0.0.20240511
+Version: 7.0.0.20240519
 Summary: Typing stubs for flake8
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-flake8` aims to provide accurate annotations
 for `flake8==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/api/legacy.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/api/legacy.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/checker.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/checker.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/exceptions.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/formatting/base.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/formatting/base.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/formatting/default.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/formatting/default.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/main/application.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/main/application.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/options/manager.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/options/manager.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import argparse
 from _typeshed import Incomplete
 from collections.abc import Callable, Sequence
 from enum import Enum
 from logging import Logger
-from typing import Any, Final
+from typing import Any
 
 from ..plugins.finder import Plugins
 
 LOG: Logger
 
 class _ARG(Enum):
-    NO: Final = 1
+    NO = 1
 
 class Option:
     short_option_name: Incomplete
     long_option_name: Incomplete
     option_args: Incomplete
     action: Incomplete
     default: Incomplete
```

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/plugins/finder.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/plugins/finder.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/plugins/pycodestyle.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/plugins/pycodestyle.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/plugins/pyflakes.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/plugins/pyflakes.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/processor.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/processor.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/statistics.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/statistics.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/style_guide.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/style_guide.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from .formatting.base import BaseFormatter
 from .statistics import Statistics
 
 __all__ = ("StyleGuide",)
 
 class Selected(enum.Enum):
-    Explicitly: str
-    Implicitly: str
+    Explicitly = "explicitly selected"
+    Implicitly = "implicitly selected"
 
 class Ignored(enum.Enum):
-    Explicitly: str
-    Implicitly: str
+    Explicitly = "explicitly ignored"
+    Implicitly = "implicitly ignored"
 
 class Decision(enum.Enum):
-    Ignored: str
-    Selected: str
+    Ignored = "ignored error"
+    Selected = "selected error"
 
 class DecisionEngine:
     cache: Incomplete
     selected_explicitly: Incomplete
     ignored_explicitly: Incomplete
     selected: Incomplete
     ignored: Incomplete
```

### Comparing `types-flake8-7.0.0.20240511/flake8-stubs/utils.pyi` & `types-flake8-7.0.0.20240519/flake8-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-7.0.0.20240511/setup.py` & `types-flake8-7.0.0.20240519/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-flake8` aims to provide accurate annotations
 for `flake8==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240511",
+      version="7.0.0.20240519",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8.md",
```

### Comparing `types-flake8-7.0.0.20240511/types_flake8.egg-info/PKG-INFO` & `types-flake8-7.0.0.20240519/types_flake8.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8
-Version: 7.0.0.20240511
+Version: 7.0.0.20240519
 Summary: Typing stubs for flake8
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-flake8` aims to provide accurate annotations
 for `flake8==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `5445a4a243f5e41c9b4ab8b4ffa93da0820218bb` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
 pytype 2024.4.11.
```

### Comparing `types-flake8-7.0.0.20240511/types_flake8.egg-info/SOURCES.txt` & `types-flake8-7.0.0.20240519/types_flake8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

