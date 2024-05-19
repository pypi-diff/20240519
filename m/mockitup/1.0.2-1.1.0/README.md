# Comparing `tmp/mockitup-1.0.2.tar.gz` & `tmp/mockitup-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockitup-1.0.2.tar", last modified: Fri Jun 16 05:37:10 2023, max compression
+gzip compressed data, was "mockitup-1.1.0.tar", last modified: Sun May 19 07:15:52 2024, max compression
```

## Comparing `mockitup-1.0.2.tar` & `mockitup-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 05:36:53.000000 mockitup-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-06-16 05:37:10.242501 mockitup-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-16 05:36:53.000000 mockitup-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-16 05:36:53.000000 mockitup-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:37:10.242501 mockitup-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/src/mockitup/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/arguments_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/src/mockitup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 05:36:53.000000 mockitup-1.0.2/tests/test_async_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-16 05:36:53.000000 mockitup-1.0.2/tests/test_composer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:15:52.395047 mockitup-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-19 07:15:40.000000 mockitup-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-19 07:15:52.395047 mockitup-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-19 07:15:40.000000 mockitup-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-19 07:15:40.000000 mockitup-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:15:52.395047 mockitup-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:15:52.395047 mockitup-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:15:52.395047 mockitup-1.1.0/src/mockitup/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-19 07:15:40.000000 mockitup-1.1.0/src/mockitup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-19 07:15:40.000000 mockitup-1.1.0/src/mockitup/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-19 07:15:40.000000 mockitup-1.1.0/src/mockitup/arguments_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7364 2024-05-19 07:15:40.000000 mockitup-1.1.0/src/mockitup/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-19 07:15:40.000000 mockitup-1.1.0/src/mockitup/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:15:52.395047 mockitup-1.1.0/src/mockitup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-19 07:15:52.000000 mockitup-1.1.0/src/mockitup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 07:15:52.000000 mockitup-1.1.0/src/mockitup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:15:52.000000 mockitup-1.1.0/src/mockitup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-19 07:15:52.000000 mockitup-1.1.0/src/mockitup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 07:15:52.000000 mockitup-1.1.0/src/mockitup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:15:52.395047 mockitup-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 07:15:40.000000 mockitup-1.1.0/tests/test_async_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-19 07:15:40.000000 mockitup-1.1.0/tests/test_composer.py
```

### Comparing `mockitup-1.0.2/LICENSE` & `mockitup-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.2/PKG-INFO` & `mockitup-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockitup
-Version: 1.0.2
+Version: 1.1.0
 Summary: A `unittest.mock` wrapper for easier mocking
 Author-email: Shacham Ginat <shacham6@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Shacham Ginat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,21 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Requires-Python: <4.0,>=3.8
+Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyHamcrest>=2.0.2
+Requires-Dist: typing-extensions>=3.10.0
+Requires-Dist: PyHamcrest>=2.0.2
+Requires-Dist: typing-extensions>=3.10.0
 
 ![Logo](imgs/logo.svg)
 
 `mockitup` is a small package that provides a DSL for quickly configuring mock behaviors.
 
 <!-- You can read more in our [documentation](https://shacham6.github.io/mockitup/) website. -->
```

### Comparing `mockitup-1.0.2/README.md` & `mockitup-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.2/pyproject.toml` & `mockitup-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 authors = [
     {name = "Shacham Ginat", email = "shacham6@gmail.com"},
 ]
-requires-python = ">=3.8,<4.0"
+requires-python = ">=3.8.1,<4.0"
 dependencies = [
     "PyHamcrest>=2.0.2",
     "typing-extensions>=3.10.0",
     "PyHamcrest>=2.0.2",
     "typing-extensions>=3.10.0",
 ]
 name = "mockitup"
-version = "1.0.2"
+version = "1.1.0"
 description = "A `unittest.mock` wrapper for easier mocking"
 
 license = { file = "LICENSE" }
 readme = "README.md"
 
 [tool.pdm]
 [tool.pdm.dev-dependencies]
```

### Comparing `mockitup-1.0.2/src/mockitup/actions.py` & `mockitup-1.1.0/src/mockitup/actions.py`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.2/src/mockitup/arguments_matcher.py` & `mockitup-1.1.0/src/mockitup/arguments_matcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,35 +18,35 @@
         registered_len = len(self.args) + len(self.kwargs)
         provided_len = len(args) + len(kwargs)
         if registered_len == provided_len == 0:
             return True, "Arguments matched"
 
         # Lengths don't have to match in case of `ANY_ARGS` wildcard.
         if self.args[0] is ANY_ARGS:
-            return True, "Matched wildcard `ANY_ARGS`"
+            return True, "Matched wildcard 'ANY_ARGS'"
 
         if registered_len != provided_len:
             return False, "Length of provided positional arguments isn't the same as the registered"
 
         for index, (registered, provided) in enumerate(zip(self.args, args)):
             matched = self.__match_values(registered, provided)
             if not matched:
                 return False, (f"Positional arguments at index {index} didn't match "
-                               f"(registered: `{registered}`, provided: `{provided}`)")
+                               f"(registered: '{registered}', provided: '{provided}')")
 
         # Should have same keys
         if set(self.kwargs) != set(kwargs):
             return False, "Length of provided named arguments isn't the same as the registered"
 
         for key in self.kwargs:
             registered = self.kwargs[key]
             provided = kwargs[key]
             if not self.__match_values(registered, provided):
-                return False, (f"Named arguments at key `{key}` didn't match "
-                               f"(registered: `{registered}`, provided: `{provided}`)")
+                return False, (f"Named arguments at key '{key}' didn't match "
+                               f"(registered: '{registered}', provided: '{provided}')")
         return True, "Arguments matched"
 
     @staticmethod
     def __match_values(registered_value: Any, provided_value: Any) -> bool:
         if registered_value is ANY_ARG:
             return True
```

### Comparing `mockitup-1.0.2/src/mockitup/composer.py` & `mockitup-1.1.0/src/mockitup/composer.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         def was_met(self) -> bool:
             return bool(self.__match_results)
 
         def assert_met(self) -> None:
             if not self.__match_results:
                 mock_name = self.__mock._extract_mock_name()
                 args, kwargs = self.__args
-                message = (f"Expected mock `{mock_name}` to be called with "
+                message = (f"Expected mock '{mock_name}' to be called with "
                            f"(args: '{args}', kwargs: '{kwargs}'), but wasn't")
                 raise ExpectationNotFulfilled(
                     message,
                     mock=self.__mock,
                     expected_arguments=self.__args,
                 )
```

### Comparing `mockitup-1.0.2/src/mockitup/proxies.py` & `mockitup-1.1.0/src/mockitup/proxies.py`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.2/src/mockitup.egg-info/PKG-INFO` & `mockitup-1.1.0/src/mockitup.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockitup
-Version: 1.0.2
+Version: 1.1.0
 Summary: A `unittest.mock` wrapper for easier mocking
 Author-email: Shacham Ginat <shacham6@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Shacham Ginat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,17 +21,21 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Requires-Python: <4.0,>=3.8
+Requires-Python: <4.0,>=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: PyHamcrest>=2.0.2
+Requires-Dist: typing-extensions>=3.10.0
+Requires-Dist: PyHamcrest>=2.0.2
+Requires-Dist: typing-extensions>=3.10.0
 
 ![Logo](imgs/logo.svg)
 
 `mockitup` is a small package that provides a DSL for quickly configuring mock behaviors.
 
 <!-- You can read more in our [documentation](https://shacham6.github.io/mockitup/) website. -->
```

### Comparing `mockitup-1.0.2/tests/test_async_mocks.py` & `mockitup-1.1.0/tests/test_async_mocks.py`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.2/tests/test_composer.py` & `mockitup-1.1.0/tests/test_composer.py`

 * *Files identical despite different names*

