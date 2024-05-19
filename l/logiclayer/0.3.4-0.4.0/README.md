# Comparing `tmp/logiclayer-0.3.4.tar.gz` & `tmp/logiclayer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer-0.3.4.tar", max compression
+gzip compressed data, was "logiclayer-0.4.0.tar", max compression
```

## Comparing `logiclayer-0.3.4.tar` & `logiclayer-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-05-03 23:00:48.417325 logiclayer-0.3.4/LICENSE
--rw-r--r--   0        0        0     3574 2024-05-03 23:00:48.417325 logiclayer-0.3.4/PACKAGE.md
--rw-r--r--   0        0        0      639 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/__init__.py
--rw-r--r--   0        0        0      894 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/auth.py
--rw-r--r--   0        0        0      623 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/common.py
--rw-r--r--   0        0        0     2689 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/decorators.py
--rw-r--r--   0        0        0     5314 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/logiclayer.py
--rw-r--r--   0        0        0     4154 2024-05-03 23:00:48.417325 logiclayer-0.3.4/logiclayer/module.py
--rw-r--r--   0        0        0      600 2024-05-03 23:00:48.421326 logiclayer-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 logiclayer-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-19 02:52:10.134817 logiclayer-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3574 2024-05-19 02:52:10.134817 logiclayer-0.4.0/PACKAGE.md
+-rw-r--r--   0        0        0      742 2024-05-19 02:52:10.134817 logiclayer-0.4.0/logiclayer/__init__.py
+-rw-r--r--   0        0        0     1411 2024-05-19 02:52:10.134817 logiclayer-0.4.0/logiclayer/auth.py
+-rw-r--r--   0        0        0      845 2024-05-19 02:52:10.134817 logiclayer-0.4.0/logiclayer/common.py
+-rw-r--r--   0        0        0     2689 2024-05-19 02:52:10.134817 logiclayer-0.4.0/logiclayer/decorators.py
+-rw-r--r--   0        0        0     5314 2024-05-19 02:52:10.134817 logiclayer-0.4.0/logiclayer/logiclayer.py
+-rw-r--r--   0        0        0     4154 2024-05-19 02:52:10.134817 logiclayer-0.4.0/logiclayer/module.py
+-rw-r--r--   0        0        0      605 2024-05-19 02:52:10.134817 logiclayer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 logiclayer-0.4.0/PKG-INFO
```

### Comparing `logiclayer-0.3.4/LICENSE` & `logiclayer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.4/PACKAGE.md` & `logiclayer-0.4.0/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.4/logiclayer/__init__.py` & `logiclayer-0.4.0/logiclayer/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """LogicLayer module."""
 
 __title__ = "logiclayer"
 __description__ = (
     "A framework to quickly compose and use multiple functionalities as endpoints."
 )
-__version__ = "0.3.4"
+__version__ = "0.4.0"
 
 __all__ = (
     "AuthProvider",
     "AuthToken",
     "AuthTokenType",
     "exception_handler",
     "healthcheck",
     "LogicLayer",
+    "LogicLayerException",
     "LogicLayerModule",
     "ModuleStatus",
+    "NotAuthorized",
     "on_shutdown",
     "on_startup",
     "route",
 )
 
-from .auth import AuthProvider, AuthToken, AuthTokenType
+from .auth import AuthProvider, AuthToken, AuthTokenType, NotAuthorized
+from .common import LogicLayerException
 from .decorators import exception_handler, healthcheck, on_shutdown, on_startup, route
 from .logiclayer import LogicLayer
 from .module import LogicLayerModule, ModuleStatus
```

### Comparing `logiclayer-0.3.4/logiclayer/common.py` & `logiclayer-0.4.0/logiclayer/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 T = TypeVar("T")
 CallableMayReturnAwaitable = Callable[..., Union[T, Awaitable[T]]]
 CallableMayReturnCoroutine = Callable[..., Union[T, Coroutine[Any, Any, T]]]
 
 LOGICLAYER_METHOD_ATTR = "_llmethod"
 
 
+class LogicLayerException(Exception):
+    """Common base class for exceptions in the LogicLayer package."""
+
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+        self.message = message
+
+
 async def _await_for_it(check: CallableMayReturnAwaitable[Any]) -> Any:
     """Wraps a function, which might be synchronous or asynchronous, into an
     asynchronous function, which returns the value wrapped in a coroutine.
     """
     result = check()
     if inspect.isawaitable(result):
         return await result
```

### Comparing `logiclayer-0.3.4/logiclayer/decorators.py` & `logiclayer-0.4.0/logiclayer/decorators.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.4/logiclayer/logiclayer.py` & `logiclayer-0.4.0/logiclayer/logiclayer.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.4/logiclayer/module.py` & `logiclayer-0.4.0/logiclayer/module.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.4/pyproject.toml` & `logiclayer-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "logiclayer"
-version = "0.3.4"
+version = "0.4.0"
 description = "A framework to quickly compose and use multiple functionalities as endpoints."
 authors = ["Francisco Abarzua <francisco@datawheel.us>"]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/logiclayer"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio = "^3.4.0"
-fastapi = ">=0.100 <1.0"
+fastapi-slim = ">=0.111 <1.0"
 pydantic = "^2.5.0"
 
 [tool.poetry.group.dev.dependencies]
-httpx = ">=0.20.0"
+httpx = ">=0.27.0"
 pytest = "~8.1.0"
 ruff = "^0.4.0"
 uvicorn = "^0.29.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `logiclayer-0.3.4/PKG-INFO` & `logiclayer-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: logiclayer
-Version: 0.3.4
+Version: 0.4.0
 Summary: A framework to quickly compose and use multiple functionalities as endpoints.
 Home-page: https://github.com/Datawheel/logiclayer
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncio (>=3.4.0,<4.0.0)
-Requires-Dist: fastapi (>=0.100,<1.0)
+Requires-Dist: fastapi-slim (>=0.111,<1.0)
 Requires-Dist: pydantic (>=2.5.0,<3.0.0)
 Project-URL: Repository, https://github.com/Datawheel/logiclayer
 Description-Content-Type: text/markdown
 
 A simple framework to quickly compose and use multiple functionalities as endpoints.  
 LogicLayer is built upon FastAPI to provide a simple way to group functionalities into reusable modules.
```

