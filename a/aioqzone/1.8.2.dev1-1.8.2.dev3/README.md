# Comparing `tmp/aioqzone-1.8.2.dev1.tar.gz` & `tmp/aioqzone-1.8.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqzone-1.8.2.dev1.tar", max compression
+gzip compressed data, was "aioqzone-1.8.2.dev3.tar", max compression
```

## Comparing `aioqzone-1.8.2.dev1.tar` & `aioqzone-1.8.2.dev3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    34523 2024-01-21 01:31:17.718241 aioqzone-1.8.2.dev1/LICENSE
--rw-r--r--   0        0        0     3058 2024-01-21 01:31:17.718241 aioqzone-1.8.2.dev1/README.md
--rw-r--r--   0        0        0     2303 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/__init__.py
--rw-r--r--   0        0        0      175 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/api/__init__.py
--rw-r--r--   0        0        0       56 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/api/h5/__init__.py
--rw-r--r--   0        0        0     8707 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/api/h5/model.py
--rw-r--r--   0        0        0     6334 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/api/login/__init__.py
--rw-r--r--   0        0        0     2597 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/api/login/_base.py
--rw-r--r--   0        0        0      639 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/exception.py
--rw-r--r--   0        0        0      551 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/message.py
--rw-r--r--   0        0        0      164 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/__init__.py
--rw-r--r--   0        0        0     4423 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/api/__init__.py
--rw-r--r--   0        0        0     5696 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/api/feed.py
--rw-r--r--   0        0        0     2673 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/api/profile.py
--rw-r--r--   0        0        0     5864 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/api/request.py
--rw-r--r--   0        0        0     7895 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/api/response.py
--rw-r--r--   0        0        0     1438 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/protocol/__init__.py
--rw-r--r--   0        0        0      631 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/protocol/config.py
--rw-r--r--   0        0        0     1618 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/model/protocol/entity.py
--rw-r--r--   0        0        0       39 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/utils/__init__.py
--rw-r--r--   0        0        0     2654 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/utils/entity.py
--rw-r--r--   0        0        0      591 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/utils/regex.py
--rw-r--r--   0        0        0      948 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/utils/retry.py
--rw-r--r--   0        0        0     2769 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/aioqzone/utils/time.py
--rw-r--r--   0        0        0      146 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/__init__.py
--rw-r--r--   0        0        0     4577 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/base.py
--rw-r--r--   0        0        0     1440 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/constant.py
--rw-r--r--   0        0        0     1361 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/exception.py
--rw-r--r--   0        0        0     1667 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/message.py
--rw-r--r--   0        0        0        8 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/py.typed
--rw-r--r--   0        0        0     7467 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/qr/__init__.py
--rw-r--r--   0        0        0      591 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/qr/type.py
--rw-r--r--   0        0        0      611 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/type.py
--rw-r--r--   0        0        0       93 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/__init__.py
--rw-r--r--   0        0        0      892 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/_model.py
--rw-r--r--   0        0        0     6128 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/__init__.py
--rw-r--r--   0        0        0     1649 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/_model.py
--rw-r--r--   0        0        0     3326 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/capsess.py
--rw-r--r--   0        0        0      288 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/pil_utils.py
--rw-r--r--   0        0        0       77 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/select/__init__.py
--rw-r--r--   0        0        0     2935 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/select/_types.py
--rw-r--r--   0        0        0       75 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/slide/__init__.py
--rw-r--r--   0        0        0     5232 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/captcha/slide/_types.py
--rw-r--r--   0        0        0     5249 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/encrypt.py
--rw-r--r--   0        0        0     2489 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/h5.py
--rw-r--r--   0        0        0    10288 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/up/web.py
--rw-r--r--   0        0        0      204 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/utils/encrypt.py
--rw-r--r--   0        0        0      728 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/utils/iter.py
--rw-r--r--   0        0        0     1964 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/utils/jsjson.py
--rw-r--r--   0        0        0     1497 2024-01-21 01:31:17.722241 aioqzone-1.8.2.dev1/src/qqqr/utils/net.py
--rw-r--r--   0        0        0     4695 1970-01-01 00:00:00.000000 aioqzone-1.8.2.dev1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-19 05:55:11.669037 aioqzone-1.8.2.dev3/LICENSE
+-rw-r--r--   0        0        0     3057 2024-05-19 05:55:11.669037 aioqzone-1.8.2.dev3/README.md
+-rw-r--r--   0        0        0     2311 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/__init__.py
+-rw-r--r--   0        0        0      175 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/h5/__init__.py
+-rw-r--r--   0        0        0     8707 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/h5/model.py
+-rw-r--r--   0        0        0     6334 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/login/__init__.py
+-rw-r--r--   0        0        0     2597 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/api/login/_base.py
+-rw-r--r--   0        0        0      639 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/exception.py
+-rw-r--r--   0        0        0      551 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/message.py
+-rw-r--r--   0        0        0      164 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/__init__.py
+-rw-r--r--   0        0        0     4475 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/__init__.py
+-rw-r--r--   0        0        0     5696 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/feed.py
+-rw-r--r--   0        0        0     2674 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/profile.py
+-rw-r--r--   0        0        0     5864 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/request.py
+-rw-r--r--   0        0        0     7895 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/api/response.py
+-rw-r--r--   0        0        0     1439 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/config.py
+-rw-r--r--   0        0        0     1618 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/entity.py
+-rw-r--r--   0        0        0       39 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/__init__.py
+-rw-r--r--   0        0        0     2654 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/entity.py
+-rw-r--r--   0        0        0      592 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/regex.py
+-rw-r--r--   0        0        0      940 2024-05-19 05:55:11.673037 aioqzone-1.8.2.dev3/src/aioqzone/utils/retry.py
+-rw-r--r--   0        0        0     2769 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/aioqzone/utils/time.py
+-rw-r--r--   0        0        0      146 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/__init__.py
+-rw-r--r--   0        0        0     4577 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/base.py
+-rw-r--r--   0        0        0     1440 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/constant.py
+-rw-r--r--   0        0        0     1361 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/exception.py
+-rw-r--r--   0        0        0     1667 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/message.py
+-rw-r--r--   0        0        0        8 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/py.typed
+-rw-r--r--   0        0        0     7513 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/qr/__init__.py
+-rw-r--r--   0        0        0      591 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/qr/type.py
+-rw-r--r--   0        0        0      611 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/type.py
+-rw-r--r--   0        0        0       93 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/_model.py
+-rw-r--r--   0        0        0     6128 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/__init__.py
+-rw-r--r--   0        0        0     1649 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/_model.py
+-rw-r--r--   0        0        0     3318 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/capsess.py
+-rw-r--r--   0        0        0      288 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/pil_utils.py
+-rw-r--r--   0        0        0       77 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/select/__init__.py
+-rw-r--r--   0        0        0     2935 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/select/_types.py
+-rw-r--r--   0        0        0       75 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/slide/__init__.py
+-rw-r--r--   0        0        0     5232 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/captcha/slide/_types.py
+-rw-r--r--   0        0        0     5249 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/encrypt.py
+-rw-r--r--   0        0        0     2489 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/h5.py
+-rw-r--r--   0        0        0    10320 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/up/web.py
+-rw-r--r--   0        0        0      204 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/encrypt.py
+-rw-r--r--   0        0        0      726 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/iter.py
+-rw-r--r--   0        0        0     2062 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/jsjson.py
+-rw-r--r--   0        0        0     1511 2024-05-19 05:55:11.677037 aioqzone-1.8.2.dev3/src/qqqr/utils/net.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 aioqzone-1.8.2.dev3/PKG-INFO
```

### Comparing `aioqzone-1.8.2.dev1/LICENSE` & `aioqzone-1.8.2.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/README.md` & `aioqzone-1.8.2.dev3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # aioqzone
 
 aioqzone封装了一些Qzone接口。
 
 [![python](https://img.shields.io/pypi/pyversions/aioqzone?logo=python&logoColor=white)][home]
 [![version](https://img.shields.io/pypi/v/aioqzone?logo=python)][pypi]
 [![style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![discuss](https://img.shields.io/badge/dynamic/xml?style=social&logo=telegram&label=Discuss&query=%2F%2Fdiv%5B%40class%3D%22tgme_page_extra%22%5D&url=https%3A%2F%2Ft.me%2Faioqzone_chatroom)](https://t.me/aioqzone_chatrooom)
+[![discuss](https://img.shields.io/badge/dynamic/xml?style=social&logo=telegram&label=Discuss&query=%2F%2Fdiv%5B%40class%3D%22tgme_page_extra%22%5D&url=https%3A%2F%2Ft.me%2Faioqzone_chatroom)](https://t.me/aioqzone_chatroom)
 
 [English](README_en.md) | 简体中文
 
 > [!WARNING]
 > aioqzone 仍在开发阶段，任何功能和接口都有可能在未来的版本中发生变化。
 
 > [!IMPORTANT]
```

### Comparing `aioqzone-1.8.2.dev1/pyproject.toml` & `aioqzone-1.8.2.dev3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioqzone"
-version = "1.8.2.dev1"
+version = "1.8.2.dev3"
 description = "A Python wrapper for Qzone login and H5 APIs."
 authors = ["aioqzone <zzzzss990315@gmail.com>"]
 license = "AGPL-3.0"
 readme = "README.md"
 homepage = "https://github.com/aioqzone/aioqzone"
 repository = "https://github.com/aioqzone/aioqzone"
 documentation = "https://aioqzone.github.io/aioqzone"
@@ -32,27 +32,27 @@
 pydantic = "^2.0.3"
 pydantic-settings = "^2.0.2"
 rsa = "^4.8"
 tenacity = "^8.2.3"
 exceptiongroup = "^1.1.1"
 tylisten = "^2.1.3"
 pillow = "^10.0.1"
-pychaosvm = { version = "~0.3.4", source = "aioqzone-index" }
+pychaosvm = { version = ">=0.3.4,<0.5.0", source = "aioqzone-index" }
 slide-tc = {version = "~0.1.1", optional = true, source = "aioqzone-index" }
 
 [tool.poetry.extras]
 slide-captcha = ["slide-tc"]
 
 # dependency groups
 [tool.poetry.group.test]
 optional = false
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.4.0"
-pytest-asyncio = "~0.21.0"
+pytest = "^8.2.0"
+pytest-asyncio = "~0.21.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 black = "*"
```

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/api/h5/model.py` & `aioqzone-1.8.2.dev3/src/aioqzone/api/h5/model.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/api/login/__init__.py` & `aioqzone-1.8.2.dev3/src/aioqzone/api/login/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/api/login/_base.py` & `aioqzone-1.8.2.dev3/src/aioqzone/api/login/_base.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/exception.py` & `aioqzone-1.8.2.dev3/src/aioqzone/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/message.py` & `aioqzone-1.8.2.dev3/src/aioqzone/message.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/api/__init__.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 TyRequest = t.TypeVar("TyRequest", bound=QzoneRequestParams)
 TyResponse = t.TypeVar("TyResponse", bound=QzoneResponse)
 TyHttpMethod = t.Union[t.Literal["GET"], t.Literal["POST"]]
 
 
 class QzoneApi(BaseModel, t.Generic[TyRequest, TyResponse]):
+    """The base class for all Qzone APIs below."""
+
     host: t.ClassVar[str] = "https://h5.qzone.qq.com"
     http_method: t.ClassVar[TyHttpMethod]
     path: t.ClassVar[str]
 
     keep_alive: t.ClassVar[bool] = True
     accept: t.ClassVar[t.Optional[str]] = None
     referer: str = "https://h5.qzone.qq.com/"
```

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/api/feed.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/api/feed.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/api/profile.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/api/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Qzone uses different feed schemes for ``/mqzone/profile``. This module patches :mod:`.feed`.
 """
+
 import typing as t
 
 from pydantic import AliasPath, BaseModel, Field, HttpUrl, field_validator, model_validator
 
 from .feed import (
     CommentItem,
     FeedComment,
```

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/api/request.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/api/request.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/api/response.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/api/response.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/protocol/__init__.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module defines types that are used internally by aioqzone and its plugins.
 These types are not designed to represent responses from Qzone.
 """
+
 from pydantic import BaseModel
 
 from .config import *
 from .entity import *
 
 
 class PersudoCurkey(str):
```

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/protocol/config.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/config.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/model/protocol/entity.py` & `aioqzone-1.8.2.dev3/src/aioqzone/model/protocol/entity.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/utils/entity.py` & `aioqzone-1.8.2.dev3/src/aioqzone/utils/entity.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/utils/regex.py` & `aioqzone-1.8.2.dev3/src/aioqzone/utils/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 some patterns for matching html and so on.
 """
+
 import re
 
 # use this to match qzone api response
 response_callback = re.compile(r"callback\(\s*(\{.*\})\s*\)", re.S | re.I)
 # use this to get unikey & curkey of a html
 uni_cur_key = re.compile(r'data-unikey="([^"]*)"[^d]*data-curkey="([^"]*)"')
```

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/utils/retry.py` & `aioqzone-1.8.2.dev3/src/aioqzone/utils/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 
 
 class RetryIfCode(retry_if_exception, Generic[_E]):
     _exc_cls: ClassVar[Type[_E]]  # type: ignore
 
     @classmethod
     @abstractmethod
-    def get_code(cls, exc: _E) -> int:
-        ...
+    def get_code(cls, exc: _E) -> int: ...
 
     def __init__(self, *code: int) -> None:
         super().__init__(lambda exc: isinstance(exc, self._exc_cls) and self.get_code(exc) in code)
 
 
 class retry_if_status(RetryIfCode[ClientResponseError]):
     _exc_cls = ClientResponseError
```

### Comparing `aioqzone-1.8.2.dev1/src/aioqzone/utils/time.py` & `aioqzone-1.8.2.dev3/src/aioqzone/utils/time.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/base.py` & `aioqzone-1.8.2.dev3/src/qqqr/base.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/constant.py` & `aioqzone-1.8.2.dev3/src/qqqr/constant.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/exception.py` & `aioqzone-1.8.2.dev3/src/qqqr/exception.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/message.py` & `aioqzone-1.8.2.dev3/src/qqqr/message.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/qr/__init__.py` & `aioqzone-1.8.2.dev3/src/qqqr/qr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,18 @@
             if m:
                 r = FetchDevUinResp.model_validate_json(m.group(1))
                 push_qr = r.code == 22028 and dev_mid_sig is not None and self.uin in r.uin_list
 
         return QrSession(await self.show(push_qr), login_sig=login_sig)
 
     async def show(self, push_qr=False) -> QR:
+        """``ptqrshow`` api.
+
+        :param push_qr: push QR to mobile client.
+        """
         data = {
             "appid": self.app.appid,
             "daid": self.app.daid,
             "pt_3rd_aid": 0,
             "t": random(),
             "u1": self.proxy.s_url,
         }
@@ -121,15 +125,15 @@
         if cookie:
             cookie.set(cookie.key, "", "")
         return await self.show(push_qr=False)
 
     async def poll(self, sess: QrSession) -> PollResp:
         """Poll QR status.
 
-        :raise `httpx.HTTPStatusError`: if response status code != 200
+        :raise `aiohttp.ClientResponseError`: if response status code != 200
 
         :return: a poll response object
         """
         const = {
             "h": 1,
             "t": 1,
             "g": 1,
@@ -164,25 +168,25 @@
     async def login(
         self,
         *,
         refresh_times: int = 6,
         poll_freq: float = 3,
     ):
         """Loop until cookie is returned or max `refresh_times` exceeds.
-        - This method will emit :meth:`QrEvent.QrFetched` event if a new qrcode is fetched.
-        - If qr is not scanned after `refresh_times`, it will raise :exc:`asyncio.TimeoutError`.
-        - If :obj:`QrEvent.refresh_flag` is set, it will refresh qrcode at once without increasing expire counter.
-        - If :obj:`QrEvent.cancel_flag` is set, it will raise :exc:`UserBreak` before next polling.
+        - This method will emit :obj:`.qr_fetched` event if a new qrcode is fetched.
+        - If qr is not scanned after `refresh_times`, it will raise :exc:`UserTimeout`.
+        - If :obj:`.refresh` is set, it will refresh qrcode at once without increasing expire counter.
+        - If :obj:`.cancel` is set, it will raise :exc:`UserBreak` before next polling.
 
         :meta public:
         :param refresh_times: max qr expire times.
         :param poll_freq: interval between two status polling, in seconds, default as 3.
 
         :raise `UserTimeout`: if qr is not scanned after `refresh_times` expires.
-        :raise `UserBreak`: if :obj:`QrEvent.cancel_flag` is set.
+        :raise `UserBreak`: if :obj:`.cancel` is set.
         """
         self.refresh.clear()
         self.cancel.clear()
 
         cnt_expire = 0
         renew = False
         sess = await self.new()
```

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/qr/type.py` & `aioqzone-1.8.2.dev3/src/qqqr/qr/type.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/type.py` & `aioqzone-1.8.2.dev3/src/qqqr/type.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/_model.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/_model.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/captcha/__init__.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/captcha/_model.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/_model.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/captcha/capsess.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/capsess.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,15 @@
                 await r.text("utf8"),
                 ip=ip or self.prehandle.uip,
                 ua=ua or client.headers["User-Agent"],
                 mouse_track=await self.mouse_track,
             )
 
     @abstractmethod
-    async def get_captcha_problem(self, client: ClientAdapter):
-        ...
+    async def get_captcha_problem(self, client: ClientAdapter): ...
 
     @abstractmethod
     async def solve_captcha(self) -> str:
         """If failed to solve captcha, return an empty string."""
         return ""
 
     @classmethod
```

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/captcha/select/_types.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/select/_types.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/captcha/slide/_types.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/captcha/slide/_types.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/encrypt.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/encrypt.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/h5.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/h5.py`

 * *Files identical despite different names*

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/up/web.py` & `aioqzone-1.8.2.dev3/src/qqqr/up/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             self.client, self.app.appid, str(self.login_page_url), fake_ip=fake_ip
         )
 
     async def new(self):
         """Create a :class:`UpWebSession`. This will call `check` api of Qzone, and receive result
         about whether this login needs a captcha, sms verification, etc.
 
-        :raise `httpx.HTTPStatusError`:
+        :raise `aiohttp.ClientResponseError`: if response status != 200
 
         :return: a up login session
         """
         return UpWebSession(await self._pt_login_sig())
 
     async def check(self, sess: UpWebSession):
         data = {
```

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/utils/iter.py` & `aioqzone-1.8.2.dev3/src/qqqr/utils/iter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import typing as t
 
 T = t.TypeVar("T")
 D = t.TypeVar("D")
 
 
 @t.overload
-def first(it: t.Iterable[T], pred: t.Optional[t.Callable[[T], t.Optional[object]]] = None) -> T:
-    ...
+def first(
+    it: t.Iterable[T], pred: t.Optional[t.Callable[[T], t.Optional[object]]] = None
+) -> T: ...
 
 
 @t.overload
 def first(
     it: t.Iterable[T],
     pred: t.Optional[t.Callable[[T], t.Optional[object]]] = None,
     *,
     default: D,
-) -> t.Union[T, D]:
-    ...
+) -> t.Union[T, D]: ...
 
 
 def first(
     it: t.Iterable[T],
     pred: t.Optional[t.Callable[[T], t.Optional[object]]] = None,
     *,
     default: D = ...,
```

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/utils/jsjson.py` & `aioqzone-1.8.2.dev3/src/qqqr/utils/jsjson.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 logger = logging.getLogger(__name__)
 JsonDict = Dict[Union[str, int], "JsonValue"]
 JsonList = List["JsonValue"]
 JsonValue = Union[bool, int, str, JsonDict, JsonList]
 
 
 class AstLoader:
-    """`AstLoader` uses standard :mod:`ast` module to parse the js/json"""
+    """:class:`AstLoader` uses standard :mod:`ast` module to parse the js/json"""
 
     class RewriteUndef(ast.NodeTransformer):
+        """
+        :meta private:
+        """
+
         const = {
             "undefined": ast.Constant(value=None),
             "null": ast.Constant(value=None),
             "true": ast.Constant(value=True),
             "false": ast.Constant(value=False),
         }
 
@@ -24,33 +28,33 @@
             if node.id in self.const:
                 return self.const[node.id]
             return ast.Str(s=node.id)
 
     @classmethod
     def json_loads(cls, js: str, filename: str = "stdin") -> JsonValue:
         """
-        The json_loads function loads a JSON object from a js/json string. It uses standard
+        The :meth:`~AstLoader.json_loads` function loads a JSON object from a js/json string. It uses standard
         :mod:`ast` module to parse the js/json.
 
         :param js: Used to Pass the js/json string to be parsed.
         :param filename: Used to Specify the name of the file that is being read. This is only for debug use.
-        :return: A jsonvalue object.
+        :return: A :obj:`JsonValue` object.
         """
         js = dedent(js).replace(r"\/", "/")
         node = ast.parse(js, mode="eval")
         node = ast.fix_missing_locations(cls.RewriteUndef().visit(node))
         code = compile(node, filename, mode="eval")
         return eval(code)
 
 
 def json_loads(js: str) -> JsonValue:
-    """The json_loads function converts a string representation of JS/JSON data into a Python object.
+    """The :meth:`json_loads` function converts a string representation of JS/JSON data into a Python object.
     Current implementation is using :external+python:mod:`ast`.
 
-    If you need more parameters or another implementation, call `xxxLoader.json_loads` instead.
-
     .. seealso:: :meth:`.AstLoader.json_loads`
 
+    If you need more parameters or another implementation, call ``xxxLoader.json_loads`` instead.
+
     :param js: Used to Pass the JS/JSON string.
-    :return: A jsonvalue object.
+    :return: A :obj:`JsonValue` object.
     """
     return AstLoader.json_loads(js)
```

### Comparing `aioqzone-1.8.2.dev1/src/qqqr/utils/net.py` & `aioqzone-1.8.2.dev3/src/qqqr/utils/net.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from aiohttp import ClientResponseError
 from aiohttp import ClientSession as ClientAdapter
 
 __all__ = ["raise_for_status", "get_all_cookie", "ClientAdapter"]
 
 
 def raise_for_status(response: Response, *accept_code: int):
-    """A checker more strict than :meth:`~httpx.Response.raise_for_status`.
+    """A checker more strict than :meth:`~aiohttp.ClientResponse.raise_for_status`.
 
     :param response: Client response to check.
     :param accept_code: Overwrite codes that can be accepted, If not given, default is `(200, )`
 
-    :raise `httpx.HTTPStatusError`: if status not in :obj:`accept_code`
+    :raise `aiohttp.ClientResponseError`: if status not in :obj:`accept_code`
     """
     response.raise_for_status
     accept_code = accept_code or (200,)
     if response.status not in accept_code:
         response.release()
         raise ClientResponseError(
             response.request_info,
```

### Comparing `aioqzone-1.8.2.dev1/PKG-INFO` & `aioqzone-1.8.2.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqzone
-Version: 1.8.2.dev1
+Version: 1.8.2.dev3
 Summary: A Python wrapper for Qzone login and H5 APIs.
 Home-page: https://github.com/aioqzone/aioqzone
 License: AGPL-3.0
 Keywords: qzone-api,autologin,asyncio-spider
 Author: aioqzone
 Author-email: zzzzss990315@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: slide-captcha
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
 Requires-Dist: pillow (>=10.0.1,<11.0.0)
-Requires-Dist: pychaosvm (>=0.3.4,<0.4.0)
+Requires-Dist: pychaosvm (>=0.3.4,<0.5.0)
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.2,<3.0.0)
 Requires-Dist: rsa (>=4.8,<5.0)
 Requires-Dist: slide-tc (>=0.1.1,<0.2.0) ; extra == "slide-captcha"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tylisten (>=2.1.3,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/aioqzone/aioqzone/issues
@@ -39,15 +39,15 @@
 # aioqzone
 
 aioqzone封装了一些Qzone接口。
 
 [![python](https://img.shields.io/pypi/pyversions/aioqzone?logo=python&logoColor=white)][home]
 [![version](https://img.shields.io/pypi/v/aioqzone?logo=python)][pypi]
 [![style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![discuss](https://img.shields.io/badge/dynamic/xml?style=social&logo=telegram&label=Discuss&query=%2F%2Fdiv%5B%40class%3D%22tgme_page_extra%22%5D&url=https%3A%2F%2Ft.me%2Faioqzone_chatroom)](https://t.me/aioqzone_chatrooom)
+[![discuss](https://img.shields.io/badge/dynamic/xml?style=social&logo=telegram&label=Discuss&query=%2F%2Fdiv%5B%40class%3D%22tgme_page_extra%22%5D&url=https%3A%2F%2Ft.me%2Faioqzone_chatroom)](https://t.me/aioqzone_chatroom)
 
 [English](README_en.md) | 简体中文
 
 > [!WARNING]
 > aioqzone 仍在开发阶段，任何功能和接口都有可能在未来的版本中发生变化。
 
 > [!IMPORTANT]
```

