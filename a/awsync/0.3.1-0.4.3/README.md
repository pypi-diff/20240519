# Comparing `tmp/awsync-0.3.1.tar.gz` & `tmp/awsync-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsync-0.3.1.tar", max compression
+gzip compressed data, was "awsync-0.4.3.tar", max compression
```

## Comparing `awsync-0.3.1.tar` & `awsync-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-01 04:32:50.769212 awsync-0.3.1/LICENSE
--rw-r--r--   0        0        0     2082 2024-05-14 01:49:11.328354 awsync-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.855130 awsync-0.3.1/awsync/__init__.py
--rw-r--r--   0        0        0      592 2024-05-14 21:30:49.438223 awsync-0.3.1/awsync/__main__.py
--rw-r--r--   0        0        0     6960 2024-05-14 21:12:15.693164 awsync-0.3.1/awsync/client.py
--rw-r--r--   0        0        0        0 2024-05-01 04:07:11.852130 awsync-0.3.1/awsync/models/__init__.py
--rw-r--r--   0        0        0     3062 2024-05-10 03:09:12.698260 awsync-0.3.1/awsync/models/aws.py
--rw-r--r--   0        0        0     1433 2024-05-01 19:56:43.825054 awsync-0.3.1/awsync/models/http.py
--rw-r--r--   0        0        0      282 2024-05-10 04:58:06.020609 awsync-0.3.1/awsync/models/strenum.py
--rw-r--r--   0        0        0        0 2024-05-01 20:49:43.288001 awsync-0.3.1/awsync/py.typed
--rw-r--r--   0        0        0    10212 2024-05-14 21:30:36.245222 awsync-0.3.1/awsync/request.py
--rw-r--r--   0        0        0     1376 2024-05-14 21:32:37.363229 awsync-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 awsync-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-19 03:38:51.872069 awsync-0.4.3/LICENSE
+-rw-r--r--   0        0        0     1841 2024-05-19 03:38:51.872069 awsync-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/__main__.py
+-rw-r--r--   0        0        0     6960 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/client.py
+-rw-r--r--   0        0        0        0 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/models/__init__.py
+-rw-r--r--   0        0        0     3062 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/models/aws.py
+-rw-r--r--   0        0        0     1433 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/models/http.py
+-rw-r--r--   0        0        0      282 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/models/strenum.py
+-rw-r--r--   0        0        0        0 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/py.typed
+-rw-r--r--   0        0        0    10212 2024-05-19 03:38:51.872069 awsync-0.4.3/awsync/request.py
+-rw-r--r--   0        0        0     1672 2024-05-19 03:38:51.876068 awsync-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 awsync-0.4.3/PKG-INFO
```

### Comparing `awsync-0.3.1/LICENSE` & `awsync-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `awsync-0.3.1/README.md` & `awsync-0.4.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # awsync
 
 ![CICD](https://github.com/JKCT/awsync/actions/workflows/cicd.yaml/badge.svg)
 
 An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 
+Read [the documentation](https://jkct.github.io/awsync/).
+
 **NOTE: Currently a work in progress!**
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
 "Module main."
@@ -36,37 +38,27 @@
     run(main())
 ```
 
 ## Local Developer Setup
 
 Requirements:
 
-- [make](https://www.gnu.org/software/make/)
-- [python3](https://www.python.org/)
+- [mise](https://mise.jdx.dev/)
+- [python](https://www.python.org/) 3.8 or greater
 - [poetry](https://python-poetry.org/)
 
+### Repository Mangement
+
+This repository uses [mise](https://mise.jdx.dev/) for tool and task management.
+
+List all available commands with `mise tasks`.
+
 ### Package Management
 
-- `make init` install/update dependencies, alias for `poetry install --sync`.
-- `poetry add` add a dependency ie. `poetry add pydantic`.
+This repository uses [poetry](https://python-poetry.org/) for python package management.
+
+- `poetry install --sync` install/update dependencies, aliased to `mise run init`.
+- `poetry add` add a dependency ie. `poetry add black`.
 - `poetry add -D` add a development dependency ie. `poetry add -D black`.
-- `poetry remove` remove a dependency ie. `poetry remove pydantic`.
-- `poetry shell` activate the python virtual environment.
+- `poetry remove` remove a dependency ie. `poetry remove black`.
+- `poetry shell` activate the python virtual environment for access to installed packages.
 - `exit` exit the python virtual environment.
-
-### Repository Mangement
-
-- `make run` runs the main module.
-- `make pr` runs all pull request pre-checks below.
-- `make format` runs code formatter.
-- `make lint` checks code linting.
-- `make test` runs tests.
-
-## Repository TODO:
-
-- Code generation [from JSON](https://github.com/boto/botocore/tree/develop/botocore/data)
-- Automatic Publish CICD
-- Documentation with [mkDocs](https://squidfunk.github.io/mkdocs-material/)
-- Test Makefile replacements
-  - [mise](https://mise.jdx.dev/)
-  - [Poetry run](https://python-poetry.org/docs/cli/#run)
-  - [doit](https://pydoit.org/)
```

### Comparing `awsync-0.3.1/awsync/__main__.py` & `awsync-0.4.3/awsync/__main__.py`

 * *Files identical despite different names*

### Comparing `awsync-0.3.1/awsync/client.py` & `awsync-0.4.3/awsync/client.py`

 * *Files identical despite different names*

### Comparing `awsync-0.3.1/awsync/models/aws.py` & `awsync-0.4.3/awsync/models/aws.py`

 * *Files identical despite different names*

### Comparing `awsync-0.3.1/awsync/models/http.py` & `awsync-0.4.3/awsync/models/http.py`

 * *Files identical despite different names*

### Comparing `awsync-0.3.1/awsync/request.py` & `awsync-0.4.3/awsync/request.py`

 * *Files identical despite different names*

### Comparing `awsync-0.3.1/pyproject.toml` & `awsync-0.4.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 [tool.poetry]
 name = "awsync"
-version = "0.3.1"
+version = "0.4.3"
 description = "An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable."
 license = "Apache-2.0"
 authors = ["JKCT <jkct@visceralfx.com>"]
 readme = "README.md"
 packages = [{include = "awsync"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
 ]
 keywords = ["aws", "async", "boto", "request", "sdk", "typed"]
 repository = "https://github.com/JKCT/awsync"
-include = ["py.typed"]
+documentation = "https://jkct.github.io/awsync/"
+include = ["py.typed"] # Typed marker file to indicate package type support
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.0"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-asyncio = "^0.23.6"
+mkdocs-material = "^9.5.23"
 
 [tool.mypy]
 strict = true
 color_output = true
 cache_dir = "/tmp/cache/.mypy_cache"
 
 [tool.coverage.run]
-omit = ["__main__.py"]
+omit = ["__main__.py"] # Exclude files from test coverage
 
 [tool.coverage.report]
-exclude_also = [
+exclude_also = [ # Exclude code branches by pattern from test coverage
     "async def list_stack_resources",
     "async def get_resource",
     "async def invoke",
     ]
 
 [tool.pytest.ini_options]
 testpaths = "tests"
 cache_dir = "/tmp/cache/.pytest_cache"
+# Require 100% coverage, use exclusions above instead of decreasing percent.
 addopts = "-vv --cov=awsync --cov-report term-missing:skip-covered --cov-fail-under=100"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `awsync-0.3.1/PKG-INFO` & `awsync-0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsync
-Version: 0.3.1
+Version: 0.4.3
 Summary: An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 Home-page: https://github.com/JKCT/awsync
 License: Apache-2.0
 Keywords: aws,async,boto,request,sdk,typed
 Author: JKCT
 Author-email: jkct@visceralfx.com
 Requires-Python: >=3.8,<4.0
@@ -15,23 +15,26 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Project-URL: Documentation, https://jkct.github.io/awsync/
 Project-URL: Repository, https://github.com/JKCT/awsync
 Description-Content-Type: text/markdown
 
 # awsync
 
 ![CICD](https://github.com/JKCT/awsync/actions/workflows/cicd.yaml/badge.svg)
 
 An asynchronous, fully-typed AWS API library with a focus on being understandable, reliable, and maintainable.
 
+Read [the documentation](https://jkct.github.io/awsync/).
+
 **NOTE: Currently a work in progress!**
 Only a few API methods currently implemented for testing and development.
 
 ## Usage
 
 ```python
 "Module main."
@@ -60,38 +63,28 @@
     run(main())
 ```
 
 ## Local Developer Setup
 
 Requirements:
 
-- [make](https://www.gnu.org/software/make/)
-- [python3](https://www.python.org/)
+- [mise](https://mise.jdx.dev/)
+- [python](https://www.python.org/) 3.8 or greater
 - [poetry](https://python-poetry.org/)
 
+### Repository Mangement
+
+This repository uses [mise](https://mise.jdx.dev/) for tool and task management.
+
+List all available commands with `mise tasks`.
+
 ### Package Management
 
-- `make init` install/update dependencies, alias for `poetry install --sync`.
-- `poetry add` add a dependency ie. `poetry add pydantic`.
+This repository uses [poetry](https://python-poetry.org/) for python package management.
+
+- `poetry install --sync` install/update dependencies, aliased to `mise run init`.
+- `poetry add` add a dependency ie. `poetry add black`.
 - `poetry add -D` add a development dependency ie. `poetry add -D black`.
-- `poetry remove` remove a dependency ie. `poetry remove pydantic`.
-- `poetry shell` activate the python virtual environment.
+- `poetry remove` remove a dependency ie. `poetry remove black`.
+- `poetry shell` activate the python virtual environment for access to installed packages.
 - `exit` exit the python virtual environment.
 
-### Repository Mangement
-
-- `make run` runs the main module.
-- `make pr` runs all pull request pre-checks below.
-- `make format` runs code formatter.
-- `make lint` checks code linting.
-- `make test` runs tests.
-
-## Repository TODO:
-
-- Code generation [from JSON](https://github.com/boto/botocore/tree/develop/botocore/data)
-- Automatic Publish CICD
-- Documentation with [mkDocs](https://squidfunk.github.io/mkdocs-material/)
-- Test Makefile replacements
-  - [mise](https://mise.jdx.dev/)
-  - [Poetry run](https://python-poetry.org/docs/cli/#run)
-  - [doit](https://pydoit.org/)
-
```

