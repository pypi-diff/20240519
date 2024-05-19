# Comparing `tmp/flarejax-0.2.3.tar.gz` & `tmp/flarejax-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarejax-0.2.3.tar", last modified: Sat May  4 21:55:02 2024, max compression
+gzip compressed data, was "flarejax-0.2.4.tar", last modified: Sun May 19 16:06:14 2024, max compression
```

## Comparing `flarejax-0.2.3.tar` & `flarejax-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-04 21:55:02.773078 flarejax-0.2.3/
--rw-r--r--   0 anton     (1000) anton     (1000)     2472 2024-05-04 21:55:02.773078 flarejax-0.2.3/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)     2170 2024-04-23 20:44:59.000000 flarejax-0.2.3/README.md
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-04 21:55:02.773078 flarejax-0.2.3/flarejax/
--rw-r--r--   0 anton     (1000) anton     (1000)      719 2024-05-04 21:54:58.000000 flarejax-0.2.3/flarejax/__init__.py
--rw-r--r--   0 anton     (1000) anton     (1000)     3459 2024-04-23 00:20:31.000000 flarejax-0.2.3/flarejax/_config.py
--rw-r--r--   0 anton     (1000) anton     (1000)     4687 2024-05-04 21:44:21.000000 flarejax-0.2.3/flarejax/_frozen.py
--rw-r--r--   0 anton     (1000) anton     (1000)    13521 2024-05-04 21:52:24.000000 flarejax-0.2.3/flarejax/_module.py
--rw-r--r--   0 anton     (1000) anton     (1000)     7633 2024-05-04 21:52:32.000000 flarejax-0.2.3/flarejax/_mtypes.py
--rw-r--r--   0 anton     (1000) anton     (1000)     2872 2024-04-23 00:21:25.000000 flarejax-0.2.3/flarejax/_serial.py
-drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-04 21:55:02.773078 flarejax-0.2.3/flarejax.egg-info/
--rw-r--r--   0 anton     (1000) anton     (1000)     2472 2024-05-04 21:55:02.000000 flarejax-0.2.3/flarejax.egg-info/PKG-INFO
--rw-r--r--   0 anton     (1000) anton     (1000)      298 2024-05-04 21:55:02.000000 flarejax-0.2.3/flarejax.egg-info/SOURCES.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-05-04 21:55:02.000000 flarejax-0.2.3/flarejax.egg-info/dependency_links.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       36 2024-05-04 21:55:02.000000 flarejax-0.2.3/flarejax.egg-info/requires.txt
--rw-r--r--   0 anton     (1000) anton     (1000)        9 2024-05-04 21:55:02.000000 flarejax-0.2.3/flarejax.egg-info/top_level.txt
--rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-05-04 21:55:02.773078 flarejax-0.2.3/setup.cfg
--rw-r--r--   0 anton     (1000) anton     (1000)      684 2024-05-04 16:49:17.000000 flarejax-0.2.3/setup.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-19 16:06:14.007153 flarejax-0.2.4/
+-rw-r--r--   0 anton     (1000) anton     (1000)     2933 2024-05-19 16:06:14.007153 flarejax-0.2.4/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)     2621 2024-05-19 16:04:33.000000 flarejax-0.2.4/README.md
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-19 16:06:14.003819 flarejax-0.2.4/flarejax/
+-rw-r--r--   0 anton     (1000) anton     (1000)      732 2024-05-19 16:06:06.000000 flarejax-0.2.4/flarejax/__init__.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     3664 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_config.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     5909 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_frozen.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     3041 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_modify.py
+-rw-r--r--   0 anton     (1000) anton     (1000)    10874 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_module.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     7368 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_mtypes.py
+-rw-r--r--   0 anton     (1000) anton     (1000)     2950 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_serial.py
+-rw-r--r--   0 anton     (1000) anton     (1000)      150 2024-05-19 16:04:33.000000 flarejax-0.2.4/flarejax/_typecheck.py
+drwxr-xr-x   0 anton     (1000) anton     (1000)        0 2024-05-19 16:06:14.007153 flarejax-0.2.4/flarejax.egg-info/
+-rw-r--r--   0 anton     (1000) anton     (1000)     2933 2024-05-19 16:06:13.000000 flarejax-0.2.4/flarejax.egg-info/PKG-INFO
+-rw-r--r--   0 anton     (1000) anton     (1000)      341 2024-05-19 16:06:13.000000 flarejax-0.2.4/flarejax.egg-info/SOURCES.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        1 2024-05-19 16:06:13.000000 flarejax-0.2.4/flarejax.egg-info/dependency_links.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       27 2024-05-19 16:06:13.000000 flarejax-0.2.4/flarejax.egg-info/requires.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)        9 2024-05-19 16:06:13.000000 flarejax-0.2.4/flarejax.egg-info/top_level.txt
+-rw-r--r--   0 anton     (1000) anton     (1000)       38 2024-05-19 16:06:14.007153 flarejax-0.2.4/setup.cfg
+-rw-r--r--   0 anton     (1000) anton     (1000)      730 2024-05-19 16:04:33.000000 flarejax-0.2.4/setup.py
```

### Comparing `flarejax-0.2.3/PKG-INFO` & `flarejax-0.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-Metadata-Version: 2.1
-Name: flarejax
-Version: 0.2.3
-Summary: Pytree modules classes with easy manipulation and serialization
-Home-page: https://github.com/pwolle/flarejax
-Author: Paul Wollenhaupt
-Author-email: paul.wollenhaupt@gmail.com
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # FlareJax
 Simple pytree module classes for Jax, strongly inspired by [Equinox](https://github.com/patrick-kidger/equinox)
 - Referential transparency via strict immutability
 - Easy manipulation using `.at` & `.set`
 - Safe serialization including hyperparameters
 - Bound methods and function transformations are also modules
 - Auxillary information in key paths for filtered transformations
 
-## Installation
-Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
-```bash
-pip install flarejax
-```
 
 ## Quick Examples
 Modules work similar to dataclasses, but with the added benefit of being pytrees. Making them compatible with all Jax function transformations.
 ```python
 import flarejax as fj
 
 class Linear(fj.Module):
     # The __init__ method is automatically generated
     w: jax.Array
     b: jax.Array
 
-    # Non-pytree fields are marked with leaf=True
-    aux: None = fj.field(leaf=False, default=None)
+    # only jax arrays and modules are considered pytree leaves
+    aux: None = None
 
     # additional intialization methods via classmethods
     @classmethod
     def init(cls, key, dim_in, dim):
-        w = jax.random.normal(key, (dim, dim_in))
+        w = jax.random.normal(key, (dim, dim_in)) * 0.02
         b = jax.numpy.zeros((dim,))
         return cls(w=w, b=b)
 
     def __call__(self, x):
         return self.w @ x + self.b
 
 key = jax.random.PRNGKey(42)
@@ -58,30 +43,39 @@
 
 Although modules are immutable, modified copies can be created using the `at` property.
 ```python
 w_new = jax.numpy.ones((2, 3))
 model = model.at[0].w.set(w_new)
 ```
 
-Turning train mode off for the first layer is only a simple call to `set`.
-```python
-model = model.at[0].config["train"].set(False)
-```
-
 The model can be serialized and deserialized using `fj.save` and `fj.load`.
 ```python
 fj.save("model.npz", model)
 model = fj.load("model.npz")
 ```
 
 Flarejax includes wrappers of the Jax function transformations, which return callable modules.
 ```python
 model = fj.VMap(model)
 model = fj.Jit(model)
 ```
 
-## Roadmap
-- [x] Filtered transformations based on key paths
+## Installation
+Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
+```bash
+pip install flarejax
+```
+
+## Design
+Flarejax modules sacrifice some flexibility for the sake of a unified interface and safety. Flarejax code should alway be easy to reason about and should not contain any footguns from using python magic.
+1. Everything is immutable and 
+2. module fields can be either jax arrays, other modules or json-like data.
 
+This makes it harder to use other jax libraries in flarejax modules. It is recommended to wrap the needed functionality in a module.
+Most jax libraries should be compatible with flarejax modules, since they are simply callable pytrees.
+
+## Roadmap
+- [ ] Filtered grad transformation based on key paths
+- [ ] Pretty printing for modules
 
 ## See also
 - The beautiful [Equinox](https://github.com/patrick-kidger/equinox) library
```

### Comparing `flarejax-0.2.3/README.md` & `flarejax-0.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,43 @@
+Metadata-Version: 2.1
+Name: flarejax
+Version: 0.2.4
+Summary: Immutable pytree modules classes with easy manipulation and serialization
+Home-page: https://github.com/pwolle/flarejax
+Author: Paul Wollenhaupt
+Author-email: paul.wollenhaupt@gmail.com
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
 # FlareJax
 Simple pytree module classes for Jax, strongly inspired by [Equinox](https://github.com/patrick-kidger/equinox)
 - Referential transparency via strict immutability
 - Easy manipulation using `.at` & `.set`
 - Safe serialization including hyperparameters
 - Bound methods and function transformations are also modules
 - Auxillary information in key paths for filtered transformations
 
-## Installation
-Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
-```bash
-pip install flarejax
-```
 
 ## Quick Examples
 Modules work similar to dataclasses, but with the added benefit of being pytrees. Making them compatible with all Jax function transformations.
 ```python
 import flarejax as fj
 
 class Linear(fj.Module):
     # The __init__ method is automatically generated
     w: jax.Array
     b: jax.Array
 
-    # Non-pytree fields are marked with leaf=True
-    aux: None = fj.field(leaf=False, default=None)
+    # only jax arrays and modules are considered pytree leaves
+    aux: None = None
 
     # additional intialization methods via classmethods
     @classmethod
     def init(cls, key, dim_in, dim):
-        w = jax.random.normal(key, (dim, dim_in))
+        w = jax.random.normal(key, (dim, dim_in)) * 0.02
         b = jax.numpy.zeros((dim,))
         return cls(w=w, b=b)
 
     def __call__(self, x):
         return self.w @ x + self.b
 
 key = jax.random.PRNGKey(42)
@@ -48,30 +53,39 @@
 
 Although modules are immutable, modified copies can be created using the `at` property.
 ```python
 w_new = jax.numpy.ones((2, 3))
 model = model.at[0].w.set(w_new)
 ```
 
-Turning train mode off for the first layer is only a simple call to `set`.
-```python
-model = model.at[0].config["train"].set(False)
-```
-
 The model can be serialized and deserialized using `fj.save` and `fj.load`.
 ```python
 fj.save("model.npz", model)
 model = fj.load("model.npz")
 ```
 
 Flarejax includes wrappers of the Jax function transformations, which return callable modules.
 ```python
 model = fj.VMap(model)
 model = fj.Jit(model)
 ```
 
-## Roadmap
-- [x] Filtered transformations based on key paths
+## Installation
+Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
+```bash
+pip install flarejax
+```
+
+## Design
+Flarejax modules sacrifice some flexibility for the sake of a unified interface and safety. Flarejax code should alway be easy to reason about and should not contain any footguns from using python magic.
+1. Everything is immutable and 
+2. module fields can be either jax arrays, other modules or json-like data.
 
+This makes it harder to use other jax libraries in flarejax modules. It is recommended to wrap the needed functionality in a module.
+Most jax libraries should be compatible with flarejax modules, since they are simply callable pytrees.
+
+## Roadmap
+- [ ] Filtered grad transformation based on key paths
+- [ ] Pretty printing for modules
 
 ## See also
 - The beautiful [Equinox](https://github.com/patrick-kidger/equinox) library
```

### Comparing `flarejax-0.2.3/flarejax/_config.py` & `flarejax-0.2.4/flarejax/_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,153 @@
 import functools
 import json
-from typing import Hashable, Self, TypeVar
+from typing import Any, Generic, Self, TypeVar
 
 from ._frozen import FrozenMappingHashable, FrozenSequence
+from ._typecheck import typecheck
 
 __all__ = [
-    "valid_conifg_types",
+    "is_valid_conifg_type",
     "ConfigMapping",
     "ConfigSequence",
-    "to_immutable",
+    "coerce_config_type",
     "ConfigEncoder",
     "ConfigDecoder",
 ]
 
 
-def valid_conifg_types(value):
+@typecheck
+def is_valid_conifg_type(value) -> bool:
     if value is None:
         return True
 
     if isinstance(value, (bool, int, float, str)):
         return True
 
     if isinstance(value, (ConfigMapping, ConfigSequence)):
         return True
 
     return False
 
 
-H = TypeVar("H", bound=Hashable)
+H = TypeVar("H")
 
 
-class ConfigMapping(FrozenMappingHashable[str, H]):
+@typecheck
+class ConfigMapping(FrozenMappingHashable[str, H], Generic[H]):
     def __post_init__(self: Self) -> None:
-        super().__post_init__()
+        _data = dict(self._data)
 
-        if not all(isinstance(k, str) for k in self):
-            raise TypeError("All keys must be strings")
+        for k, v in _data.items():
+            _data[k] = coerce_config_type(v)  # type: ignore
 
-        if not all(isinstance(v, Hashable) for v in self.values()):
-            raise TypeError("All values must be hashable")
+        object.__setattr__(self, "_data", _data)
+        super().__post_init__()
 
-        if not all(valid_conifg_types(v) for v in self.values()):
-            raise TypeError("Invalid value type")
+        for k, v in self.items():
+            if not isinstance(k, str):
+                error = f"All keys must be strings, got {k}"
+                raise TypeError(error)
 
     def __repr__(self: Self) -> str:
         return f"{self.__class__.__name__}({dict(self._data)})"
 
-    # since hashing would be O(n) we cache the result
-    @functools.cached_property
-    def _hash(self: Self) -> int:
-        unfolded = []
-
-        for key in sorted(self, key=hash):
-            unfolded.append((key, self[key]))
 
-        return hash(tuple(unfolded))
-
-    def __hash__(self: Self) -> int:
-        return self._hash
+@typecheck
+class ConfigSequence(FrozenSequence[H], Generic[H]):
+    def __post_init__(self) -> None:
+        _data = list(self._data)
 
+        for i, v in enumerate(_data):
+            _data[i] = coerce_config_type(v)  # type: ignore
 
-class ConfigSequence(FrozenSequence[Hashable]):
-    def __post_init__(self):
+        object.__setattr__(self, "_data", _data)
         super().__post_init__()
 
-        if not all(isinstance(v, Hashable) for v in self):
-            raise TypeError("All values must be hashable")
-
-        if not all(valid_conifg_types(v) for v in self):
-            raise TypeError("Invalid value type")
-
     def __repr__(self: Self) -> str:
         return f"{self.__class__.__name__}({list(self._data)})"
 
     # since hashing would be O(n) we cache the result
     @functools.cached_property
     def _hash(self: Self) -> int:
         return hash(self._data)
 
     def __hash__(self):
         return self._hash
 
 
-def to_immutable(
-    data,
+@typecheck
+def _ismapping(obj: Any) -> bool:
+    try:
+        _ = (lambda **kwargs: kwargs)(**obj)  # type: ignore
+        return True
+    except TypeError:
+        return False
+
+
+@typecheck
+def _issequence(obj: Any) -> bool:
+    try:
+        _ = (lambda *args: args)(*obj)  # type: ignore
+        return True
+    except TypeError:
+        return False
+
+
+@typecheck
+def coerce_config_type(
+    data: Any,
 ) -> None | bool | int | float | str | ConfigMapping | ConfigSequence:
     if data is None:
         return data
 
     if isinstance(data, (bool, int, float, str)):
         return data
 
     if isinstance(data, (ConfigMapping, ConfigSequence)):
         return data
 
-    if isinstance(data, dict):
+    if _ismapping(data):
         data_dict = {}
 
         for key, value in data.items():
-            data_dict[key] = to_immutable(value)
+            data_dict[key] = coerce_config_type(value)
 
         return ConfigMapping(data_dict)
 
-    if isinstance(data, (list, tuple)):
+    if _issequence(data):
         data_list = []
 
         for value in data:
-            data_list.append(to_immutable(value))
+            data_list.append(coerce_config_type(value))
 
         return ConfigSequence(data_list)
 
     error = f"Invalid value type: {data}"
     raise TypeError(error)
 
 
+@typecheck
 class ConfigEncoder(json.JSONEncoder):
-    def default(self, obj):
+    def default(self: Self, obj) -> dict[str, Any] | list[Any] | Any:
         if isinstance(obj, ConfigMapping):
             return dict(obj)
 
         if isinstance(obj, ConfigSequence):
             return list(obj)
 
         return super().default(obj)
 
 
+@typecheck
 class ConfigDecoder(json.JSONDecoder):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         super().__init__(object_hook=self.object_hook, *args, **kwargs)
 
-    def object_hook(self, obj):
+    def object_hook(self: Self, obj) -> ConfigMapping | ConfigSequence | Any:
         if isinstance(obj, dict):
             return ConfigMapping(obj)
 
         if isinstance(obj, list):
             return ConfigSequence(obj)
 
         return obj
```

### Comparing `flarejax-0.2.3/flarejax/_frozen.py` & `flarejax-0.2.4/flarejax/_frozen.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,79 +11,99 @@
     Self,
     Sequence,
     TypeVar,
     ValuesView,
     overload,
 )
 
+from ._typecheck import typecheck
+
 __all__ = [
     "FrozenMapping",
     "FrozenMappingHashable",
     "FrozenSequence",
 ]
 
 K = TypeVar("K", bound=Hashable)
 T = TypeVar("T")
 H = TypeVar("H", bound=Hashable)
 
 
+@typecheck
 @dataclasses.dataclass(frozen=True)
 class FrozenMapping(Generic[K, T]):
-    _data: Mapping[K, T]
+    _data: Mapping[K, T] = dataclasses.field(default_factory=lambda: {})
 
     def __post_init__(self: Self) -> None:
+        # cast to MappingProxyType to make it harder to modify
         object.__setattr__(self, "_data", MappingProxyType(self._data))
 
     def __repr__(self: Self) -> str:
         return f"{self.__class__.__name__}({dict(self._data)})"
 
-    def __getitem__(self: Self, key) -> T:
+    def __getitem__(self: Self, key: K) -> T:
         return self._data[key]
 
     def __iter__(self: Self) -> Iterator[K]:
         return iter(self._data)
 
     def __len__(self: Self) -> int:
         return len(self._data)
 
-    def __contains__(self: Self, key) -> bool:
+    def __contains__(self: Self, key: K, /) -> bool:
         return key in self._data
 
-    def __eq__(self: Self, other: object) -> bool:
+    def __eq__(self: Self, other: object, /) -> bool:
         if not isinstance(other, FrozenMapping):
             return False
 
         return self._data == other._data
 
-    def __ne__(self: Self, other: object) -> bool:
+    def __ne__(self: Self, other: object, /) -> bool:
         return not self == other
 
     def keys(self: Self) -> KeysView[K]:
         return self._data.keys()
 
     def values(self: Self) -> ValuesView[T]:
         return self._data.values()
 
     def items(self: Self) -> ItemsView[K, T]:
         return self._data.items()
 
-    def update(self: Self, other: Mapping[K, T]) -> Self:
+    def update(self: Self, other: Mapping[K, T], /) -> Self:
         return type(self)({**self._data, **other})
 
-    def pop(self: Self, key: K) -> tuple[Self, T]:
-        data = dict(self._data)
-        value = data.pop(key)
-        return type(self)(data), value
+    def pop(self: Self, key: K, /, *d: T) -> tuple[Self, T]:
+        if len(d) > 1:
+            error = f"pop expected at most 2 arguments, {len(d) + 1} given"
+            raise TypeError(error)
+
+        _data = dict(self._data)
+        value = _data.pop(key, *d)
+        return type(self)(_data), value
 
-    def get(self: Self, key: K, default: T) -> T:
+    def get(self: Self, key: K, /, default: T) -> T:
         return self._data.get(key, default)
 
+    def __frozen_set_item__(self: Self, key: Hashable, value: T) -> Self:
+        return dataclasses.replace(self, _data={**self._data, key: value})
+
+    def __frozen_del_item__(self: Self, key: K) -> Self:
+        data = dict(self._data)
+        del data[key]
+        return dataclasses.replace(self, _data=data)
+
 
+@typecheck
 class FrozenMappingHashable(FrozenMapping[K, H]):
     def __post_init__(self: Self) -> None:
+        # TODO maybe add nested coercion to hashable mapping and sequence
+        super().__post_init__()
+
         if not all(isinstance(k, Hashable) for k in self):
             raise TypeError("All keys must be hashable")
 
         if not all(isinstance(v, Hashable) for v in self.values()):
             raise TypeError("All values must be hashable")
 
     # since hashing would be O(n) we cache the result
@@ -96,76 +116,87 @@
 
         return hash(tuple(unfolded))
 
     def __hash__(self: Self) -> int:
         return self._hash
 
 
+@typecheck
 @dataclasses.dataclass(frozen=True)
 class FrozenSequence(Generic[T]):
-    _data: Sequence[T]
+    _data: Sequence[T] = dataclasses.field(default_factory=lambda: ())
 
     def __post_init__(self: Self) -> None:
         object.__setattr__(self, "_data", tuple(self._data))
 
     def __repr__(self: Self) -> str:
         return f"{self.__class__.__name__}({list(self._data)})"
 
     @overload
-    def __getitem__(self: Self, key: int) -> T: ...
+    def __getitem__(self: Self, key: int, /) -> T: ...
 
     @overload
-    def __getitem__(self: Self, key: slice) -> "FrozenSequence[T]": ...
+    def __getitem__(self: Self, key: slice, /) -> "FrozenSequence[T]": ...
 
-    def __getitem__(self: Self, key: int | slice) -> T | "FrozenSequence[T]":
+    def __getitem__(self: Self, key: int | slice, /) -> T | "FrozenSequence[T]":
         if isinstance(key, slice):
             return FrozenSequence(self._data[key])
 
         return self._data[key]
 
     def __iter__(self: Self) -> Iterator[T]:
         return iter(self._data)
 
     def __len__(self: Self) -> int:
         return len(self._data)
 
-    def __contains__(self: Self, value: T) -> bool:
+    def __contains__(self: Self, value: T, /) -> bool:
         return value in self._data
 
     def __reverse__(self: Self) -> Self:
         return type(self)(tuple(reversed(self._data)))
 
-    def __eq__(self: Self, other: object) -> bool:
+    def __eq__(self: Self, other: object, /) -> bool:
         if not isinstance(other, FrozenSequence):
             return False
 
         return self._data == other._data
 
-    def __ne__(self: Self, other: object) -> bool:
+    def __ne__(self: Self, other: object, /) -> bool:
         return not self == other
 
     def index(self: Self, value: T, start: int = 0, stop: int = -1) -> int:
         return self._data.index(value, start, stop)
 
-    def count(self: Self, value: T) -> int:
+    def count(self: Self, value: T, /) -> int:
         return self._data.count(value)
 
-    def append(self: Self, value: T) -> Self:
+    def append(self: Self, value: T, /) -> Self:
         return type(self)(tuple(self._data) + (value,))
 
-    def extend(self: Self, values: Sequence[T]) -> Self:
+    def extend(self: Self, values: Sequence[T], /) -> Self:
         return type(self)(tuple(self._data) + tuple(values))
 
-    def insert(self: Self, index: int, value: T) -> Self:
+    def insert(self: Self, index: int, value: T, /) -> Self:
         data = list(self._data)
         data.insert(index, value)
         return type(self)(data)
 
-    def remove(self: Self, value: T) -> Self:
+    def remove(self: Self, value: T, /) -> Self:
         data = list(self._data)
         data.remove(value)
         return type(self)(data)
 
-    def pop(self: Self, index: int = -1) -> tuple[Self, T]:
+    def pop(self: Self, index: int = -1, /) -> tuple[Self, T]:
         data = list(self._data)
         value = data.pop(index)
         return type(self)(data), value
+
+    def __frozen_set_item__(self: Self, key: int, value: T) -> Self:
+        data = list(self._data)
+        data[key] = value  # type: ignore
+        return dataclasses.replace(self, _data=data)
+
+    def __frozen_del_item__(self: Self, key: int) -> Self:
+        data = list(self._data)
+        del data[key]
+        return dataclasses.replace(self, _data=data)
```

### Comparing `flarejax-0.2.3/flarejax/_mtypes.py` & `flarejax-0.2.4/flarejax/_mtypes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,169 +1,174 @@
-import dataclasses
 import functools
-from typing import Callable, Hashable, Mapping, Self
+from typing import Any, Callable, Generic, Self, TypeVar
 
 import jax
 
-from ._config import ConfigMapping, valid_conifg_types
-from ._frozen import FrozenMapping, FrozenMappingHashable, FrozenSequence
-from ._module import FieldKey, Module, field
+from ._config import ConfigMapping, ConfigSequence, coerce_config_type
+from ._frozen import FrozenMapping, FrozenSequence
+from ._module import FieldKey, Module, field, is_leaf
+from ._typecheck import typecheck
 
 __all__ = [
     "ModuleMapping",
     "ModuleSequence",
     "Sequential",
     "Jit",
     "VMap",
     "Partial",
 ]
 
+M = TypeVar("M")
 
-class ModuleMapping(FrozenMapping[str, Module | Hashable], Module):
-    def __post_init__(self: Self) -> None:
-        super().__post_init__()
 
-        if not all(isinstance(key, str) for key in self):
-            error = "Keys mus be valid strings."
-            raise TypeError(error)
+@typecheck
+class ModuleMapping(FrozenMapping[str, M], Module, Generic[M]):
+    def __post_init__(self: Self) -> None:
+        _data = dict(self._data)
 
-        for key, value in self.items():
-            if isinstance(value, (Module, jax.Array)):
+        for k, v in _data.items():
+            if is_leaf(v):
                 continue
 
-            if valid_conifg_types(value):
-                continue
+            _data[k] = coerce_config_type(v)  # type: ignore
 
-            error = (
-                f"'{self.__class__.__name__}' values must be Modules, jax"
-                f"arrays or config tyes, but got '{value}' for key '{key}'."
-            )
-            raise TypeError(error)
+        object.__setattr__(self, "_data", _data)
+        super().__post_init__()
 
-    def __repr__(self: Self) -> str:
-        return f"{self.__class__.__name__}({dict(self._data)})"
+        if "_leaves" in self:
+            error = "Key '_leaves' is reserved for internal use."
+            raise ValueError(error)
 
-    def __frozen_set_item__(self: Self, key: Hashable, value: Module) -> Self:
-        return dataclasses.replace(self, _data={**self._data, key: value})
+        for k, v in self.items():
+            if not isinstance(k, str):
+                error = f"All keys must be strings, got {k}"
+                raise TypeError(error)
 
-    def __frozen_del_item__(self: Self, key: str) -> Self:
-        data = dict(self._data)
-        del data[key]
-        return dataclasses.replace(self, _data=data)
+    def __repr__(self: Self) -> str:
+        return f"{self.__class__.__name__}({dict(self._data)})"
 
     def tree_flatten_with_keys(
         self: Self,
-    ) -> tuple[
-        tuple[tuple[FieldKey, dict[Hashable, Module]]],
-        ConfigMapping,
-    ]:
-        active = {}
-        static = {}
-
-        for key, value in self.items():
-            if isinstance(value, (Module, jax.Array)):
-                active[key] = value
-            else:
-                static[key] = value
+    ) -> tuple[tuple[tuple[FieldKey, Any], ...], ConfigMapping]:
+        items_active = []
+        items_static = {}
+
+        keys_leaves = []
+        keys_module = sorted(self.keys())
+
+        for module_key in keys_module:
+            value = self[module_key]
+
+            if is_leaf(value):
+                keys_leaves.append(module_key)
+                continue
+
+            items_static[module_key] = value
+
+        items_static["_leaves"] = ConfigSequence(keys_leaves)
+        items_static = ConfigMapping(items_static)
+
+        for module_key in keys_leaves:
+            value = self[module_key]
+            assert is_leaf(value)
+
+            tree_key = FieldKey(
+                name=module_key,
+                type=type(self),
+                tree=items_static,
+            )
+            items_active.append((tree_key, value))
 
-        active_key = FieldKey(
-            name="_data",
-            hint=type(self),
-            grad=True,
-            attr=False,
-            meta=FrozenMappingHashable({}),
-            conf=self.config,
-        )
-        return ((active_key, active),), ConfigMapping(static)
+        return tuple(items_active), items_static
 
     @classmethod
     def tree_unflatten(
         cls,
-        static: Mapping,
-        active: Mapping,
+        static: ConfigMapping,
+        active: tuple[M, ...],
     ) -> Self:
-        print(static, active)
-        return cls({**static, **active[0]})
+        static, leaves = static.pop("_leaves")
+
+        active_items: dict[str, M] = {}
+        assert isinstance(leaves, ConfigSequence)
+
+        for i, k in enumerate(leaves):
+            active_items[k] = active[i]
 
+        return cls({**active_items, **static})
 
-class ModuleSequence(FrozenSequence[Module | Hashable], Module):
+
+@typecheck
+class ModuleSequence(FrozenSequence[M], Module, Generic[M]):
     def __post_init__(self: Self) -> None:
-        super().__post_init__()
+        _data = list(self._data)
 
-        for value in self:
-            if isinstance(value, (Module, jax.Array)):
+        for i, v in enumerate(_data):
+            if is_leaf(v):
                 continue
 
-            if valid_conifg_types(value):
-                continue
+            _data[i] = coerce_config_type(v)  # type: ignore
 
-            error = (
-                f"'{self.__class__.__name__}' values must be Modules, jax"
-                f"arrays or config tyes, but got '{value}'."
-            )
-            raise TypeError(error)
+        object.__setattr__(self, "_data", _data)
+        super().__post_init__()
 
     def __repr__(self: Self) -> str:
         return f"{self.__class__.__name__}({list(self._data)})"
 
-    def __frozen_set_item__(self: Self, key: int, value: Module) -> Self:
-        data = list(self._data)
-        data[key] = value
-        return dataclasses.replace(self, _data=data)
-
-    def __frozen_del_item__(self: Self, key: int) -> Self:
-        data = list(self._data)
-        del data[key]
-        return dataclasses.replace(self, _data=data)
-
     def tree_flatten_with_keys(
         self: Self,
-    ) -> tuple[tuple[tuple[FieldKey, list[Module]]], ConfigMapping]:
-        active = []
-        static = {}
-
-        for i, value in enumerate(self):
-            if isinstance(value, (Module, jax.Array)):
-                active.append(value)
-            else:
-                static[i] = value
+    ) -> tuple[tuple[tuple[FieldKey, Module], ...], ConfigMapping]:
+        items_active = []
+        items_static = {}
 
-        active_key = FieldKey(
-            name="_data",
-            hint=type(self),
-            grad=True,
-            attr=False,
-            meta=FrozenMappingHashable({}),
-            conf=self.config,
-        )
-        return ((active_key, active),), ConfigMapping(static)
+        for i, v in enumerate(self):
+            if is_leaf(v):
+                continue
+
+            items_static[str(i)] = v
+
+        items_static = ConfigMapping(items_static)
+
+        for v in self:
+            if not is_leaf(v):
+                continue
+
+            key = FieldKey(
+                name="_data",
+                type=type(self),
+                tree=items_static,
+            )
+            items_active.append((key, v))
+
+        return tuple(items_active), items_static
 
     @classmethod
     def tree_unflatten(
         cls,
-        static: list[Hashable],
-        active: tuple[list[Module]],
+        static: ConfigMapping,
+        active: tuple[M, ...],
     ) -> Self:
         active_index = 0
-        static_index = 0
         values = []
 
-        for i in range(len(static) + len(active[0])):
+        for i in range(len(static) + len(active)):
+            i = str(i)
+
             if i in static:
-                values.append(static[static_index])
-                static_index += 1
+                values.append(static[i])
 
             else:
-                values.append(active[0][active_index])
+                values.append(active[active_index])
                 active_index += 1
 
         return cls(values)
 
 
-class Sequential(ModuleSequence):
+@typecheck
+class Sequential(ModuleSequence[M], Generic[M]):
     def __post_init__(self: Self) -> None:
         super().__post_init__()
 
         if not all(callable(layer) for layer in self):
             error = "All layers must be callable."
             raise ValueError(error)
 
@@ -176,14 +181,15 @@
 
 
 @jax.jit
 def _jit_apply_layer(layer, *args, **kwargs):
     return layer(*args, **kwargs)
 
 
+@typecheck
 class Jit(Module):
     """
     Wrap a module into a Jitted module, that can be used in Jax transformations.
 
     Attributes:
     ---
     module: Module
@@ -197,14 +203,15 @@
             error = f"Module {self.module} is not callable."
             raise ValueError(error)
 
     def __call__(self: Self, *args, **kwargs):
         return _jit_apply_layer(self.module, *args, **kwargs)
 
 
+@typecheck
 class VMap(Module):
     """
     A wrapper of 'jax.vmap', that returns a module, such that is compatible with
     module functionalities like serialization and the Jax Pytree utilities.
 
     Attributes:
     ---
@@ -232,14 +239,15 @@
         return jax.vmap(
             self.module,
             self.in_axes,
             self.out_axes,
         )(*args, **kwargs)
 
 
+@typecheck
 class Partial(Module):
     """
     A wrapper of 'functools.partial', that returns a module, such that is compatible
     with module functionalities like serialization and the Jax Pytree utilities.
 
     Attributes:
     ---
```

### Comparing `flarejax-0.2.3/flarejax/_serial.py` & `flarejax-0.2.4/flarejax/_serial.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 from typing import Any
 
 import jax.numpy as jnp
 import jax.tree_util as jtu
 
 from ._config import ConfigEncoder, ConfigDecoder
 from ._module import GLOBAL_MODULE_REGISTRY, Module, get_module_name
+from ._typecheck import typecheck
 
 __all__ = [
     "save_module",
     "load_module",
 ]
 
 
+@typecheck
 def treedef_to_dict(treedef, /) -> dict[str, Any] | None:
     """
     Convert a PyTree tree definition into a nested dictionary.
     """
     if treedef.node_data() is None:
         return None
 
@@ -30,14 +32,15 @@
     return {
         "__module_name": name,
         "aux_data": node_data[1],
         "children": [treedef_to_dict(child) for child in treedef.children()],
     }
 
 
+@typecheck
 def dict_to_treedef(data, /) -> jtu.PyTreeDef:
     """
     Convert a nested dictionary created by 'treedef_to_dict' back into a PyTree.
     """
     if data is None:
         return jtu.PyTreeDef.make_from_node_data_and_children(
             jtu.default_registry, None, []
@@ -52,14 +55,15 @@
     return jtu.PyTreeDef.make_from_node_data_and_children(
         jtu.default_registry,
         (cls, data["aux_data"]),
         (dict_to_treedef(child) for child in data["children"]),
     )
 
 
+@typecheck
 def save_module(path: str, tree: Module | list | dict | tuple | None) -> None:
     """
     Save a module to disk.
     This is done by fist flattening the module using the PyTree API, then the
     leaves are saved to disk as numpy arrays and the tree structure is
     serialized to JSON and also saved in the same zip archive.
     """
@@ -72,14 +76,15 @@
     treedef = treedef_to_dict(treedef)
     treedef = json.dumps(treedef, indent=2, cls=ConfigEncoder)
 
     arrays["treedef"] = treedef
     jnp.savez(path, **arrays)
 
 
+@typecheck
 def load_module(path: str) -> Module | list | dict | tuple | None:
     """
     Load a module from disk, which was saved using the 'save_module' function.
 
     Example
     ---
     >>> module = {"key": "value"}
```

### Comparing `flarejax-0.2.3/flarejax.egg-info/PKG-INFO` & `flarejax-0.2.4/flarejax.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 Metadata-Version: 2.1
 Name: flarejax
-Version: 0.2.3
-Summary: Pytree modules classes with easy manipulation and serialization
+Version: 0.2.4
+Summary: Immutable pytree modules classes with easy manipulation and serialization
 Home-page: https://github.com/pwolle/flarejax
 Author: Paul Wollenhaupt
 Author-email: paul.wollenhaupt@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # FlareJax
 Simple pytree module classes for Jax, strongly inspired by [Equinox](https://github.com/patrick-kidger/equinox)
 - Referential transparency via strict immutability
 - Easy manipulation using `.at` & `.set`
 - Safe serialization including hyperparameters
 - Bound methods and function transformations are also modules
 - Auxillary information in key paths for filtered transformations
 
-## Installation
-Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
-```bash
-pip install flarejax
-```
 
 ## Quick Examples
 Modules work similar to dataclasses, but with the added benefit of being pytrees. Making them compatible with all Jax function transformations.
 ```python
 import flarejax as fj
 
 class Linear(fj.Module):
     # The __init__ method is automatically generated
     w: jax.Array
     b: jax.Array
 
-    # Non-pytree fields are marked with leaf=True
-    aux: None = fj.field(leaf=False, default=None)
+    # only jax arrays and modules are considered pytree leaves
+    aux: None = None
 
     # additional intialization methods via classmethods
     @classmethod
     def init(cls, key, dim_in, dim):
-        w = jax.random.normal(key, (dim, dim_in))
+        w = jax.random.normal(key, (dim, dim_in)) * 0.02
         b = jax.numpy.zeros((dim,))
         return cls(w=w, b=b)
 
     def __call__(self, x):
         return self.w @ x + self.b
 
 key = jax.random.PRNGKey(42)
@@ -58,30 +53,39 @@
 
 Although modules are immutable, modified copies can be created using the `at` property.
 ```python
 w_new = jax.numpy.ones((2, 3))
 model = model.at[0].w.set(w_new)
 ```
 
-Turning train mode off for the first layer is only a simple call to `set`.
-```python
-model = model.at[0].config["train"].set(False)
-```
-
 The model can be serialized and deserialized using `fj.save` and `fj.load`.
 ```python
 fj.save("model.npz", model)
 model = fj.load("model.npz")
 ```
 
 Flarejax includes wrappers of the Jax function transformations, which return callable modules.
 ```python
 model = fj.VMap(model)
 model = fj.Jit(model)
 ```
 
-## Roadmap
-- [x] Filtered transformations based on key paths
+## Installation
+Memmpy can be installed directly from PyPI using `pip`. It requires Python 3.10+ and Jax 0.4.26+.
+```bash
+pip install flarejax
+```
+
+## Design
+Flarejax modules sacrifice some flexibility for the sake of a unified interface and safety. Flarejax code should alway be easy to reason about and should not contain any footguns from using python magic.
+1. Everything is immutable and 
+2. module fields can be either jax arrays, other modules or json-like data.
 
+This makes it harder to use other jax libraries in flarejax modules. It is recommended to wrap the needed functionality in a module.
+Most jax libraries should be compatible with flarejax modules, since they are simply callable pytrees.
+
+## Roadmap
+- [ ] Filtered grad transformation based on key paths
+- [ ] Pretty printing for modules
 
 ## See also
 - The beautiful [Equinox](https://github.com/patrick-kidger/equinox) library
```

### Comparing `flarejax-0.2.3/setup.py` & `flarejax-0.2.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,20 +6,25 @@
     long_description = fh.read()
 
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
+description = (
+    "Immutable pytree modules classes with easy manipulation and serialization"
+)
+
+
 setup(
     name="flarejax",
     version=__version__,
     packages=find_packages(where="."),
     python_requires=">=3.10",
     install_requires=requirements,
-    description="Pytree modules classes with easy manipulation and serialization",
+    description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pwolle/flarejax",
     author="Paul Wollenhaupt",
     author_email="paul.wollenhaupt@gmail.com",
 )
```

