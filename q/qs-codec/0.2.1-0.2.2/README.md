# Comparing `tmp/qs_codec-0.2.1.tar.gz` & `tmp/qs_codec-0.2.2.tar.gz`

## Comparing `qs_codec-0.2.1.tar` & `qs_codec-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qs_codec-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.2.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.2.1/requirements_dev.txt
--rw-r--r--   0        0        0    28785 2020-02-02 00:00:00.000000 qs_codec-0.2.1/docs/README.rst
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/__init__.py
--rw-r--r--   0        0        0     6715 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/decode.py
--rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/encode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/__init__.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/charset.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/duplicates.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/format.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/list_format.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/enums/sentinel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/decode_options.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/encode_options.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/undefined.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/models/weak_wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/__init__.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/decode_utils.py
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/encode_utils.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/str_utils.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 qs_codec-0.2.1/src/qs_codec/utils/utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/__init__.py
--rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/compare_outputs.sh
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/package.json
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/qs.js
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/qs.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/comparison/test_cases.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/e2e/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/e2e/e2e_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/__init__.py
--rw-r--r--   0        0        0    29989 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/decode_test.py
--rw-r--r--   0        0        0    50930 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/encode_test.py
--rw-r--r--   0        0        0    22214 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/example_test.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/fixed_qs_issues_test.py
--rw-r--r--   0        0        0    14896 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/utils_test.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.2.1/tests/unit/weakref_test.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.2.1/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.2.1/LICENSE
--rw-r--r--   0        0        0    36399 2020-02-02 00:00:00.000000 qs_codec-0.2.1/README.rst
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 qs_codec-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    38005 2020-02-02 00:00:00.000000 qs_codec-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 qs_codec-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 qs_codec-0.2.2/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 qs_codec-0.2.2/requirements_dev.txt
+-rw-r--r--   0        0        0    28807 2020-02-02 00:00:00.000000 qs_codec-0.2.2/docs/README.rst
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/__init__.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/decode.py
+-rw-r--r--   0        0        0    10386 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/encode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/__init__.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/charset.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/duplicates.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/format.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/list_format.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/enums/sentinel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/decode_options.py
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/encode_options.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/undefined.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/models/weak_wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/__init__.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/decode_utils.py
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/encode_utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/str_utils.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 qs_codec-0.2.2/src/qs_codec/utils/utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/__init__.py
+-rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/compare_outputs.sh
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/package.json
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/qs.js
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/qs.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/comparison/test_cases.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/e2e/__init__.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/e2e/e2e_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0    30061 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/decode_test.py
+-rw-r--r--   0        0        0    51290 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/encode_test.py
+-rw-r--r--   0        0        0    22222 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/example_test.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/fixed_qs_issues_test.py
+-rw-r--r--   0        0        0    14910 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/utils_test.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 qs_codec-0.2.2/tests/unit/weakref_test.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 qs_codec-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 qs_codec-0.2.2/LICENSE
+-rw-r--r--   0        0        0    36421 2020-02-02 00:00:00.000000 qs_codec-0.2.2/README.rst
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 qs_codec-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    38027 2020-02-02 00:00:00.000000 qs_codec-0.2.2/PKG-INFO
```

### Comparing `qs_codec-0.2.1/CHANGELOG.md` & `qs_codec-0.2.2/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.2.2
+
+* [FEAT] `decode` returns `dict[str, Any]` instead of `dict` ([#4](https://github.com/techouse/qs_codec/pull/4))
+* [FIX] fix decoding encoded square brackets in key names
+
 ## 0.2.1
 
 * [CHORE] update dependencies
 
 ## 0.2.0
 
 * [CHORE] update dependencies
```

### Comparing `qs_codec-0.2.1/CODE-OF-CONDUCT.md` & `qs_codec-0.2.2/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/docs/README.rst` & `qs_codec-0.2.2/docs/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 .. code:: python
 
    import qs_codec, typing as t
 
    def decode(
        value: t.Optional[t.Union[str, t.Mapping]],
        options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
-   ) -> dict:
+   ) -> t.Dict[str, t.Any]:
        """Decodes a str or Mapping into a Dict. 
        
        Providing custom DecodeOptions will override the default behavior."""
        pass
 
 :py:attr:`decode <qs_codec.decode>` allows you to create nested ``dict``\ s within your query
 strings, by surrounding the name of sub-keys with square brackets
@@ -299,47 +299,47 @@
 for example, ``a[999999999]`` and it will take significant time to iterate
 over this huge ``list``.
 
 .. code:: python
 
    import qs_codec
 
-   assert qs_codec.decode('a[100]=b') == {'a': {100: 'b'}}
+   assert qs_codec.decode('a[100]=b') == {'a': {'100': 'b'}}
 
 This limit can be overridden by passing an :py:attr:`list_limit <qs_codec.models.decode_options.DecodeOptions.list_limit>`
 option:
 
 .. code:: python
 
    import qs_codec
 
    assert qs_codec.decode(
        'a[1]=b',
        qs_codec.DecodeOptions(list_limit=0),
-   ) == {'a': {1: 'b'}}
+   ) == {'a': {'1': 'b'}}
 
 To disable ``list`` parsing entirely, set :py:attr:`parse_lists <qs_codec.models.decode_options.DecodeOptions.parse_lists>`
 to ``False``.
 
 .. code:: python
 
    import qs_codec
 
    assert qs_codec.decode(
        'a[]=b',
        qs_codec.DecodeOptions(parse_lists=False),
-   ) == {'a': {0: 'b'}}
+   ) == {'a': {'0': 'b'}}
 
 If you mix notations, :py:attr:`decode <qs_codec.decode>` will merge the two items into a ``dict``:
 
 .. code:: python
 
    import qs_codec
 
-   assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {0: 'b', 'b': 'c'}}
+   assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {'0': 'b', 'b': 'c'}}
 
 You can also create ``list``\ s of ``dict``\ s:
 
 .. code:: python
 
    import qs_codec
```

### Comparing `qs_codec-0.2.1/src/qs_codec/decode.py` & `qs_codec-0.2.2/src/qs_codec/decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,33 @@
 from .enums.duplicates import Duplicates
 from .enums.sentinel import Sentinel
 from .models.decode_options import DecodeOptions
 from .models.undefined import Undefined
 from .utils.utils import Utils
 
 
-def decode(value: t.Optional[t.Union[str, t.Mapping]], options: DecodeOptions = DecodeOptions()) -> dict:
+def decode(
+    value: t.Optional[t.Union[str, t.Dict[str, t.Any]]], options: DecodeOptions = DecodeOptions()
+) -> t.Dict[str, t.Any]:
     """
     Decodes a ``str`` or ``Mapping`` into a ``dict``.
 
     Providing custom ``DecodeOptions`` will override the default behavior.
     """
+    obj: t.Dict[str, t.Any] = {}
+
     if not value:
-        return dict()
+        return obj
 
-    if not isinstance(value, (str, t.Mapping)):
+    if not isinstance(value, (str, dict)):
         raise ValueError("The input must be a String or a Dict")
 
-    temp_obj: t.Optional[t.Mapping] = _parse_query_string_values(value, options) if isinstance(value, str) else value
-    obj: t.Dict = dict()
+    temp_obj: t.Optional[t.Dict[str, t.Any]] = (
+        _parse_query_string_values(value, options) if isinstance(value, str) else value
+    )
 
     # Iterate over the keys and setup the new object
     if temp_obj:
         for key, val in temp_obj.items():
             new_obj: t.Any = _parse_keys(key, val, options, isinstance(value, str))
             obj = Utils.merge(obj, new_obj, options)  # type: ignore [assignment]
 
@@ -45,18 +50,19 @@
 def _parse_array_value(value: t.Any, options: DecodeOptions) -> t.Any:
     if isinstance(value, str) and value and options.comma and "," in value:
         return value.split(",")
 
     return value
 
 
-def _parse_query_string_values(value: str, options: DecodeOptions) -> t.Dict:
-    obj: t.Dict = dict()
+def _parse_query_string_values(value: str, options: DecodeOptions) -> t.Dict[str, t.Any]:
+    obj: t.Dict[str, t.Any] = {}
 
     clean_str: str = value.replace("?", "", 1) if options.ignore_query_prefix else value
+    clean_str = clean_str.replace("%5B", "[").replace("%5b", "[").replace("%5D", "]").replace("%5d", "]")
     limit: t.Optional[int] = None if isinf(options.parameter_limit) else options.parameter_limit  # type: ignore [assignment]
     parts: t.List[str]
     if isinstance(options.delimiter, re.Pattern):
         parts = re.split(options.delimiter, clean_str) if not limit else re.split(options.delimiter, clean_str)[:limit]
     else:
         parts = clean_str.split(options.delimiter) if not limit else clean_str.split(options.delimiter)[:limit]
 
@@ -114,15 +120,15 @@
 def _parse_object(
     chain: t.Union[t.List[str], t.Tuple[str, ...]], val: t.Any, options: DecodeOptions, values_parsed: bool
 ) -> t.Any:
     leaf: t.Any = val if values_parsed else _parse_array_value(val, options)
 
     i: int
     for i in reversed(range(len(chain))):
-        obj: t.Optional[t.Any]
+        obj: t.Optional[t.Union[t.Dict[str, t.Any], t.List[t.Any]]]
         root: str = chain[i]
 
         if root == "[]" and options.parse_lists:
             if options.allow_empty_lists and leaf == "":
                 obj = []
             else:
                 obj = list(leaf) if isinstance(leaf, (list, tuple)) else [leaf]
@@ -136,27 +142,27 @@
             index: t.Optional[int]
             try:
                 index = int(decoded_root, 10)
             except (ValueError, TypeError):
                 index = None
 
             if not options.parse_lists and decoded_root == "":
-                obj = {0: leaf}
+                obj = {"0": leaf}
             elif (
                 index is not None
                 and index >= 0
                 and root != decoded_root
                 and str(index) == decoded_root
                 and options.parse_lists
                 and index <= options.list_limit
             ):
                 obj = [Undefined() for _ in range(index + 1)]
                 obj[index] = leaf
             else:
-                obj[index if index is not None else decoded_root] = leaf
+                obj[str(index) if index is not None else decoded_root] = leaf
 
         leaf = obj
 
     return leaf
 
 
 def _parse_keys(given_key: t.Optional[str], val: t.Any, options: DecodeOptions, values_parsed: bool) -> t.Any:
```

### Comparing `qs_codec-0.2.1/src/qs_codec/encode.py` & `qs_codec-0.2.2/src/qs_codec/encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 def _encode(
     value: t.Any,
     is_undefined: bool,
     side_channel: WeakKeyDictionary,
     prefix: t.Optional[str],
     comma_round_trip: t.Optional[bool],
     encoder: t.Optional[t.Callable[[t.Any, t.Optional[Charset], t.Optional[Format]], str]],
-    serialize_date: t.Callable[[datetime], str],
+    serialize_date: t.Callable[[datetime], t.Optional[str]],
     sort: t.Optional[t.Callable[[t.Any, t.Any], int]],
     filter: t.Optional[t.Union[t.Callable, t.List[t.Union[str, int]]]],
     formatter: t.Optional[t.Callable[[str], str]],
     format: Format = Format.RFC3986,
     generate_array_prefix: t.Callable[[str, t.Optional[str]], str] = ListFormat.INDICES.generator,
     allow_empty_lists: bool = False,
     strict_null_handling: bool = False,
```

### Comparing `qs_codec-0.2.1/src/qs_codec/enums/format.py` & `qs_codec-0.2.2/src/qs_codec/enums/format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/enums/list_format.py` & `qs_codec-0.2.2/src/qs_codec/enums/list_format.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/enums/sentinel.py` & `qs_codec-0.2.2/src/qs_codec/enums/sentinel.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/models/decode_options.py` & `qs_codec-0.2.2/src/qs_codec/models/decode_options.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/models/encode_options.py` & `qs_codec-0.2.2/src/qs_codec/models/encode_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """Use the ``filter`` option to restrict which keys will be included in the encoded output.
     If you pass a ``Callable``, it will be called for each key to obtain the replacement value.
     If you pass a ``list``, it will be used to select properties and ``list`` indices to be encoded."""
 
     skip_nulls: bool = False
     """Set to ``True`` to completely skip encoding keys with ``None`` values."""
 
-    serialize_date: t.Callable[[datetime], str] = EncodeUtils.serialize_date
+    serialize_date: t.Callable[[datetime], t.Optional[str]] = EncodeUtils.serialize_date
     """If you only want to override the serialization of ``datetime`` objects, you can provide a ``Callable``."""
 
     encoder: t.Callable[[t.Any, t.Optional[Charset], t.Optional[Format]], str] = field(  # type: ignore [assignment]
         default_factory=EncodeUtils.encode  # type: ignore [arg-type]
     )
     """Set an ``Encoder`` to affect the encoding of values.
     Note: the ``encoder`` option does not apply if ``encode`` is ``False``."""
```

### Comparing `qs_codec-0.2.1/src/qs_codec/models/weak_wrapper.py` & `qs_codec-0.2.2/src/qs_codec/models/weak_wrapper.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/utils/decode_utils.py` & `qs_codec-0.2.2/src/qs_codec/utils/decode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/utils/encode_utils.py` & `qs_codec-0.2.2/src/qs_codec/utils/encode_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/utils/str_utils.py` & `qs_codec-0.2.2/src/qs_codec/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/src/qs_codec/utils/utils.py` & `qs_codec-0.2.2/src/qs_codec/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 
 class Utils:
     """A collection of utility methods used by the library."""
 
     @staticmethod
     def merge(
-        target: t.Optional[t.Union[t.Mapping, t.List, t.Tuple]],
-        source: t.Optional[t.Union[t.Mapping, t.List, t.Tuple, t.Any]],
+        target: t.Optional[t.Union[t.Mapping[str, t.Any], t.List[t.Any], t.Tuple]],
+        source: t.Optional[t.Union[t.Mapping[str, t.Any], t.List[t.Any], t.Tuple, t.Any]],
         options: DecodeOptions = DecodeOptions(),
-    ) -> t.Union[t.Dict, t.List, t.Tuple, t.Any]:
+    ) -> t.Union[t.Dict[str, t.Any], t.List, t.Tuple, t.Any]:
         """Merge two objects together."""
         if source is None:
             return target
 
         if not isinstance(source, t.Mapping):
             if isinstance(target, (list, tuple)):
                 if any(isinstance(el, Undefined) for el in target):
@@ -56,58 +56,58 @@
                         if isinstance(target, tuple):
                             target = list(target)
                         target.append(source)
             elif isinstance(target, t.Mapping):
                 if isinstance(source, (list, tuple)):
                     target = {
                         **target,
-                        **{i: item for i, item in enumerate(source) if not isinstance(item, Undefined)},
+                        **{str(i): item for i, item in enumerate(source) if not isinstance(item, Undefined)},
                     }
             elif source is not None:
                 if not isinstance(target, (list, tuple)) and isinstance(source, (list, tuple)):
                     return [target, *filter(lambda el: not isinstance(el, Undefined), source)]
                 return [target, source]
 
             return target
 
         if target is None or not isinstance(target, t.Mapping):
             if isinstance(target, (list, tuple)):
                 return {
-                    **{i: item for i, item in enumerate(target) if not isinstance(item, Undefined)},
+                    **{str(i): item for i, item in enumerate(target) if not isinstance(item, Undefined)},
                     **source,
                 }
 
             return [
                 el
                 for el in (target if isinstance(target, (list, tuple)) else [target])
                 if not isinstance(el, Undefined)
             ] + [
                 el
                 for el in (source if isinstance(source, (list, tuple)) else [source])
                 if not isinstance(el, Undefined)
             ]
 
-        merge_target: t.Dict = (
-            dict(enumerate(el for el in source if not isinstance(el, Undefined)))
+        merge_target: t.Dict[str, t.Any] = (
+            {str(i): el for i, el in enumerate(source) if not isinstance(el, Undefined)}
             if isinstance(target, (list, tuple)) and not isinstance(source, (list, tuple))
             else copy.deepcopy(dict(target) if not isinstance(target, dict) else target)
         )
 
         return {
             **merge_target,
             **{
-                key: Utils.merge(merge_target[key], value, options) if key in merge_target else value
+                str(key): Utils.merge(merge_target[key], value, options) if key in merge_target else value
                 for key, value in source.items()
             },
         }
 
     @staticmethod
-    def compact(value: t.Dict) -> t.Dict:
+    def compact(value: t.Dict[str, t.Any]) -> t.Dict[str, t.Any]:
         """Remove all `Undefined` values from a dictionary."""
-        queue: t.List[t.Dict] = [{"obj": {"o": value}, "prop": "o"}]
+        queue: t.List[t.Dict[str, t.Any]] = [{"obj": {"o": value}, "prop": "o"}]
         refs: t.List = []
 
         for i in range(len(queue)):  # pylint: disable=C0200
             item: t.Mapping = queue[i]
             obj: t.Mapping = item["obj"][item["prop"]]
 
             keys: t.List = list(obj.keys())
```

### Comparing `qs_codec-0.2.1/tests/comparison/qs.py` & `qs_codec-0.2.2/tests/comparison/qs.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/tests/unit/decode_test.py` & `qs_codec-0.2.2/tests/unit/decode_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def test_throws_an_error_if_the_input_is_not_a_string_or_a_dict(self) -> None:
         with pytest.raises(ValueError):
             decode(123)
 
     @pytest.mark.parametrize(
         "encoded, decoded, options",
         [
-            ("0=foo", {0: "foo"}, None),
+            ("0=foo", {"0": "foo"}, None),
             ("foo=c++", {"foo": "c  "}, None),
             ("a[>=]=23", {"a": {">=": "23"}}, None),
             ("a[<=>]==23", {"a": {"<=>": "=23"}}, None),
             ("a[==]=23", {"a": {"==": "23"}}, None),
             ("foo", {"foo": None}, DecodeOptions(strict_null_handling=True)),
             ("foo", {"foo": ""}, None),
             ("foo=", {"foo": ""}, None),
@@ -185,22 +185,22 @@
         assert decode("a[b][]=c&a[b][]=d") == {"a": {"b": ["c", "d"]}}
         assert decode("a[>=]=25") == {"a": {">=": "25"}}
 
     def test_allows_to_specify_list_indices(self) -> None:
         assert decode("a[1]=c&a[0]=b&a[2]=d") == {"a": ["b", "c", "d"]}
         assert decode("a[1]=c&a[0]=b") == {"a": ["b", "c"]}
         assert decode("a[1]=c", DecodeOptions(list_limit=20)) == {"a": ["c"]}
-        assert decode("a[1]=c", DecodeOptions(list_limit=0)) == {"a": {1: "c"}}
+        assert decode("a[1]=c", DecodeOptions(list_limit=0)) == {"a": {"1": "c"}}
         assert decode("a[1]=c") == {"a": ["c"]}
 
     def test_limits_specific_list_indices_to_list_limit(self) -> None:
         assert decode("a[20]=a", DecodeOptions(list_limit=20)) == {"a": ["a"]}
-        assert decode("a[21]=a", DecodeOptions(list_limit=20)) == {"a": {21: "a"}}
+        assert decode("a[21]=a", DecodeOptions(list_limit=20)) == {"a": {"21": "a"}}
         assert decode("a[20]=a") == {"a": ["a"]}
-        assert decode("a[21]=a") == {"a": {21: "a"}}
+        assert decode("a[21]=a") == {"a": {"21": "a"}}
 
     def test_supports_keys_that_begin_with_a_number(self) -> None:
         assert decode("a[12b]=c") == {"a": {"12b": "c"}}
 
     def test_supports_encoded_equals_signs(self) -> None:
         assert decode("he%3Dllo=th%3Dere") == {"he=llo": "th=ere"}
 
@@ -213,19 +213,19 @@
         assert decode('operators=[">=", "<="]') == {"operators": '[">=", "<="]'}
 
     def test_allows_empty_values(self) -> None:
         assert decode("") == {}
         assert decode(None) == {}
 
     def test_transforms_lists_to_dicts(self) -> None:
-        assert decode("foo[0]=bar&foo[bad]=baz") == {"foo": {0: "bar", "bad": "baz"}}
-        assert decode("foo[bad]=baz&foo[0]=bar") == {"foo": {"bad": "baz", 0: "bar"}}
-        assert decode("foo[bad]=baz&foo[]=bar") == {"foo": {"bad": "baz", 0: "bar"}}
-        assert decode("foo[]=bar&foo[bad]=baz") == {"foo": {0: "bar", "bad": "baz"}}
-        assert decode("foo[bad]=baz&foo[]=bar&foo[]=foo") == {"foo": {"bad": "baz", 0: "bar", 1: "foo"}}
+        assert decode("foo[0]=bar&foo[bad]=baz") == {"foo": {"0": "bar", "bad": "baz"}}
+        assert decode("foo[bad]=baz&foo[0]=bar") == {"foo": {"bad": "baz", "0": "bar"}}
+        assert decode("foo[bad]=baz&foo[]=bar") == {"foo": {"bad": "baz", "0": "bar"}}
+        assert decode("foo[]=bar&foo[bad]=baz") == {"foo": {"0": "bar", "bad": "baz"}}
+        assert decode("foo[bad]=baz&foo[]=bar&foo[]=foo") == {"foo": {"bad": "baz", "0": "bar", "1": "foo"}}
         assert decode("foo[0][a]=a&foo[0][b]=b&foo[1][a]=aa&foo[1][b]=bb") == {
             "foo": [{"a": "a", "b": "b"}, {"a": "aa", "b": "bb"}]
         }
 
     def test_transforms_lists_to_dicts_dot_notation(self) -> None:
         assert decode("foo[0].baz=bar&fool.bad=baz", DecodeOptions(allow_dots=True)) == {
             "foo": [{"baz": "bar"}],
@@ -241,26 +241,26 @@
         }
         assert decode("foo[0].baz[0]=15&foo[0].bar=2", DecodeOptions(allow_dots=True)) == {
             "foo": [{"baz": ["15"], "bar": "2"}]
         }
         assert decode("foo[0].baz[0]=15&foo[0].baz[1]=16&foo[0].bar=2", DecodeOptions(allow_dots=True)) == {
             "foo": [{"baz": ["15", "16"], "bar": "2"}]
         }
-        assert decode("foo.bad=baz&foo[0]=bar", DecodeOptions(allow_dots=True)) == {"foo": {"bad": "baz", 0: "bar"}}
-        assert decode("foo.bad=baz&foo[]=bar", DecodeOptions(allow_dots=True)) == {"foo": {"bad": "baz", 0: "bar"}}
-        assert decode("foo[]=bar&foo.bad=baz", DecodeOptions(allow_dots=True)) == {"foo": {0: "bar", "bad": "baz"}}
+        assert decode("foo.bad=baz&foo[0]=bar", DecodeOptions(allow_dots=True)) == {"foo": {"bad": "baz", "0": "bar"}}
+        assert decode("foo.bad=baz&foo[]=bar", DecodeOptions(allow_dots=True)) == {"foo": {"bad": "baz", "0": "bar"}}
+        assert decode("foo[]=bar&foo.bad=baz", DecodeOptions(allow_dots=True)) == {"foo": {"0": "bar", "bad": "baz"}}
         assert decode("foo.bad=baz&foo[]=bar&foo[]=foo", DecodeOptions(allow_dots=True)) == {
-            "foo": {"bad": "baz", 0: "bar", 1: "foo"}
+            "foo": {"bad": "baz", "0": "bar", "1": "foo"}
         }
         assert decode("foo[0].a=a&foo[0].b=b&foo[1].a=aa&foo[1].b=bb", DecodeOptions(allow_dots=True)) == {
             "foo": [{"a": "a", "b": "b"}, {"a": "aa", "b": "bb"}]
         }
 
     def test_correctly_prunes_undefined_values_when_converting_a_list_to_a_dict(self) -> None:
-        assert decode("a[2]=b&a[99999999]=c") == {"a": {2: "b", 99999999: "c"}}
+        assert decode("a[2]=b&a[99999999]=c") == {"a": {"2": "b", "99999999": "c"}}
 
     def test_supports_malformed_uri_characters(self) -> None:
         assert decode("{%:%}", DecodeOptions(strict_null_handling=True)) == {"{%:%}": None}
         assert decode("{%:%}=") == {"{%:%}": ""}
         assert decode("foo=%:%}") == {"foo": "%:%}"}
 
     def test_does_not_produce_empty_keys(self) -> None:
@@ -303,16 +303,16 @@
     def test_parses_jquery_param_strings(self) -> None:
         assert decode(
             # readable: str = 'filter[0][]=int1&filter[0][]==&filter[0][]=77&filter[]=and&filter[2][]=int2&filter[2][]==&filter[2][]=8'
             "filter%5B0%5D%5B%5D=int1&filter%5B0%5D%5B%5D=%3D&filter%5B0%5D%5B%5D=77&filter%5B%5D=and&filter%5B2%5D%5B%5D=int2&filter%5B2%5D%5B%5D=%3D&filter%5B2%5D%5B%5D=8"
         ) == {"filter": [["int1", "=", "77"], "and", ["int2", "=", "8"]]}
 
     def test_continues_parsing_when_no_parent_is_found(self) -> None:
-        assert decode("[]=&a=b") == {0: "", "a": "b"}
-        assert decode("[]&a=b", DecodeOptions(strict_null_handling=True)) == {0: None, "a": "b"}
+        assert decode("[]=&a=b") == {"0": "", "a": "b"}
+        assert decode("[]&a=b", DecodeOptions(strict_null_handling=True)) == {"0": None, "a": "b"}
         assert decode("[foo]=bar") == {"foo": "bar"}
 
     def test_does_not_error_when_parsing_a_very_long_list(self) -> None:
         buf: str = "a[]=a"
         while getsizeof(buf) < 128 * 1024:
             buf += "&"
             buf += buf
@@ -329,24 +329,24 @@
     def test_allows_overriding_parameter_limit(self) -> None:
         assert decode("a=b&c=d", DecodeOptions(parameter_limit=1)) == {"a": "b"}
 
     def test_allows_setting_the_parameter_limit_to_infinity(self) -> None:
         assert decode("a=b&c=d", DecodeOptions(parameter_limit=float("inf"))) == {"a": "b", "c": "d"}
 
     def test_allows_overriding_list_limit(self) -> None:
-        assert decode("a[0]=b", DecodeOptions(list_limit=-1)) == {"a": {0: "b"}}
+        assert decode("a[0]=b", DecodeOptions(list_limit=-1)) == {"a": {"0": "b"}}
         assert decode("a[0]=b", DecodeOptions(list_limit=0)) == {"a": ["b"]}
-        assert decode("a[-1]=b", DecodeOptions(list_limit=-1)) == {"a": {-1: "b"}}
-        assert decode("a[-1]=b", DecodeOptions(list_limit=0)) == {"a": {-1: "b"}}
-        assert decode("a[0]=b&a[1]=c", DecodeOptions(list_limit=-1)) == {"a": {0: "b", 1: "c"}}
-        assert decode("a[0]=b&a[1]=c", DecodeOptions(list_limit=0)) == {"a": {0: "b", 1: "c"}}
+        assert decode("a[-1]=b", DecodeOptions(list_limit=-1)) == {"a": {"-1": "b"}}
+        assert decode("a[-1]=b", DecodeOptions(list_limit=0)) == {"a": {"-1": "b"}}
+        assert decode("a[0]=b&a[1]=c", DecodeOptions(list_limit=-1)) == {"a": {"0": "b", "1": "c"}}
+        assert decode("a[0]=b&a[1]=c", DecodeOptions(list_limit=0)) == {"a": {"0": "b", "1": "c"}}
 
     def test_allows_disabling_list_parsing(self) -> None:
-        assert decode("a[0]=b&a[1]=c", DecodeOptions(parse_lists=False)) == {"a": {0: "b", 1: "c"}}
-        assert decode("a[]=b", DecodeOptions(parse_lists=False)) == {"a": {0: "b"}}
+        assert decode("a[0]=b&a[1]=c", DecodeOptions(parse_lists=False)) == {"a": {"0": "b", "1": "c"}}
+        assert decode("a[]=b", DecodeOptions(parse_lists=False)) == {"a": {"0": "b"}}
 
     def test_allows_for_query_string_prefix(self) -> None:
         assert decode("?foo=bar", DecodeOptions(ignore_query_prefix=True)) == {"foo": "bar"}
         assert decode("foo=bar", DecodeOptions(ignore_query_prefix=True)) == {"foo": "bar"}
         assert decode("?foo=bar", DecodeOptions(ignore_query_prefix=False)) == {"?foo": "bar"}
 
     def test_parses_a_dict(self) -> None:
@@ -482,15 +482,15 @@
         expected["a"]["hasOwnProperty"] = "d"
         assert decode("a[b]=c&a[hasOwnProperty]=d") == expected
 
         assert decode(None) == {}
 
         expected_list: t.Dict[str, t.Any] = {}
         expected_list["a"] = {}
-        expected_list["a"][0] = "b"
+        expected_list["a"]["0"] = "b"
         expected_list["a"]["c"] = "d"
         assert decode("a[]=b&a[c]=d") == expected_list
 
     def test_can_parse_with_custom_encoding(self) -> None:
         def _decode(s: t.Optional[str], charset: t.Optional[Charset]) -> t.Any:
             if s is None:
                 return None
@@ -529,18 +529,18 @@
             ("=a&=b", {}),
             ("=a&foo=b", {"foo": "b"}),
             ("a[]=b&a=c&=", {"a": ["b", "c"]}),
             ("a[]=b&a=c&=", {"a": ["b", "c"]}),
             ("a[0]=b&a=c&=", {"a": ["b", "c"]}),
             ("a=b&a[]=c&=", {"a": ["b", "c"]}),
             ("a=b&a[0]=c&=", {"a": ["b", "c"]}),
-            ("[]=a&[]=b& []=1", {0: "a", 1: "b", " ": ["1"]}),
-            ("[0]=a&[1]=b&a[0]=1&a[1]=2", {0: "a", 1: "b", "a": ["1", "2"]}),
+            ("[]=a&[]=b& []=1", {"0": "a", "1": "b", " ": ["1"]}),
+            ("[0]=a&[1]=b&a[0]=1&a[1]=2", {"0": "a", "1": "b", "a": ["1", "2"]}),
             ("[deep]=a&[deep]=2", {"deep": ["a", "2"]}),
-            ("%5B0%5D=a&%5B1%5D=b", {0: "a", 1: "b"}),
+            ("%5B0%5D=a&%5B1%5D=b", {"0": "a", "1": "b"}),
         ],
     )
     def test_parses_empty_keys(self, encoded: str, decoded: t.Mapping) -> None:
         assert decode(encoded) == decoded
 
 
 class TestCharset:
```

### Comparing `qs_codec-0.2.1/tests/unit/encode_test.py` & `qs_codec-0.2.2/tests/unit/encode_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -817,14 +817,26 @@
             == "utf8=%E2%9C%93&a=%C3%A6"
         )
         assert (
             encode({"a": "æ"}, options=EncodeOptions(charset_sentinel=True, charset=Charset.LATIN1))
             == "utf8=%26%2310003%3B&a=%E6"
         )
 
+    def test_strict_null_handling_works_with_null_serialize_date(self) -> None:
+        assert (
+            encode(
+                {"key": datetime.now()},
+                options=EncodeOptions(
+                    strict_null_handling=True,
+                    serialize_date=lambda _: None,
+                ),
+            )
+            == "key"
+        )
+
     def test_does_not_mutate_the_options_argument(self) -> None:
         options = EncodeOptions()
         encode({}, options)
         assert options == EncodeOptions()
 
     def test_strict_null_handling_works_with_custom_filter(self) -> None:
         options = EncodeOptions(strict_null_handling=True, filter=lambda prefix, value: value)
```

### Comparing `qs_codec-0.2.1/tests/unit/example_test.py` & `qs_codec-0.2.2/tests/unit/example_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,24 +126,24 @@
         assert qs_codec.decode("a[]=&a[]=b") == {"a": ["", "b"]}
         assert qs_codec.decode("a[0]=b&a[1]=&a[2]=c") == {"a": ["b", "", "c"]}
 
         # **qs_codec** will also limit specifying indices in a `list` to a maximum index of `20`.
         # Any `list` members with an index of greater than `20` will instead be converted to a `dict` with the index as
         # the key. This is needed to handle cases when someone sent, for example, `a[999999999]` and it will take
         # significant time to iterate over this huge `list`.
-        assert qs_codec.decode("a[100]=b") == {"a": {100: "b"}}
+        assert qs_codec.decode("a[100]=b") == {"a": {"100": "b"}}
 
         # This limit can be overridden by passing an `DecodeOptions.list_limit` option:
-        assert qs_codec.decode("a[1]=b", qs_codec.DecodeOptions(list_limit=0)) == {"a": {1: "b"}}
+        assert qs_codec.decode("a[1]=b", qs_codec.DecodeOptions(list_limit=0)) == {"a": {"1": "b"}}
 
         # To disable List parsing entirely, set `DecodeOptions.parse_lists` to `False`.
-        assert qs_codec.decode("a[]=b", qs_codec.DecodeOptions(parse_lists=False)) == {"a": {0: "b"}}
+        assert qs_codec.decode("a[]=b", qs_codec.DecodeOptions(parse_lists=False)) == {"a": {"0": "b"}}
 
         # If you mix notations, **qs_codec** will merge the two items into a `dict`:
-        assert qs_codec.decode("a[0]=b&a[b]=c") == {"a": {0: "b", "b": "c"}}
+        assert qs_codec.decode("a[0]=b&a[b]=c") == {"a": {"0": "b", "b": "c"}}
 
         # You can also create `list`s of `dict`s:
         # (**qs_codec** cannot convert nested `dict`s, such as `'a={b:1},{c:d}'`)
         assert qs_codec.decode("a[][b]=c") == {"a": [{"b": "c"}]}
 
     def test_primitive_or_scalar_values(self):
         # By default, all values are parsed as `str`s.
```

### Comparing `qs_codec-0.2.1/tests/unit/utils_test.py` & `qs_codec-0.2.2/tests/unit/utils_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,15 +417,15 @@
             ),
         ],
     )
     def test_unescape(self, escaped: str, unescaped: str) -> None:
         assert DecodeUtils.unescape(escaped) == unescaped
 
     def test_merges_dict_with_list(self) -> None:
-        assert Utils.merge({0: "a"}, [Undefined(), "b"]) == {0: "a", 1: "b"}
+        assert Utils.merge({"0": "a"}, [Undefined(), "b"]) == {"0": "a", "1": "b"}
 
     def test_merges_two_dicts_with_the_same_key_and_different_values(self) -> None:
         assert Utils.merge({"foo": [{"a": "a", "b": "b"}, {"a": "aa"}]}, {"foo": [Undefined(), {"b": "bb"}]}) == {
             "foo": [{"a": "a", "b": "b"}, {"a": "aa", "b": "bb"}]
         }
 
     def test_merges_two_dicts_with_the_same_key_and_different_list_values(self) -> None:
@@ -446,33 +446,33 @@
         assert Utils.merge({"a": "b"}, {"a": "c"}) == {"a": ["b", "c"]}
 
     def test_merges_standalone_and_object_into_array(self) -> None:
         assert Utils.merge({"foo": "bar"}, {"foo": {"first": "123"}}) == {"foo": ["bar", {"first": "123"}]}
 
     def test_merges_standalone_and_two_objects_into_array(self) -> None:
         assert Utils.merge({"foo": ["bar", {"first": "123"}]}, {"foo": {"second": "456"}}) == {
-            "foo": {0: "bar", 1: {"first": "123"}, "second": "456"}
+            "foo": {"0": "bar", "1": {"first": "123"}, "second": "456"}
         }
 
     def test_merges_object_sandwiched_by_two_standalones_into_array(self) -> None:
         assert Utils.merge({"foo": ["bar", {"first": "123", "second": "456"}]}, {"foo": "baz"}) == {
             "foo": ["bar", {"first": "123", "second": "456"}, "baz"]
         }
 
     def test_merges_two_arrays_into_an_array(self) -> None:
         assert Utils.merge({"foo": ["baz"]}, {"foo": ["bar", "xyzzy"]}) == {"foo": ["baz", "bar", "xyzzy"]}
 
     def test_merges_object_into_array(self) -> None:
-        assert Utils.merge({"foo": ["bar"]}, {"foo": {"baz": "xyzzy"}}) == {"foo": {0: "bar", "baz": "xyzzy"}}
+        assert Utils.merge({"foo": ["bar"]}, {"foo": {"baz": "xyzzy"}}) == {"foo": {"0": "bar", "baz": "xyzzy"}}
 
     def test_merges_array_into_object(self) -> None:
         assert Utils.merge(
             {"foo": {"bar": "baz"}},
             {"foo": ["xyzzy"]},
-        ) == {"foo": {"bar": "baz", 0: "xyzzy"}}
+        ) == {"foo": {"bar": "baz", "0": "xyzzy"}}
 
     def test_combine_both_arrays(self) -> None:
         a = [1]
         b = [2]
         combined = Utils.combine(a, b)
 
         assert a == [1]
```

### Comparing `qs_codec-0.2.1/tests/unit/weakref_test.py` & `qs_codec-0.2.2/tests/unit/weakref_test.py`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/.gitignore` & `qs_codec-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/LICENSE` & `qs_codec-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/README.rst` & `qs_codec-0.2.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 .. code:: python
 
    import qs_codec, typing as t
 
    def decode(
        value: t.Optional[t.Union[str, t.Mapping]],
        options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
-   ) -> dict:
+   ) -> t.Dict[str, t.Any]:
        """Decodes a str or Mapping into a Dict. 
        
        Providing custom DecodeOptions will override the default behavior."""
        pass
 
 `decode <https://techouse.github.io/qs_codec/qs_codec.html#module-qs_codec.decode>`__ allows you to create nested ``dict``\ s within your query
 strings, by surrounding the name of sub-keys with square brackets
@@ -324,47 +324,47 @@
 for example, ``a[999999999]`` and it will take significant time to iterate
 over this huge ``list``.
 
 .. code:: python
 
    import qs_codec
 
-   assert qs_codec.decode('a[100]=b') == {'a': {100: 'b'}}
+   assert qs_codec.decode('a[100]=b') == {'a': {'100': 'b'}}
 
 This limit can be overridden by passing an `list_limit <https://techouse.github.io/qs_codec/qs_codec.models.html#qs_codec.models.decode_options.DecodeOptions.list_limit>`__
 option:
 
 .. code:: python
 
    import qs_codec
 
    assert qs_codec.decode(
        'a[1]=b',
        qs_codec.DecodeOptions(list_limit=0),
-   ) == {'a': {1: 'b'}}
+   ) == {'a': {'1': 'b'}}
 
 To disable ``list`` parsing entirely, set `parse_lists <https://techouse.github.io/qs_codec/qs_codec.models.html#qs_codec.models.decode_options.DecodeOptions.parse_lists>`__
 to ``False``.
 
 .. code:: python
 
    import qs_codec
 
    assert qs_codec.decode(
        'a[]=b',
        qs_codec.DecodeOptions(parse_lists=False),
-   ) == {'a': {0: 'b'}}
+   ) == {'a': {'0': 'b'}}
 
 If you mix notations, `decode <https://techouse.github.io/qs_codec/qs_codec.models.html#qs_codec.decode>`__ will merge the two items into a ``dict``:
 
 .. code:: python
 
    import qs_codec
 
-   assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {0: 'b', 'b': 'c'}}
+   assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {'0': 'b', 'b': 'c'}}
 
 You can also create ``list``\ s of ``dict``\ s:
 
 .. code:: python
 
    import qs_codec
```

### Comparing `qs_codec-0.2.1/pyproject.toml` & `qs_codec-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qs_codec-0.2.1/PKG-INFO` & `qs_codec-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qs-codec
-Version: 0.2.1
+Version: 0.2.2
 Summary: A query string encoding and decoding library for Python. Ported from qs for JavaScript.
 Project-URL: Homepage, https://techouse.github.io/qs_codec/
 Project-URL: Documentation, https://techouse.github.io/qs_codec/
 Project-URL: Source, https://github.com/techouse/qs_codec
 Project-URL: Changelog, https://github.com/techouse/qs_codec/blob/master/CHANGELOG.md
 Project-URL: Sponsor, https://github.com/sponsors/techouse
 Project-URL: PayPal, https://paypal.me/ktusar
@@ -68,15 +68,15 @@
 .. code:: python
 
    import qs_codec, typing as t
 
    def decode(
        value: t.Optional[t.Union[str, t.Mapping]],
        options: qs_codec.DecodeOptions = qs_codec.DecodeOptions(),
-   ) -> dict:
+   ) -> t.Dict[str, t.Any]:
        """Decodes a str or Mapping into a Dict. 
        
        Providing custom DecodeOptions will override the default behavior."""
        pass
 
 `decode <https://techouse.github.io/qs_codec/qs_codec.html#module-qs_codec.decode>`__ allows you to create nested ``dict``\ s within your query
 strings, by surrounding the name of sub-keys with square brackets
@@ -359,47 +359,47 @@
 for example, ``a[999999999]`` and it will take significant time to iterate
 over this huge ``list``.
 
 .. code:: python
 
    import qs_codec
 
-   assert qs_codec.decode('a[100]=b') == {'a': {100: 'b'}}
+   assert qs_codec.decode('a[100]=b') == {'a': {'100': 'b'}}
 
 This limit can be overridden by passing an `list_limit <https://techouse.github.io/qs_codec/qs_codec.models.html#qs_codec.models.decode_options.DecodeOptions.list_limit>`__
 option:
 
 .. code:: python
 
    import qs_codec
 
    assert qs_codec.decode(
        'a[1]=b',
        qs_codec.DecodeOptions(list_limit=0),
-   ) == {'a': {1: 'b'}}
+   ) == {'a': {'1': 'b'}}
 
 To disable ``list`` parsing entirely, set `parse_lists <https://techouse.github.io/qs_codec/qs_codec.models.html#qs_codec.models.decode_options.DecodeOptions.parse_lists>`__
 to ``False``.
 
 .. code:: python
 
    import qs_codec
 
    assert qs_codec.decode(
        'a[]=b',
        qs_codec.DecodeOptions(parse_lists=False),
-   ) == {'a': {0: 'b'}}
+   ) == {'a': {'0': 'b'}}
 
 If you mix notations, `decode <https://techouse.github.io/qs_codec/qs_codec.models.html#qs_codec.decode>`__ will merge the two items into a ``dict``:
 
 .. code:: python
 
    import qs_codec
 
-   assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {0: 'b', 'b': 'c'}}
+   assert qs_codec.decode('a[0]=b&a[b]=c') == {'a': {'0': 'b', 'b': 'c'}}
 
 You can also create ``list``\ s of ``dict``\ s:
 
 .. code:: python
 
    import qs_codec
```

