# Comparing `tmp/clargs-0.6.1.tar.gz` & `tmp/clargs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clargs-0.6.1.tar", last modified: Fri Jul 28 18:38:40 2023, max compression
+gzip compressed data, was "clargs-0.7.0.tar", last modified: Sun May 19 18:35:01 2024, max compression
```

## Comparing `clargs-0.6.1.tar` & `clargs-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-28 18:38:31.000000 clargs-0.6.1/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 18:38:31.000000 clargs-0.6.1/.github/workflows/upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 18:38:31.000000 clargs-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 18:38:31.000000 clargs-0.6.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-28 18:38:40.791039 clargs-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-07-28 18:38:31.000000 clargs-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/0_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/1_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/2_show_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/3_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/4_parse_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    20370 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/5_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-28 18:38:31.000000 clargs-0.6.1/examples/__generate_example_output__.sh
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 18:38:31.000000 clargs-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 18:38:40.791039 clargs-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.787039 clargs-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/src/clargs/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/aap_from_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/clargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-28 18:38:31.000000 clargs-0.6.1/src/clargs/helper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/src/clargs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 18:38:40.000000 clargs-0.6.1/src/clargs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 18:38:40.791039 clargs-0.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 18:38:31.000000 clargs-0.6.1/test/test_docsparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-07-28 18:38:31.000000 clargs-0.6.1/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-28 18:38:31.000000 clargs-0.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.082004 clargs-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.086004 clargs-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 18:34:49.000000 clargs-0.7.0/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-19 18:34:49.000000 clargs-0.7.0/.github/workflows/upload.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 18:34:49.000000 clargs-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-19 18:34:49.000000 clargs-0.7.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-19 18:35:01.090004 clargs-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-05-19 18:34:49.000000 clargs-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.086004 clargs-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/1_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/2_show_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/3_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/4_parse_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20370 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/5_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/6_validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1596 2024-05-19 18:34:49.000000 clargs-0.7.0/examples/__generate_example_output__.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 18:34:49.000000 clargs-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:35:01.090004 clargs-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.086004 clargs-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/src/clargs/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/aap_from_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/clargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 18:34:49.000000 clargs-0.7.0/src/clargs/helper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/src/clargs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 18:35:01.000000 clargs-0.7.0/src/clargs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:35:01.090004 clargs-0.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-19 18:34:49.000000 clargs-0.7.0/test/test_docsparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26301 2024-05-19 18:34:49.000000 clargs-0.7.0/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 18:34:49.000000 clargs-0.7.0/test/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 18:34:49.000000 clargs-0.7.0/tox.ini
```

### Comparing `clargs-0.6.1/.github/workflows/run-tests.yml` & `clargs-0.7.0/.github/workflows/run-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,20 @@
   workflow_call: {}
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.10', '3.11']
+        python-version: ['3.10', '3.11', '3.12']
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install tox tox-gh-actions
     - name: Test with tox
```

### Comparing `clargs-0.6.1/.github/workflows/upload.yml` & `clargs-0.7.0/.github/workflows/upload.yml`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/LICENCE.txt` & `clargs-0.7.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/PKG-INFO` & `clargs-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: clargs
-Version: 0.6.1
-Summary: Easily generate commandline apps from your functions, based on type hints
-Author-email: Claude <pypi@claude.nl>
-Project-URL: Homepage, https://github.com/reinhrst/clargs
-Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENCE.txt
-
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
 
 - **Hit the ground running**: With a single line, an existing function is turned into a command line program
 - **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
 - **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
@@ -138,19 +124,33 @@
 
 
 #### `clargs.Count`
 
 Is an alias for `int` (should be recognised by static type-checkers).
 Counts how often a parameter is present (mostly used in `--verbose --verbose --verbose` parameters)
 
+#### `clargs.ExistingDirectoryPath`
+
+Is an alias for `pathlib.Path` (should be recognised by static type-checkers).
+It adds validation to confirm that the path is existing, and is a directory.
+
+#### `clargs.ExistingFilePath`
+
+Is an alias for `pathlib.Path` (should be recognised by static type-checkers).
+It adds validation to confirm that the path is existing, and is a file.
+
 ### Custom Type
 
-I hope to add types quickly in future versions.
+TODO: Describe how to make custom functions.
+
+### Validation
 
-In the meantime, any type not listed here will also work as long as an explicit conversion function is defined.
+Experimental support for validation is added, see [this example][6].
+There is no clean way yet to give a proper custom error message in case of an
+exception.
 
 ## Subparsers
 
 Using subparsers it's possible to add multiple functions to your cli. See [an example here][4]
 
 ## Debug output
 
@@ -201,10 +201,11 @@
 There are many other solutions to create command line interfaces from functions.
 I don't think it makes sense to create a comparison list of features now, only to have it be not up to date anymore tomorrow.
 
 The reasons that I developed `clargs` is because I could not find any solution that made me happy (based on the features and properties I describe above).
 
 
 [2]: https://peps.python.org/pep-0484/
-[3]: examples/
-[4]: examples/4_parse_groups.py
-[5]: examples/5_logging.py
+[3]: https://github.com/reinhrst/clargs/tree/main/examples/
+[4]: https://github.com/reinhrst/clargs/tree/main/examples/4_parse_groups.py
+[5]: https://github.com/reinhrst/clargs/tree/main/examples/5_logging.py
+[6]: https://github.com/reinhrst/clargs/tree/main/examples/6_validation.py
```

### Comparing `clargs-0.6.1/README.md` & `clargs-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: clargs
+Version: 0.7.0
+Summary: Easily generate commandline apps from your functions, based on type hints
+Author-email: Claude <pypi@claude.nl>
+Project-URL: Homepage, https://github.com/reinhrst/clargs
+Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENCE.txt
+
 # Clargs
 
 The goal of the `clargs` package is to create commandline interfaces from function signatures.
 
 - **Hit the ground running**: With a single line, an existing function is turned into a command line program
 - **Extensible**: It is flexible enough to do everything that `argparse` does, and keeps you in control
 - **No magic**: All the extension does is call commands in `argparse`; you can log and see these commands
@@ -124,19 +138,33 @@
 
 
 #### `clargs.Count`
 
 Is an alias for `int` (should be recognised by static type-checkers).
 Counts how often a parameter is present (mostly used in `--verbose --verbose --verbose` parameters)
 
+#### `clargs.ExistingDirectoryPath`
+
+Is an alias for `pathlib.Path` (should be recognised by static type-checkers).
+It adds validation to confirm that the path is existing, and is a directory.
+
+#### `clargs.ExistingFilePath`
+
+Is an alias for `pathlib.Path` (should be recognised by static type-checkers).
+It adds validation to confirm that the path is existing, and is a file.
+
 ### Custom Type
 
-I hope to add types quickly in future versions.
+TODO: Describe how to make custom functions.
+
+### Validation
 
-In the meantime, any type not listed here will also work as long as an explicit conversion function is defined.
+Experimental support for validation is added, see [this example][6].
+There is no clean way yet to give a proper custom error message in case of an
+exception.
 
 ## Subparsers
 
 Using subparsers it's possible to add multiple functions to your cli. See [an example here][4]
 
 ## Debug output
 
@@ -187,10 +215,11 @@
 There are many other solutions to create command line interfaces from functions.
 I don't think it makes sense to create a comparison list of features now, only to have it be not up to date anymore tomorrow.
 
 The reasons that I developed `clargs` is because I could not find any solution that made me happy (based on the features and properties I describe above).
 
 
 [2]: https://peps.python.org/pep-0484/
-[3]: examples/
-[4]: examples/4_parse_groups.py
-[5]: examples/5_logging.py
+[3]: https://github.com/reinhrst/clargs/tree/main/examples/
+[4]: https://github.com/reinhrst/clargs/tree/main/examples/4_parse_groups.py
+[5]: https://github.com/reinhrst/clargs/tree/main/examples/5_logging.py
+[6]: https://github.com/reinhrst/clargs/tree/main/examples/6_validation.py
```

### Comparing `clargs-0.6.1/examples/0_basic.py` & `clargs-0.7.0/examples/0_basic.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/examples/1_flags.py` & `clargs-0.7.0/examples/1_flags.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/examples/2_show_defaults.py` & `clargs-0.7.0/examples/2_show_defaults.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/examples/3_list.py` & `clargs-0.7.0/examples/3_list.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/examples/4_parse_groups.py` & `clargs-0.7.0/examples/4_parse_groups.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/examples/5_logging.py` & `clargs-0.7.0/examples/5_logging.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/examples/__generate_example_output__.sh` & `clargs-0.7.0/examples/__generate_example_output__.sh`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/pyproject.toml` & `clargs-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/src/clargs/__init__.py` & `clargs-0.7.0/src/clargs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     run,
 )
 
 from .helper_types import (
     Flag,
     Count,
     ListOfAtLeastOne,
+    ExistingFilePath,
+    ExistingDirectoryPath,
 )
 
 from .aap_from_data import GetArgsFromTypeException
 
 __all__ = [
     "Clargs",
     "Settings",
@@ -28,10 +30,12 @@
     "create_parser",
     "add_to_parser",
     "add_subparser",
     "create_parser_and_run",
     "run",
     "Flag",
     "Count",
-    "ListOfAtLeatOne",
+    "ListOfAtLeastOne",
     "GetArgsFromTypeException",
+    "ExistingFilePath",
+    "ExistingDirectoryPath",
 ]
```

### Comparing `clargs-0.6.1/src/clargs/aap_from_data.py` & `clargs-0.7.0/src/clargs/aap_from_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,19 +256,22 @@
                 and aap.nargs not in ["*", "?"]
             ):
                 aap = aap.with_fields({"required": True})
 
         # overwrite any explicitly set data
         aap = aap.with_fields(self.extra_info.add_argument_parameters)
 
-        if self.extra_info.validate:
-            assert aap.type
+        if self.extra_info.validate is not clargs.NOT_SET:
+            assert not isinstance(aap.type, clargs.NOT_SET_TYPE)
+            originaltype = aap.type
 
             def validate(*args, **kwargs):
-                result = aap.type(*args, **kwargs)
+                result = originaltype(*args, **kwargs)
                 if not self.extra_info.validate(result):
                     raise ValueError("Problem with validation")
                 return result
 
+            validate.__name__ = f"{originaltype.__name__}-validation"
+
             aap = aap.with_fields({"type": validate})
 
         return (self.get_all_param_names(), aap)
```

### Comparing `clargs-0.6.1/src/clargs/clargs.py` & `clargs-0.7.0/src/clargs/clargs.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/src/clargs/docsparser.py` & `clargs-0.7.0/src/clargs/docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/src/clargs/helper_types.py` & `clargs-0.7.0/src/clargs/helper_types.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import pathlib
 from . import clargs
 import typing as t
 
 
 class BooleanOptionalActionException(Exception):
     pass
 
@@ -33,9 +34,23 @@
         nargs=clargs.UNSET,
         action="count",
         default=0,
         required=False,
     ),
 ]
 
+ExistingDirectoryPath = t.Annotated[
+    pathlib.Path,
+    clargs.extra_info(
+        validate=lambda p: p.is_dir(),
+    ),
+]
+
+ExistingFilePath = t.Annotated[
+    pathlib.Path,
+    clargs.extra_info(
+        validate=lambda p: p.is_file(),
+    ),
+]
+
 TYPE = t.TypeVar("TYPE")
 ListOfAtLeastOne = t.Annotated[list[TYPE], clargs.extra_info(nargs="+")]
```

### Comparing `clargs-0.6.1/src/clargs.egg-info/PKG-INFO` & `clargs-0.7.0/src/clargs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clargs
-Version: 0.6.1
+Version: 0.7.0
 Summary: Easily generate commandline apps from your functions, based on type hints
 Author-email: Claude <pypi@claude.nl>
 Project-URL: Homepage, https://github.com/reinhrst/clargs
 Project-URL: Bug Tracker, https://github.com/reinhrst/clargs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -138,19 +138,33 @@
 
 
 #### `clargs.Count`
 
 Is an alias for `int` (should be recognised by static type-checkers).
 Counts how often a parameter is present (mostly used in `--verbose --verbose --verbose` parameters)
 
+#### `clargs.ExistingDirectoryPath`
+
+Is an alias for `pathlib.Path` (should be recognised by static type-checkers).
+It adds validation to confirm that the path is existing, and is a directory.
+
+#### `clargs.ExistingFilePath`
+
+Is an alias for `pathlib.Path` (should be recognised by static type-checkers).
+It adds validation to confirm that the path is existing, and is a file.
+
 ### Custom Type
 
-I hope to add types quickly in future versions.
+TODO: Describe how to make custom functions.
+
+### Validation
 
-In the meantime, any type not listed here will also work as long as an explicit conversion function is defined.
+Experimental support for validation is added, see [this example][6].
+There is no clean way yet to give a proper custom error message in case of an
+exception.
 
 ## Subparsers
 
 Using subparsers it's possible to add multiple functions to your cli. See [an example here][4]
 
 ## Debug output
 
@@ -201,10 +215,11 @@
 There are many other solutions to create command line interfaces from functions.
 I don't think it makes sense to create a comparison list of features now, only to have it be not up to date anymore tomorrow.
 
 The reasons that I developed `clargs` is because I could not find any solution that made me happy (based on the features and properties I describe above).
 
 
 [2]: https://peps.python.org/pep-0484/
-[3]: examples/
-[4]: examples/4_parse_groups.py
-[5]: examples/5_logging.py
+[3]: https://github.com/reinhrst/clargs/tree/main/examples/
+[4]: https://github.com/reinhrst/clargs/tree/main/examples/4_parse_groups.py
+[5]: https://github.com/reinhrst/clargs/tree/main/examples/5_logging.py
+[6]: https://github.com/reinhrst/clargs/tree/main/examples/6_validation.py
```

### Comparing `clargs-0.6.1/src/clargs.egg-info/SOURCES.txt` & `clargs-0.7.0/src/clargs.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 .github/workflows/upload.yml
 examples/0_basic.py
 examples/1_flags.py
 examples/2_show_defaults.py
 examples/3_list.py
 examples/4_parse_groups.py
 examples/5_logging.py
+examples/6_validation.py
 examples/__generate_example_output__.sh
 src/clargs/__init__.py
 src/clargs/aap_from_data.py
 src/clargs/clargs.py
 src/clargs/docsparser.py
 src/clargs/helper_types.py
 src/clargs.egg-info/PKG-INFO
 src/clargs.egg-info/SOURCES.txt
 src/clargs.egg-info/dependency_links.txt
 src/clargs.egg-info/top_level.txt
 test/test_docsparser.py
-test/test_simple.py
+test/test_simple.py
+test/test_validation.py
```

### Comparing `clargs-0.6.1/test/test_docsparser.py` & `clargs-0.7.0/test/test_docsparser.py`

 * *Files identical despite different names*

### Comparing `clargs-0.6.1/test/test_simple.py` & `clargs-0.7.0/test/test_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,26 @@
     return "SUCCESS"
 
 
 def setUpModule():
     logging.basicConfig(level=logging.DEBUG, stream=sys.stdout)
 
 
+def expectedFailureIf(condition):
+    """The test is marked as an expectedFailure if the condition is satisfied."""
+
+    def wrapper(func):
+        if condition:
+            return unittest.expectedFailure(func)
+        else:
+            return func
+
+    return wrapper
+
+
 class Base(unittest.TestCase):
     @contextlib.contextmanager
     def assertExit(self, *, msg: t.Optional[str] = None, regex: t.Optional[str] = None):
         capture = io.StringIO()
         with self.assertRaises(SystemExit), contextlib.redirect_stderr(capture):
             yield
         capturestr = capture.getvalue()
@@ -396,15 +408,16 @@
         with self.assertExit(msg="invalid choice: 4 (choose from 1, 2, 3, 5, 7, 11)"):
             parser.parse_args(["4"])
         with self.assertExit(msg="invalid choice: 4 (choose from 1, 2, 3, 5, 7, 11)"):
             parser.parse_args(["1", "2", "4"])
         with self.assertExit(msg="invalid choice: 4 (choose from 1, 2, 3, 5, 7, 11)"):
             parser.parse_args(["1", "2", "4", "11"])
 
-    @unittest.expectedFailure  # seems to be an issue in argparse
+    # seems to be an issue in argparse, fixed in 3.12
+    @expectedFailureIf(sys.version_info < (3, 12))
     def test_list_int_literal_empty_list(self):
         def function(numbers: t.List[t.Literal[1, 2, 3, 5, 7, 11]]):
             pass
 
         parser = clargs.create_parser(function)
         args = parser.parse_args([])
         self.assertEqual(vars(args), {"_clargs_func_": function, "numbers": []})
```

### Comparing `clargs-0.6.1/tox.ini` & `clargs-0.7.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tox]
 requires =
     tox>=4
-env_list = lint, type, py{310,311}
+env_list = lint, type, py{310,311,312}
 
 [gh-actions]
 python =
     3.10: py310
-    3.11: py311, types, lint
+    3.11: py311
+    3.12: py312, types, lint
 
 [testenv]
 description = run unit tests
 commands =
     python -m unittest discover --start test --buffer
 
 [testenv:lint]
```

