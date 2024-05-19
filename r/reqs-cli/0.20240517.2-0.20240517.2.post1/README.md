# Comparing `tmp/reqs_cli-0.20240517.2.tar.gz` & `tmp/reqs_cli-0.20240517.2.post1.tar.gz`

## Comparing `reqs_cli-0.20240517.2.tar` & `reqs_cli-0.20240517.2.post1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.copier-answers-py.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.coveragerc
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/noxfile.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ruff.toml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.circleci/config.yml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.mise/config.toml
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.mise/tasks/hello
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ci/.gitignore
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ci/pytest.ini
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/ci/test-reports/tests.pytests.xml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/mise/config.toml
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/mise/tasks/bootstrap
--rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/mise/tasks/bump
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/base.in
--rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/base.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/ci.in
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/ci.txt
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/dev.in
--rw-r--r--   0        0        0    34736 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/requirements/dev.txt
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/tasks_lib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/cli.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/config.py
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/utils.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/__init__.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/test_cli.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/test_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/foo/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/requirements/base.in
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/requirements/ci.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg1/requirements/dev.in
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg3/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg3/requirements/base.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg4/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg4/requirements/base.in
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/src/reqs/tests/pkg4/requirements/foo.in
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/.gitignore
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/hatch.toml
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/pyproject.toml
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/readme.md
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2/PKG-INFO
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.copier-answers-py.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.coveragerc
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/noxfile.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/ruff.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.circleci/config.yml
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.mise/config.toml
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.mise/tasks/hello
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/ci/.gitignore
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/ci/pytest.ini
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/mise/config.toml
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/mise/tasks/bootstrap
+-rwxr-xr-x   0        0        0     2442 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/mise/tasks/bump
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/requirements/base.in
+-rw-r--r--   0        0        0     7069 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/requirements/base.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/requirements/ci.in
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/requirements/ci.txt
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/requirements/dev.in
+-rw-r--r--   0        0        0    34736 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/requirements/dev.txt
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/tasks_lib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/cli.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/config.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/test_cli.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/test_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg1/foo/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg1/requirements/base.in
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg1/requirements/ci.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg1/requirements/dev.in
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg3/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg3/requirements/base.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg4/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg4/requirements/base.in
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/src/reqs/tests/pkg4/requirements/foo.in
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/.gitignore
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/hatch.toml
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/readme.md
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 reqs_cli-0.20240517.2.post1/PKG-INFO
```

### Comparing `reqs_cli-0.20240517.2/.pre-commit-config.yaml` & `reqs_cli-0.20240517.2.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/noxfile.py` & `reqs_cli-0.20240517.2.post1/noxfile.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/ruff.toml` & `reqs_cli-0.20240517.2.post1/ruff.toml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/.circleci/config.yml` & `reqs_cli-0.20240517.2.post1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/ci/pytest.ini` & `reqs_cli-0.20240517.2.post1/ci/pytest.ini`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/mise/tasks/bump` & `reqs_cli-0.20240517.2.post1/mise/tasks/bump`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/requirements/base.txt` & `reqs_cli-0.20240517.2.post1/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/requirements/ci.txt` & `reqs_cli-0.20240517.2.post1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/requirements/dev.txt` & `reqs_cli-0.20240517.2.post1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/src/reqs/cli.py` & `reqs_cli-0.20240517.2.post1/src/reqs/cli.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/src/reqs/config.py` & `reqs_cli-0.20240517.2.post1/src/reqs/config.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/src/reqs/utils.py` & `reqs_cli-0.20240517.2.post1/src/reqs/utils.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/src/reqs/tests/test_cli.py` & `reqs_cli-0.20240517.2.post1/src/reqs/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/src/reqs/tests/test_config.py` & `reqs_cli-0.20240517.2.post1/src/reqs/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/hatch.toml` & `reqs_cli-0.20240517.2.post1/hatch.toml`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/readme.md` & `reqs_cli-0.20240517.2.post1/readme.md`

 * *Files identical despite different names*

### Comparing `reqs_cli-0.20240517.2/PKG-INFO` & `reqs_cli-0.20240517.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: reqs-cli
-Version: 0.20240517.2
+Version: 0.20240517.2.post1
 Author-email: Randy Syring <randy.syring@level12.io>
 Requires-Dist: build==1.2.1
 Requires-Dist: click==8.1.7
 Requires-Dist: coverage==7.5.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==24.0
 Requires-Dist: pip-tools==7.4.1
```

