# Comparing `tmp/pysimplecli-1.0.1.tar.gz` & `tmp/pysimplecli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysimplecli-1.0.1.tar", max compression
+gzip compressed data, was "pysimplecli-1.0.3.tar", max compression
```

## Comparing `pysimplecli-1.0.1.tar` & `pysimplecli-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5726 2024-05-13 18:00:30.368552 pysimplecli-1.0.1/README.md
--rw-r--r--   0        0        0     2262 2024-05-13 19:46:01.049607 pysimplecli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       64 2024-04-29 23:39:55.371531 pysimplecli-1.0.1/simplecli/__init__.py
--rw-r--r--   0        0        0    14885 2024-05-13 17:53:55.198588 pysimplecli-1.0.1/simplecli/simplecli.py
--rw-r--r--   0        0        0     6218 1970-01-01 00:00:00.000000 pysimplecli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5940 2024-05-19 20:48:42.974579 pysimplecli-1.0.3/README.md
+-rw-r--r--   0        0        0     2410 2024-05-19 21:02:16.079271 pysimplecli-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-29 23:39:55.371531 pysimplecli-1.0.3/simplecli/__init__.py
+-rw-r--r--   0        0        0    15063 2024-05-19 20:48:42.974899 pysimplecli-1.0.3/simplecli/simplecli.py
+-rw-r--r--   0        0        0     6432 1970-01-01 00:00:00.000000 pysimplecli-1.0.3/PKG-INFO
```

### Comparing `pysimplecli-1.0.1/README.md` & `pysimplecli-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # pysimplecli
 
 [![codecov](https://codecov.io/gh/inno/pysimplecli/branch/main/graph/badge.svg?token=T6NP6XSKJG)](https://codecov.io/gh/inno/pysimplecli)
 [![CI](https://github.com/inno/pysimplecli/actions/workflows/main.yml/badge.svg)](https://github.com/inno/pysimplecli/actions/workflows/main.yml)
 
-Want to turn your script into a command line utility, but don't want the overhead of [argparse](https://docs.python.org/library/argparse.html)? *You've come to the right place!*
+Want to turn your script into a command line utility, but don't want the overhead of [argparse](https://docs.python.org/library/argparse.html)?
+
+*You've come to the right place!*
 
 Simply import and wrap whatever function you'd like to expose. That's it!
 
 Function variables are turned into CLI parameters, complete with input validation and help text generated from inline comments.
 
 
 ## Install from PyPI
@@ -148,14 +150,22 @@
 
 *Only* simple variable types (`bool`, `float`, `int`, `str`) are currently supported. Mapping and sequence types might be supported in the future but anything else is beyond the scope of this utility.
 
 ### Only one `@wrap` allowed per file
 
 With more than one decorator, it's impossible to tell which function you'd like to wrap. Because of this, we enforce a single `@wrap` per file. Importing modules using `pysimplecli` is supported, as is calling said wrapped functions.
 
+### Truth table for boolean parameters
+
+| Parameter Default | Without Argument | With Argument |
+| --- | --- | --- |
+| `True` | `True` | `False` |
+| `False` | `False` | `True` |
+| no default | `False` | `True` |
+
 ## How It Works
 
 The `wrap` decorator takes the annotated parameters of a given function and maps them to corresponding command-line arguments. It relies heavily on Python's `inspect` and `tokenize` modules to gather parameters, parse comments for parameter descriptions, determine default functionality, etc...  In fact, a core part of this module is a are heavily extended `inspect.Parameter` objects.
 
 ## Why not just use `argparse`?
 
 `argparse` is great for advanced input control. Unfortunately, that level of control means considerably more overhead for simple utilities. To be clear, this is not intended to replace `argparse`. `simplecli` is meant to easily expose a python function as a script.
```

### Comparing `pysimplecli-1.0.1/pyproject.toml` & `pysimplecli-1.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = [
+    "poetry-core>=1.0.0",
+    "poetry-dynamic-versioning>=1.0.0,<2.0.0",
+]
+build-backend = "poetry_dynamic_versioning.backend"
+
 
 [tool.coverage.report]
 show_missing = true
 omit = [
     "*/usr/local/lib*",
     "*/lib/python*/*",
     "lib/*",
@@ -32,15 +36,15 @@
 shell = """
     poetry run coverage run \
     && poetry run coverage html \
     && open htmlcov/index.html
 """
 [tool.poetry]
 name = "pysimplecli"
-version = "1.0.1"
+version = "1.0.3"  # Placeholder
 description = "Easily turn functions into command line utilities"
 authors = ["Clif Bratcher <cebratcher@gmail.com>"]
 readme = "README.md"
 packages = [
     {include = "simplecli"}
 ]
 
@@ -54,14 +58,18 @@
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.8"
 coverage = "^7.4.4"
 flake8 = "^7.0.0"
 poethepoet = "*"
 ruff = "^0.3.4"
 
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff]
 line-length = 79
```

### Comparing `pysimplecli-1.0.1/simplecli/simplecli.py` & `pysimplecli-1.0.3/simplecli/simplecli.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,18 +34,20 @@
 # 2023 - Clif Bratcher WIP
 
 
 class Empty:
     pass
 
 
+class DefaultIfBool:
+    pass
+
+
 _wrapped = False
-# Overloaded placeholder for a potential boolean
-DefaultIfBool = "Crazy going slowly am I, 6, 5, 4, 3, 2, 1, switch!"
-ValueType = Union[type[Empty], bool, float, int, str]
+ValueType = Union[type[DefaultIfBool], type[Empty], bool, float, int, str]
 ArgDict = dict[str, ValueType]
 ArgList = list[str]
 
 
 class Param(inspect.Parameter):
     internal_only: bool  # Do not pass to wrapped function
     _required: bool  # Exit if a value is not present
@@ -204,14 +206,15 @@
                 expected_type(value)
                 return True
             except ValueError:
                 pass
         return passed
 
     def set_value(self, value: ValueType) -> None:
+        result = value
         if self.validate(value) is False:
             raise ValueError(
                 f"'{self.help_name}' must be of type {self.help_type}"
             )
         # Handle datatypes
         args = get_args(self.annotation)
         if args:
@@ -221,21 +224,18 @@
                     contextlib.suppress(ValueError),
                 ):
                     self._value = type_arg(value)
             return
         if value is DefaultIfBool:
             if bool not in self.datatypes:
                 raise ValueError(f"'{self.help_name}' requires a value")
-            if self.default != Empty:
-                self._value = self.annotation(self.default)
-                return
-            else:
-                self._value = self.annotation(True)
-                return
-        self._value = self.annotation(value)
+            result = self.default if self.default is not Empty else True
+        elif bool in self.datatypes and self.default is Empty:
+            result = value
+        self._value = self.annotation(result)
 
 
 def tokenize_string(string: str) -> Generator[TokenInfo, None, None]:
     return generate_tokens(io.StringIO(string).readline)
 
 
 def help_text(
@@ -311,14 +311,20 @@
     missing_params = []
     try:
         for param in params:
             # Positional arguments take precedence
             if pos_args:
                 param.set_value(pos_args.pop(0))
             elif param.name in kw_args:
+                if kw_args[param.name] is DefaultIfBool:
+                    # Invert the default value
+                    param.set_value(
+                        True if param.default is Empty else not param.default
+                    )
+                    continue
                 param.set_value(kw_args[param.name])
                 continue
             elif param.required:
                 missing_params.append(param)
                 continue
     except ValueError as e:
         exit(e.args[0])
```

### Comparing `pysimplecli-1.0.1/PKG-INFO` & `pysimplecli-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysimplecli
-Version: 1.0.1
+Version: 1.0.3
 Summary: Easily turn functions into command line utilities
 Author: Clif Bratcher
 Author-email: cebratcher@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,17 @@
 Description-Content-Type: text/markdown
 
 # pysimplecli
 
 [![codecov](https://codecov.io/gh/inno/pysimplecli/branch/main/graph/badge.svg?token=T6NP6XSKJG)](https://codecov.io/gh/inno/pysimplecli)
 [![CI](https://github.com/inno/pysimplecli/actions/workflows/main.yml/badge.svg)](https://github.com/inno/pysimplecli/actions/workflows/main.yml)
 
-Want to turn your script into a command line utility, but don't want the overhead of [argparse](https://docs.python.org/library/argparse.html)? *You've come to the right place!*
+Want to turn your script into a command line utility, but don't want the overhead of [argparse](https://docs.python.org/library/argparse.html)?
+
+*You've come to the right place!*
 
 Simply import and wrap whatever function you'd like to expose. That's it!
 
 Function variables are turned into CLI parameters, complete with input validation and help text generated from inline comments.
 
 
 ## Install from PyPI
@@ -162,14 +164,22 @@
 
 *Only* simple variable types (`bool`, `float`, `int`, `str`) are currently supported. Mapping and sequence types might be supported in the future but anything else is beyond the scope of this utility.
 
 ### Only one `@wrap` allowed per file
 
 With more than one decorator, it's impossible to tell which function you'd like to wrap. Because of this, we enforce a single `@wrap` per file. Importing modules using `pysimplecli` is supported, as is calling said wrapped functions.
 
+### Truth table for boolean parameters
+
+| Parameter Default | Without Argument | With Argument |
+| --- | --- | --- |
+| `True` | `True` | `False` |
+| `False` | `False` | `True` |
+| no default | `False` | `True` |
+
 ## How It Works
 
 The `wrap` decorator takes the annotated parameters of a given function and maps them to corresponding command-line arguments. It relies heavily on Python's `inspect` and `tokenize` modules to gather parameters, parse comments for parameter descriptions, determine default functionality, etc...  In fact, a core part of this module is a are heavily extended `inspect.Parameter` objects.
 
 ## Why not just use `argparse`?
 
 `argparse` is great for advanced input control. Unfortunately, that level of control means considerably more overhead for simple utilities. To be clear, this is not intended to replace `argparse`. `simplecli` is meant to easily expose a python function as a script.
```

