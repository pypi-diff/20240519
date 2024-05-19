# Comparing `tmp/kiclearance-0.0.1.tar.gz` & `tmp/kiclearance-0.0.2.tar.gz`

## Comparing `kiclearance-0.0.1.tar` & `kiclearance-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 kiclearance-0.0.1/requirements.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 kiclearance-0.0.1/kiclearance/__init__.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 kiclearance-0.0.1/kiclearance/__main__.py
--rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 kiclearance-0.0.1/kiclearance/kiclearance.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 kiclearance-0.0.1/.gitignore
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 kiclearance-0.0.1/README.rst
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 kiclearance-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 kiclearance-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 kiclearance-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 kiclearance-0.0.2/kiclearance/__init__.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 kiclearance-0.0.2/kiclearance/__main__.py
+-rw-r--r--   0        0        0     9854 2020-02-02 00:00:00.000000 kiclearance-0.0.2/kiclearance/kiclearance.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 kiclearance-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 kiclearance-0.0.2/README.rst
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kiclearance-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 kiclearance-0.0.2/PKG-INFO
```

### Comparing `kiclearance-0.0.1/kiclearance/__main__.py` & `kiclearance-0.0.2/kiclearance/__main__.py`

 * *Files identical despite different names*

### Comparing `kiclearance-0.0.1/kiclearance/kiclearance.py` & `kiclearance-0.0.2/kiclearance/kiclearance.py`

 * *Files identical despite different names*

### Comparing `kiclearance-0.0.1/README.rst` & `kiclearance-0.0.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -45,13 +45,13 @@
 Example
 ---------------------------------------
 A complete example can be found `here <https://github.com/upb-lea/KiClearance/tree/main/examples>`__.
 
 Documentation
 ---------------------------------------
 
-Find the documentation `here <https://upb-lea.github.io/KiClearance/intro.html>`__.
+Find the documentation `here <https://upb-lea.github.io/KiClearance/index.html>`__.
 
 
 Troubleshooting
 ---------------------------------------
 This program has so far been tested only on linux.
```

### Comparing `kiclearance-0.0.1/pyproject.toml` & `kiclearance-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kiclearance"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     { name = "UPB-LEA" },
 ]
 description = "Generate clearance rules for KiCAD by a table."
 readme = "README.rst"
 requires-python = "~=3.8"
 classifiers = [
@@ -66,8 +66,8 @@
 [tool.ruff.lint.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
-line-ending = "auto"
+line-ending = "auto"
```

### Comparing `kiclearance-0.0.1/PKG-INFO` & `kiclearance-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kiclearance
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate clearance rules for KiCAD by a table.
 Project-URL: Homepage, https://github.com/upb-lea/kiclearance
 Project-URL: Issues, https://github.com/upb-lea/kiclearance/issues
 Author: UPB-LEA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -61,13 +61,13 @@
 Example
 ---------------------------------------
 A complete example can be found `here <https://github.com/upb-lea/KiClearance/tree/main/examples>`__.
 
 Documentation
 ---------------------------------------
 
-Find the documentation `here <https://upb-lea.github.io/KiClearance/intro.html>`__.
+Find the documentation `here <https://upb-lea.github.io/KiClearance/index.html>`__.
 
 
 Troubleshooting
 ---------------------------------------
 This program has so far been tested only on linux.
```

