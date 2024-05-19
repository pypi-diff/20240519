# Comparing `tmp/promplate-0.3.4.6.tar.gz` & `tmp/promplate-0.3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate-0.3.4.6.tar", max compression
+gzip compressed data, was "promplate-0.3.4.7.tar", max compression
```

## Comparing `promplate-0.3.4.6.tar` & `promplate-0.3.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1926 2024-05-17 19:21:07.427084 promplate-0.3.4.6/README.md
--rw-r--r--   0        0        0       43 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/__init__.py
--rw-r--r--   0        0        0      101 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/__init__.py
--rw-r--r--   0        0        0     2250 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/callback.py
--rw-r--r--   0        0        0    16908 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/node.py
--rw-r--r--   0        0        0     1273 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/utils.py
--rw-r--r--   0        0        0        0 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/__init__.py
--rw-r--r--   0        0        0     1007 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/base.py
--rw-r--r--   0        0        0      114 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/openai/__init__.py
--rw-r--r--   0        0        0     4007 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/openai/v0.py
--rw-r--r--   0        0        0     5818 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/openai/v1.py
--rw-r--r--   0        0        0       85 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/__init__.py
--rw-r--r--   0        0        0     1577 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/builder.py
--rw-r--r--   0        0        0     3108 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/chat.py
--rw-r--r--   0        0        0     7920 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/template.py
--rw-r--r--   0        0        0     3680 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/utils.py
--rw-r--r--   0        0        0     1538 2024-05-17 19:21:07.427084 promplate-0.3.4.6/pyproject.toml
--rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 promplate-0.3.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1926 2024-05-19 21:31:52.056619 promplate-0.3.4.7/README.md
+-rw-r--r--   0        0        0       43 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/chain/__init__.py
+-rw-r--r--   0        0        0     2250 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/chain/callback.py
+-rw-r--r--   0        0        0    17281 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/chain/node.py
+-rw-r--r--   0        0        0     1273 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/chain/utils.py
+-rw-r--r--   0        0        0        0 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/llm/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/llm/base.py
+-rw-r--r--   0        0        0      114 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4007 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/llm/openai/v0.py
+-rw-r--r--   0        0        0     5818 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/llm/openai/v1.py
+-rw-r--r--   0        0        0       85 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/prompt/__init__.py
+-rw-r--r--   0        0        0     1577 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/prompt/builder.py
+-rw-r--r--   0        0        0     3108 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/prompt/chat.py
+-rw-r--r--   0        0        0     7920 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/prompt/template.py
+-rw-r--r--   0        0        0     3680 2024-05-19 21:31:52.056619 promplate-0.3.4.7/promplate/prompt/utils.py
+-rw-r--r--   0        0        0     1538 2024-05-19 21:31:52.056619 promplate-0.3.4.7/pyproject.toml
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 promplate-0.3.4.7/PKG-INFO
```

### Comparing `promplate-0.3.4.6/README.md` & `promplate-0.3.4.7/README.md`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/chain/callback.py` & `promplate-0.3.4.7/promplate/chain/callback.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/chain/node.py` & `promplate-0.3.4.7/promplate/chain/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 from inspect import isclass
 from itertools import accumulate
-from typing import Callable, Mapping, MutableMapping, overload
+from typing import Callable, Mapping, MutableMapping, TypeVar, overload
 
 from ..llm.base import *
 from ..prompt.template import Context, Loader, SafeChainMapContext, Template
 from .callback import BaseCallback, Callback
 from .utils import accumulate_any, resolve
 
+C = TypeVar("C", bound="ChainContext")
+
 
 class ChainContext(SafeChainMapContext):
     @overload
-    def __init__(self): ...
+    def __new__(cls): ...
 
     @overload
-    def __init__(self, least: MutableMapping | None = None): ...
+    def __new__(cls, least: C, *maps: Mapping) -> C: ...
 
     @overload
-    def __init__(self, least: MutableMapping | None = None, *maps: Mapping): ...
+    def __new__(cls, least: MutableMapping | None = None, *maps: Mapping): ...
 
     def __init__(self, least: MutableMapping | None = None, *maps: Mapping):
         super().__init__({} if least is None else least, *maps)  # type: ignore
 
+    def __new__(cls, *args, **kwargs):  # type: ignore
+        try:
+            least = args[0]
+        except IndexError:
+            least = kwargs.get("least")
+        if isinstance(least, cls) and least.__class__ is not cls:
+            return least.__class__(*args, **kwargs)
+
+        return super().__new__(cls, *args, **kwargs)
+
     @classmethod
     def ensure(cls, context):
         return context if isinstance(context, cls) else cls(context)
 
     @property
     def result(self):
         return self.__getitem__("__result__")
```

### Comparing `promplate-0.3.4.6/promplate/chain/utils.py` & `promplate-0.3.4.7/promplate/chain/utils.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/llm/base.py` & `promplate-0.3.4.7/promplate/llm/base.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/llm/openai/v0.py` & `promplate-0.3.4.7/promplate/llm/openai/v0.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/llm/openai/v1.py` & `promplate-0.3.4.7/promplate/llm/openai/v1.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/prompt/builder.py` & `promplate-0.3.4.7/promplate/prompt/builder.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/prompt/chat.py` & `promplate-0.3.4.7/promplate/prompt/chat.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/prompt/template.py` & `promplate-0.3.4.7/promplate/prompt/template.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/promplate/prompt/utils.py` & `promplate-0.3.4.7/promplate/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.6/pyproject.toml` & `promplate-0.3.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promplate"
-version = "0.3.4.6"
+version = "0.3.4.7"
 description = "Prompt engineering framework for humans"
 homepage = "https://promplate.dev/"
 documentation = "https://docs.py.promplate.dev/"
 repository = "https://github.com/promplate/core"
 authors = ["Muspi Merol <me@promplate.dev>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `promplate-0.3.4.6/PKG-INFO` & `promplate-0.3.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate
-Version: 0.3.4.6
+Version: 0.3.4.7
 Summary: Prompt engineering framework for humans
 Home-page: https://promplate.dev/
 License: MIT
 Keywords: prompt,template,nlp,llm
 Author: Muspi Merol
 Author-email: me@promplate.dev
 Requires-Python: >=3.10,<4.0
```

