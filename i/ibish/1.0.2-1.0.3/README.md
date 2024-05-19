# Comparing `tmp/ibish-1.0.2.tar.gz` & `tmp/ibish-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibish-1.0.2.tar", max compression
+gzip compressed data, was "ibish-1.0.3.tar", max compression
```

## Comparing `ibish-1.0.2.tar` & `ibish-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-03-29 11:01:15.396134 ibish-1.0.2/LICENSE
--rw-r--r--   0        0        0       33 2024-03-29 11:01:15.396134 ibish-1.0.2/README.md
--rw-r--r--   0        0        0     6790 2024-03-29 11:01:53.248355 ibish-1.0.2/ibish/__init__.py
--rw-r--r--   0        0        0     7713 2024-03-29 11:01:15.396134 ibish-1.0.2/ibish/compiler.py
--rw-r--r--   0        0        0     6415 2024-03-29 11:01:55.300366 ibish-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1545 1970-01-01 00:00:00.000000 ibish-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-19 14:48:47.708545 ibish-1.0.3/LICENSE
+-rw-r--r--   0        0        0       33 2024-05-19 14:48:47.708545 ibish-1.0.3/README.md
+-rw-r--r--   0        0        0     6874 2024-05-19 14:49:27.276437 ibish-1.0.3/ibish/__init__.py
+-rw-r--r--   0        0        0     7713 2024-05-19 14:48:47.708545 ibish-1.0.3/ibish/compiler.py
+-rw-r--r--   0        0        0     6153 2024-05-19 14:49:29.220466 ibish-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1538 1970-01-01 00:00:00.000000 ibish-1.0.3/PKG-INFO
```

### Comparing `ibish-1.0.2/LICENSE` & `ibish-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ibish-1.0.2/ibish/__init__.py` & `ibish-1.0.3/ibish/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     replace_parameter,
     rewrite_join,
 )
 from ibis.common.patterns import replace
 
 from ibish.compiler import Offset, translate
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 __all__ = ("connect",)
 
 
 @replace(PandasJoin)
 def sort_before_join(_):
     return _.copy(
@@ -235,12 +235,16 @@
     )
     pipeline = backend.explain(expr)
     print(pipeline)  # noqa: T201
 
     result = expr.execute()
     print(result)  # noqa: T201
 
-    join = t.join(t, ["year"]).select("year")
+    join = (
+        t.filter(lambda t: t.year == 2007)
+        .join(backend.table("q"), ["year"])
+        .select("year")
+    )
     print(backend.explain(join))  # noqa: T201
 
     result = join.execute()
     print(result)  # noqa: T201
```

### Comparing `ibish-1.0.2/ibish/compiler.py` & `ibish-1.0.3/ibish/compiler.py`

 * *Files identical despite different names*

### Comparing `ibish-1.0.2/pyproject.toml` & `ibish-1.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ibish"
-version = "1.0.2"
+version = "1.0.3"
 packages = [{ include = "ibish" }]
 homepage = "https://github.com/cpcloud/ibish"
 repository = "https://github.com/cpcloud/ibish"
 description = "The Unix backend for Ibis"
 authors = ["Ibis Maintainers <maintainers@ibis-project.org>"]
 maintainers = ["Ibis Maintainers <maintainers@ibis-project.org>"]
 license = "Apache-2.0"
@@ -26,15 +26,15 @@
 ]
 
 [tool.poetry.urls]
 "Issue Tracker" = "https://github.com/cpcloud/ibish/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ibis-framework = "^8.0.0"
+ibis-framework = "^9"
 pandas = "^2.2.1"
 pyarrow = "^15.0.2"
 
 [tool.poetry.group.dev.dependencies]
 codespell = { version = ">=2.2.6,<3", extras = [
   "hard-encoding-detection",
   "toml",
@@ -58,45 +58,29 @@
 [tool.pytest.ini_options]
 doctest_optionflags = [
   "NORMALIZE_WHITESPACE",
   "IGNORE_EXCEPTION_DETAIL",
   "ELLIPSIS",
 ]
 xfail_strict = true
-addopts = [
-  "--strict-markers",
-  "--strict-config",
-  "--benchmark-disable",
-  "--benchmark-group-by=name",
-  "--benchmark-sort=name",
-]
+addopts = ["--strict-markers", "--strict-config"]
 norecursedirs = [
-  "**/snapshots",
-  ".benchmarks",
   ".direnv",
   ".git",
   ".github",
-  ".hypothesis",
   ".pytest_cache",
-  ".streamlit",
-  "LICENSES",
-  "ci",
-  "conda-lock",
-  "dev",
-  "docker",
-  "docs",
   "nix",
   "result*",
 ]
 empty_parameter_set_mark = "fail_at_collect"
 
 [tool.ruff]
 line-length = 88
 respect-gitignore = true
-exclude = [".direnv", "result-*", "*_py310.py", "decompiled.py"]
+exclude = [".direnv", "result-*"]
 target-version = "py39"
 
 [tool.ruff.lint]
 select = [
   "B",   # flake8-bugbear
   "BLE", # flake8-blind-except
   "C4",  # comprehensions
```

### Comparing `ibish-1.0.2/PKG-INFO` & `ibish-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibish
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Unix backend for Ibis
 Home-page: https://github.com/cpcloud/ibish
 License: Apache-2.0
 Author: Ibis Maintainers
 Author-email: maintainers@ibis-project.org
 Maintainer: Ibis Maintainers
 Maintainer-email: maintainers@ibis-project.org
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Dist: ibis-framework (>=8.0.0,<9.0.0)
+Requires-Dist: ibis-framework (>=9,<10)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Project-URL: Issue Tracker, https://github.com/cpcloud/ibish/issues
 Project-URL: Repository, https://github.com/cpcloud/ibish
 Description-Content-Type: text/markdown
 
 # ibish
```

