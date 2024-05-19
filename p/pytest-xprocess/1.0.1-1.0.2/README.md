# Comparing `tmp/pytest-xprocess-1.0.1.tar.gz` & `tmp/pytest-xprocess-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-xprocess-1.0.1.tar", last modified: Sun Mar 31 19:29:14 2024, max compression
+gzip compressed data, was "pytest-xprocess-1.0.2.tar", last modified: Sun May 19 16:11:01 2024, max compression
```

## Comparing `pytest-xprocess-1.0.1.tar` & `pytest-xprocess-1.0.2.tar`

### file list

```diff
@@ -1,74 +1,30 @@
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-03-31 19:29:14.780570 pytest-xprocess-1.0.1/
--rw-r--r--   0 gfvante    (501) staff       (20)     1054 2022-08-15 09:33:20.000000 pytest-xprocess-1.0.1/LICENSE
--rw-r--r--   0 gfvante    (501) staff       (20)       98 2024-03-31 19:14:23.000000 pytest-xprocess-1.0.1/MANIFEST.in
--rw-r--r--   0 gfvante    (501) staff       (20)     3742 2024-03-31 19:29:14.780496 pytest-xprocess-1.0.1/PKG-INFO
--rwxr-xr-x   0 gfvante    (501) staff       (20)     2851 2024-03-31 19:20:11.000000 pytest-xprocess-1.0.1/README.rst
--rw-r--r--   0 gfvante    (501) staff       (20)      108 2023-01-05 15:26:55.000000 pytest-xprocess-1.0.1/pyproject.toml
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-03-31 19:29:14.780184 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/
--rw-r--r--   0 gfvante    (501) staff       (20)     3742 2024-03-31 19:29:14.000000 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/PKG-INFO
--rw-r--r--   0 gfvante    (501) staff       (20)     3433 2024-03-31 19:29:14.000000 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/SOURCES.txt
--rw-r--r--   0 gfvante    (501) staff       (20)        1 2024-03-31 19:29:14.000000 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/dependency_links.txt
--rw-r--r--   0 gfvante    (501) staff       (20)       47 2024-03-31 19:29:14.000000 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/entry_points.txt
--rw-r--r--   0 gfvante    (501) staff       (20)       19 2024-03-31 19:29:14.000000 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/requires.txt
--rw-r--r--   0 gfvante    (501) staff       (20)        9 2024-03-31 19:29:14.000000 pytest-xprocess-1.0.1/pytest_xprocess.egg-info/top_level.txt
--rw-r--r--   0 gfvante    (501) staff       (20)     1127 2024-03-31 19:29:14.780978 pytest-xprocess-1.0.1/setup.cfg
--rwxr-xr-x   0 gfvante    (501) staff       (20)      231 2024-03-31 19:28:06.000000 pytest-xprocess-1.0.1/setup.py
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-03-31 19:29:14.766641 pytest-xprocess-1.0.1/tests/
--rw-r--r--   0 gfvante    (501) staff       (20)     6148 2024-03-23 15:03:33.000000 pytest-xprocess-1.0.1/tests/.DS_Store
--rw-r--r--   0 gfvante    (501) staff       (20)    53248 2024-03-23 15:04:10.000000 pytest-xprocess-1.0.1/tests/.coverage
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-03-31 19:29:14.779009 pytest-xprocess-1.0.1/tests/__pycache__/
--rw-r--r--   0 gfvante    (501) staff       (20)     2127 2024-03-20 01:17:29.000000 pytest-xprocess-1.0.1/tests/__pycache__/conftest.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1246 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/conftest.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1240 2024-03-23 15:02:14.000000 pytest-xprocess-1.0.1/tests/__pycache__/conftest.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1254 2022-08-15 09:49:37.000000 pytest-xprocess-1.0.1/tests/__pycache__/conftest.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1248 2024-03-23 15:02:54.000000 pytest-xprocess-1.0.1/tests/__pycache__/conftest.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     5131 2024-03-16 13:52:34.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_callback.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2563 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_callback.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2557 2024-03-16 14:12:49.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_callback.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2591 2022-09-11 13:44:16.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_callback.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2585 2024-03-16 14:13:36.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_callback.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2265 2024-03-16 13:52:34.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_functional_workflow.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1615 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_functional_workflow.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1609 2024-03-16 14:12:49.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_functional_workflow.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1611 2022-08-15 10:35:51.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_functional_workflow.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1605 2024-03-16 14:13:36.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_functional_workflow.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     3023 2024-03-16 13:52:34.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_interruption_clean_up.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2061 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_interruption_clean_up.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2055 2024-03-16 14:12:49.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_interruption_clean_up.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2057 2022-08-15 10:35:51.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_interruption_clean_up.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2051 2024-03-16 14:13:36.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_interruption_clean_up.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      673 2024-03-16 17:23:19.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_parallel.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)    12855 2024-03-23 15:03:32.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_initialization.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     5639 2023-01-05 14:24:18.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_initialization.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     5633 2024-03-23 15:02:14.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_initialization.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     5601 2022-08-15 10:35:51.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_initialization.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     5595 2024-03-23 15:02:54.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_initialization.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)    16639 2024-03-16 13:52:34.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_termination.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     7446 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_termination.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     7440 2024-03-16 14:12:49.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_termination.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     7240 2022-08-15 10:35:51.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_termination.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     7234 2024-03-16 14:13:36.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_process_termination.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      670 2024-03-16 13:52:34.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_resource_cleanup.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      602 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_resource_cleanup.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      596 2024-03-16 14:12:49.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_resource_cleanup.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      598 2022-08-15 10:35:51.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_resource_cleanup.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      592 2024-03-16 14:13:36.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_resource_cleanup.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     2748 2024-03-16 13:52:34.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_startup_timeout.cpython-311-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1578 2022-11-27 16:01:10.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_startup_timeout.cpython-38-pytest-7.2.0.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1572 2024-03-16 14:12:49.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_startup_timeout.cpython-38-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1592 2022-08-29 10:08:08.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_startup_timeout.cpython-39-pytest-7.1.2.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)     1586 2024-03-16 14:13:36.000000 pytest-xprocess-1.0.1/tests/__pycache__/test_startup_timeout.cpython-39-pytest-8.1.1.pyc
--rw-r--r--   0 gfvante    (501) staff       (20)      698 2024-03-19 20:43:38.000000 pytest-xprocess-1.0.1/tests/conftest.py
--rw-r--r--   0 gfvante    (501) staff       (20)     2822 2023-01-05 14:10:05.000000 pytest-xprocess-1.0.1/tests/server.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1620 2022-09-11 13:43:14.000000 pytest-xprocess-1.0.1/tests/test_callback.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1331 2022-08-15 09:38:43.000000 pytest-xprocess-1.0.1/tests/test_functional_workflow.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1841 2022-08-15 09:38:43.000000 pytest-xprocess-1.0.1/tests/test_interruption_clean_up.py
--rw-r--r--   0 gfvante    (501) staff       (20)     5360 2024-03-23 15:07:22.000000 pytest-xprocess-1.0.1/tests/test_process_initialization.py
--rw-r--r--   0 gfvante    (501) staff       (20)     3115 2022-08-15 09:38:43.000000 pytest-xprocess-1.0.1/tests/test_process_termination.py
--rw-r--r--   0 gfvante    (501) staff       (20)      104 2022-08-15 09:33:20.000000 pytest-xprocess-1.0.1/tests/test_resource_cleanup.py
--rw-r--r--   0 gfvante    (501) staff       (20)     1027 2022-08-29 10:05:40.000000 pytest-xprocess-1.0.1/tests/test_startup_timeout.py
--rw-r--r--   0 gfvante    (501) staff       (20)      882 2024-03-19 20:43:38.000000 pytest-xprocess-1.0.1/tox.ini
-drwxr-xr-x   0 gfvante    (501) staff       (20)        0 2024-03-31 19:29:14.779807 pytest-xprocess-1.0.1/xprocess/
--rw-r--r--   0 gfvante    (501) staff       (20)      241 2023-01-04 19:02:09.000000 pytest-xprocess-1.0.1/xprocess/__init__.py
--rw-r--r--   0 gfvante    (501) staff       (20)     3572 2023-09-23 15:09:28.000000 pytest-xprocess-1.0.1/xprocess/pytest_xprocess.py
--rw-r--r--   0 gfvante    (501) staff       (20)    16279 2024-03-23 15:07:22.000000 pytest-xprocess-1.0.1/xprocess/xprocess.py
+drwxrwxr-x   0 gfioravante  (1000) gfioravante  (1000)        0 2024-05-19 16:11:01.739675 pytest-xprocess-1.0.2/
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1054 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/LICENSE
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)       98 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/MANIFEST.in
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1626 2024-05-19 16:11:01.739675 pytest-xprocess-1.0.2/PKG-INFO
+-rwxrwxr-x   0 gfioravante  (1000) gfioravante  (1000)      734 2024-05-19 15:57:24.000000 pytest-xprocess-1.0.2/README.rst
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)      108 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/pyproject.toml
+drwxrwxr-x   0 gfioravante  (1000) gfioravante  (1000)        0 2024-05-19 16:11:01.735675 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1626 2024-05-19 16:11:01.000000 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)      637 2024-05-19 16:11:01.000000 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)        1 2024-05-19 16:11:01.000000 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)       47 2024-05-19 16:11:01.000000 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/entry_points.txt
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)       19 2024-05-19 16:11:01.000000 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/requires.txt
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)        9 2024-05-19 16:11:01.000000 pytest-xprocess-1.0.2/pytest_xprocess.egg-info/top_level.txt
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1182 2024-05-19 16:11:01.739675 pytest-xprocess-1.0.2/setup.cfg
+-rwxrwxr-x   0 gfioravante  (1000) gfioravante  (1000)      206 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/setup.py
+drwxrwxr-x   0 gfioravante  (1000) gfioravante  (1000)        0 2024-05-19 16:11:01.739675 pytest-xprocess-1.0.2/tests/
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)      698 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/conftest.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     2822 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/server.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1620 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_callback.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1331 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_functional_workflow.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1841 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_interruption_clean_up.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     5360 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_process_initialization.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     3115 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_process_termination.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)      104 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_resource_cleanup.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     1027 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tests/test_startup_timeout.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)      882 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/tox.ini
+drwxrwxr-x   0 gfioravante  (1000) gfioravante  (1000)        0 2024-05-19 16:11:01.739675 pytest-xprocess-1.0.2/xprocess/
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)      241 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/xprocess/__init__.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)     3572 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/xprocess/pytest_xprocess.py
+-rw-rw-r--   0 gfioravante  (1000) gfioravante  (1000)    16279 2024-05-19 15:41:14.000000 pytest-xprocess-1.0.2/xprocess/xprocess.py
```

### Comparing `pytest-xprocess-1.0.1/LICENSE` & `pytest-xprocess-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/setup.cfg` & `pytest-xprocess-1.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [metadata]
 name = pytest-xprocess
 author = Holger Krekel
+version = 1.0.2
 author_email = holger@merlinux.eu
 license = MIT
 license_files = LICENSE
 url = https://github.com/pytest-dev/pytest-xprocess/
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 description = A pytest plugin for managing processes across test runs.
 classifiers = 
 	Framework :: Pytest
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
+	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Testing
 	Topic :: Software Development :: Libraries
 	Topic :: Utilities
 
 [options]
 packages = find:
-python_requires = >= 3.9
+python_requires = >= 3.8
 
 [options.packages.find]
 exclude = docs, tests
 
 [options.entry_points]
 pytest11 = 
 	xprocess = xprocess.pytest_xprocess
```

### Comparing `pytest-xprocess-1.0.1/tests/conftest.py` & `pytest-xprocess-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/server.py` & `pytest-xprocess-1.0.2/tests/server.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/test_callback.py` & `pytest-xprocess-1.0.2/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/test_functional_workflow.py` & `pytest-xprocess-1.0.2/tests/test_functional_workflow.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/test_interruption_clean_up.py` & `pytest-xprocess-1.0.2/tests/test_interruption_clean_up.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/test_process_initialization.py` & `pytest-xprocess-1.0.2/tests/test_process_initialization.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/test_process_termination.py` & `pytest-xprocess-1.0.2/tests/test_process_termination.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tests/test_startup_timeout.py` & `pytest-xprocess-1.0.2/tests/test_startup_timeout.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/tox.ini` & `pytest-xprocess-1.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/xprocess/pytest_xprocess.py` & `pytest-xprocess-1.0.2/xprocess/pytest_xprocess.py`

 * *Files identical despite different names*

### Comparing `pytest-xprocess-1.0.1/xprocess/xprocess.py` & `pytest-xprocess-1.0.2/xprocess/xprocess.py`

 * *Files identical despite different names*

