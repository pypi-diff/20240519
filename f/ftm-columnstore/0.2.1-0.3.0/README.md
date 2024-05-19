# Comparing `tmp/ftm_columnstore-0.2.1.tar.gz` & `tmp/ftm_columnstore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftm_columnstore-0.2.1.tar", max compression
+gzip compressed data, was "ftm_columnstore-0.3.0.tar", max compression
```

## Comparing `ftm_columnstore-0.2.1.tar` & `ftm_columnstore-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2022-10-06 10:32:22.190067 ftm_columnstore-0.2.1/LICENSE
--rw-r--r--   0        0        0     1675 2023-10-20 05:57:45.228164 ftm_columnstore-0.2.1/README.md
--rw-r--r--   0        0        0      624 2023-11-14 07:07:22.488995 ftm_columnstore-0.2.1/ftm_columnstore/__init__.py
--rw-r--r--   0        0        0     1985 2023-10-20 05:44:54.544953 ftm_columnstore-0.2.1/ftm_columnstore/cli.py
--rw-r--r--   0        0        0    10556 2023-10-20 05:44:54.544953 ftm_columnstore-0.2.1/ftm_columnstore/engine.py
--rw-r--r--   0        0        0     2271 2023-10-20 05:44:54.544953 ftm_columnstore-0.2.1/ftm_columnstore/phonetic.py
--rw-r--r--   0        0        0      380 2023-11-14 07:07:22.488995 ftm_columnstore-0.2.1/ftm_columnstore/settings.py
--rw-r--r--   0        0        0     2461 2023-10-20 05:44:54.544953 ftm_columnstore-0.2.1/ftm_columnstore/statements.py
--rw-r--r--   0        0        0     2880 2023-10-20 05:44:54.544953 ftm_columnstore-0.2.1/ftm_columnstore/store.py
--rw-r--r--   0        0        0     1579 2023-11-14 07:07:22.488995 ftm_columnstore-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 ftm_columnstore-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-06 10:32:22.190067 ftm_columnstore-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1675 2023-10-20 05:57:45.228164 ftm_columnstore-0.3.0/README.md
+-rw-r--r--   0        0        0      624 2024-05-19 01:38:51.140349 ftm_columnstore-0.3.0/ftm_columnstore/__init__.py
+-rw-r--r--   0        0        0     1985 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/cli.py
+-rw-r--r--   0        0        0    10556 2024-05-19 00:19:38.798693 ftm_columnstore-0.3.0/ftm_columnstore/engine.py
+-rw-r--r--   0        0        0     2271 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/phonetic.py
+-rw-r--r--   0        0        0      380 2024-05-19 01:38:51.140349 ftm_columnstore-0.3.0/ftm_columnstore/settings.py
+-rw-r--r--   0        0        0     2461 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/statements.py
+-rw-r--r--   0        0        0     2880 2023-10-20 05:44:54.544953 ftm_columnstore-0.3.0/ftm_columnstore/store.py
+-rw-r--r--   0        0        0     1592 2024-05-19 01:38:51.140349 ftm_columnstore-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2968 1970-01-01 00:00:00.000000 ftm_columnstore-0.3.0/PKG-INFO
```

### Comparing `ftm_columnstore-0.2.1/LICENSE` & `ftm_columnstore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/README.md` & `ftm_columnstore-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/ftm_columnstore/__init__.py` & `ftm_columnstore-0.3.0/ftm_columnstore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 logging.getLogger("numpy.core.fromnumeric").setLevel(logging.ERROR)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
 
 # FIXME sqlalchemy monkey patch not working
 nomenklatura.settings.DB_URL = "sqlite:///:memory:"
 
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 __all__ = ["get_engine", "get_store"]
```

### Comparing `ftm_columnstore-0.2.1/ftm_columnstore/cli.py` & `ftm_columnstore-0.3.0/ftm_columnstore/cli.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/ftm_columnstore/engine.py` & `ftm_columnstore-0.3.0/ftm_columnstore/engine.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/ftm_columnstore/phonetic.py` & `ftm_columnstore-0.3.0/ftm_columnstore/phonetic.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/ftm_columnstore/statements.py` & `ftm_columnstore-0.3.0/ftm_columnstore/statements.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/ftm_columnstore/store.py` & `ftm_columnstore-0.3.0/ftm_columnstore/store.py`

 * *Files identical despite different names*

### Comparing `ftm_columnstore-0.2.1/pyproject.toml` & `ftm_columnstore-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftm-columnstore"
-version = "0.2.1"
+version = "0.3.0"
 description = "Column store implementation for ftm data based on clickhouse"
 authors = ["Simon Wörpel <simon@investigativedata.org>"]
 license = "GPL3"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftm-columnstore"
 repository = "https://github.com/investigativedata/ftm-columnstore"
 documentation = "https://github.com/investigativedata/ftm-columnstore"
@@ -22,41 +22,41 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/investigativedata/ftm-columnstore/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 banal = "^1.0.6"
-typer = "^0.9.0"
-clickhouse-driver = {extras = ["numpy"], version = "^0.2.6"}
-orjson = "^3.9.10"
-pyicu = "^2.12"
+typer = "^0.12.3"
+clickhouse-driver = {extras = ["numpy"], version = "^0.2.7"}
+pyicu = "^2.13.1"
 libindic-soundex = "^1.0.2"
 libindic-utils = "^1.0.3"
 metaphone = "^0.6"
-pandas = "^2.1.3"
-rich = "^13.6.0"
-ftmq = "^0.5.0"
+pandas = "^2.2.2"
+rich = "^13.7.1"
+ftmq = "^0.6.4"
 
 
 [tool.poetry.group.dev.dependencies]
 absolufy-imports = "^0.3.1"
 ipdb = "^0.13.13"
 black = "^23.11.0"
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 mypy = "^1.7.0"
-pytest = "^7.4.3"
+pytest = "^8.2.0"
 pytest-cov = "^4.1.0"
 pytest-env = ">=1.1.1"
 pre-commit = "^3.5.0"
 bump2version = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 env = [
     "NOMENKLATURA_STATEMENT_TABLE=test_table",
-    "LOG_LEVEL=DEBUG"
+    "LOG_LEVEL=DEBUG",
+    "MAX_SQL_AGG_GROUPS=11"
 ]
```

### Comparing `ftm_columnstore-0.2.1/PKG-INFO` & `ftm_columnstore-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: ftm-columnstore
-Version: 0.2.1
+Version: 0.3.0
 Summary: Column store implementation for ftm data based on clickhouse
 Home-page: https://github.com/investigativedata/ftm-columnstore
 License: GPL3
 Author: Simon Wörpel
 Author-email: simon@investigativedata.org
 Requires-Python: >=3.11,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: banal (>=1.0.6,<2.0.0)
-Requires-Dist: clickhouse-driver[numpy] (>=0.2.6,<0.3.0)
-Requires-Dist: ftmq (>=0.5.0,<0.6.0)
+Requires-Dist: clickhouse-driver[numpy] (>=0.2.7,<0.3.0)
+Requires-Dist: ftmq (>=0.6.4,<0.7.0)
 Requires-Dist: libindic-soundex (>=1.0.2,<2.0.0)
 Requires-Dist: libindic-utils (>=1.0.3,<2.0.0)
 Requires-Dist: metaphone (>=0.6,<0.7)
-Requires-Dist: orjson (>=3.9.10,<4.0.0)
-Requires-Dist: pandas (>=2.1.3,<3.0.0)
-Requires-Dist: pyicu (>=2.12,<3.0)
-Requires-Dist: rich (>=13.6.0,<14.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: pyicu (>=2.13.1,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftm-columnstore/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftm-columnstore
 Project-URL: Repository, https://github.com/investigativedata/ftm-columnstore
 Description-Content-Type: text/markdown
 
 [![ftm-columnstore on pypi](https://img.shields.io/pypi/v/ftm-columnstore)](https://pypi.org/project/ftm-columnstore/) [![Python test and package](https://github.com/investigativedata/ftm-columnstore/actions/workflows/python.yml/badge.svg)](https://github.com/investigativedata/ftm-columnstore/actions/workflows/python.yml) [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit) [![Coverage Status](https://coveralls.io/repos/github/investigativedata/ftm-columnstore/badge.svg?branch=main)](https://coveralls.io/github/investigativedata/ftm-columnstore?branch=main) [![GPL-3.0 License](https://img.shields.io/pypi/l/ftm-columnstore)](./LICENSE)
```

