# Comparing `tmp/reqs_cli-0.20240518.0a0.tar.gz` & `tmp/reqs_cli-0.20240518.0a1.tar.gz`

## Comparing `reqs_cli-0.20240518.0a0.tar` & `reqs_cli-0.20240518.0a1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.copier-answers-py.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.coveragerc
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/noxfile.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/ruff.toml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.circleci/config.yml
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.mise/config.toml
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.mise/tasks/hello
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/ci/.gitignore
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/ci/pytest.ini
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/mise/config.toml
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/mise/tasks/bootstrap
--rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/mise/tasks/bump
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/requirements/base.in
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/requirements/base.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/requirements/ci.in
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/requirements/ci.txt
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/requirements/dev.in
--rw-r--r--   0        0        0    34736 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/requirements/dev.txt
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/tasks_lib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/cli.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/config.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/utils.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/__init__.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/test_cli.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg1/foo/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg1/requirements/base.in
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg1/requirements/ci.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg1/requirements/dev.in
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg3/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg3/requirements/base.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg4/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg4/requirements/base.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/src/reqs/tests/pkg4/requirements/foo.in
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/.gitignore
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/hatch.toml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/pyproject.toml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/readme.md
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a0/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.copier-answers-py.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.coveragerc
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/noxfile.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/ruff.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.circleci/config.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.mise/config.toml
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.mise/tasks/hello
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/ci/.gitignore
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/ci/pytest.ini
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/mise/config.toml
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/mise/tasks/bootstrap
+-rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/mise/tasks/bump
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/requirements/base.in
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/requirements/base.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/requirements/ci.in
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/requirements/ci.txt
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/requirements/dev.in
+-rw-r--r--   0        0        0    34736 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/requirements/dev.txt
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/tasks_lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/cli.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/config.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/utils.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/test_cli.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg1/foo/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg1/requirements/base.in
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg1/requirements/ci.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg1/requirements/dev.in
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg3/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg3/requirements/base.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg4/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg4/requirements/base.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/src/reqs/tests/pkg4/requirements/foo.in
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/.gitignore
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/hatch.toml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/readme.md
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 reqs_cli-0.20240518.0a1/PKG-INFO
```

### Comparing `reqs_cli-0.20240518.0a0/.pre-commit-config.yaml` & `reqs_cli-0.20240518.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/noxfile.py` & `reqs_cli-0.20240518.0a1/noxfile.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/ruff.toml` & `reqs_cli-0.20240518.0a1/ruff.toml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/.circleci/config.yml` & `reqs_cli-0.20240518.0a1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/.github/workflows/pypi.yaml` & `reqs_cli-0.20240518.0a1/.github/workflows/pypi.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+# Example:
+#  - https://github.com/pallets/flask/blob/main/.github/workflows/tests.yaml
+# TODO:
+# GH release
+# Environment protection
+#  - https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment
+# Separate build & release
 name: pypi publish
 
 on:
-  push
-    # tags:
-    #   - 'v*.*.*'  # Triggers on version tags like v1.0.0
+  push:
+    branches:
+      - main
+    tags:
+      - 'v*.*.*'
 
 jobs:
   build:
     name: Build project using hatch
 
     runs-on: ubuntu-latest
```

### Comparing `reqs_cli-0.20240518.0a0/ci/pytest.ini` & `reqs_cli-0.20240518.0a1/ci/pytest.ini`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/mise/tasks/bump` & `reqs_cli-0.20240518.0a1/mise/tasks/bump`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/requirements/base.txt` & `reqs_cli-0.20240518.0a1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/requirements/ci.txt` & `reqs_cli-0.20240518.0a1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/requirements/dev.txt` & `reqs_cli-0.20240518.0a1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/src/reqs/cli.py` & `reqs_cli-0.20240518.0a1/src/reqs/cli.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/src/reqs/config.py` & `reqs_cli-0.20240518.0a1/src/reqs/config.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/src/reqs/utils.py` & `reqs_cli-0.20240518.0a1/src/reqs/utils.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/src/reqs/tests/test_cli.py` & `reqs_cli-0.20240518.0a1/src/reqs/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/src/reqs/tests/test_config.py` & `reqs_cli-0.20240518.0a1/src/reqs/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/hatch.toml` & `reqs_cli-0.20240518.0a1/hatch.toml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/readme.md` & `reqs_cli-0.20240518.0a1/readme.md`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240518.0a0/PKG-INFO` & `reqs_cli-0.20240518.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: reqs-cli
-Version: 0.20240518.0a0
+Version: 0.20240518.0a1
 Author-email: Randy Syring <randy.syring@level12.io>
 Requires-Dist: build==1.2.1
 Requires-Dist: click==8.1.7
 Requires-Dist: coverage==7.5.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==24.0
 Requires-Dist: pip-tools==7.4.1
```

