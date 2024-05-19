# Comparing `tmp/hypercoast-0.3.2.tar.gz` & `tmp/hypercoast-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercoast-0.3.2.tar", last modified: Fri May 10 13:58:00 2024, max compression
+gzip compressed data, was "hypercoast-0.3.3.tar", last modified: Sun May 19 04:02:05 2024, max compression
```

## Comparing `hypercoast-0.3.2.tar` & `hypercoast-0.3.3.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.063677 hypercoast-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.055677 hypercoast-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.055677 hypercoast-0.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.059677 hypercoast-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-10 13:57:48.000000 hypercoast-0.3.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.063677 hypercoast-0.3.2/HyperCoast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-10 13:58:00.000000 hypercoast-0.3.2/HyperCoast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-10 13:58:00.000000 hypercoast-0.3.2/HyperCoast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:58:00.000000 hypercoast-0.3.2/HyperCoast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-10 13:58:00.000000 hypercoast-0.3.2/HyperCoast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-10 13:58:00.000000 hypercoast-0.3.2/HyperCoast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 13:58:00.000000 hypercoast-0.3.2/HyperCoast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-10 13:57:48.000000 hypercoast-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-10 13:57:48.000000 hypercoast-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-10 13:58:00.063677 hypercoast-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-10 13:57:48.000000 hypercoast-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.059677 hypercoast-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/emit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.063677 hypercoast-0.3.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/examples/emit.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/examples/pace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/hypercoast.md
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.063677 hypercoast-0.3.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/pace.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/ui.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 13:57:48.000000 hypercoast-0.3.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.063677 hypercoast-0.3.2/hypercoast/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 13:57:48.000000 hypercoast-0.3.2/hypercoast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-10 13:57:48.000000 hypercoast-0.3.2/hypercoast/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-10 13:57:48.000000 hypercoast-0.3.2/hypercoast/emit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13933 2024-05-10 13:57:48.000000 hypercoast-0.3.2/hypercoast/hypercoast.py
--rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-05-10 13:57:48.000000 hypercoast-0.3.2/hypercoast/pace.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-10 13:57:48.000000 hypercoast-0.3.2/hypercoast/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-10 13:57:48.000000 hypercoast-0.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-10 13:57:48.000000 hypercoast-0.3.2/pyproject-codespell.precommit-toml
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-10 13:57:48.000000 hypercoast-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 13:57:48.000000 hypercoast-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-10 13:57:48.000000 hypercoast-0.3.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:58:00.063677 hypercoast-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:58:00.063677 hypercoast-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 13:57:48.000000 hypercoast-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-10 13:57:48.000000 hypercoast-0.3.2/tests/test_hypercoast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.483397 hypercoast-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.471397 hypercoast-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.475397 hypercoast-0.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.475397 hypercoast-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-19 04:01:53.000000 hypercoast-0.3.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.483397 hypercoast-0.3.3/HyperCoast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-19 04:02:05.000000 hypercoast-0.3.3/HyperCoast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-19 04:02:05.000000 hypercoast-0.3.3/HyperCoast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:02:05.000000 hypercoast-0.3.3/HyperCoast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 04:02:05.000000 hypercoast-0.3.3/HyperCoast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-19 04:02:05.000000 hypercoast-0.3.3/HyperCoast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 04:02:05.000000 hypercoast-0.3.3/HyperCoast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-19 04:01:53.000000 hypercoast-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-19 04:01:53.000000 hypercoast-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-19 04:02:05.483397 hypercoast-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-19 04:01:53.000000 hypercoast-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.479397 hypercoast-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/emit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.479397 hypercoast-0.3.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/examples/emit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/examples/pace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/examples/search_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/hypercoast.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.479397 hypercoast-0.3.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/pace.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/ui.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-19 04:01:53.000000 hypercoast-0.3.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.483397 hypercoast-0.3.3/hypercoast/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-19 04:01:53.000000 hypercoast-0.3.3/hypercoast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-05-19 04:01:53.000000 hypercoast-0.3.3/hypercoast/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37765 2024-05-19 04:01:53.000000 hypercoast-0.3.3/hypercoast/emit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-05-19 04:01:53.000000 hypercoast-0.3.3/hypercoast/hypercoast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13758 2024-05-19 04:01:53.000000 hypercoast-0.3.3/hypercoast/pace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-05-19 04:01:53.000000 hypercoast-0.3.3/hypercoast/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-19 04:01:53.000000 hypercoast-0.3.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-19 04:01:53.000000 hypercoast-0.3.3/pyproject-codespell.precommit-toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-19 04:01:53.000000 hypercoast-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-19 04:01:53.000000 hypercoast-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-19 04:01:53.000000 hypercoast-0.3.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:02:05.483397 hypercoast-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:02:05.483397 hypercoast-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 04:01:53.000000 hypercoast-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-19 04:01:53.000000 hypercoast-0.3.3/tests/test_hypercoast.py
```

### Comparing `hypercoast-0.3.2/.github/workflows/docs-build.yml` & `hypercoast-0.3.3/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.github/workflows/docs.yml` & `hypercoast-0.3.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.github/workflows/installation.yml` & `hypercoast-0.3.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.github/workflows/macos.yml` & `hypercoast-0.3.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.github/workflows/pypi.yml` & `hypercoast-0.3.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.github/workflows/ubuntu.yml` & `hypercoast-0.3.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.github/workflows/windows.yml` & `hypercoast-0.3.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.gitignore` & `hypercoast-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/.pre-commit-config.yaml` & `hypercoast-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/HyperCoast.egg-info/PKG-INFO` & `hypercoast-0.3.3/HyperCoast.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,16 @@
 Requires-Dist: s3fs
 Requires-Dist: scipy
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: cartopy; extra == "extra"
+Requires-Dist: earthaccess; extra == "extra"
+Requires-Dist: mapclassify; extra == "extra"
 
 # HyperCoast
 
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/HyperCoast/blob/main)
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
```

### Comparing `hypercoast-0.3.2/HyperCoast.egg-info/SOURCES.txt` & `hypercoast-0.3.3/HyperCoast.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 docs/index.md
 docs/installation.md
 docs/pace.md
 docs/ui.md
 docs/usage.md
 docs/examples/emit.ipynb
 docs/examples/pace.ipynb
+docs/examples/search_data.ipynb
 docs/overrides/main.html
 hypercoast/__init__.py
 hypercoast/common.py
 hypercoast/emit.py
 hypercoast/hypercoast.py
 hypercoast/pace.py
 hypercoast/ui.py
```

### Comparing `hypercoast-0.3.2/LICENSE` & `hypercoast-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/PKG-INFO` & `hypercoast-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HyperCoast
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python package for processing hyperspectral data in coastal regions
 Author-email: Qiusheng Wu <giswqs@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/opengeos/HyperCoast
 Keywords: HyperCoast
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,16 @@
 Requires-Dist: s3fs
 Requires-Dist: scipy
 Requires-Dist: xarray
 Provides-Extra: all
 Requires-Dist: HyperCoast[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: cartopy; extra == "extra"
+Requires-Dist: earthaccess; extra == "extra"
+Requires-Dist: mapclassify; extra == "extra"
 
 # HyperCoast
 
 [![image](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/opengeos/HyperCoast/blob/main)
 [![image](https://img.shields.io/pypi/v/HyperCoast.svg)](https://pypi.python.org/pypi/HyperCoast)
 [![image](https://static.pepy.tech/badge/hypercoast)](https://pepy.tech/project/hypercoast)
 [![image](https://img.shields.io/conda/vn/conda-forge/hypercoast.svg)](https://anaconda.org/conda-forge/hypercoast)
```

### Comparing `hypercoast-0.3.2/README.md` & `hypercoast-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/docs/contributing.md` & `hypercoast-0.3.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/docs/examples/emit.ipynb` & `hypercoast-0.3.3/docs/examples/emit.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/docs/examples/pace.ipynb` & `hypercoast-0.3.3/docs/examples/pace.ipynb`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/docs/index.md` & `hypercoast-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/docs/installation.md` & `hypercoast-0.3.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/hypercoast/emit.py` & `hypercoast-0.3.3/hypercoast/emit.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/hypercoast/hypercoast.py` & `hypercoast-0.3.3/hypercoast/hypercoast.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Main module."""
 
 import ipyleaflet
 import leafmap
 import xarray as xr
 import numpy as np
-from .common import download_file, netcdf_groups
-from .emit import read_emit, plot_emit, viz_emit, emit_to_netcdf, emit_to_image
+from .common import *
+from .emit import *
 from .pace import *
 from .ui import SpectralWidget
 
 
 class Map(leafmap.Map):
     """
     A class that extends leafmap.Map to provide additional functionality for hypercoast.
@@ -36,15 +36,15 @@
         Args:
             **kwargs: Arbitrary keyword arguments that are passed to the parent class's add_layer method.
         """
 
         if isinstance(obj, str):
             if obj == "spectral":
 
-                SpectralWidget(self, position=position)
+                SpectralWidget(self, position=position, **kwargs)
                 self.set_plot_options(add_marker_cluster=True)
             else:
                 super().add(obj, **kwargs)
 
         else:
             super().add(obj, **kwargs)
```

### Comparing `hypercoast-0.3.2/hypercoast/pace.py` & `hypercoast-0.3.3/hypercoast/pace.py`

 * *Files identical despite different names*

### Comparing `hypercoast-0.3.2/hypercoast/ui.py` & `hypercoast-0.3.3/hypercoast/ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains the user interface for the hypercoast package.
 """
 
 import os
 import ipyleaflet
+import bqplot
 import ipywidgets as widgets
 import numpy as np
 import xarray as xr
 from bqplot import pyplot as plt
 from IPython.core.display import display
 from ipyfilechooser import FileChooser
 from .pace import extract_pace
@@ -22,24 +23,36 @@
         _output_widget (widgets.Output): The output widget to display results.
         _output_control (ipyleaflet.WidgetControl): The control for the output widget.
         _on_map_interaction (function): Function to handle map interactions.
         _spectral_widget (SpectralWidget): The spectral widget itself.
         _spectral_control (ipyleaflet.WidgetControl): The control for the spectral widget.
     """
 
-    def __init__(self, host_map, position="topright"):
+    def __init__(self, host_map, stack=True, position="topright"):
         """
         Initializes a new instance of the SpectralWidget class.
 
         Args:
             host_map (Map): The map to host the widget.
             position (str, optional): The position of the widget on the map. Defaults to "topright".
         """
         self._host_map = host_map
         self.on_close = None
+        self._stack = stack
+        self._show_plot = False
+
+        fig_margin = {"top": 20, "bottom": 35, "left": 50, "right": 20}
+        fig = plt.figure(
+            # title=None,
+            fig_margin=fig_margin,
+            layout={"width": "500px", "height": "300px"},
+        )
+
+        self._fig = fig
+        self._host_map._fig = fig
 
         close_btn = widgets.Button(
             icon="times",
             tooltip="Close the widget",
             button_style="primary",
             layout=widgets.Layout(width="32px"),
         )
@@ -47,23 +60,32 @@
         reset_btn = widgets.Button(
             icon="trash",
             tooltip="Remove all markers",
             button_style="primary",
             layout=widgets.Layout(width="32px"),
         )
 
+        stack_btn = widgets.ToggleButton(
+            value=stack,
+            icon="area-chart",
+            button_style="primary",
+            layout=widgets.Layout(width="32px"),
+        )
+
         def reset_btn_click(_):
             if hasattr(self._host_map, "_plot_marker_cluster"):
                 self._host_map._plot_marker_cluster.markers = []
                 self._host_map._plot_markers = []
 
             if hasattr(self._host_map, "_spectral_data"):
                 self._host_map._spectral_data = {}
 
             self._output_widget.clear_output()
+            self._show_plot = False
+            plt.clear()
 
         reset_btn.on_click(reset_btn_click)
 
         save_btn = widgets.Button(
             icon="floppy-o",
             tooltip="Save the data to a CSV",
             button_style="primary",
@@ -108,15 +130,15 @@
             self.cleanup()
 
         close_btn.on_click(close_widget)
 
         layer_names = list(host_map.cog_layer_dict.keys())
         layers_widget = widgets.Dropdown(options=layer_names)
         layers_widget.layout.width = "18ex"
-        super().__init__([layers_widget, reset_btn, save_btn, close_btn])
+        super().__init__([layers_widget, stack_btn, reset_btn, save_btn, close_btn])
 
         output = widgets.Output()
         output_control = ipyleaflet.WidgetControl(widget=output, position="bottomright")
         self._output_widget = output
         self._output_control = output_control
         self._host_map.add(output_control)
 
@@ -126,65 +148,72 @@
         def handle_interaction(**kwargs):
 
             latlon = kwargs.get("coordinates")
             lat = latlon[0]
             lon = latlon[1]
             if kwargs.get("type") == "click":
                 layer_name = layers_widget.value
-                with self._output_widget:
-                    self._output_widget.clear_output()
 
-                    if not hasattr(self._host_map, "_plot_markers"):
-                        self._host_map._plot_markers = []
-                    markers = self._host_map._plot_markers
-                    marker_cluster = self._host_map._plot_marker_cluster
-                    markers.append(ipyleaflet.Marker(location=latlon))
-                    marker_cluster.markers = markers
-                    self._host_map._plot_marker_cluster = marker_cluster
-
-                    ds = self._host_map.cog_layer_dict[layer_name]["xds"]
-                    if self._host_map.cog_layer_dict[layer_name]["type"] == "EMIT":
-                        da = ds.sel(latitude=lat, longitude=lon, method="nearest")[
-                            "reflectance"
-                        ]
-
-                        if "wavelengths" not in self._host_map._spectral_data:
-                            self._host_map._spectral_data["wavelengths"] = ds[
-                                "wavelengths"
-                            ].values
-                    elif self._host_map.cog_layer_dict[layer_name]["type"] == "PACE":
-                        try:
-                            da = extract_pace(ds, lat, lon)
-                        except:
-                            da = xr.DataArray(
-                                np.full(len(ds["wavelength"]), np.nan),
-                                dims=["wavelength"],
-                                coords={"wavelength": ds["wavelength"]},
-                            )
-                        if "wavelengths" not in self._host_map._spectral_data:
-                            self._host_map._spectral_data["wavelengths"] = ds[
-                                "wavelength"
-                            ].values
-
-                    self._host_map._spectral_data[f"({lat:.4f} {lon:.4f})"] = da.values
-
-                    da[da < 0] = np.nan
-                    # fig, ax = plt.subplots()
-                    # da.plot.line(ax=ax)
-                    # display(fig)
-                    fig_margin = {"top": 20, "bottom": 35, "left": 50, "right": 20}
-                    fig = plt.figure(
-                        # title=None,
-                        fig_margin=fig_margin,
-                        layout={"width": "500px", "height": "300px"},
-                    )
+                if not hasattr(self._host_map, "_plot_markers"):
+                    self._host_map._plot_markers = []
+                markers = self._host_map._plot_markers
+                marker_cluster = self._host_map._plot_marker_cluster
+                markers.append(ipyleaflet.Marker(location=latlon))
+                marker_cluster.markers = markers
+                self._host_map._plot_marker_cluster = marker_cluster
+
+                ds = self._host_map.cog_layer_dict[layer_name]["xds"]
+                if self._host_map.cog_layer_dict[layer_name]["type"] == "EMIT":
+                    da = ds.sel(latitude=lat, longitude=lon, method="nearest")[
+                        "reflectance"
+                    ]
+
+                    if "wavelengths" not in self._host_map._spectral_data:
+                        self._host_map._spectral_data["wavelengths"] = ds[
+                            "wavelengths"
+                        ].values
+                elif self._host_map.cog_layer_dict[layer_name]["type"] == "PACE":
+                    try:
+                        da = extract_pace(ds, lat, lon)
+                    except:
+                        da = xr.DataArray(
+                            np.full(len(ds["wavelength"]), np.nan),
+                            dims=["wavelength"],
+                            coords={"wavelength": ds["wavelength"]},
+                        )
+                    if "wavelengths" not in self._host_map._spectral_data:
+                        self._host_map._spectral_data["wavelengths"] = ds[
+                            "wavelength"
+                        ].values
+
+                self._host_map._spectral_data[f"({lat:.4f} {lon:.4f})"] = da.values
+
+                da[da < 0] = np.nan
+                if not stack_btn.value:
+                    plt.clear()
                     plt.plot(da.coords[da.dims[0]].values, da.values)
-                    plt.xlabel("Wavelength (nm)")
-                    plt.ylabel("Reflectance")
-                    plt.show()
+                else:
+                    color = np.random.rand(
+                        3,
+                    )
+                    plt.plot(da.coords[da.dims[0]].values, da.values, color=color)
+                    try:
+                        if isinstance(self._fig.axes[0], bqplot.ColorAxis):
+                            self._fig.axes = self._fig.axes[1:]
+                        elif isinstance(self._fig.axes[-1], bqplot.ColorAxis):
+                            self._fig.axes = self._fig.axes[:-1]
+                    except:
+                        pass
+                plt.xlabel("Wavelength (nm)")
+                plt.ylabel("Reflectance")
+
+                if not self._show_plot:
+                    with self._output_widget:
+                        plt.show()
+                        self._show_plot = True
 
                 self._host_map.default_style = {"cursor": "crosshair"}
 
         self._host_map.on_interaction(handle_interaction)
         self._on_map_interaction = handle_interaction
 
         self._spectral_widget = self
```

### Comparing `hypercoast-0.3.2/mkdocs.yml` & `hypercoast-0.3.3/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
           execute: True
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["ignore.ipynb"]
+          execute_ignore: ["search_data.ipynb"]
 
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -76,14 +76,15 @@
     - Installation: installation.md
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/opengeos/HyperCoast/issues
     - Examples:
+          - examples/search_data.ipynb
           - examples/emit.ipynb
           - examples/pace.ipynb
     - API Reference:
           - common module: common.md
           - emit module: emit.md
           - hypercoast module: hypercoast.md
           - pace module: pace.md
```

### Comparing `hypercoast-0.3.2/pyproject.toml` & `hypercoast-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "HyperCoast"
-version = "0.3.2"
+version = "0.3.3"
 dynamic = [
     "dependencies",
 ]
 description = "A Python package for processing hyperspectral data in coastal regions"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -31,14 +31,16 @@
 [project.optional-dependencies]
 all = [
     "HyperCoast[extra]",
 ]
 
 extra = [
     "cartopy",
+    "earthaccess",
+    "mapclassify",
 ]
 
 
 [tool]
 [tool.setuptools.packages.find]
 include = ["hypercoast*"]
 exclude = ["docs*"]
@@ -48,15 +50,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.3.2"
+current_version = "0.3.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

