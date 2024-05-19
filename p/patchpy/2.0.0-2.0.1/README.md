# Comparing `tmp/patchpy-2.0.0.tar.gz` & `tmp/patchpy-2.0.1.tar.gz`

## Comparing `patchpy-2.0.0.tar` & `patchpy-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 patchpy-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 patchpy-2.0.0/.python-version
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 patchpy-2.0.0/patchpy.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 patchpy-2.0.0/requirements-dev.lock
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 patchpy-2.0.0/requirements.lock
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 patchpy-2.0.0/test_patchpy.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 patchpy-2.0.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 patchpy-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 patchpy-2.0.0/README.md
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 patchpy-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 patchpy-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 patchpy-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 patchpy-2.0.1/.python-version
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 patchpy-2.0.1/patchpy.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 patchpy-2.0.1/requirements-dev.lock
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 patchpy-2.0.1/requirements.lock
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 patchpy-2.0.1/test_patchpy.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 patchpy-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 patchpy-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 patchpy-2.0.1/README.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 patchpy-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 patchpy-2.0.1/PKG-INFO
```

### Comparing `patchpy-2.0.0/.pre-commit-config.yaml` & `patchpy-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.0/patchpy.py` & `patchpy-2.0.1/patchpy.py`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.0/requirements-dev.lock` & `patchpy-2.0.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.0/test_patchpy.py` & `patchpy-2.0.1/test_patchpy.py`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.0/LICENSE.txt` & `patchpy-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.0/README.md` & `patchpy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.0/pyproject.toml` & `patchpy-2.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "patchpy"
-version = "2.0.0"
+version = "2.0.1"
 description = "A modern Python library for patch file parsing (diff file parsing)"
 authors = [
     { name = "Matthew D. Scholefield", email = "matthew331199@gmail.com" },
 ]
 dependencies = ["more-itertools>=10.2.0"]
 readme = "README.md"
 requires-python = ">= 3.9"
@@ -21,14 +21,14 @@
 managed = true
 dev-dependencies = ["pre-commit>=3.7.1", "pytest>=8.2.0"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
-packages = ["patchpy"]
+include = ["patchpy.py"]
 
 [tool.ruff]
 target-version = "py39"
 
 [tool.ruff.format]
 quote-style = "single"
```

### Comparing `patchpy-2.0.0/PKG-INFO` & `patchpy-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: patchpy
-Version: 2.0.0
+Version: 2.0.1
 Summary: A modern Python library for patch file parsing (diff file parsing)
 Author-email: "Matthew D. Scholefield" <matthew331199@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Requires-Python: >=3.9
 Requires-Dist: more-itertools>=10.2.0
 Description-Content-Type: text/markdown
```

