# Comparing `tmp/that_depends-1.7.0.tar.gz` & `tmp/that_depends-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.7.0.tar", max compression
+gzip compressed data, was "that_depends-1.7.1.tar", max compression
```

## Comparing `that_depends-1.7.0.tar` & `that_depends-1.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.7.0/LICENSE
--rw-r--r--   0        0        0     1710 2024-05-12 20:23:56.338518 that_depends-1.7.0/README.md
--rw-r--r--   0        0        0     1515 2024-05-15 16:11:20.814470 that_depends-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      164 2024-05-09 18:37:39.636094 that_depends-1.7.0/that_depends/__init__.py
--rw-r--r--   0        0        0     1990 2024-05-13 16:35:18.245230 that_depends-1.7.0/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.7.0/that_depends/injection.py
--rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.7.0/that_depends/providers/__init__.py
--rw-r--r--   0        0        0      775 2024-05-13 16:35:18.256594 that_depends-1.7.0/that_depends/providers/base.py
--rw-r--r--   0        0        0      608 2024-05-13 16:35:18.258303 that_depends-1.7.0/that_depends/providers/collections.py
--rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.7.0/that_depends/providers/context_resources.py
--rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.7.0/that_depends/providers/factories.py
--rw-r--r--   0        0        0     4071 2024-05-15 16:03:10.739869 that_depends-1.7.0/that_depends/providers/resources.py
--rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.7.0/that_depends/providers/singleton.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.7.0/that_depends/py.typed
--rw-r--r--   0        0        0     2190 1970-01-01 00:00:00.000000 that_depends-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-30 10:36:32.829777 that_depends-1.7.1/LICENSE
+-rw-r--r--   0        0        0     2610 2024-05-18 07:27:14.545884 that_depends-1.7.1/README.md
+-rw-r--r--   0        0        0     1515 2024-05-19 12:00:00.535185 that_depends-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-19 11:59:39.574505 that_depends-1.7.1/that_depends/__init__.py
+-rw-r--r--   0        0        0     1992 2024-05-19 11:59:39.575220 that_depends-1.7.1/that_depends/container.py
+-rw-r--r--   0        0        0     1068 2024-05-19 11:59:39.575705 that_depends-1.7.1/that_depends/injection.py
+-rw-r--r--   0        0        0      739 2024-05-09 12:44:56.346923 that_depends-1.7.1/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-19 11:59:39.576197 that_depends-1.7.1/that_depends/providers/base.py
+-rw-r--r--   0        0        0      536 2024-05-19 11:59:39.576360 that_depends-1.7.1/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     4255 2024-05-13 16:56:14.984100 that_depends-1.7.1/that_depends/providers/context_resources.py
+-rw-r--r--   0        0        0     1920 2024-05-13 16:35:20.734286 that_depends-1.7.1/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     4069 2024-05-19 11:59:39.576855 that_depends-1.7.1/that_depends/providers/resources.py
+-rw-r--r--   0        0        0     1547 2024-05-13 16:35:20.477615 that_depends-1.7.1/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.7.1/that_depends/py.typed
+-rw-r--r--   0        0        0     3090 1970-01-01 00:00:00.000000 that_depends-1.7.1/PKG-INFO
```

### Comparing `that_depends-1.7.0/LICENSE` & `that_depends-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `that_depends-1.7.0/pyproject.toml` & `that_depends-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.7.0"
+version = "1.7.1"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.7.0/that_depends/container.py` & `that_depends-1.7.1/that_depends/container.py`

 * *Files identical despite different names*

```diff
@@ -41,15 +41,15 @@
     def resolver(cls, item: type[T] | typing.Callable[P, T]) -> typing.Callable[[], typing.Awaitable[T]]:
         async def _inner() -> T:
             return await cls.resolve(item)
 
         return _inner
 
     @classmethod
-    async def resolve(cls, object_to_resolve: type[T] | typing.Callable[P, T]) -> T:
+    async def resolve(cls, object_to_resolve: type[T] | typing.Callable[..., T]) -> T:
         signature = inspect.signature(object_to_resolve)
         kwargs = {}
         providers = cls.get_providers()
         for field_name, field_value in signature.parameters.items():
             if field_value.default is not inspect.Parameter.empty or field_name in ("_", "__"):
                 continue
```

### Comparing `that_depends-1.7.0/that_depends/injection.py` & `that_depends-1.7.1/that_depends/injection.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from that_depends.providers import AbstractProvider
 
 
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 
-def inject(func: typing.Callable[P, typing.Awaitable[T]]) -> typing.Callable[P, typing.Awaitable[T]]:
+def inject(
+    func: typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]],
+) -> typing.Callable[P, typing.Coroutine[typing.Any, typing.Any, T]]:
     signature = inspect.signature(func)
 
     @functools.wraps(func)
     async def inner(*args: P.args, **kwargs: P.kwargs) -> T:
         for field_name, field_value in signature.parameters.items():
             if not isinstance(field_value.default, AbstractProvider):
                 continue
```

### Comparing `that_depends-1.7.0/that_depends/providers/__init__.py` & `that_depends-1.7.1/that_depends/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.7.0/that_depends/providers/base.py` & `that_depends-1.7.1/that_depends/providers/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import abc
 import typing
 
 
 T = typing.TypeVar("T")
+R = typing.TypeVar("R")
+T_co = typing.TypeVar("T_co", covariant=True)
 
 
-class AbstractProvider(typing.Generic[T], abc.ABC):
+class AbstractProvider(typing.Generic[T_co], abc.ABC):
     """Abstract Provider Class."""
 
     @abc.abstractmethod
-    async def async_resolve(self) -> T:
+    async def async_resolve(self) -> T_co:
         """Resolve dependency asynchronously."""
 
     @abc.abstractmethod
-    def sync_resolve(self) -> T:
+    def sync_resolve(self) -> T_co:
         """Resolve dependency synchronously."""
 
-    async def __call__(self) -> T:
+    async def __call__(self) -> T_co:
         return await self.async_resolve()
 
     def override(self, mock: object) -> None:
         self._override = mock
 
     def reset_override(self) -> None:
         self._override = None
```

### Comparing `that_depends-1.7.0/that_depends/providers/collections.py` & `that_depends-1.7.1/that_depends/providers/collections.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from that_depends.providers.base import AbstractProvider
 
 
 T = typing.TypeVar("T")
 
 
-class List(AbstractProvider[T]):
+class List(AbstractProvider[list[T]]):
     def __init__(self, *providers: AbstractProvider[T]) -> None:
         self._providers = providers
 
-    async def async_resolve(self) -> list[T]:  # type: ignore[override]
+    async def async_resolve(self) -> list[T]:
         return [await x.async_resolve() for x in self._providers]
 
-    def sync_resolve(self) -> list[T]:  # type: ignore[override]
+    def sync_resolve(self) -> list[T]:
         return [x.sync_resolve() for x in self._providers]
 
-    async def __call__(self) -> list[T]:  # type: ignore[override]
+    async def __call__(self) -> list[T]:
         return await self.async_resolve()
```

### Comparing `that_depends-1.7.0/that_depends/providers/context_resources.py` & `that_depends-1.7.1/that_depends/providers/context_resources.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.7.0/that_depends/providers/factories.py` & `that_depends-1.7.1/that_depends/providers/factories.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.7.0/that_depends/providers/resources.py` & `that_depends-1.7.1/that_depends/providers/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 T = typing.TypeVar("T")
 P = typing.ParamSpec("P")
 
 
 class Resource(AbstractResource[T]):
     def __init__(
         self,
-        creator: typing.Callable[..., typing.Iterator[T]],
+        creator: typing.Callable[P, typing.Iterator[T]],
         *args: P.args,
         **kwargs: P.kwargs,
     ) -> None:
         if not inspect.isgeneratorfunction(creator):
             msg = "Resource must be generator function"
             raise RuntimeError(msg)
```

### Comparing `that_depends-1.7.0/that_depends/providers/singleton.py` & `that_depends-1.7.1/that_depends/providers/singleton.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.7.0/PKG-INFO` & `that_depends-1.7.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,71 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.7.0
+Version: 1.7.1
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 "That Depends"
 ==
-[![GitHub issues](https://img.shields.io/github/issues/modern-python/that-depends)](https://github.com/modern-python/that-depends/issues)
-[![GitHub forks](https://img.shields.io/github/forks/modern-python/that-depends)](https://github.com/modern-python/that-depends/network)
-[![GitHub stars](https://img.shields.io/github/stars/modern-python/that-depends)](https://github.com/modern-python/that-depends/stargazers)
+[![PyPI version](https://badge.fury.io/py/that-depends.svg)](https://pypi.python.org/pypi/that-depends)
+[![Supported versions](https://img.shields.io/pypi/pyversions/that-depends.svg)](https://pypi.python.org/pypi/that-depends)
 [![GitHub license](https://img.shields.io/github/license/modern-python/that-depends)](https://github.com/modern-python/that-depends/blob/main/LICENSE)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/modern-python/that-depends/python-package.yml)](https://github.com/modern-python/that-depends/actions)
+[![Doc](https://readthedocs.org/projects/that-depends/badge/?version=latest&style=flat)](https://that-depends.readthedocs.io)
+[![GitHub stars](https://img.shields.io/github/stars/modern-python/that-depends)](https://github.com/modern-python/that-depends/stargazers)
 
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
+📚 [Documentation](https://that-depends.readthedocs.io)
+
 It is production-ready and gives you the following:
 - Fully-async simple DI framework with IOC-container.
 - Python 3.10-3.12 support.
 - Full coverage by types annotations (mypy in strict mode).
 - FastAPI and Litestar compatibility.
 - Zero dependencies.
 - Overriding dependencies for tests.
 
-# Main characteristics:
-1. Fully async -> means every dependency resolving is async, so you should construct with `await` keyword:
-```python
-from tests.container import DIContainer
+# Projects with `That Depends`:
+- [fastapi-sqlalchemy-template](https://github.com/modern-python/fastapi-sqlalchemy-template) - FastAPI template with sqlalchemy2 and PostgreSQL
+- [litestar-sqlalchemy-template](https://github.com/modern-python/litestar-sqlalchemy-template) - LiteStar template with sqlalchemy2 and PostgreSQL
 
-async def main():
-    some_dependency = await DIContainer.independent_factory()
+# Main decisions:
+1. By default, dependency resolving is async:
+```python
+some_dependency = await DIContainer.dependent_factory()
 ```
-2. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
+2. Sync resolving is also possible, but will fail in case of async dependencies:
+```python
+sync_resource = DIContainer.sync_resource.sync_resolve()  # this will work
+async_resource = DIContainer.async_resource.sync_resolve()  # this will fail with RuntimeError
 
+# but this will work
+async_resource = await DIContainer.async_resource()
+async_resource = DIContainer.async_resource.sync_resolve()
+```
+3. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
 ```python
 from tests import container
 from that_depends import Provide, inject
 
-
 @inject
 async def some_function(
-        independent_factory: container.SimpleFactory = Provide[container.DIContainer.independent_factory],
+    simple_factory: container.SimpleFactory = Provide[container.DIContainer.simple_factory],
 ) -> None:
-    assert independent_factory.dep1
+    assert simple_factory.dep1
 ```
 
 # Quickstart
 ## Install
-
 ```bash
 pip install that-depends
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

