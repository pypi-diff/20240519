# Comparing `tmp/quart_rate_limiter-0.8.0.tar.gz` & `tmp/quart_rate_limiter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quart_rate_limiter-0.8.0.tar", max compression
+gzip compressed data, was "quart_rate_limiter-0.9.0.tar", max compression
```

## Comparing `quart_rate_limiter-0.8.0.tar` & `quart_rate_limiter-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1050 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/LICENSE
--rw-r--r--   0        0        0     4727 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/README.rst
--rw-r--r--   0        0        0     2195 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    11529 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/src/quart_rate_limiter/__init__.py
--rw-r--r--   0        0        0        7 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/src/quart_rate_limiter/py.typed
--rw-r--r--   0        0        0     1186 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/src/quart_rate_limiter/redis_store.py
--rw-r--r--   0        0        0     1573 2023-01-21 15:31:31.427998 quart_rate_limiter-0.8.0/src/quart_rate_limiter/store.py
--rw-r--r--   0        0        0     5754 1970-01-01 00:00:00.000000 quart_rate_limiter-0.8.0/setup.py
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 quart_rate_limiter-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4727 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/README.rst
+-rw-r--r--   0        0        0     2196 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11550 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/src/quart_rate_limiter/__init__.py
+-rw-r--r--   0        0        0        7 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/src/quart_rate_limiter/py.typed
+-rw-r--r--   0        0        0     1186 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/src/quart_rate_limiter/redis_store.py
+-rw-r--r--   0        0        0     1573 2023-10-07 16:56:14.291530 quart_rate_limiter-0.9.0/src/quart_rate_limiter/store.py
+-rw-r--r--   0        0        0     5928 1970-01-01 00:00:00.000000 quart_rate_limiter-0.9.0/PKG-INFO
```

### Comparing `quart_rate_limiter-0.8.0/LICENSE` & `quart_rate_limiter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quart_rate_limiter-0.8.0/README.rst` & `quart_rate_limiter-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `quart_rate_limiter-0.8.0/pyproject.toml` & `quart_rate_limiter-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "quart-rate-limiter"
-version = "0.8.0"
+version = "0.9.0"
 description = "A Quart extension to provide rate limiting support"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["src/quart_rate_limiter/py.typed"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/pgjones/quart-rate-limiter/"
 
 [tool.black]
 line-length = 100
-target-version = ["py37"]
+target-version = ["py38"]
 
 [tool.isort]
 combine_as_imports = true
 force_grid_wrap = 0
 include_trailing_comma = true
 known_first_party = "quart_rate_limiter, tests"
 line_length = 100
@@ -57,16 +57,16 @@
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module =["redis.*"]
 ignore_missing_imports = true
 
 [tool.poetry.dependencies]
-python = ">=3.7"
-quart = ">=0.15"
+python = ">=3.8"
+quart = ">=0.19"
 redis = { version = ">=4.4.0", optional = true }
 
 [tool.poetry.dev-dependencies]
 tox = "*"
 
 [tool.poetry.extras]
 redis = ["redis"]
```

### Comparing `quart_rate_limiter-0.8.0/src/quart_rate_limiter/__init__.py` & `quart_rate_limiter-0.9.0/src/quart_rate_limiter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, TypeVar, Union
 
-from quart import Blueprint, current_app, Quart, request, Response
+from flask.sansio.blueprints import Blueprint
+from quart import current_app, Quart, request, Response
 from quart.typing import RouteCallable, WebsocketCallable
 from werkzeug.exceptions import TooManyRequests
 
 from .store import MemoryStore, RateLimiterStoreABC
 
 QUART_RATE_LIMITER_LIMITS_ATTRIBUTE = "_quart_rate_limiter_limits"
 QUART_RATE_LIMITER_EXEMPT_ATTRIBUTE = "_quart_rate_limiter_exempt"
@@ -99,15 +100,15 @@
         rate_limits.extend(limits)
         setattr(func, QUART_RATE_LIMITER_LIMITS_ATTRIBUTE, rate_limits)
         return func
 
     return decorator
 
 
-def rate_exempt(func: Callable) -> Callable:
+def rate_exempt(func: T) -> T:
     """A decorator to mark the route as exempt from rate limits.
 
     This should be used to wrap a route handler (or view function) to
     ensure no rate limits are applied to the route. Note that it is
     important that this decorator be wrapped by the route decorator
     and not vice, versa, as below.
```

### Comparing `quart_rate_limiter-0.8.0/src/quart_rate_limiter/redis_store.py` & `quart_rate_limiter-0.9.0/src/quart_rate_limiter/redis_store.py`

 * *Files identical despite different names*

### Comparing `quart_rate_limiter-0.8.0/src/quart_rate_limiter/store.py` & `quart_rate_limiter-0.9.0/src/quart_rate_limiter/store.py`

 * *Files identical despite different names*

### Comparing `quart_rate_limiter-0.8.0/PKG-INFO` & `quart_rate_limiter-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 Metadata-Version: 2.1
 Name: quart-rate-limiter
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Quart extension to provide rate limiting support
 Home-page: https://github.com/pgjones/quart-rate-limiter/
 License: MIT
 Author: pgjones
 Author-email: philip.graham.jones@googlemail.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: redis
-Requires-Dist: quart (>=0.15)
+Requires-Dist: quart (>=0.19)
 Requires-Dist: redis (>=4.4.0) ; extra == "redis"
 Project-URL: Repository, https://github.com/pgjones/quart-rate-limiter/
 Description-Content-Type: text/x-rst
 
 Quart-Rate-Limiter
 ==================
```

