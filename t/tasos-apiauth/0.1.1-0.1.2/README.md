# Comparing `tmp/tasos_apiauth-0.1.1.tar.gz` & `tmp/tasos_apiauth-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tasos_apiauth-0.1.1.tar", max compression
+gzip compressed data, was "tasos_apiauth-0.1.2.tar", max compression
```

## Comparing `tasos_apiauth-0.1.1.tar` & `tasos_apiauth-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1094 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/LICENSE
--rw-r--r--   0        0        0     8508 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/README.md
--rw-r--r--   0        0        0     2837 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       64 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/__init__.py
--rw-r--r--   0        0        0      899 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/api/__init__.py
--rw-r--r--   0        0        0     4891 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/api/base.py
--rw-r--r--   0        0        0     6525 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/api/group.py
--rw-r--r--   0        0        0     3213 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/api/permission.py
--rw-r--r--   0        0        0     4921 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/api/user.py
--rw-r--r--   0        0        0     5211 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/auth.py
--rw-r--r--   0        0        0    13903 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/cli.py
--rw-r--r--   0        0        0     1365 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/config.py
--rw-r--r--   0        0        0     1797 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/db.py
--rw-r--r--   0        0        0     7994 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/helpers.py
--rw-r--r--   0        0        0     6022 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/apiauth/model.py
--rw-r--r--   0        0        0        0 2024-03-17 19:08:09.466018 tasos_apiauth-0.1.1/tasos/py.typed
--rw-r--r--   0        0        0     9134 1970-01-01 00:00:00.000000 tasos_apiauth-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8508 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/README.md
+-rw-r--r--   0        0        0     2885 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/__init__.py
+-rw-r--r--   0        0        0      899 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/api/__init__.py
+-rw-r--r--   0        0        0     4891 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/api/base.py
+-rw-r--r--   0        0        0     6525 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/api/group.py
+-rw-r--r--   0        0        0     3213 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/api/permission.py
+-rw-r--r--   0        0        0     4921 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/api/user.py
+-rw-r--r--   0        0        0     5211 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/auth.py
+-rw-r--r--   0        0        0    13903 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/cli.py
+-rw-r--r--   0        0        0     1365 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/config.py
+-rw-r--r--   0        0        0     1797 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/db.py
+-rw-r--r--   0        0        0     7994 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/helpers.py
+-rw-r--r--   0        0        0     6022 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/apiauth/model.py
+-rw-r--r--   0        0        0        0 2024-05-19 18:05:48.900333 tasos_apiauth-0.1.2/tasos/py.typed
+-rw-r--r--   0        0        0     9134 1970-01-01 00:00:00.000000 tasos_apiauth-0.1.2/PKG-INFO
```

### Comparing `tasos_apiauth-0.1.1/LICENSE` & `tasos_apiauth-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/README.md` & `tasos_apiauth-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/pyproject.toml` & `tasos_apiauth-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tasos-apiauth"
-version = "0.1.1"
+version = "0.1.2"
 description = "A re-usable FastAPI library that implements authentication, users, groups and permission handling."
 authors = ["tristeng <tristen.georgiou@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [
     {include = "tasos"}
 ]
@@ -13,36 +13,36 @@
 Homepage = "https://github.com/tristeng/tasos-apiauth"
 Repository = "https://github.com/tristeng/tasos-apiauth.git"
 Issues = "https://github.com/tristeng/tasos-apiauth/issues"
 Changelog = "https://github.com/tristeng/tasos-apiauth/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-fastapi = "^0.110.0"
-python-multipart = "0.0.7"
+fastapi = "^0.111.0"
+python-multipart = "0.0.9"
 python-jose = {extras = ["cryptography"], version = "^3.3.0"}
 passlib = {extras = ["bcrypt"], version = "^1.7.4"}
-sqlalchemy = {extras = ["asyncio"], version = "^2.0.25"}
-pydantic = {extras = ["email", "dotenv"], version = "^2.6.0"}
-pydantic-settings = "^2.1.0"
+sqlalchemy = {extras = ["asyncio"], version = "^2.0.30"}
+pydantic = {extras = ["email", "dotenv"], version = "^2.7.1"}
+pydantic-settings = "^2.2.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.4"
-pytest-cov = "^4.1.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
 pytest-env = "^1.1.3"
-pytest-asyncio = "^0.23.4"
-httpx = "^0.26.0"
-aiosqlite = "^0.19.0"
-mypy = "^1.8.0"
-sqlalchemy = {extras = ["mypy"], version = "^2.0.25"}
+pytest-asyncio = "^0.23.7"
+httpx = "^0.27.0"
+aiosqlite = "^0.20.0"
+mypy = "^1.10.0"
+sqlalchemy = {extras = ["mypy"], version = "^2.0.30"}
 flake8 = "^7.0.0"
 types-python-jose = "^3.3.4.20240106"
-types-passlib = "^1.7.7.20240106"
-black = "^24.1.1"
-uvicorn = "^0.27.0"
+types-passlib = "^1.7.7.20240327"
+black = "^24.4.2"
+uvicorn = "^0.29.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -96,15 +96,15 @@
 check_untyped_defs = true
 no_implicit_reexport = true
 
 # for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
-module = "httpx.*"
-ignore_missing_imports = true
+module = "tests.apiauth.api.*"  # NOTE: httpx release > 0.27 will fix this
+ignore_errors = true
 
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
```

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/api/__init__.py` & `tasos_apiauth-0.1.2/tasos/apiauth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/api/base.py` & `tasos_apiauth-0.1.2/tasos/apiauth/api/base.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/api/group.py` & `tasos_apiauth-0.1.2/tasos/apiauth/api/group.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/api/permission.py` & `tasos_apiauth-0.1.2/tasos/apiauth/api/permission.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/api/user.py` & `tasos_apiauth-0.1.2/tasos/apiauth/api/user.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/auth.py` & `tasos_apiauth-0.1.2/tasos/apiauth/auth.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/cli.py` & `tasos_apiauth-0.1.2/tasos/apiauth/cli.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/config.py` & `tasos_apiauth-0.1.2/tasos/apiauth/config.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/db.py` & `tasos_apiauth-0.1.2/tasos/apiauth/db.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/helpers.py` & `tasos_apiauth-0.1.2/tasos/apiauth/helpers.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/tasos/apiauth/model.py` & `tasos_apiauth-0.1.2/tasos/apiauth/model.py`

 * *Files identical despite different names*

### Comparing `tasos_apiauth-0.1.1/PKG-INFO` & `tasos_apiauth-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tasos-apiauth
-Version: 0.1.1
+Version: 0.1.2
 Summary: A re-usable FastAPI library that implements authentication, users, groups and permission handling.
 License: MIT
 Author: tristeng
 Author-email: tristen.georgiou@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fastapi (>=0.110.0,<0.111.0)
+Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: passlib[bcrypt] (>=1.7.4,<2.0.0)
-Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
-Requires-Dist: pydantic[dotenv,email] (>=2.6.0,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: pydantic[dotenv,email] (>=2.7.1,<3.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
-Requires-Dist: python-multipart (==0.0.7)
-Requires-Dist: sqlalchemy[asyncio] (>=2.0.25,<3.0.0)
+Requires-Dist: python-multipart (==0.0.9)
+Requires-Dist: sqlalchemy[asyncio] (>=2.0.30,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Tasos API Authentication Library
 ![python package](https://github.com/tristeng/tasos-apiauth/actions/workflows/python-package.yml/badge.svg)  
 
 A re-usable library that implements authentication, users, groups and permission handling for FastAPI. This library
 is meant to allow a FastAPI developer to get up and running quickly with functions to register, authenticate and manage
```

