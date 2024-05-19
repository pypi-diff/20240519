# Comparing `tmp/panoptes-aag-0.0.3.tar.gz` & `tmp/panoptes_aag-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptes-aag-0.0.3.tar", last modified: Sun Sep  3 01:00:14 2023, max compression
+gzip compressed data, was "panoptes_aag-0.0.5.tar", last modified: Sun May 19 19:43:09 2024, max compression
```

## Comparing `panoptes-aag-0.0.3.tar` & `panoptes_aag-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (999)      586 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.537358 panoptes-aag-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      960 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/.github/workflows/create-release.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     1481 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/.github/workflows/pythontest.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      566 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)      490 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (999)       86 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (999)       54 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (999)      271 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (999)     1084 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (999)     6899 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     6323 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (999)     1154 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)       71 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (999)       73 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (999)    10038 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (999)       76 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (999)      977 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (999)       66 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (999)       70 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (999)      233 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)      355 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)     2147 2023-09-03 01:00:14.545358 panoptes-aag-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      708 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/src/aag/
--rw-r--r--   0 runner    (1001) docker     (999)      582 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/aag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1361 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/aag/cli.py
--rw-r--r--   0 runner    (1001) docker     (999)     1227 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/aag/commands.py
--rw-r--r--   0 runner    (1001) docker     (999)      514 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/aag/server.py
--rw-r--r--   0 runner    (1001) docker     (999)     1574 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/aag/settings.py
--rw-r--r--   0 runner    (1001) docker     (999)    14115 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/src/aag/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     6899 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      854 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       44 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      297 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-09-03 01:00:14.000000 panoptes-aag-0.0.3/src/panoptes_aag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 01:00:14.541358 panoptes-aag-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      271 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)     3095 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/tests/test_weather.py
--rw-r--r--   0 runner    (1001) docker     (999)     2690 2023-09-03 00:58:41.000000 panoptes-aag-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.069082 panoptes_aag-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.057082 panoptes_aag-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.061082 panoptes_aag-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/.github/workflows/create-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/.github/workflows/pythontest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-05-19 19:43:09.069082 panoptes_aag-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.065082 panoptes_aag-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.065082 panoptes_aag-0.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-19 19:43:09.069082 panoptes_aag-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.065082 panoptes_aag-0.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.065082 panoptes_aag-0.0.5/src/aag/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/aag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/aag/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/aag/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/aag/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/aag/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/src/aag/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.069082 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7763 2024-05-19 19:43:09.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 19:43:09.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:43:09.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 19:43:09.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:43:08.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-19 19:43:09.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 19:43:09.000000 panoptes_aag-0.0.5/src/panoptes_aag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:43:09.065082 panoptes_aag-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/tests/test_weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-19 19:42:19.000000 panoptes_aag-0.0.5/tox.ini
```

### Comparing `panoptes-aag-0.0.3/.coveragerc` & `panoptes_aag-0.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/.github/workflows/create-release.yaml` & `panoptes_aag-0.0.5/.github/workflows/create-release.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 name: Create GitHub Release
 
 jobs:
   publish:
     name: Push Release to PyPi
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@master
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@master
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install ".[building,docs,testing]"
       - name: tox clean and build
         run: |
           tox -e clean
           tox -e build
-      - name: tox publish
-        env:
-          TWINE_USERNAME: ${{ secrets.PYPI_USERNAME }}
-          TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-        run: |
-          twine check dist/*
-          tox -e publish -- --repository pypi
+      - name: Publish package
+        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `panoptes-aag-0.0.3/.github/workflows/pythontest.yaml` & `panoptes_aag-0.0.5/.github/workflows/pythontest.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -2,46 +2,43 @@
 
 on: [ push, pull_request ]
 jobs:
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ "3.11" ]
+        python-version: [ "3.12" ]
     steps:
       - name: Checkout code
-        uses: actions/checkout@v3
+        uses: actions/checkout@master
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@master
         with:
           python-version: ${{ matrix.python-version }}
       - name: Lint with flake8
         run: |
           pip install flake8
           # stop the build if there are Python syntax errors or undefined names
           flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
           # exit-zero treats all errors as warnings.
           flake8 . --count --exit-zero --max-complexity=10 --max-line-length=100 --statistics
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ "3.11" ]
+        python-version: [ "3.12" ]
     steps:
       - name: Checkout code
-        uses: actions/checkout@v3
+        uses: actions/checkout@master
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@master
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install
         run: pip install ".[building,testing]"
       - name: Test
         run: pytest
-      - name: Upload coverage report to codecov.io
-        uses: codecov/codecov-action@v1
-        if: success()
+      - uses: codecov/codecov-action@v4
         with:
-          name: codecov-upload
+          name: Upload to codecov.io
           token: ${{ secrets.CODECOV_TOKEN }}
-          file: build/coverage.xml
-          fail_ci_if_error: true
+          verbose: true
```

### Comparing `panoptes-aag-0.0.3/.gitignore` & `panoptes_aag-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/LICENSE.txt` & `panoptes_aag-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/PKG-INFO` & `panoptes_aag-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: panoptes-aag
-Version: 0.0.3
-Summary: Weather service for the Lunatico AAG CloudWatcher.
-Home-page: https://github.com/panoptes/aag-weather/
-Author: Wilfred Tyler Gee
-Author-email: wtylergee@gmail.com
-License: MIT
-Project-URL: Documentation, https://projectpanoptes.org/
-Platform: linux
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: building
-Provides-Extra: docs
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 # PANOPTES AAG weather reader
 
 [![codecov](https://codecov.io/github/panoptes/aag-weather/branch/main/graph/badge.svg?token=wwoAn40DVB)](https://codecov.io/github/panoptes/aag-weather)
 
 > Weather service for the Lunatico AAG CloudWatcher.
 
 This is a simple weather service for the Lunatico AAG CloudWatcher. It is
```

### Comparing `panoptes-aag-0.0.3/README.md` & `panoptes_aag-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,49 @@
+Metadata-Version: 2.1
+Name: panoptes-aag
+Version: 0.0.5
+Summary: Weather service for the Lunatico AAG CloudWatcher.
+Home-page: https://github.com/panoptes/aag-weather/
+Author: Wilfred Tyler Gee
+Author-email: wtylergee@gmail.com
+License: MIT
+Project-URL: Documentation, https://projectpanoptes.org/
+Platform: linux
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.11"
+Requires-Dist: astropy
+Requires-Dist: fastapi[all]
+Requires-Dist: fastapi-utils
+Requires-Dist: httpie
+Requires-Dist: pandas
+Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Requires-Dist: pyserial>=3.4
+Requires-Dist: python-dotenv
+Requires-Dist: typer[all]
+Provides-Extra: building
+Requires-Dist: pyscaffold>=4.3.1; extra == "building"
+Requires-Dist: pyscaffoldext-markdown; extra == "building"
+Requires-Dist: tox; extra == "building"
+Requires-Dist: twine; extra == "building"
+Provides-Extra: docs
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: piccolo-theme; extra == "docs"
+Requires-Dist: pytest_mpl; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Provides-Extra: testing
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: tox; extra == "testing"
+
 # PANOPTES AAG weather reader
 
 [![codecov](https://codecov.io/github/panoptes/aag-weather/branch/main/graph/badge.svg?token=wwoAn40DVB)](https://codecov.io/github/panoptes/aag-weather)
 
 > Weather service for the Lunatico AAG CloudWatcher.
 
 This is a simple weather service for the Lunatico AAG CloudWatcher. It is
```

### Comparing `panoptes-aag-0.0.3/docs/Makefile` & `panoptes_aag-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/docs/conf.py` & `panoptes_aag-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/docs/index.md` & `panoptes_aag-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/setup.cfg` & `panoptes_aag-0.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,18 @@
 install_requires = 
 	importlib-metadata; python_version<"3.11"
 	astropy
 	fastapi[all]
 	fastapi-utils
 	httpie
 	pandas
-	pydantic[dotenv]
+	pydantic
+	pydantic-settings
 	pyserial>=3.4
+	python-dotenv
 	typer[all]
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `panoptes-aag-0.0.3/setup.py` & `panoptes_aag-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/src/aag/__init__.py` & `panoptes_aag-0.0.5/src/aag/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/src/aag/cli.py` & `panoptes_aag-0.0.5/src/aag/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,27 @@
 from rich import print
 
 from aag.weather import CloudSensor
 
 app = typer.Typer()
 readings_table = Table()
 
+format_lookup = {
+    '.csv': 'ascii.csv',
+    '.ecsv': 'ascii.ecsv',
+    '.json': 'pandas.json',
+}
+
 
 @app.command(name='capture')
 def capture(
-        output: Path = typer.Option('weather.csv', help='Output filename, defaults to an astropy ECSV file.'),
-        verbose: bool = typer.Option(False, help='Verbose output.'),
+        output: Path = typer.Option('weather.ecsv',
+                                    help='Output filename with format determined by extension, '
+                                         'defaults to an astropy ECSV file.'),
+        verbose: bool = typer.Option(False, help='Show the weather readings.'),
 ):
     """Captures readings continuously."""
     sensor = CloudSensor()
     print(f'Sensor: {sensor}')
 
     def callback(reading):
         global readings_table
@@ -28,21 +36,24 @@
         else:
             readings_table.add_row(reading)
 
         if verbose:
             print(reading)
 
         if output is not None:
-            readings_table.write(output, overwrite=True, format='ascii.ecsv', delimiter=',')
-
-    # Blocking
-    sensor.capture(callback=callback)
+            readings_table.write(output, overwrite=True, format=format_lookup.get(output.suffix))
 
-    if output is not None:
-        print(f'Data saved to {output}')
+    try:
+        # Blocking.
+        sensor.capture(callback=callback)
+    except KeyboardInterrupt:
+        print('Stopping capture.')
+    finally:
+        if output is not None:
+            print(f'\nData saved to [green]{output}[/green]')
 
 
 @app.command(name='serve')
 def serve(
         port: int = typer.Option(8080, help='Port to serve on.'),
         host: str = typer.Option('localhost', help='Host to serve on.'),
 ):
```

### Comparing `panoptes-aag-0.0.3/src/aag/commands.py` & `panoptes_aag-0.0.5/src/aag/commands.py`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/src/aag/server.py` & `panoptes_aag-0.0.5/src/aag/server.py`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/src/aag/settings.py` & `panoptes_aag-0.0.5/src/aag/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from pydantic import BaseSettings, BaseModel
+from pydantic_settings import BaseSettings
+from pydantic import BaseModel
 from enum import StrEnum
 
 
 class WhichUnits(StrEnum):
     metric = 'metric'
     imperial = 'imperial'
     none = 'none'
@@ -32,16 +33,16 @@
 
 class WeatherSettings(BaseSettings):
     serial_port: str = '/dev/ttyUSB0'
     safety_delay: float = 15  # minutes
     capture_delay: float = 30  # seconds
     num_readings: int = 10
     ignore_unsafe: bool | None = None  # None, otherwise can be a list, e.g. 'rain','cloud','gust','wind'
-    thresholds = Thresholds()
-    heater = Heater()
+    thresholds: Thresholds = Thresholds()
+    heater: Heater = Heater()
 
     class Config:
         env_prefix = 'AAG_'
         env_file = 'config.env'
         env_nested_delimiter = '__'
```

### Comparing `panoptes-aag-0.0.3/src/aag/weather.py` & `panoptes_aag-0.0.5/src/aag/weather.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,22 +23,25 @@
             **kwargs: Keyword arguments for the WeatherSettings class.
         """
         self.config = WeatherSettings(**kwargs)
 
         try:
             self._sensor: serial.Serial = serial.serial_for_url(self.config.serial_port,
                                                                 baudrate=9600,
-                                                                timeout=1)
+                                                                timeout=1,
+                                                                do_not_open=True
+                                                                )
+            if connect:
+                self._sensor.open()
+                self._sensor.reset_input_buffer()
+                self._sensor.reset_output_buffer()
         except serial.serialutil.SerialException as e:
             print(f'[red]Unable to connect to weather sensor. Check the port. {e}')
             raise e
 
-        self._sensor.reset_input_buffer()
-        self._sensor.reset_output_buffer()
-
         self.handshake_block = r'\x11\s{12}0'
 
         # Set up a queue for readings
         self.readings = deque(maxlen=self.config.num_readings)
 
         self.name: str = 'CloudWatcher'
         self.firmware: str | None = None
@@ -76,14 +79,16 @@
         Args:
             raise_exceptions: Whether to raise exceptions, default True.
 
         Returns:
             True if connected, False otherwise.
         """
         try:
+            self._sensor.is_open or self._sensor.open()
+
             # Initialize and get static values.
             self.name = self.query(WeatherCommand.GET_INTERNAL_NAME)
             self.firmware = self.query(WeatherCommand.GET_FIRMWARE)
             self.serial_number = self.query(WeatherCommand.GET_SERIAL_NUMBER, parse_type=str)[0:4]
 
             # Check if we have wind speed.
             self.has_anemometer = self.query(WeatherCommand.CAN_GET_WINDSPEED, parse_type=bool)
@@ -113,34 +118,42 @@
                 if callback is not None:
                     callback(reading)
 
                 time.sleep(self.config.capture_delay)
         except KeyboardInterrupt:
             pass
 
-    def get_reading(self, units: WhichUnits = 'none') -> dict:
+    def get_reading(self, units: WhichUnits = 'none', get_errors: bool = False, avg_times: int = 3) -> dict:
         """ Get a single reading of all values.
 
         Args:
             units: The astropy units to return the reading in, default 'none',
                 can be 'metric' or 'imperial'.
+            get_errors: Whether to get the internal errors, default False.
+            avg_times: The number of times to average the readings, default 3.
 
         Returns:
             A dictionary of readings.
         """
+
+        def avg_times(fn, n=avg_times):
+            return round(sum(fn() for _ in range(n)) / n, 3)
+
         reading = {
             'timestamp': datetime.now().isoformat(),
-            'ambient_temp': self.get_ambient_temperature(),
-            'sky_temp': self.get_sky_temperature(),
-            'wind_speed': self.get_wind_speed(),
-            'rain_frequency': self.get_rain_frequency(),
+            'ambient_temp': avg_times(self.get_ambient_temperature),
+            'sky_temp': avg_times(self.get_sky_temperature),
+            'wind_speed': avg_times(self.get_wind_speed),
+            'rain_frequency': avg_times(self.get_rain_frequency),
             'pwm': self.get_pwm(),
-            **{f'error_{i}': err for i, err in enumerate(self.get_errors())}
         }
 
+        if get_errors:
+            reading.update(**{f'error_{i:02d}': err for i, err in enumerate(self.get_errors())})
+
         # Add the safety values.
         reading = self.get_safe_reading(reading)
 
         # Add astropy units if requested.
         if units != 'none':
             # First make them metric units.
             reading['ambient_temp'] *= u.Celsius
@@ -168,36 +181,36 @@
         """
         reading['cloud_condition'] = 'unknown'
         temp_diff = reading['sky_temp'] - reading['ambient_temp']
         if temp_diff >= self.thresholds.very_cloudy:
             reading['cloud_condition'] = 'very cloudy'
         elif temp_diff >= self.thresholds.cloudy:
             reading['cloud_condition'] = 'cloudy'
-        elif temp_diff < self.thresholds.cloudy:
+        else:
             reading['cloud_condition'] = 'clear'
 
         reading['wind_condition'] = 'unknown'
         if reading['wind_speed'] is not None:
             if reading['wind_speed'] >= self.thresholds.very_gusty:
                 reading['wind_condition'] = 'very gusty'
             elif reading['wind_speed'] >= self.thresholds.gusty:
                 reading['wind_condition'] = 'gusty'
             elif reading['wind_speed'] >= self.thresholds.very_windy:
                 reading['wind_condition'] = 'very windy'
             elif reading['wind_speed'] >= self.thresholds.windy:
                 reading['wind_condition'] = 'windy'
-            elif reading['wind_speed'] < self.thresholds.windy:
+            else:
                 reading['wind_condition'] = 'calm'
 
         reading['rain_condition'] = 'unknown'
         if reading['rain_frequency'] <= self.thresholds.rainy:
             reading['rain_condition'] = 'rainy'
         elif reading['rain_frequency'] <= self.thresholds.wet:
             reading['rain_condition'] = 'wet'
-        elif reading['rain_frequency'] > self.thresholds.wet:
+        else:
             reading['rain_condition'] = 'dry'
 
         reading['cloud_safe'] = True if reading['cloud_condition'] == 'clear' else False
         reading['wind_safe'] = True if reading['wind_condition'] == 'calm' else False
         reading['rain_safe'] = True if reading['rain_condition'] == 'dry' else False
 
         reading['is_safe'] = True if reading['cloud_safe'] and reading['wind_safe'] and reading['rain_safe'] else False
@@ -336,15 +349,14 @@
             cmd_params: Any parameters to send with the command.
             cmd_delim: The command delimiter, default '!'.
 
         Returns:
             The number of bytes written.
         """
         full_cmd = f'{cmd.value}{cmd_params}{cmd_delim}'
-        print(f'Writing command {full_cmd!r}')
         return self._sensor.write(full_cmd.encode())
 
     def read(self, return_raw: bool = False, verbose: bool = False, *args, **kwargs) -> list:
         """Reads a response from the sensor.
 
         The CloudWatcher always returns blocks of 15 characters, with each command
         returning one or more information blocks followed by a handshake block.
```

### Comparing `panoptes-aag-0.0.3/src/panoptes_aag.egg-info/PKG-INFO` & `panoptes_aag-0.0.5/src/panoptes_aag.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,48 @@
 Metadata-Version: 2.1
 Name: panoptes-aag
-Version: 0.0.3
+Version: 0.0.5
 Summary: Weather service for the Lunatico AAG CloudWatcher.
 Home-page: https://github.com/panoptes/aag-weather/
 Author: Wilfred Tyler Gee
 Author-email: wtylergee@gmail.com
 License: MIT
 Project-URL: Documentation, https://projectpanoptes.org/
 Platform: linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8
+License-File: LICENSE.txt
+Requires-Dist: importlib-metadata; python_version < "3.11"
+Requires-Dist: astropy
+Requires-Dist: fastapi[all]
+Requires-Dist: fastapi-utils
+Requires-Dist: httpie
+Requires-Dist: pandas
+Requires-Dist: pydantic
+Requires-Dist: pydantic-settings
+Requires-Dist: pyserial>=3.4
+Requires-Dist: python-dotenv
+Requires-Dist: typer[all]
 Provides-Extra: building
+Requires-Dist: pyscaffold>=4.3.1; extra == "building"
+Requires-Dist: pyscaffoldext-markdown; extra == "building"
+Requires-Dist: tox; extra == "building"
+Requires-Dist: twine; extra == "building"
 Provides-Extra: docs
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: piccolo-theme; extra == "docs"
+Requires-Dist: pytest_mpl; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
 Provides-Extra: testing
-License-File: LICENSE.txt
+Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest-cov; extra == "testing"
+Requires-Dist: tox; extra == "testing"
 
 # PANOPTES AAG weather reader
 
 [![codecov](https://codecov.io/github/panoptes/aag-weather/branch/main/graph/badge.svg?token=wwoAn40DVB)](https://codecov.io/github/panoptes/aag-weather)
 
 > Weather service for the Lunatico AAG CloudWatcher.
```

### Comparing `panoptes-aag-0.0.3/src/panoptes_aag.egg-info/SOURCES.txt` & `panoptes_aag-0.0.5/src/panoptes_aag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panoptes-aag-0.0.3/tests/test_weather.py` & `panoptes_aag-0.0.5/tests/test_weather.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,65 +15,89 @@
 def test_bad_port():
     os.environ['AAG_SERIAL_PORT'] = 'bad://'
 
     # Should raise an exception
     with pytest.raises(Exception):
         CloudSensor(connect=False)
 
+    # Should raise an exception
+    with pytest.raises(Exception):
+        CloudSensor(connect=True)
+
 
 def test_connect_loop():
     with pytest.raises(Exception):
         CloudSensor(connect=True, serial_port='loop://')
 
     sensor = CloudSensor(connect=False, serial_port='loop://')
     is_connected = sensor.connect(raise_exceptions=False)
     assert isinstance(sensor, CloudSensor)
     assert is_connected is False
     assert sensor.is_connected is False
 
+def test_str():
+    sensor = CloudSensor(connect=False, serial_port='loop://')
+    sensor.firmware = '5.12-fake'
+    sensor.serial_number = '1234567890'
+    assert str(sensor) == 'CloudSensor(CloudWatcher, FW=5.12-fake, SN=1234567890, port=loop://)'
+
 
 def test_get_safe_reading():
     os.environ['AAG_SERIAL_PORT'] = 'loop://'
     sensor = CloudSensor(connect=False)
     assert isinstance(sensor, CloudSensor)
     assert not sensor.is_connected
     assert sensor.connect(raise_exceptions=False) is False
 
-    # Make a fake reading entry.
+    # Make a fake reading that's safe.
     reading = {
-        'wind_speed': 10,
+        'wind_speed': 6,
         'ambient_temp': 20,
-        'sky_temp': 10,
+        'sky_temp': -20,
         'timestamp': '2021-01-01T00:00:00',
-        'rain_frequency': 2500,
+        'rain_frequency': 2600,
         'pwm': 0,
     }
+    sensor.readings.append(reading)
+
+    # Check is safe.
+    reading = sensor.get_safe_reading(reading=reading)
+    print(reading)
+    assert sensor.is_safe is True
+    assert reading['is_safe'] is True
+    assert reading['cloud_safe'] is True
+    assert reading['rain_safe'] is True
+    assert reading['wind_safe'] is True
+    assert reading['cloud_condition'] == 'clear'
+    assert reading['rain_condition'] == 'dry'
+    assert reading['wind_condition'] == 'calm'
 
-    # Check safety.
+    # Make very cloudy
+    reading['ambient_temp'] = 20
+    reading['sky_temp'] = 10
     reading = sensor.get_safe_reading(reading=reading)
+    assert sensor.is_safe is False
     assert reading['is_safe'] is False
     assert reading['cloud_safe'] is False
     assert reading['cloud_condition'] == 'very cloudy'
 
-    # Make safe
-    reading['ambient_temp'] = 20
-    reading['sky_temp'] = -20
-    print(reading)
+    # Make cloudy
+    reading['ambient_temp'] = 15
+    reading['sky_temp'] = -10
     reading = sensor.get_safe_reading(reading=reading)
-    print(reading)
-    assert reading['is_safe'] is True
-    assert reading['cloud_safe'] is True
-    assert reading['cloud_condition'] == 'clear'
+    assert sensor.is_safe is False
+    assert reading['cloud_condition'] == 'cloudy'
 
     # Make windy
     reading['wind_speed'] = 51
     reading = sensor.get_safe_reading(reading=reading)
     assert reading['is_safe'] is False
     assert reading['wind_safe'] is False
     assert reading['wind_condition'] == 'windy'
+    assert sensor.is_safe is False
 
     reading['wind_speed'] = 76
     reading = sensor.get_safe_reading(reading=reading)
     assert reading['wind_condition'] == 'very windy'
 
     reading['wind_speed'] = 101
     reading = sensor.get_safe_reading(reading=reading)
```

### Comparing `panoptes-aag-0.0.3/tox.ini` & `panoptes_aag-0.0.5/tox.ini`

 * *Files identical despite different names*

