# Comparing `tmp/pytest_localftpserver-1.3.1.tar.gz` & `tmp/pytest_localftpserver-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_localftpserver-1.3.1.tar", last modified: Fri May 17 20:08:20 2024, max compression
+gzip compressed data, was "pytest_localftpserver-1.3.2.tar", last modified: Sun May 19 18:04:21 2024, max compression
```

## Comparing `pytest_localftpserver-1.3.1.tar` & `pytest_localftpserver-1.3.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.950363 pytest_localftpserver-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.946363 pytest_localftpserver-1.3.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.946363 pytest_localftpserver-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/.github/workflows/CI_CD_actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-17 20:08:20.950363 pytest_localftpserver-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.946363 pytest_localftpserver-1.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.942363 pytest_localftpserver-1.3.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.946363 pytest_localftpserver-1.3.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/_templates/autosummary/method.rst
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/api_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     9117 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.950363 pytest_localftpserver-1.3.1/pytest_localftpserver/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/pytest_localftpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/pytest_localftpserver/default_keycert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    12737 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/pytest_localftpserver/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/pytest_localftpserver/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    38317 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/pytest_localftpserver/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.950363 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 20:08:20.000000 pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:08:20.950363 pytest_localftpserver-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:20.950363 pytest_localftpserver-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/not_a_valid_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/test_keycert.pem
--rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/test_pytest_localftpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/test_pytest_localftpserver_TLS.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tests/test_pytest_localftpserver_with_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-17 20:08:16.000000 pytest_localftpserver-1.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.926660 pytest_localftpserver-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.918660 pytest_localftpserver-1.3.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.918660 pytest_localftpserver-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/.github/workflows/CI_CD_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-19 18:04:21.926660 pytest_localftpserver-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.922660 pytest_localftpserver-1.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.914660 pytest_localftpserver-1.3.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.922660 pytest_localftpserver-1.3.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/_templates/autosummary/method.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/api_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9117 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.922660 pytest_localftpserver-1.3.2/pytest_localftpserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/pytest_localftpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/pytest_localftpserver/default_keycert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    12737 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/pytest_localftpserver/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/pytest_localftpserver/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38317 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/pytest_localftpserver/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.926660 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 18:04:21.000000 pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:04:21.926660 pytest_localftpserver-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:21.926660 pytest_localftpserver-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/not_a_valid_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/test_keycert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    27354 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/test_pytest_localftpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/test_pytest_localftpserver_TLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tests/test_pytest_localftpserver_with_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-19 18:04:14.000000 pytest_localftpserver-1.3.2/tox.ini
```

### Comparing `pytest_localftpserver-1.3.1/.coveragerc` & `pytest_localftpserver-1.3.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/.github/workflows/CI_CD_actions.yml` & `pytest_localftpserver-1.3.2/.github/workflows/CI_CD_actions.yml`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/.gitignore` & `pytest_localftpserver-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/CONTRIBUTING.rst` & `pytest_localftpserver-1.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/HISTORY.rst` & `pytest_localftpserver-1.3.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/LICENSE` & `pytest_localftpserver-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/Makefile` & `pytest_localftpserver-1.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/PKG-INFO` & `pytest_localftpserver-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_localftpserver
-Version: 1.3.1
+Version: 1.3.2
 Summary: A PyTest plugin which provides an FTP fixture for your tests
 Author-email: Oz N Tiram <oz.tiram@gmail.com>
 Project-URL: homepage, https://github.com/oz123/pytest-localftpserver
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,15 +23,14 @@
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pyftpdlib>=1.2.0
 Requires-Dist: PyOpenSSL
 Requires-Dist: pytest
-Requires-Dist: wget
 
 PyTest FTP Server
 =================
 
 
 .. image:: https://img.shields.io/pypi/v/pytest_localftpserver.svg
         :target:  https://pypi.org/project/pytest-localftpserver/
```

### Comparing `pytest_localftpserver-1.3.1/README.rst` & `pytest_localftpserver-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/docs/Makefile` & `pytest_localftpserver-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/docs/_templates/autosummary/class.rst` & `pytest_localftpserver-1.3.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/docs/conf.py` & `pytest_localftpserver-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/docs/installation.rst` & `pytest_localftpserver-1.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/docs/make.bat` & `pytest_localftpserver-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/docs/usage.rst` & `pytest_localftpserver-1.3.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/pyproject.toml` & `pytest_localftpserver-1.3.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,14 @@
   'Topic :: Software Development :: Testing :: Mocking'
 ]
 
 dependencies = [
   'pyftpdlib>=1.2.0',
   'PyOpenSSL',
   'pytest',
-  'wget'
 ]
 
 [tool.setuptools]
 packages = ["pytest_localftpserver"]
 
 [project.entry-points.pytest11]
 localftpserver = "pytest_localftpserver.plugin"
```

### Comparing `pytest_localftpserver-1.3.1/pytest_localftpserver/default_keycert.pem` & `pytest_localftpserver-1.3.2/pytest_localftpserver/default_keycert.pem`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/pytest_localftpserver/helper_functions.py` & `pytest_localftpserver-1.3.2/pytest_localftpserver/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/pytest_localftpserver/plugin.py` & `pytest_localftpserver-1.3.2/pytest_localftpserver/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/pytest_localftpserver/servers.py` & `pytest_localftpserver-1.3.2/pytest_localftpserver/servers.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/PKG-INFO` & `pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_localftpserver
-Version: 1.3.1
+Version: 1.3.2
 Summary: A PyTest plugin which provides an FTP fixture for your tests
 Author-email: Oz N Tiram <oz.tiram@gmail.com>
 Project-URL: homepage, https://github.com/oz123/pytest-localftpserver
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
@@ -23,15 +23,14 @@
 Classifier: Topic :: Software Development :: Testing :: Mocking
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: pyftpdlib>=1.2.0
 Requires-Dist: PyOpenSSL
 Requires-Dist: pytest
-Requires-Dist: wget
 
 PyTest FTP Server
 =================
 
 
 .. image:: https://img.shields.io/pypi/v/pytest_localftpserver.svg
         :target:  https://pypi.org/project/pytest-localftpserver/
```

### Comparing `pytest_localftpserver-1.3.1/pytest_localftpserver.egg-info/SOURCES.txt` & `pytest_localftpserver-1.3.2/pytest_localftpserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/tests/test_helper_functions.py` & `pytest_localftpserver-1.3.2/tests/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/tests/test_keycert.pem` & `pytest_localftpserver-1.3.2/tests/test_keycert.pem`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/tests/test_pytest_localftpserver.py` & `pytest_localftpserver-1.3.2/tests/test_pytest_localftpserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 Tests for `pytest_localftpserver` module.
 """
 
 from ftplib import FTP, FTP_TLS, error_perm
 import logging
 import os
+import urllib.request
 
 import pytest
-import wget
 
 from pytest_localftpserver.plugin import PytestLocalFTPServer
 from pytest_localftpserver.servers import USE_PROCESS
 from pytest_localftpserver.helper_functions import DEFAULT_CERTFILE
 
 
 from ssl import SSLContext, PROTOCOL_TLS_CLIENT, TLSVersion
@@ -154,22 +154,18 @@
         Tempdir to download files to
     base_url: str
         Base ur to the ftp server to mimic its folder structure
     url_iterable: iterable of urls
         Contains urls to check
     """
     # checking files by url
-    download_dir = tmpdir.mkdir("download_url")
     for url in url_iterable:
         _, filename = os.path.split(os.path.relpath(url, base_url))
-        download_file = download_dir.join(filename)
-        wget.download(url, str(download_file))
-        with open(str(download_file)) as f:
-            assert f.read() == filename
-    download_dir.remove()
+        with urllib.request.urlopen(url) as response:
+            assert response.read() == filename.encode()
 
 
 def check_get_file_contents(
     tmpdir,
     path_list,
     iterable_len,
     files_on_server,
```

### Comparing `pytest_localftpserver-1.3.1/tests/test_pytest_localftpserver_TLS.py` & `pytest_localftpserver-1.3.2/tests/test_pytest_localftpserver_TLS.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/tests/test_pytest_localftpserver_with_env_var.py` & `pytest_localftpserver-1.3.2/tests/test_pytest_localftpserver_with_env_var.py`

 * *Files identical despite different names*

### Comparing `pytest_localftpserver-1.3.1/tox.ini` & `pytest_localftpserver-1.3.2/tox.ini`

 * *Files identical despite different names*

