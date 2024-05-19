# Comparing `tmp/atpbar-2.0.0.tar.gz` & `tmp/atpbar-2.0.1.tar.gz`

## Comparing `atpbar-2.0.0.tar` & `atpbar-2.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/__about__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/funcs.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/machine.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/py.typed
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/stream.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/__init__.py
--rwxr-xr-x   0        0        0     3692 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/barjupyter.py
--rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/bartty.py
--rwxr-xr-x   0        0        0     3140 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/base.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/create.py
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/txtprint.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/detect/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/detect/jupy.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/presentation/detect/spy.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/__init__.py
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/complement.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/pickup.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/report.py
--rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 atpbar-2.0.0/atpbar/progressreport/reporter.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 atpbar-2.0.0/.gitignore
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 atpbar-2.0.0/LICENSE
--rw-r--r--   0        0        0    15398 2020-02-02 00:00:00.000000 atpbar-2.0.0/README.md
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 atpbar-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    16356 2020-02-02 00:00:00.000000 atpbar-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/__about__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/__init__.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/funcs.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/machine.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/py.typed
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/stream.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/__init__.py
+-rwxr-xr-x   0        0        0     3692 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/barjupyter.py
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/bartty.py
+-rwxr-xr-x   0        0        0     3140 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/base.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/create.py
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/txtprint.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/detect/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/detect/jupy.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/presentation/detect/spy.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/__init__.py
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/complement.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/pickup.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/report.py
+-rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 atpbar-2.0.1/atpbar/progressreport/reporter.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 atpbar-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 atpbar-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 atpbar-2.0.1/README.md
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 atpbar-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 atpbar-2.0.1/PKG-INFO
```

### Comparing `atpbar-2.0.0/atpbar/funcs.py` & `atpbar-2.0.1/atpbar/funcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,14 +56,23 @@
     -------
     None
 
     """
     _machine.flush()
 
 
+@contextlib.contextmanager
+def flushing() -> Iterator[None]:
+    '''Flushes progress bars on exit'''
+    try:
+        yield
+    finally:
+        flush()
+
+
 def disable() -> None:
     """disables progress bars
 
     This function needs to be called in the main process before
     `atpbar()` or `find_reporter()` is used.
 
     Returns
```

### Comparing `atpbar-2.0.0/atpbar/machine.py` & `atpbar-2.0.1/atpbar/machine.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/main.py` & `atpbar-2.0.1/atpbar/main.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/stream.py` & `atpbar-2.0.1/atpbar/stream.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/barjupyter.py` & `atpbar-2.0.1/atpbar/presentation/barjupyter.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/bartty.py` & `atpbar-2.0.1/atpbar/presentation/bartty.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/base.py` & `atpbar-2.0.1/atpbar/presentation/base.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/create.py` & `atpbar-2.0.1/atpbar/presentation/create.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/txtprint.py` & `atpbar-2.0.1/atpbar/presentation/txtprint.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/detect/jupy.py` & `atpbar-2.0.1/atpbar/presentation/detect/jupy.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/presentation/detect/spy.py` & `atpbar-2.0.1/atpbar/presentation/detect/spy.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/progressreport/complement.py` & `atpbar-2.0.1/atpbar/progressreport/complement.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/progressreport/pickup.py` & `atpbar-2.0.1/atpbar/progressreport/pickup.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/progressreport/report.py` & `atpbar-2.0.1/atpbar/progressreport/report.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/atpbar/progressreport/reporter.py` & `atpbar-2.0.1/atpbar/progressreport/reporter.py`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/.gitignore` & `atpbar-2.0.1/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -156,7 +156,12 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# macOS
+*.DS_Store
+.AppleDouble
+.LSOverride
```

### Comparing `atpbar-2.0.0/LICENSE` & `atpbar-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atpbar-2.0.0/pyproject.toml` & `atpbar-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,37 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [project.optional-dependencies]
 jupyter = ["ipywidgets>=8.1"]
 tests = ["pytest-console-scripts>=1.4", "pytest-cov>=5.0", "pytest>=8.2"]
+doc = ["mkdocs-material>=9.5", "pymdown-extensions>=10.8"]
 
 [project.urls]
 Homepage = "https://github.com/alphatwirl/atpbar"
 
 [tool.hatch.version]
 source = "regex_commit"
 path = "atpbar/__about__.py"
 tag_sign = false
 
 [tool.hatch.build.targets.sdist]
 include = ["/atpbar"]
 
+[tool.pytest.ini_options]
+addopts = """
+--doctest-modules
+--doctest-glob='*.md'
+--ignore=examples/
+--ignore=atpbar/presentation/
+"""
+# doctest_optionflags = ["ELLIPSIS", "NORMALIZE_WHITESPACE",]
+doctest_optionflags = ["ELLIPSIS"]
+
 [tool.black]
 # Doesn't appear to be effective with VSCode extension Black Formatter
 skip-string-normalization = true
 
 [tool.isort]
 profile = "black"
```

