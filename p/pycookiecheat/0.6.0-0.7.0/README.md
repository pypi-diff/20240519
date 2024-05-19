# Comparing `tmp/pycookiecheat-0.6.0.tar.gz` & `tmp/pycookiecheat-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycookiecheat-0.6.0.tar", last modified: Fri Sep 22 21:27:59 2023, max compression
+gzip compressed data, was "pycookiecheat-0.7.0.tar", last modified: Sun May 19 21:21:33 2024, max compression
```

## Comparing `pycookiecheat-0.6.0.tar` & `pycookiecheat-0.7.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.946025 pycookiecheat-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.942025 pycookiecheat-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      650 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.942025 pycookiecheat-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-09-22 21:27:59.946025 pycookiecheat-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 21:27:59.946025 pycookiecheat-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.942025 pycookiecheat-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.946025 pycookiecheat-0.6.0/src/pycookiecheat/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/src/pycookiecheat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/src/pycookiecheat/chrome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/src/pycookiecheat/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/src/pycookiecheat/firefox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.946025 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2023-09-22 21:27:59.000000 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-09-22 21:27:59.000000 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 21:27:59.000000 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 21:27:59.000000 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-09-22 21:27:59.000000 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-22 21:27:59.000000 pycookiecheat-0.6.0/src/pycookiecheat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 21:27:59.946025 pycookiecheat-0.6.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4558 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/tests/test_chrome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/tests/test_firefox.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-09-22 21:27:45.000000 pycookiecheat-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.781867 pycookiecheat-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.777867 pycookiecheat-0.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.777867 pycookiecheat-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-19 21:21:33.781867 pycookiecheat-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/flake.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/flake.nix
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:21:33.781867 pycookiecheat-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.773867 pycookiecheat-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.777867 pycookiecheat-0.7.0/src/pycookiecheat/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/src/pycookiecheat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/src/pycookiecheat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/src/pycookiecheat/chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/src/pycookiecheat/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/src/pycookiecheat/firefox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.777867 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-19 21:21:33.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 21:21:33.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:21:33.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 21:21:33.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:21:24.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-19 21:21:33.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 21:21:33.000000 pycookiecheat-0.7.0/src/pycookiecheat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:21:33.777867 pycookiecheat-0.7.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5876 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/tests/test_chrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12329 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/tests/test_firefox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-19 21:21:18.000000 pycookiecheat-0.7.0/tox.ini
```

### Comparing `pycookiecheat-0.6.0/.github/FUNDING.yml` & `pycookiecheat-0.7.0/.github/FUNDING.yml`

 * *Files 26% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 github: [n8henrie]
 custom: ["https://n8henrie.com/donate"]
 patreon: n8henrie
 open_collective: # Replace with a single Open Collective username
 ko_fi: # Replace with a single Ko-fi username
 tidelift: # Replace with a single Tidelift platform-name/package-name e.g., npm/babel
 community_bridge: # Replace with a single Community Bridge project-name e.g., cloud-foundry
-liberapay: # Replace with a single Liberapay username
+liberapay: n8henrie
 issuehunt: # Replace with a single IssueHunt username
 otechie: # Replace with a single Otechie username
```

### Comparing `pycookiecheat-0.6.0/.github/ISSUE_TEMPLATE.md` & `pycookiecheat-0.7.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pycookiecheat-0.6.0/.github/PULL_REQUEST_TEMPLATE.md` & `pycookiecheat-0.7.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pycookiecheat-0.6.0/.github/stale.yml` & `pycookiecheat-0.7.0/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `pycookiecheat-0.6.0/.github/workflows/python-package.yml` & `pycookiecheat-0.7.0/.github/workflows/python-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -4,53 +4,49 @@
   push:
     branches: [ master, dev ]
   pull_request:
     branches: [ master, dev ]
 
 jobs:
   build:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version:
-          - "3.7"
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
+          - "3.12"
 
     env:
-      TOX_TESTENV_PASSENV: "XAUTHORITY DISPLAY TEST_BROWSER_NAME TEST_BROWSER_PATH"
+      TOX_OVERRIDE: "testenv.pass_env+=XAUTHORITY,DISPLAY,TEST_BROWSER_NAME,TEST_BROWSER_PATH"
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
-    - name: pip cache
-      uses: actions/cache@v2
-      with:
-        path: ~/.cache/pip
-        key: ${{ runner.os }}-pip-${{ hashFiles('**/requirements*.txt') }}
-        restore-keys: |
-          ${{ runner.os }}-pip-
+        cache: 'pip'
     - name: Install tox
-      run: python -m pip install "tox>=3,<4"
+      run: python -m pip install .[test]
     - name: Install Brave
+      # https://brave.com/linux/#release-channel-installation
       run: |
         sudo apt-get update
         sudo apt-get install -y apt-transport-https curl
-        curl -s https://brave-browser-apt-release.s3.brave.com/brave-core.asc | sudo apt-key add -
-        echo "deb [arch=amd64] https://brave-browser-apt-release.s3.brave.com/ stable main" | sudo tee /etc/apt/sources.list.d/brave-browser-release.list
+        sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg
+        echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main" |
+          sudo tee /etc/apt/sources.list.d/brave-browser-release.list
         sudo apt-get update
         sudo apt-get install --yes brave-browser
     - name: Run tests via tox (Chromium)
       run: xvfb-run -- python -m tox -e py
     - name: Run tests via tox (Brave)
       env:
         TEST_BROWSER_NAME: Brave
         TEST_BROWSER_PATH: /usr/bin/brave-browser
       run: xvfb-run -- python -m tox -e py
-    - if: "matrix.python-version == '3.9'"
+    - if: "matrix.python-version == '3.12'"
       name: Lint
       run: python -m tox -e lint
```

### Comparing `pycookiecheat-0.6.0/.github/workflows/python-publish.yml` & `pycookiecheat-0.7.0/.github/workflows/python-publish.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 on:
   push:
     tags:
       - '*'
 
 jobs:
   deploy:
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: '3.x'
+        cache: 'pip'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install build setuptools wheel twine
+        python -m pip install .[dev]
     - name: Build and publish
       env:
         TWINE_USERNAME: __token__
         TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
       run: |
         python -m build
         python -m twine upload dist/*
```

### Comparing `pycookiecheat-0.6.0/CHANGELOG.md` & `pycookiecheat-0.7.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 # [Changelog](https://keepachangelog.com)
 
+## v0.7.0 :: 20240105
+
+- Now requires python >= 3.8
+    - 3.7 is now EoL: https://devguide.python.org/versions/
+    - pycookiecheat seems to build and run on 3.7, but several test
+      dependencies require versions that are either incompatible with 3.12 or
+      3.7
+- Add `BrowserType` enum
+    - Instead of passing a string (e.g. "chrome"), please import and use a
+      `BrowserType` (e.g. `BrowserType.CHROME`)
+    - Add deprecation warning for passing strings
+- Added a nix flake to facilitate testing multiple python versions
+- Add basic logging
+- Add CLI tool
+- Add `as_cookies` parameter to allow returning `list[Cookie]` instead of
+  `dict` (without breaking backward compatibility)
+- Loosen dependency constrains, which should make usage as a library easier
+
 ## v0.6.0 :: 20230324
 
-- Add firefox support , thanks to @grandchild
+- Add firefox support, thanks to @grandchild
     - Also would like to welcome @grandchild as a new member of the
       pycookiecheat team!
 
 ## v0.5.0 :: 20230324
 
 - Add support for Brave thanks to @chrisgavin!
 - Add support for Slack thanks to @hraftery!
```

### Comparing `pycookiecheat-0.6.0/CONTRIBUTING.md` & `pycookiecheat-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pycookiecheat-0.6.0/LICENSE` & `pycookiecheat-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycookiecheat-0.6.0/PKG-INFO` & `pycookiecheat-0.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: pycookiecheat
-Version: 0.6.0
+Version: 0.7.0
 Summary: Borrow cookies from your browser's authenticated session for use in Python scripts.
 Author-email: Nathan Henrie <nate@n8henrie.com>
 License: MIT
 Project-URL: homepage, https://github.com/n8henrie/pycookiecheat
 Keywords: pycookiecheat,chrome,chromium cookies,cookies,firefox
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: cryptography==41.0.4
-Requires-Dist: keyring==23.0.0
+Requires-Dist: cryptography==42.*
+Requires-Dist: keyring==25.*
 Provides-Extra: test
-Requires-Dist: black==22.12.0; extra == "test"
-Requires-Dist: flake8-docstrings==1.5.0; extra == "test"
-Requires-Dist: flake8-import-order==0.18.1; extra == "test"
-Requires-Dist: flake8==3.8.4; extra == "test"
-Requires-Dist: mypy==0.991; extra == "test"
-Requires-Dist: pep8-naming==0.11.1; extra == "test"
-Requires-Dist: playwright==1.14.1; extra == "test"
-Requires-Dist: pycodestyle==2.6.0; extra == "test"
-Requires-Dist: pylint==2.7.2; extra == "test"
-Requires-Dist: pytest==7.2.0; extra == "test"
-Requires-Dist: tox==4.2.8; extra == "test"
+Requires-Dist: black==24.*; extra == "test"
+Requires-Dist: flake8-docstrings==1.*; extra == "test"
+Requires-Dist: flake8-import-order==0.18.*; extra == "test"
+Requires-Dist: flake8==7.*; extra == "test"
+Requires-Dist: mypy==1.*; extra == "test"
+Requires-Dist: pep8-naming==0.13.*; extra == "test"
+Requires-Dist: playwright==1.*; extra == "test"
+Requires-Dist: pycodestyle==2.*; extra == "test"
+Requires-Dist: pytest==8.*; extra == "test"
+Requires-Dist: tox==4.*; extra == "test"
 Provides-Extra: dev
-Requires-Dist: build==0.6.0.post1; extra == "dev"
-Requires-Dist: twine==3.4.2; extra == "dev"
-Requires-Dist: wheel==0.37.0; extra == "dev"
+Requires-Dist: build==1.*; extra == "dev"
+Requires-Dist: twine==5.*; extra == "dev"
+Requires-Dist: wheel==0.43.*; extra == "dev"
 
 # pycookiecheat
 
 [![master branch build
 status](https://github.com/n8henrie/pycookiecheat/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/n8henrie/pycookiecheat/actions/workflows/python-package.yml)
 
 Borrow cookies from your browser's authenticated session for use in Python
@@ -46,15 +45,16 @@
 -   Free software: MIT
 -   Documentation: http://n8h.me/HufI1w
 
 ## Installation
 
 **NB:** Use `pip` and `python` instead of `pip3` and `python3` if you're still
 on Python 2 and using pycookiecheat < v0.4.0. pycookiecheat >= v0.4.0 requires
-Python 3.5+, and may soon go to 3.6+.
+Python 3 and in general will aim to support python versions that are stable and
+not yet end-of-life: <https://devguide.python.org/versions>.
 
 - `python3 -m pip install pycookiecheat`
 
 ### Installation notes regarding alternative keyrings on Linux
 
 See [#12](https://github.com/n8henrie/pycookiecheat/issues/12). Chrome is now
 using a few different keyrings to store your `Chrome Safe Storage` password,
@@ -74,36 +74,63 @@
 1. `git clone https://github.com/n8henrie/pycookiecheat.git`
 1. `cd pycookiecheat`
 1. `python3 -m venv .venv`
 1. `./.venv/bin/python -m pip install -e .[dev]`
 
 ## Usage
 
+### As a Command-Line Tool
+
+As of v0.7.0, pycookiecheat includes a command line tool for ease of use. By
+default it prints the cookies to stdout as JSON but can also output a file in
+Netscape Cookie File Format.
+
+After installation, the CLI tool can be run as a python module `python -m` or
+with a standalone console script:
+
+```console
+$ pycookiecheat --help
+usage: pycookiecheat [-h] -u URL [-b BROWSER] [-o OUTPUT_FILE]
+
+Copy cookies from Chrome or Firefox and output as json
+
+options:
+  -h, --help            show this help message and exit
+  -u URL, --url URL     requires scheme (e.g. `https://`)
+  -b BROWSER, --browser BROWSER
+  -o OUTPUT_FILE, --output-file OUTPUT_FILE
+                        Output to this file in netscape cookie file format
+```
+
+### As a Python Library
+
 ```python
-from pycookiecheat import chrome_cookies
+from pycookiecheat import BrowserType, chrome_cookies
 import requests
 
-url = 'http://example.com/fake.html'
+url = 'https://n8henrie.com'
 
 # Uses Chrome's default cookies filepath by default
 cookies = chrome_cookies(url)
 r = requests.get(url, cookies=cookies)
+
+# Using an alternate browser
+cookies = chrome_cookies(url, browser=BrowserType.CHROMIUM)
 ```
 
 Use the `cookie_file` keyword-argument to specify a different filepath for the
 cookies-file: `chrome_cookies(url, cookie_file='/abspath/to/cookies')`
 
-Keep in mind that pycookiecheat defaults to looking for cookies for Google
-Chrome, not Chromium, so if you're using the latter, you'll need to manually
-specify something like `"/home/username/.config/chromium/Default/Cookies"` (for
-Linux) as your `cookie_file`.
+You may be able to retrieve cookies for alternative Chromium-based browsers by
+manually specifying something like
+`"/home/username/.config/BrowserName/Default/Cookies"` as your `cookie_file`.
 
 ## Features
 
-- Returns decrypted cookies from Google Chrome, Brave, or Slack, on OSX or
+- Returns decrypted cookies from Google Chrome, Brave, or Slack, on MacOS or
   Linux.
 - Optionally outputs cookies to file (thanks to Muntashir Al-Islam!)
 
 ## FAQ / Troubleshooting
 
 ### How about Windows?
 
@@ -137,17 +164,35 @@
 
 ## Buy Me a Coffee
 
 [☕️](https://n8henrie.com/donate)
 
 # [Changelog](https://keepachangelog.com)
 
+## v0.7.0 :: 20240105
+
+- Now requires python >= 3.8
+    - 3.7 is now EoL: https://devguide.python.org/versions/
+    - pycookiecheat seems to build and run on 3.7, but several test
+      dependencies require versions that are either incompatible with 3.12 or
+      3.7
+- Add `BrowserType` enum
+    - Instead of passing a string (e.g. "chrome"), please import and use a
+      `BrowserType` (e.g. `BrowserType.CHROME`)
+    - Add deprecation warning for passing strings
+- Added a nix flake to facilitate testing multiple python versions
+- Add basic logging
+- Add CLI tool
+- Add `as_cookies` parameter to allow returning `list[Cookie]` instead of
+  `dict` (without breaking backward compatibility)
+- Loosen dependency constrains, which should make usage as a library easier
+
 ## v0.6.0 :: 20230324
 
-- Add firefox support , thanks to @grandchild
+- Add firefox support, thanks to @grandchild
     - Also would like to welcome @grandchild as a new member of the
       pycookiecheat team!
 
 ## v0.5.0 :: 20230324
 
 - Add support for Brave thanks to @chrisgavin!
 - Add support for Slack thanks to @hraftery!
```

### Comparing `pycookiecheat-0.6.0/README.md` & `pycookiecheat-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 -   Free software: MIT
 -   Documentation: http://n8h.me/HufI1w
 
 ## Installation
 
 **NB:** Use `pip` and `python` instead of `pip3` and `python3` if you're still
 on Python 2 and using pycookiecheat < v0.4.0. pycookiecheat >= v0.4.0 requires
-Python 3.5+, and may soon go to 3.6+.
+Python 3 and in general will aim to support python versions that are stable and
+not yet end-of-life: <https://devguide.python.org/versions>.
 
 - `python3 -m pip install pycookiecheat`
 
 ### Installation notes regarding alternative keyrings on Linux
 
 See [#12](https://github.com/n8henrie/pycookiecheat/issues/12). Chrome is now
 using a few different keyrings to store your `Chrome Safe Storage` password,
@@ -37,36 +38,63 @@
 1. `git clone https://github.com/n8henrie/pycookiecheat.git`
 1. `cd pycookiecheat`
 1. `python3 -m venv .venv`
 1. `./.venv/bin/python -m pip install -e .[dev]`
 
 ## Usage
 
+### As a Command-Line Tool
+
+As of v0.7.0, pycookiecheat includes a command line tool for ease of use. By
+default it prints the cookies to stdout as JSON but can also output a file in
+Netscape Cookie File Format.
+
+After installation, the CLI tool can be run as a python module `python -m` or
+with a standalone console script:
+
+```console
+$ pycookiecheat --help
+usage: pycookiecheat [-h] -u URL [-b BROWSER] [-o OUTPUT_FILE]
+
+Copy cookies from Chrome or Firefox and output as json
+
+options:
+  -h, --help            show this help message and exit
+  -u URL, --url URL     requires scheme (e.g. `https://`)
+  -b BROWSER, --browser BROWSER
+  -o OUTPUT_FILE, --output-file OUTPUT_FILE
+                        Output to this file in netscape cookie file format
+```
+
+### As a Python Library
+
 ```python
-from pycookiecheat import chrome_cookies
+from pycookiecheat import BrowserType, chrome_cookies
 import requests
 
-url = 'http://example.com/fake.html'
+url = 'https://n8henrie.com'
 
 # Uses Chrome's default cookies filepath by default
 cookies = chrome_cookies(url)
 r = requests.get(url, cookies=cookies)
+
+# Using an alternate browser
+cookies = chrome_cookies(url, browser=BrowserType.CHROMIUM)
 ```
 
 Use the `cookie_file` keyword-argument to specify a different filepath for the
 cookies-file: `chrome_cookies(url, cookie_file='/abspath/to/cookies')`
 
-Keep in mind that pycookiecheat defaults to looking for cookies for Google
-Chrome, not Chromium, so if you're using the latter, you'll need to manually
-specify something like `"/home/username/.config/chromium/Default/Cookies"` (for
-Linux) as your `cookie_file`.
+You may be able to retrieve cookies for alternative Chromium-based browsers by
+manually specifying something like
+`"/home/username/.config/BrowserName/Default/Cookies"` as your `cookie_file`.
 
 ## Features
 
-- Returns decrypted cookies from Google Chrome, Brave, or Slack, on OSX or
+- Returns decrypted cookies from Google Chrome, Brave, or Slack, on MacOS or
   Linux.
 - Optionally outputs cookies to file (thanks to Muntashir Al-Islam!)
 
 ## FAQ / Troubleshooting
 
 ### How about Windows?
```

### Comparing `pycookiecheat-0.6.0/pyproject.toml` & `pycookiecheat-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>65", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 79
-target_version = ['py311']
+target_version = ['py38']
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 order_by_type = false
 line_length = 79
 
@@ -21,15 +21,15 @@
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 follow_imports = "silent"
 ignore_missing_imports = true
-python_version = "3.11"
+python_version = "3.8"
 show_column_numbers = true
 warn_incomplete_stub = false
 warn_redundant_casts = true
 warn_unused_ignores = true
 
 [project]
 name = "pycookiecheat"
@@ -38,37 +38,39 @@
 license = { text = "MIT" }
 description = "Borrow cookies from your browser's authenticated session for use in Python scripts."
 authors = [ {name = "Nathan Henrie", email = "nate@n8henrie.com"} ]
 keywords = ["pycookiecheat", "chrome", "chromium cookies", "cookies", "firefox"]
 classifiers= [
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "cryptography==41.0.4",
-    "keyring==23.0.0",
+    "cryptography==42.*",
+    "keyring==25.*",
 ]
 
 [project.optional-dependencies]
 test = [
-    "black==22.12.0",
-    "flake8-docstrings==1.5.0",
-    "flake8-import-order==0.18.1",
-    "flake8==3.8.4",
-    "mypy==0.991",
-    "pep8-naming==0.11.1",
-    "playwright==1.14.1",
-    "pycodestyle==2.6.0",
-    "pylint==2.7.2",
-    "pytest==7.2.0",
-    "tox==4.2.8",
+    "black==24.*",
+    "flake8-docstrings==1.*",
+    "flake8-import-order==0.18.*",
+    "flake8==7.*",
+    "mypy==1.*",
+    "pep8-naming==0.13.*",
+    "playwright==1.*",
+    "pycodestyle==2.*",
+    "pytest==8.*",
+    "tox==4.*",
 ]
 dev = [
-    "build==0.6.0.post1",
-    "twine==3.4.2",
-    "wheel==0.37.0",
+    "build==1.*",
+    "twine==5.*",
+    "wheel==0.43.*",
 ]
+
+[project.scripts]
+pycookiecheat = "pycookiecheat.__main__:main"
```

### Comparing `pycookiecheat-0.6.0/src/pycookiecheat/chrome.py` & `pycookiecheat-0.7.0/src/pycookiecheat/chrome.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,85 @@
 """pycookiecheat.py :: Retrieve and decrypt cookies from Chrome.
 
-See relevant post at http://n8h.me/HufI1w
+See relevant post at https://n8henrie.com/2013/11/use-chromes-cookies-for-easier-downloading-with-python-requests/  # noqa
 
 Use your browser's cookies to make grabbing data from login-protected sites
 easier. Intended for use with Python Requests http://python-requests.org
 
 Accepts a URL from which it tries to extract a domain. If you want to force the
 domain, just send it the domain you'd like to use instead.
-
-Adapted from my code at http://n8h.me/HufI1w
 """
 
-import pathlib
+from __future__ import annotations
+
+import logging
 import sqlite3
 import sys
 import typing as t
 import urllib.error
 import urllib.parse
+from pathlib import Path
 
 import keyring
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import CBC
 from cryptography.hazmat.primitives.hashes import SHA1
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
 
-from pycookiecheat.common import Cookie, generate_host_keys
+from pycookiecheat.common import (
+    BrowserType,
+    Cookie,
+    deprecation_warning,
+    generate_host_keys,
+    write_cookie_file,
+)
+
+logger = logging.getLogger(__name__)
 
 
 def clean(decrypted: bytes) -> str:
     r"""Strip padding from decrypted value.
 
     Remove number indicated by padding
     e.g. if last is '\x0e' then ord('\x0e') == 14, so take off 14.
 
     Args:
         decrypted: decrypted value
     Returns:
-        Decrypted stripped of junk padding
-
+        decrypted, stripped of padding
     """
     last = decrypted[-1]
     if isinstance(last, int):
         return decrypted[:-last].decode("utf8")
-    return decrypted[: -ord(last)].decode("utf8")
+
+    try:
+        cleaned = decrypted[: -ord(last)].decode("utf8")
+    except UnicodeDecodeError:
+        logging.error(
+            "UTF8 decoding of the decrypted cookie failed. This is most often "
+            "due to attempting decryption with an incorrect key. Consider "
+            "searching the pycookiecheat issues for `UnicodeDecodeError`."
+        )
+        raise
+
+    return cleaned
 
 
 def chrome_decrypt(
     encrypted_value: bytes, key: bytes, init_vector: bytes
 ) -> str:
     """Decrypt Chrome/Chromium's encrypted cookies.
 
     Args:
         encrypted_value: Encrypted cookie from Chrome/Chromium's cookie file
         key: Key to decrypt encrypted_value
         init_vector: Initialization vector for decrypting encrypted_value
     Returns:
         Decrypted value of encrypted_value
-
     """
     # Encrypted cookies should be prefixed with 'v10' or 'v11' according to the
     # Chromium code. Strip it off.
     encrypted_value = encrypted_value[3:]
 
     cipher = Cipher(
         algorithm=AES(key),
@@ -69,227 +87,230 @@
     )
     decryptor = cipher.decryptor()
     decrypted = decryptor.update(encrypted_value) + decryptor.finalize()
 
     return clean(decrypted)
 
 
-def get_osx_config(browser: str) -> dict:
-    """Get settings for getting Chrome/Chromium cookies on OSX.
+def get_macos_config(browser: BrowserType) -> dict:
+    """Get settings for getting Chrome/Chromium cookies on MacOS.
 
     Args:
-        browser: Either "Chrome", "Chromium", "Slack", or "Brave"
+        browser: Enum variant representing browser of interest
     Returns:
         Config dictionary for Chrome/Chromium cookie decryption
-
     """
-    # Verify supported browser, fail early otherwise. Mind the capitalization,
-    # which is necessary for the password retrieval.
-    browser = browser.title()
+    app_support = Path("Library/Application Support")
+    # TODO: Refactor to exhaustive match statement once depending on >= 3.10
     try:
-        app_support = "~/Library/Application Support"
-        cookie_file = {
-            "Chrome": f"{app_support}/Google/Chrome/Default/Cookies",
-            "Chromium": f"{app_support}/Chromium/Default/Cookies",
-            "Brave": (
-                f"{app_support}/BraveSoftware/Brave-Browser/Default/Cookies"
-            ),
-            "Slack": f"{app_support}/Slack/Cookies",
+        cookies_suffix = {
+            BrowserType.CHROME: "Google/Chrome/Default/Cookies",
+            BrowserType.CHROMIUM: "Chromium/Default/Cookies",
+            BrowserType.BRAVE: "BraveSoftware/Brave-Browser/Default/Cookies",
+            BrowserType.SLACK: "Slack/Cookies",
         }[browser]
-    except KeyError:
-        raise ValueError(
-            "Browser must be either Chrome, Chromium, Slack, or Brave, "
-            "but found {browser}"
+    except KeyError as e:
+        errmsg = (
+            f"{browser} is not a valid BrowserType for {__name__}"
+            ".get_macos_config"
         )
+        raise ValueError(errmsg) from e
+    cookie_file = "~" / app_support / cookies_suffix
 
-    # Alas, the cookies can be in two places on MacOS (well, one place, but
-    # possibly via that insane sandboxing of the filesystem that goes on now)
-    # so we have to hit the filesystem to check. This is the location is Slack
-    # is installed via direct download.
-    if (
-        browser == "Slack"
-        and not pathlib.Path(cookie_file).expanduser().exists()
-    ):
+    # Slack cookies can be in two places on MacOS depending on whether it was
+    # installed from the App Store or direct download.
+    if browser is BrowserType.SLACK and not cookie_file.exists():
         # And this location if Slack is installed from App Store
         cookie_file = (
             "~/Library/Containers/com.tinyspeck.slackmacgap/Data"
-            + cookie_file[1:]
+            / app_support
+            / cookies_suffix
         )
 
-    keyring_lookup = f"{browser} Safe Storage"
-    my_pass = keyring.get_password(keyring_lookup, browser)
+    browser_name = browser.title()
+    keyring_service_name = f"{browser_name} Safe Storage"
 
-    if my_pass is None:
-        raise ValueError(
-            f"Could not find a password for the pair "
-            f"({keyring_lookup}, {browser}). Please manually verify they "
-            "exist in Keychain Access.app"
+    keyring_username = browser_name
+    if browser is BrowserType.SLACK:
+        keyring_username = "Slack Key"
+
+    key_material = keyring.get_password(keyring_service_name, keyring_username)
+    if key_material is None:
+        errmsg = (
+            "Could not find a password for the pair "
+            f"({keyring_service_name}, {keyring_username}). Please manually "
+            "verify they exist in `Keychain Access.app`."
         )
+        raise ValueError(errmsg)
 
     config = {
-        "my_pass": my_pass,
+        "key_material": key_material,
         "iterations": 1003,
         "cookie_file": cookie_file,
     }
     return config
 
 
-def get_linux_config(browser: str) -> dict:
+def get_linux_config(browser: BrowserType) -> dict:
     """Get the settings for Chrome/Chromium cookies on Linux.
 
     Args:
-        browser: Either "Chrome", "Chromium", "Slack", or "Brave"
+        browser: Enum variant representing browser of interest
     Returns:
         Config dictionary for Chrome/Chromium cookie decryption
-
     """
-    # Verify supported browser, fail early otherwise. Mind the capitalization,
-    # which is necessary for the password retrieval.
-    browser = browser.title()
-
-    try:
-        cookie_file = {
-            "Chrome": "~/.config/google-chrome/Default/Cookies",
-            "Chromium": "~/.config/chromium/Default/Cookies",
-            "Brave": "~/.config/BraveSoftware/Brave-Browser/Default/Cookies",
-            "Slack": "~/.config/Slack/Cookies",
+    cookie_file = (
+        Path("~/.config")
+        / {
+            BrowserType.CHROME: "google-chrome/Default/Cookies",
+            BrowserType.CHROMIUM: "chromium/Default/Cookies",
+            BrowserType.BRAVE: "BraveSoftware/Brave-Browser/Default/Cookies",
+            BrowserType.SLACK: "Slack/Cookies",
         }[browser]
-    except KeyError:
-        raise ValueError(
-            "Browser must be either Chrome, Chromium, Slack, or Brave, "
-            "but found {browser}"
-        )
+    )
 
     # Set the default linux password
     config = {
-        "my_pass": "peanuts",
+        "key_material": "peanuts",
         "iterations": 1,
         "cookie_file": cookie_file,
     }
 
+    browser_name = browser.title()
+
     # Try to get pass from Gnome / libsecret if it seems available
     # https://github.com/n8henrie/pycookiecheat/issues/12
-    pass_found = False
+    key_material = None
     try:
         import gi
 
         gi.require_version("Secret", "1")
         from gi.repository import Secret
     except ImportError:
-        pass
+        logger.info("Was not able to import `Secret` from `gi.repository`")
     else:
         flags = Secret.ServiceFlags.LOAD_COLLECTIONS
         service = Secret.Service.get_sync(flags)
 
         gnome_keyring = service.get_collections()
         unlocked_keyrings = service.unlock_sync(gnome_keyring).unlocked
 
         # While Slack on Linux has its own Cookies file, the password
         # is stored in a keyring named the same as Chromium's, but with
         # an "application" attribute of "Slack".
-        keyring_name = f"{browser} Safe Storage"
+        keyring_name = f"{browser_name} Safe Storage"
 
         for unlocked_keyring in unlocked_keyrings:
             for item in unlocked_keyring.get_items():
                 if item.get_label() == keyring_name:
                     item_app = item.get_attributes().get(
                         "application", browser
                     )
                     if item_app.lower() != browser.lower():
                         continue
                     item.load_secret_sync()
-                    config["my_pass"] = item.get_secret().get_text()
-                    pass_found = True
+                    key_material = item.get_secret().get_text()
                     break
             else:
                 # Inner loop didn't `break`, keep looking
                 continue
 
             # Inner loop did `break`, so `break` outer loop
             break
 
     # Try to get pass from keyring, which should support KDE / KWallet
     # if dbus-python is installed.
-    if not pass_found:
+    if key_material is None:
         try:
-            my_pass = keyring.get_password(
-                f"{browser} Keys",
-                f"{browser} Safe Storage",
+            key_material = keyring.get_password(
+                f"{browser_name} Keys",
+                f"{browser_name} Safe Storage",
             )
         except RuntimeError:
-            pass
-        else:
-            if my_pass:
-                config["my_pass"] = my_pass
+            logger.info("Was not able to access secrets from keyring")
+
+    # Overwrite the default only if a different password has been found
+    if key_material is not None:
+        config["key_material"] = key_material
 
     return config
 
 
 def chrome_cookies(
     url: str,
-    cookie_file: t.Optional[str] = None,
-    browser: str = "Chrome",
-    curl_cookie_file: t.Optional[str] = None,
+    cookie_file: t.Optional[t.Union[str, Path]] = None,
+    browser: t.Optional[BrowserType] = BrowserType.CHROME,
+    curl_cookie_file: t.Optional[t.Union[str, Path]] = None,
     password: t.Optional[t.Union[bytes, str]] = None,
-) -> dict:
-    """Retrieve cookies from Chrome/Chromium on OSX or Linux.
+    as_cookies: bool = False,
+) -> t.Union[dict, list[Cookie]]:
+    """Retrieve cookies from Chrome/Chromium on MacOS or Linux.
 
     Args:
         url: Domain from which to retrieve cookies, starting with http(s)
         cookie_file: Path to alternate file to search for cookies
-        browser: Name of the browser's cookies to read ('Chrome' or 'Chromium')
+        browser: Enum variant representing browser of interest
         curl_cookie_file: Path to save the cookie file to be used with cURL
         password: Optional system password
+        as_cookies: Return `list[Cookie]` instead of `dict`
     Returns:
         Dictionary of cookie values for URL
-
     """
     parsed_url = urllib.parse.urlparse(url)
     if parsed_url.scheme:
         domain = parsed_url.netloc
     else:
         raise urllib.error.URLError("You must include a scheme with your URL.")
 
-    # If running Chrome on OSX
+    # TODO: 20231229 remove str support after some deprecation period
+    if not isinstance(browser, BrowserType):
+        deprecation_warning(
+            "Please pass `browser` as a `BrowserType` instead of "
+            f"`{browser.__class__.__qualname__}`."
+        )
+        browser = BrowserType(browser)
+
+    # If running Chrome on MacOS
     if sys.platform == "darwin":
-        config = get_osx_config(browser)
+        config = get_macos_config(browser)
     elif sys.platform.startswith("linux"):
         config = get_linux_config(browser)
     else:
-        raise OSError("This script only works on OSX or Linux.")
+        raise OSError("This script only works on MacOS or Linux.")
 
     config.update(
         {"init_vector": b" " * 16, "length": 16, "salt": b"saltysalt"}
     )
 
-    if cookie_file:
-        cookie_file = str(pathlib.Path(cookie_file).expanduser())
-    else:
-        cookie_file = str(pathlib.Path(config["cookie_file"]).expanduser())
+    if cookie_file is None:
+        cookie_file = config["cookie_file"]
+    cookie_file = Path(cookie_file)
 
     if isinstance(password, bytes):
-        config["my_pass"] = password
+        config["key_material"] = password
     elif isinstance(password, str):
-        config["my_pass"] = password.encode("utf8")
-    elif isinstance(config["my_pass"], str):
-        config["my_pass"] = config["my_pass"].encode("utf8")
+        config["key_material"] = password.encode("utf8")
+    elif isinstance(config["key_material"], str):
+        config["key_material"] = config["key_material"].encode("utf8")
 
     kdf = PBKDF2HMAC(
         algorithm=SHA1(),
         iterations=config["iterations"],
         length=config["length"],
         salt=config["salt"],
     )
-    enc_key = kdf.derive(config["my_pass"])
+    enc_key = kdf.derive(config["key_material"])
 
     try:
-        conn = sqlite3.connect("file:{}?mode=ro".format(cookie_file), uri=True)
-    except sqlite3.OperationalError:
-        print("Unable to connect to cookie_file at: {}\n".format(cookie_file))
-        raise
+        conn = sqlite3.connect(
+            f"file:{cookie_file.expanduser()}?mode=ro", uri=True
+        )
+    except sqlite3.OperationalError as e:
+        logger.error("Unable to connect to cookie_file at %s", cookie_file)
+        raise e
 
     conn.row_factory = sqlite3.Row
 
     # Check whether the column name is `secure` or `is_secure`
     secure_column_name = "is_secure"
     for (
         sl_no,
@@ -326,12 +347,13 @@
                 )
             del row["encrypted_value"]
             cookies.append(Cookie(**row))
 
     conn.rollback()
 
     if curl_cookie_file:
-        with open(curl_cookie_file, "w") as text_file:
-            for c in cookies:
-                print(c.as_cookie_file_line(), file=text_file)
+        write_cookie_file(curl_cookie_file, cookies)
+
+    if as_cookies:
+        return cookies
 
     return {c.name: c.value for c in cookies}
```

### Comparing `pycookiecheat-0.6.0/src/pycookiecheat/firefox.py` & `pycookiecheat-0.7.0/src/pycookiecheat/firefox.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,37 @@
 domain, just send it the domain you'd like to use instead.
 
 Example:
     >>> from pycookiecheat import firefox_cookies
     >>> firefox_cookies("https://github.com")
     {'logged_in': 'yes', 'user_session': 'n3tZzN45P56Ovg5MB'}
 """
+
+from __future__ import annotations
+
 import configparser
+import logging
 import shutil
 import sqlite3
 import sys
 import tempfile
+import typing as t
 import urllib.error
 import urllib.parse
 from pathlib import Path
-from typing import Dict, List, Optional
 
-from pycookiecheat.common import Cookie, generate_host_keys
+from pycookiecheat.common import (
+    BrowserType,
+    Cookie,
+    deprecation_warning,
+    generate_host_keys,
+    write_cookie_file,
+)
 
+logger = logging.getLogger(__name__)
 
 FIREFOX_COOKIE_SELECT_SQL = """
     SELECT
         `host` AS host_key,
         name,
         value,
         `path`,
@@ -38,46 +49,44 @@
 """
 The query for selecting the cookies for a host.
 
 Rename some columns to match the Chrome cookie db row names.
 This makes the common.Cookie class simpler.
 """
 
-FIREFOX_OS_PROFILE_DIRS: Dict[str, Dict[str, str]] = {
+FIREFOX_OS_PROFILE_DIRS: dict[str, dict[str, str]] = {
     "linux": {
-        "Firefox": "~/.mozilla/firefox",
+        BrowserType.FIREFOX: "~/.mozilla/firefox",
     },
-    "osx": {
-        "Firefox": "~/Library/Application Support/Firefox/Profiles",
+    "macos": {
+        BrowserType.FIREFOX: "~/Library/Application Support/Firefox/Profiles",
     },
     "windows": {
-        "Firefox": "~/AppData/Roaming/Mozilla/Firefox/Profiles",
+        BrowserType.FIREFOX: "~/AppData/Roaming/Mozilla/Firefox/Profiles",
     },
 }
 
 
 class FirefoxProfileNotPopulatedError(Exception):
     """Raised when the Firefox profile has never been used."""
 
     pass
 
 
-def _get_profiles_dir_for_os(os: str, browser: str = "Firefox") -> Path:
+def _get_profiles_dir_for_os(
+    os: str, browser: BrowserType = BrowserType.FIREFOX
+) -> Path:
     """Retrieve the default directory containing the user profiles."""
-    browser = browser.title()
     try:
         os_config = FIREFOX_OS_PROFILE_DIRS[os]
     except KeyError:
         raise ValueError(
             f"OS must be one of {list(FIREFOX_OS_PROFILE_DIRS.keys())}"
         )
-    try:
-        return Path(os_config[browser]).expanduser()
-    except KeyError:
-        raise ValueError(f"Browser must be one of {list(os_config.keys())}")
+    return Path(os_config[browser]).expanduser()
 
 
 def _find_firefox_default_profile(firefox_dir: Path) -> str:
     """
     Return the name of the default Firefox profile.
 
     Args:
@@ -110,26 +119,26 @@
             if profiles_ini[profile].get("Default") == "1":
                 return profiles_ini[profile]["Path"]
         if profiles:
             return profiles_ini[profiles[0]]["Path"]
         raise Exception("no profiles found at {}".format(firefox_dir))
 
 
-def _copy_if_exists(src: List[Path], dest: Path) -> None:
+def _copy_if_exists(src: list[Path], dest: Path) -> None:
     for file in src:
         try:
             shutil.copy2(file, dest)
         except FileNotFoundError:
             pass
 
 
 def _load_firefox_cookie_db(
     profiles_dir: Path,
     tmp_dir: Path,
-    profile_name: Optional[str] = None,
+    profile_name: t.Optional[str] = None,
 ) -> Path:
     """
     Return a file path to the selected browser profile's cookie database.
 
     Args:
         profiles_dir: Browser+OS paths profiles_dir path
         tmp_dir: A temporary directory to copy the DB file(s) into
@@ -166,58 +175,72 @@
     with sqlite3.connect(db_file) as con:
         con.execute("PRAGMA journal_mode=OFF;")  # merge WAL
     return db_file
 
 
 def firefox_cookies(
     url: str,
-    profile_name: Optional[str] = None,
-    browser: str = "Firefox",
-    curl_cookie_file: Optional[str] = None,
-) -> Dict[str, str]:
-    """Retrieve cookies from Chrome/Chromium on OSX or Linux.
+    profile_name: t.Optional[str] = None,
+    browser: BrowserType = BrowserType.FIREFOX,
+    curl_cookie_file: t.Optional[str] = None,
+    as_cookies: bool = False,
+) -> t.Union[dict, list[Cookie]]:
+    """Retrieve cookies from Firefox on MacOS or Linux.
 
     Args:
         url: Domain from which to retrieve cookies, starting with http(s)
         profile_name: Name (or glob pattern) of the Firefox profile to search
                       for cookies -- if none given it will find the configured
                       default profile
-        browser: Name of the browser's cookies to read (must be 'Firefox')
+        browser: Enum variant representing browser of interest
         curl_cookie_file: Path to save the cookie file to be used with cURL
+        as_cookies: Return `list[Cookie]` instead of `dict`
     Returns:
         Dictionary of cookie values for URL
     """
     parsed_url = urllib.parse.urlparse(url)
     if parsed_url.scheme:
         domain = parsed_url.netloc
     else:
         raise urllib.error.URLError("You must include a scheme with your URL.")
 
     if sys.platform.startswith("linux"):
         os = "linux"
     elif sys.platform == "darwin":
-        os = "osx"
+        os = "macos"
     elif sys.platform == "win32":
         os = "windows"
     else:
         raise OSError(
             "This script only works on "
             + ", ".join(FIREFOX_OS_PROFILE_DIRS.keys())
         )
+
+    # TODO: 20231229 remove str support after some deprecation period
+    if not isinstance(browser, BrowserType):
+        deprecation_warning(
+            "Please pass `browser` as a `BrowserType` instead of "
+            f"`{browser.__class__.__qualname__}`."
+        )
+        browser = BrowserType(browser)
+
     profiles_dir = _get_profiles_dir_for_os(os, browser)
 
     cookies: list[Cookie] = []
     with tempfile.TemporaryDirectory() as tmp_dir:
         db_file = _load_firefox_cookie_db(
             profiles_dir, Path(tmp_dir), profile_name
         )
         for host_key in generate_host_keys(domain):
             with sqlite3.connect(db_file) as con:
                 con.row_factory = sqlite3.Row
                 res = con.execute(FIREFOX_COOKIE_SELECT_SQL, (host_key,))
                 for row in res.fetchall():
                     cookies.append(Cookie(**row))
+
     if curl_cookie_file:
-        with open(curl_cookie_file, "w") as text_file:
-            for c in cookies:
-                print(c.as_cookie_file_line(), file=text_file)
+        write_cookie_file(curl_cookie_file, cookies)
+
+    if as_cookies:
+        return cookies
+
     return {c.name: c.value for c in cookies}
```

### Comparing `pycookiecheat-0.6.0/src/pycookiecheat.egg-info/PKG-INFO` & `pycookiecheat-0.7.0/src/pycookiecheat.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: pycookiecheat
-Version: 0.6.0
+Version: 0.7.0
 Summary: Borrow cookies from your browser's authenticated session for use in Python scripts.
 Author-email: Nathan Henrie <nate@n8henrie.com>
 License: MIT
 Project-URL: homepage, https://github.com/n8henrie/pycookiecheat
 Keywords: pycookiecheat,chrome,chromium cookies,cookies,firefox
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: cryptography==41.0.4
-Requires-Dist: keyring==23.0.0
+Requires-Dist: cryptography==42.*
+Requires-Dist: keyring==25.*
 Provides-Extra: test
-Requires-Dist: black==22.12.0; extra == "test"
-Requires-Dist: flake8-docstrings==1.5.0; extra == "test"
-Requires-Dist: flake8-import-order==0.18.1; extra == "test"
-Requires-Dist: flake8==3.8.4; extra == "test"
-Requires-Dist: mypy==0.991; extra == "test"
-Requires-Dist: pep8-naming==0.11.1; extra == "test"
-Requires-Dist: playwright==1.14.1; extra == "test"
-Requires-Dist: pycodestyle==2.6.0; extra == "test"
-Requires-Dist: pylint==2.7.2; extra == "test"
-Requires-Dist: pytest==7.2.0; extra == "test"
-Requires-Dist: tox==4.2.8; extra == "test"
+Requires-Dist: black==24.*; extra == "test"
+Requires-Dist: flake8-docstrings==1.*; extra == "test"
+Requires-Dist: flake8-import-order==0.18.*; extra == "test"
+Requires-Dist: flake8==7.*; extra == "test"
+Requires-Dist: mypy==1.*; extra == "test"
+Requires-Dist: pep8-naming==0.13.*; extra == "test"
+Requires-Dist: playwright==1.*; extra == "test"
+Requires-Dist: pycodestyle==2.*; extra == "test"
+Requires-Dist: pytest==8.*; extra == "test"
+Requires-Dist: tox==4.*; extra == "test"
 Provides-Extra: dev
-Requires-Dist: build==0.6.0.post1; extra == "dev"
-Requires-Dist: twine==3.4.2; extra == "dev"
-Requires-Dist: wheel==0.37.0; extra == "dev"
+Requires-Dist: build==1.*; extra == "dev"
+Requires-Dist: twine==5.*; extra == "dev"
+Requires-Dist: wheel==0.43.*; extra == "dev"
 
 # pycookiecheat
 
 [![master branch build
 status](https://github.com/n8henrie/pycookiecheat/actions/workflows/python-package.yml/badge.svg?branch=master)](https://github.com/n8henrie/pycookiecheat/actions/workflows/python-package.yml)
 
 Borrow cookies from your browser's authenticated session for use in Python
@@ -46,15 +45,16 @@
 -   Free software: MIT
 -   Documentation: http://n8h.me/HufI1w
 
 ## Installation
 
 **NB:** Use `pip` and `python` instead of `pip3` and `python3` if you're still
 on Python 2 and using pycookiecheat < v0.4.0. pycookiecheat >= v0.4.0 requires
-Python 3.5+, and may soon go to 3.6+.
+Python 3 and in general will aim to support python versions that are stable and
+not yet end-of-life: <https://devguide.python.org/versions>.
 
 - `python3 -m pip install pycookiecheat`
 
 ### Installation notes regarding alternative keyrings on Linux
 
 See [#12](https://github.com/n8henrie/pycookiecheat/issues/12). Chrome is now
 using a few different keyrings to store your `Chrome Safe Storage` password,
@@ -74,36 +74,63 @@
 1. `git clone https://github.com/n8henrie/pycookiecheat.git`
 1. `cd pycookiecheat`
 1. `python3 -m venv .venv`
 1. `./.venv/bin/python -m pip install -e .[dev]`
 
 ## Usage
 
+### As a Command-Line Tool
+
+As of v0.7.0, pycookiecheat includes a command line tool for ease of use. By
+default it prints the cookies to stdout as JSON but can also output a file in
+Netscape Cookie File Format.
+
+After installation, the CLI tool can be run as a python module `python -m` or
+with a standalone console script:
+
+```console
+$ pycookiecheat --help
+usage: pycookiecheat [-h] -u URL [-b BROWSER] [-o OUTPUT_FILE]
+
+Copy cookies from Chrome or Firefox and output as json
+
+options:
+  -h, --help            show this help message and exit
+  -u URL, --url URL     requires scheme (e.g. `https://`)
+  -b BROWSER, --browser BROWSER
+  -o OUTPUT_FILE, --output-file OUTPUT_FILE
+                        Output to this file in netscape cookie file format
+```
+
+### As a Python Library
+
 ```python
-from pycookiecheat import chrome_cookies
+from pycookiecheat import BrowserType, chrome_cookies
 import requests
 
-url = 'http://example.com/fake.html'
+url = 'https://n8henrie.com'
 
 # Uses Chrome's default cookies filepath by default
 cookies = chrome_cookies(url)
 r = requests.get(url, cookies=cookies)
+
+# Using an alternate browser
+cookies = chrome_cookies(url, browser=BrowserType.CHROMIUM)
 ```
 
 Use the `cookie_file` keyword-argument to specify a different filepath for the
 cookies-file: `chrome_cookies(url, cookie_file='/abspath/to/cookies')`
 
-Keep in mind that pycookiecheat defaults to looking for cookies for Google
-Chrome, not Chromium, so if you're using the latter, you'll need to manually
-specify something like `"/home/username/.config/chromium/Default/Cookies"` (for
-Linux) as your `cookie_file`.
+You may be able to retrieve cookies for alternative Chromium-based browsers by
+manually specifying something like
+`"/home/username/.config/BrowserName/Default/Cookies"` as your `cookie_file`.
 
 ## Features
 
-- Returns decrypted cookies from Google Chrome, Brave, or Slack, on OSX or
+- Returns decrypted cookies from Google Chrome, Brave, or Slack, on MacOS or
   Linux.
 - Optionally outputs cookies to file (thanks to Muntashir Al-Islam!)
 
 ## FAQ / Troubleshooting
 
 ### How about Windows?
 
@@ -137,17 +164,35 @@
 
 ## Buy Me a Coffee
 
 [☕️](https://n8henrie.com/donate)
 
 # [Changelog](https://keepachangelog.com)
 
+## v0.7.0 :: 20240105
+
+- Now requires python >= 3.8
+    - 3.7 is now EoL: https://devguide.python.org/versions/
+    - pycookiecheat seems to build and run on 3.7, but several test
+      dependencies require versions that are either incompatible with 3.12 or
+      3.7
+- Add `BrowserType` enum
+    - Instead of passing a string (e.g. "chrome"), please import and use a
+      `BrowserType` (e.g. `BrowserType.CHROME`)
+    - Add deprecation warning for passing strings
+- Added a nix flake to facilitate testing multiple python versions
+- Add basic logging
+- Add CLI tool
+- Add `as_cookies` parameter to allow returning `list[Cookie]` instead of
+  `dict` (without breaking backward compatibility)
+- Loosen dependency constrains, which should make usage as a library easier
+
 ## v0.6.0 :: 20230324
 
-- Add firefox support , thanks to @grandchild
+- Add firefox support, thanks to @grandchild
     - Also would like to welcome @grandchild as a new member of the
       pycookiecheat team!
 
 ## v0.5.0 :: 20230324
 
 - Add support for Brave thanks to @chrisgavin!
 - Add support for Slack thanks to @hraftery!
```

### Comparing `pycookiecheat-0.6.0/src/pycookiecheat.egg-info/SOURCES.txt` & `pycookiecheat-0.7.0/src/pycookiecheat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,32 @@
 .python-version
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE
 README.md
+flake.lock
+flake.nix
 pyproject.toml
 tox.ini
 .github/FUNDING.yml
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/stale.yml
 .github/workflows/python-package.yml
 .github/workflows/python-publish.yml
 src/pycookiecheat/__init__.py
+src/pycookiecheat/__main__.py
 src/pycookiecheat/chrome.py
 src/pycookiecheat/common.py
 src/pycookiecheat/firefox.py
 src/pycookiecheat.egg-info/PKG-INFO
 src/pycookiecheat.egg-info/SOURCES.txt
 src/pycookiecheat.egg-info/dependency_links.txt
+src/pycookiecheat.egg-info/entry_points.txt
 src/pycookiecheat.egg-info/not-zip-safe
 src/pycookiecheat.egg-info/requires.txt
 src/pycookiecheat.egg-info/top_level.txt
 tests/test_chrome.py
 tests/test_common.py
 tests/test_firefox.py
```

### Comparing `pycookiecheat-0.6.0/tests/test_chrome.py` & `pycookiecheat-0.7.0/tests/test_chrome.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from tempfile import TemporaryDirectory
 from urllib.error import URLError
 from uuid import uuid4
 
 import pytest
 from playwright.sync_api import sync_playwright
 
-from pycookiecheat import chrome_cookies
-from pycookiecheat.chrome import get_linux_config, get_osx_config
+from pycookiecheat import BrowserType, chrome_cookies
+from pycookiecheat.chrome import get_linux_config, get_macos_config
 
 BROWSER = os.environ.get("TEST_BROWSER_NAME", "Chromium")
 
 
 @pytest.fixture(scope="module")
 def ci_setup() -> t.Generator:
     """Set up Chrome's cookies file and directory.
@@ -48,15 +48,15 @@
             cookies_home,
             headless=False,
             chromium_sandbox=False,
             args=["--no-sandbox", "--disable-setuid-sandbox"],
             ignore_default_args=[
                 "--use-mock-keychain",
             ],
-            executable_path=ex_path,  # type: ignore
+            executable_path=ex_path,
         )
         page = browser.new_page()
         page.goto("https://n8henrie.com")
         browser.add_cookies(
             [
                 {
                     "name": "test_pycookiecheat",
@@ -84,54 +84,97 @@
     The domain must specify a scheme (http or https).
 
     """
     with pytest.raises(URLError):
         chrome_cookies("n8henrie.com")
 
 
+def test_warns_for_string_browser(ci_setup: str) -> None:
+    """Browser should be passed as `BrowserType` and warns for strings."""
+    never_been_here = "http://{0}.com".format(uuid4())
+    with pytest.warns(
+        DeprecationWarning,
+        match=(
+            "Please pass `browser` as a `BrowserType` " "instead of `str`."
+        ),
+    ):
+        empty_dict = chrome_cookies(
+            never_been_here,
+            cookie_file=ci_setup,
+            browser=BROWSER,  # type: ignore
+        )
+    assert empty_dict == dict()
+
+
 def test_no_cookies(ci_setup: str) -> None:
     """Ensure that no cookies are returned for a fake url."""
     never_been_here = "http://{0}.com".format(uuid4())
     empty_dict = chrome_cookies(
         never_been_here,
         cookie_file=ci_setup,
-        browser=BROWSER,
+        browser=BrowserType(BROWSER),
     )
     assert empty_dict == dict()
 
 
 def test_fake_cookie(ci_setup: str) -> None:
     """Tests a fake cookie from the website below.
 
     For this to pass, you'll have to visit the url and put in "TestCookie" and
     "Just_a_test!" to set a temporary cookie with the appropriate values.
     """
-    cookies = chrome_cookies(
-        "https://n8henrie.com",
-        cookie_file=ci_setup,
-        browser=BROWSER,
+    cookies = t.cast(
+        dict,
+        chrome_cookies(
+            "https://n8henrie.com",
+            cookie_file=ci_setup,
+            browser=BrowserType(BROWSER),
+        ),
     )
     assert cookies.get("test_pycookiecheat") == "It worked!"
 
 
 def test_raises_on_wrong_browser() -> None:
     """Passing a browser other than Chrome or Chromium raises ValueError."""
     with pytest.raises(ValueError):
-        chrome_cookies("https://n8henrie.com", browser="Safari")
+        BrowserType("edge")
+
+    with pytest.raises(ValueError):
+        chrome_cookies(
+            "https://n8henrie.com",
+            browser="Safari",  # type: ignore
+        )
 
 
 def test_slack_config() -> None:
     """Tests configuring for cookies from the macos Slack app.
 
     Hard to come up with a mock test, since the only functionality provided by
     the Slack app feature is to read cookies from a different file. So opt to
     just test that new functionality with something simple and fairly robust.
     """
+    cfgs = []
     if sys.platform == "darwin":
-        cfg1 = get_osx_config("slack")
-        cfg2 = get_osx_config("SLACK")
+        cfgs.append(get_macos_config(BrowserType.SLACK))
+
+        parent = Path(
+            "~/Library/Application Support/BraveSoftware/Brave-Browser/Default"
+        )
+        parent.mkdir(parents=True)
+        (parent / "Cookies").touch()
+        cfgs.append(get_macos_config(BrowserType.SLACK))
+
+        assert cfgs[0] != cfgs[1]
     else:
-        cfg1 = get_linux_config("slack")
-        cfg2 = get_linux_config("SLACK")
+        cfgs.append(get_linux_config(BrowserType.SLACK))
+
+    for cfg in cfgs:
+        assert "Slack" in str(cfg["cookie_file"])
+
 
-    assert cfg1 == cfg2
-    assert "Slack" in cfg1["cookie_file"]
+def test_macos_bad_browser_variant() -> None:
+    """Tests the error message resulting from unrecognized BrowserType."""
+    for invalid in [BrowserType.FIREFOX, "foo"]:
+        with pytest.raises(
+            ValueError, match=f"{invalid} is not a valid BrowserType"
+        ):
+            get_macos_config(invalid)  # type: ignore
```

### Comparing `pycookiecheat-0.6.0/tests/test_common.py` & `pycookiecheat-0.7.0/tests/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for pycookiecheat.common."""
+
 from typing import Iterable
 
 import pytest
 
 from pycookiecheat.common import Cookie, generate_host_keys
```

### Comparing `pycookiecheat-0.6.0/tests/test_firefox.py` & `pycookiecheat-0.7.0/tests/test_firefox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Tests for Firefox cookies & helper functions."""
+
 import re
+import typing as t
 from datetime import datetime, timedelta
 from http.cookies import SimpleCookie
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from pathlib import Path
 from textwrap import dedent
 from threading import Thread
-from typing import Any, Iterator, Optional
 from unittest.mock import patch
 from urllib.error import URLError
 
 import pytest
 from playwright.sync_api import sync_playwright
 from pytest import FixtureRequest, TempPathFactory
 
+from pycookiecheat import BrowserType, firefox_cookies
 from pycookiecheat.firefox import (
     _find_firefox_default_profile,
     _get_profiles_dir_for_os,
     _load_firefox_cookie_db,
-    firefox_cookies,
     FirefoxProfileNotPopulatedError,
 )
 
-
 TEST_PROFILE_NAME = "test-profile"
 TEST_PROFILE_DIR = f"1234abcd.{TEST_PROFILE_NAME}"
 
 PROFILES_INI_VERSION1 = dedent(
     f"""
     [General]
     StartWithLastProfile=1
@@ -99,15 +99,15 @@
     Path={TEST_PROFILE_DIR}
     """
 )
 
 
 def _make_test_profiles(
     tmp_path: Path, profiles_ini_content: str, populate: bool = True
-) -> Iterator[Path]:
+) -> t.Iterator[Path]:
     """Create a Firefox data dir with profile & (optionally) populate it.
 
     All of the fixtures using this function use the pytest builtin `tmp_path`
     or `tmp_path_factory` fixtures to create their temporary directories.
     """
     profile_dir = tmp_path / TEST_PROFILE_DIR
     profile_dir.mkdir()
@@ -122,15 +122,15 @@
         "pycookiecheat.firefox._get_profiles_dir_for_os",
         return_value=tmp_path,
     ):
         yield tmp_path
 
 
 @pytest.fixture(scope="module")
-def profiles(tmp_path_factory: TempPathFactory) -> Iterator[Path]:
+def profiles(tmp_path_factory: TempPathFactory) -> t.Iterator[Path]:
     """Create a Firefox data dir with profiles & cookie DBs."""
     yield from _make_test_profiles(
         tmp_path_factory.mktemp("_"), PROFILES_INI_VERSION2
     )
 
 
 @pytest.fixture(
@@ -140,45 +140,45 @@
         PROFILES_INI_VERSION2,
         PROFILES_INI_VERSION1_NO_DEFAULT,
         PROFILES_INI_VERSION2_NO_DEFAULT,
     ],
 )
 def profiles_ini_versions(
     tmp_path_factory: TempPathFactory, request: FixtureRequest
-) -> Iterator[Path]:
+) -> t.Iterator[Path]:
     """Create a Firefox data dir using varius `profiles.ini` types.
 
     Use different file format versions and contents.
     """
     yield from _make_test_profiles(tmp_path_factory.mktemp("_"), request.param)
 
 
 @pytest.fixture(scope="module")
-def no_profiles(tmp_path_factory: TempPathFactory) -> Iterator[Path]:
+def no_profiles(tmp_path_factory: TempPathFactory) -> t.Iterator[Path]:
     """Create a Firefox data dir with a `profiles.ini` with no profiles."""
     yield from _make_test_profiles(
         tmp_path_factory.mktemp("_"), PROFILES_INI_EMPTY
     )
 
 
 # TODO: Making this fixture module-scoped breaks the tests using the `profiles`
 #       fixture. Find out why.
 @pytest.fixture
-def profiles_unpopulated(tmp_path: Path) -> Iterator[Path]:
+def profiles_unpopulated(tmp_path: Path) -> t.Iterator[Path]:
     """Create a Firefox data dir with valid but upopulated `profiles.ini` file.
 
     "Unpopulated" means never actually used to launch Firefox with.
     """
     yield from _make_test_profiles(
         tmp_path, PROFILES_INI_VERSION2, populate=False
     )
 
 
 @pytest.fixture(scope="session")
-def cookie_server() -> Iterator[int]:
+def cookie_server() -> t.Iterator[int]:
     """Start an `HTTPServer` on localhost which sets a cookie.
 
     Replies to GET requests by setting a "foo: bar" cookie.
     Used as fixture for testing cookie retrieval.
 
     Returns:
         The port of the server on localhost.
@@ -197,25 +197,25 @@
             this_time_tomorrow = datetime.utcnow() + timedelta(days=1)
             cookie["foo"]["expires"] = this_time_tomorrow.strftime(
                 "%a, %d %b %Y %H:%M:%S GMT"
             )
             self.send_header("Set-Cookie", cookie["foo"].OutputString())
             self.end_headers()
 
-        def log_message(self, *_: Any) -> None:
+        def log_message(self, *_: t.Any) -> None:
             pass  # Suppress logging
 
     with HTTPServer(("localhost", 0), CookieSetter) as server:
         Thread(target=server.serve_forever, daemon=True).start()
         yield server.server_port
         server.shutdown()
 
 
 @pytest.fixture
-def set_cookie(profiles: Path, cookie_server: int) -> Iterator[None]:
+def set_cookie(profiles: Path, cookie_server: int) -> t.Iterator[None]:
     """Launch Firefox and visit the cookie-setting server.
 
     The cookie is set, saved to the DB and the browser closes. Ideally the
     browser should still be running while the cookie tests run, but the
     synchronous playwright API doesn't support that.
     """
     profile_dir = profiles / TEST_PROFILE_DIR
@@ -239,36 +239,38 @@
 # _get_profiles_dir_for_os()
 
 
 @pytest.mark.parametrize(
     "os_name,expected_dir",
     [
         ("linux", "~/.mozilla/firefox"),
-        ("osx", "~/Library/Application Support/Firefox/Profiles"),
+        ("macos", "~/Library/Application Support/Firefox/Profiles"),
         ("windows", "~/AppData/Roaming/Mozilla/Firefox/Profiles"),
     ],
 )
 def test_get_profiles_dir_for_os_valid(
     os_name: str, expected_dir: str
 ) -> None:
     """Test profile paths for each OS.
 
     Test only implicit "Firefox" default, since it's the only type we currently
     support.
     """
-    profiles_dir = _get_profiles_dir_for_os(os_name, "Firefox")
+    profiles_dir = _get_profiles_dir_for_os(os_name, BrowserType.FIREFOX)
     assert profiles_dir == Path(expected_dir).expanduser()
 
 
 def test_get_profiles_dir_for_os_invalid() -> None:
     """Test invalid OS and browser names."""
     with pytest.raises(ValueError, match="OS must be one of"):
         _get_profiles_dir_for_os("invalid")
-    with pytest.raises(ValueError, match="Browser must be one of"):
-        _get_profiles_dir_for_os("linux", "invalid")
+    with pytest.raises(
+        ValueError, match="'invalid' is not a valid BrowserType"
+    ):
+        _get_profiles_dir_for_os("linux", BrowserType("invalid"))
 
 
 # _find_firefox_default_profile()
 
 
 def test_firefox_get_default_profile_valid(
     profiles_ini_versions: Path,
@@ -298,15 +300,15 @@
     assert db_path == tmp_path / "cookies.sqlite"
     assert db_path.exists()
 
 
 @pytest.mark.parametrize("profile_name", [TEST_PROFILE_DIR, None])
 def test_load_firefox_cookie_db_unpopulated(
     tmp_path: Path,
-    profile_name: Optional[str],
+    profile_name: t.Optional[str],
     profiles_unpopulated: Path,
 ) -> None:
     """Test loading Firefox cookies DB from an unpopulated profile."""
     with pytest.raises(FirefoxProfileNotPopulatedError):
         _load_firefox_cookie_db(
             profiles_unpopulated,
             tmp_path,
@@ -330,15 +332,37 @@
 
 
 # firefox_cookies()
 
 
 def test_firefox_cookies(set_cookie: None) -> None:
     """Test getting Firefox cookies after visiting a site with cookies."""
-    cookies = firefox_cookies("http://localhost", TEST_PROFILE_DIR)
+    cookies = t.cast(
+        dict, firefox_cookies("http://localhost", TEST_PROFILE_DIR)
+    )
+    assert len(cookies) > 0
+    assert cookies["foo"] == "bar"
+
+
+def test_warns_for_string_browser(set_cookie: None) -> None:
+    """Browser should be passed as `BrowserType` and warns for strings."""
+    with pytest.warns(
+        DeprecationWarning,
+        match=(
+            "Please pass `browser` as a `BrowserType` " "instead of `str`."
+        ),
+    ):
+        cookies = t.cast(
+            dict,
+            firefox_cookies(
+                "http://localhost",
+                TEST_PROFILE_DIR,
+                browser="firefox",  # type: ignore
+            ),
+        )
     assert len(cookies) > 0
     assert cookies["foo"] == "bar"
 
 
 def test_firefox_no_cookies(profiles: Path) -> None:
     """Ensure Firefox cookies for an unvisited site are empty."""
     cookies = firefox_cookies("http://example.org", TEST_PROFILE_DIR)
@@ -361,15 +385,18 @@
     firefox_cookies(
         "http://localhost",
         profile_name=TEST_PROFILE_DIR,
         curl_cookie_file=str(cookie_file),
     )
     assert cookie_file.exists()
     assert re.fullmatch(
-        r"localhost\tTRUE\t/\tFALSE\t[0-9]+\tfoo\tbar\n",
+        (
+            r"# Netscape HTTP Cookie File\nlocalhost\tTRUE\t/\tFALSE\t[0-9]+"
+            r"\tfoo\tbar\n"
+        ),
         cookie_file.read_text(),
     )
 
 
 @pytest.mark.parametrize("fake_os", ["linux", "darwin", "win32"])
 def test_firefox_cookies_os(fake_os: str, profiles: Path) -> None:
     """Ensure the few lines of OS switching code are covered by a test."""
```

### Comparing `pycookiecheat-0.6.0/tox.ini` & `pycookiecheat-0.7.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py3{7,8,9,10,11},lint
+envlist = py3{8,9,10,11,12},lint
 isolated_build = True
 
 [testenv]
 extras = test
 commands =
     python -m playwright install chromium
     python -m playwright install-deps chromium
```

