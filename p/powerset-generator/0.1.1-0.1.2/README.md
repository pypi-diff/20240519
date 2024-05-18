# Comparing `tmp/powerset_generator-0.1.1.tar.gz` & `tmp/powerset_generator-0.1.2.tar.gz`

## Comparing `powerset_generator-0.1.1.tar` & `powerset_generator-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0   593705 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/..html
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/mypy.ini
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/requirements-dev.txt
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/requirements.txt
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/ruff.toml
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/.vscode/spellright.dict
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/make.bat
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/requirements.txt
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/source/credits.rst
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/source/usage.rst
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/docs/source/yapp.rst
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/src/powerset_generator/__about__.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/src/powerset_generator/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/src/powerset_generator/py.typed
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/tests/test_powerset.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/LICENSE
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/README.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 powerset_generator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0   593705 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/..html
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/mypy.ini
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/requirements-dev.txt
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/ruff.toml
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.vscode/spellright.dict
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/credits.rst
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/usage.rst
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/docs/source/yapp.rst
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/src/powerset_generator/__about__.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/src/powerset_generator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/src/powerset_generator/py.typed
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/tests/test_powerset.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/README.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 powerset_generator-0.1.2/PKG-INFO
```

### Comparing `powerset_generator-0.1.1/..html` & `powerset_generator-0.1.2/..html`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/ruff.toml` & `powerset_generator-0.1.2/ruff.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 target-version = "py311"
 line-length = 79
+
+[lint]
+# Enable flake8-bugbear (`B`) rules, in addition to the defaults.
+select = ["E4", "E7", "E9", "F", "B"]
+
 unfixable = [
   # Don't touch unused imports
   "F401",
   # Avoid trying to fix flake8-bugbear (`B`) violations
   "B",
 ]
 
-[flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[lint]
-# Enable flake8-bugbear (`B`) rules, in addition to the defaults.
-select = ["E4", "E7", "E9", "F", "B"]
-
 # Avoid enforcing line-length violations (`E501`)
 ignore = ["E501"]
 
 # Only ignore variables named "_".
 dummy-variable-rgx = "^_$"
 
+[lint.flake8-tidy-imports]
+ban-relative-imports = "all"
 
 # Ignore `E402` (import violations) in all `__init__.py` files, and in select subdirectories.
 [lint.per-file-ignores]
 "__init__.py" = ["E402", "F401"]
 "**/{tests,docs,tools}/*" = ["E402"]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
-[isort]
+[lint.isort]
 known-first-party = ["powerset-generator"]
```

### Comparing `powerset_generator-0.1.1/.github/workflows/lint.yml` & `powerset_generator-0.1.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/.github/workflows/test.yml` & `powerset_generator-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/docs/Makefile` & `powerset_generator-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/docs/make.bat` & `powerset_generator-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/docs/source/conf.py` & `powerset_generator-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/docs/source/index.rst` & `powerset_generator-0.1.2/docs/source/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 To use powerset generator, first install it with `pip`
 
 .. code-block:: console
 
     $ pip install powerset-generator
 
-.. note:: 
-    That installation won't work until this powerset-generator package is actually published. It isn't yet.
-
 Example
 -------
 
 The root (and so far only) module is |root|,
 providing the only function, :func:`subsets`.
 
 .. code-block:: python
```

### Comparing `powerset_generator-0.1.1/docs/source/usage.rst` & `powerset_generator-0.1.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/docs/source/yapp.rst` & `powerset_generator-0.1.2/docs/source/yapp.rst`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/src/powerset_generator/__init__.py` & `powerset_generator-0.1.2/src/powerset_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/tests/test_powerset.py` & `powerset_generator-0.1.2/tests/test_powerset.py`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/.gitignore` & `powerset_generator-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/LICENSE` & `powerset_generator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/README.md` & `powerset_generator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/pyproject.toml` & `powerset_generator-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powerset_generator-0.1.1/PKG-INFO` & `powerset_generator-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerset-generator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate the power set of a collection
 Project-URL: Documentation, https://jpgoldberg.github.io/powerset-generator/
 Project-URL: Issues, https://github.com/jpgoldberg/powerset-generator/issues
 Project-URL: Source, https://github.com/jpgoldberg/powerset-generator
 Project-URL: Changelog, https://github.com/jpgoldberg/powerset-generator/blob/main/CHANGELOG.md
 Author-email: Jeffrey Goldberg <jeffrey@goldmark.org>
 License: MIT Licesne
```

