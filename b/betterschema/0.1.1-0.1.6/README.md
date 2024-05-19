# Comparing `tmp/betterschema-0.1.1.tar.gz` & `tmp/betterschema-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterschema-0.1.1.tar", last modified: Sat May 18 05:49:03 2024, max compression
+gzip compressed data, was "betterschema-0.1.6.tar", last modified: Sun May 19 18:44:05 2024, max compression
```

## Comparing `betterschema-0.1.1.tar` & `betterschema-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.561232 betterschema-0.1.1/
--rw-r--r--   0 bytedance   (501) staff       (20)      383 2024-05-18 05:49:03.560464 betterschema-0.1.1/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     2321 2024-05-18 05:27:17.000000 betterschema-0.1.1/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.544429 betterschema-0.1.1/baselib/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.550811 betterschema-0.1.1/baselib/src/
--rw-r--r--   0 bytedance   (501) staff       (20)     7321 2024-05-14 21:47:08.000000 betterschema-0.1.1/baselib/src/attr.c
--rw-r--r--   0 bytedance   (501) staff       (20)     2897 2024-05-14 20:26:09.000000 betterschema-0.1.1/baselib/src/init.c
--rw-r--r--   0 bytedance   (501) staff       (20)     1031 2024-05-18 05:27:17.000000 betterschema-0.1.1/baselib/src/module.c
--rw-r--r--   0 bytedance   (501) staff       (20)     9067 2024-05-17 00:35:11.000000 betterschema-0.1.1/baselib/src/schema.c
--rw-r--r--   0 bytedance   (501) staff       (20)    11228 2024-05-14 20:26:09.000000 betterschema-0.1.1/baselib/src/utils.c
--rw-r--r--   0 bytedance   (501) staff       (20)     5663 2024-05-13 04:14:11.000000 betterschema-0.1.1/baselib/src/watch.c
--rw-r--r--   0 bytedance   (501) staff       (20)      107 2024-04-25 00:31:56.000000 betterschema-0.1.1/pyproject.toml
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-05-18 05:49:03.561299 betterschema-0.1.1/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1125 2024-05-18 05:48:39.000000 betterschema-0.1.1/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.545459 betterschema-0.1.1/src/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.552185 betterschema-0.1.1/src/betterschema/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-18 05:01:41.000000 betterschema-0.1.1/src/betterschema/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1608 2024-05-18 05:27:17.000000 betterschema-0.1.1/src/betterschema/core.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.556620 betterschema-0.1.1/src/betterschema/old/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-18 05:01:41.000000 betterschema-0.1.1/src/betterschema/old/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5714 2024-05-18 05:27:17.000000 betterschema-0.1.1/src/betterschema/old/schema.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1240 2024-05-18 05:27:17.000000 betterschema-0.1.1/src/betterschema/render.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.559515 betterschema-0.1.1/src/betterschema.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      383 2024-05-18 05:49:03.000000 betterschema-0.1.1/src/betterschema.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      554 2024-05-18 05:49:03.000000 betterschema-0.1.1/src/betterschema.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-05-18 05:49:03.000000 betterschema-0.1.1/src/betterschema.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       35 2024-05-18 05:49:03.000000 betterschema-0.1.1/src/betterschema.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       13 2024-05-18 05:49:03.000000 betterschema-0.1.1/src/betterschema.egg-info/top_level.txt
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-18 05:49:03.558565 betterschema-0.1.1/tests/
--rw-r--r--   0 bytedance   (501) staff       (20)     1319 2024-05-18 05:27:17.000000 betterschema-0.1.1/tests/testlib.py
--rw-r--r--   0 bytedance   (501) staff       (20)      829 2024-05-18 05:27:17.000000 betterschema-0.1.1/tests/testrender.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4158 2024-05-18 05:27:17.000000 betterschema-0.1.1/tests/testschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 18:44:05.241039 betterschema-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-05-19 18:43:57.000000 betterschema-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.237038 betterschema-0.1.6/baselib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/baselib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/attr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/init.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/schema.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 18:43:57.000000 betterschema-0.1.6/baselib/src/watch.c
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-19 18:43:57.000000 betterschema-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:44:05.241039 betterschema-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-19 18:43:57.000000 betterschema-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.237038 betterschema-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/src/betterschema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:43:57.000000 betterschema-0.1.6/src/betterschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-19 18:43:57.000000 betterschema-0.1.6/src/betterschema/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-19 18:43:57.000000 betterschema-0.1.6/src/betterschema/render.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/src/betterschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 18:44:05.000000 betterschema-0.1.6/src/betterschema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:44:05.241039 betterschema-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-19 18:43:57.000000 betterschema-0.1.6/tests/testlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-19 18:43:57.000000 betterschema-0.1.6/tests/testrender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-19 18:43:57.000000 betterschema-0.1.6/tests/testschema.py
```

### Comparing `betterschema-0.1.1/README.md` & `betterschema-0.1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -18,41 +18,44 @@
 
 ```sh
 pip install betterschema
 ```
 
 ## Usage
 
-Here's a simple example of how to use betterschema:
+### Defining Schemas
+
+To define a schema, you can use the `@core.schema` decorator on a class definition. Inside the class, you can define the attributes of the schema using type hints. You can also define nested schemas within the main schema class.
 
 ```python
 import betterschema.core as core
 
 @core.schema
 class Foo:
-    foo1: str
-    foo2: int
-    foo3: bool
-    foo4: list[str]
-    foo5: core.optional[int]
-    foo6: dict[str, int]
+    foo1: str # String field
+    foo2: int # Integer field
+    foo3: bool # Boolean field
+    foo4: list[str] # List of strings
+    foo5: core.optional[int] # Optional field
+    foo6: dict[str, int] # Dictionary field
 
     @core.schema
     class EmbeddedSchema:
         bar1: str
         bar2: int
         bar3: bool
 
-    bar: EmbeddedSchema
+    bar: EmbeddedSchema # Nested schema field
+```
 
-@core.watch((Foo, "foo1"), (Foo, "foo2"))
-def watch_values(inst, name: str, old, new):
-    print(f"watch_values: {inst}.{name}, {old} -> {new}")
-    if name == "foo1" and new == "hi":
-        raise ValueError("foo1 cannot be 'hi'")
+### Creating Instances
+
+You can create instances of the schema by passing a dictionary with the required fields to the schema class constructor. The data will be validated against the schema automatically.
+
+```python
 
 # Creating an instance of the schema
 foo = Foo({
     "foo1": "hello",
     "foo2": 0,
     "foo3": True,
     "foo4": ["a", "b", "c"],
@@ -60,34 +63,78 @@
     "bar": Foo.EmbeddedSchema({
         "bar1": "world",
         "bar2": 20,
         "bar3": False,
     })
 })
 
+# For nested schemas, you can also give a dictionary directly
+foo = Foo({
+    "foo1": "hello",
+    "foo2": 0,
+    "foo3": True,
+    "foo4": ["a", "b", "c"],
+    "foo6": {"a": 1, "b": 2},
+    "bar": {
+        "bar1": "world",
+        "bar2": 20,
+        "bar3": False,
+    }
+})
+
+```
+
+### Updating Values
+
+You can update the values of the schema attributes directly. The data will be validated on each update.
+
+```python
+
 # Updating values
 foo.foo1 = "hello2"
 foo.foo2 = 1
-foo.foo3 = True
 
-# Checking values
-assert foo.foo1 == "hello2"
-assert foo.foo2 == 1
-assert foo.foo3 == True
+# if you try to set an invalid value, it will raise an exception
+foo.foo1 = 1  # This will raise a TypeError
+
+# you can also specify a dictionary to update multiple values at once
+# in order to do this, you need to use the `<<` operator
+foo << {
+    "foo1": "hello3",
+    "foo2": 2,
+}
+
+# for nested schemas, you can update the whole schema at once 
+foo.bar = {
+    "bar1": "world2",
+    "bar2": 30,
+    "bar3": True,
+}
+
+# or use the `<<` operator to do partial updates
+
+foo.bar << {
+    "bar1": "world3",
+    "bar2": 40,
+}
 
-# Watching values
-foo.foo1 = "hi"  # This will raise a ValueError
 ```
 
-## Running Tests
+### Watching Values
 
-You can run the included unit tests to ensure everything is working correctly:
+You can define watchers to monitor changes to specific attributes of the schema. Watchers are defined using the `@core.watch` decorator, which takes a tuple of the form `(schema_class, attribute_name)` as an argument.
+
+```python
+
+@core.watch((Foo, "foo1"), (Foo, "foo2"))
+def watch_values(inst, name: str, old, new):
+    print(f"watch_values: {inst}.{name}, {old} -> {new}")
+    if name == "foo1" and new == "hi":
+        raise ValueError("foo1 cannot be 'hi'")
 
-```sh
-python -m unittest discover
 ```
 
 ## Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.
 
 ## License
```

### Comparing `betterschema-0.1.1/baselib/src/attr.c` & `betterschema-0.1.6/baselib/src/attr.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.1/baselib/src/init.c` & `betterschema-0.1.6/baselib/src/init.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.1/baselib/src/module.c` & `betterschema-0.1.6/baselib/src/module.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.1/baselib/src/schema.c` & `betterschema-0.1.6/baselib/src/schema.c`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
   const char *obj_name = PyObject_GetNameStr(obj);
   if (obj_name == NULL) {
     PyErr_SetString(PyExc_AttributeError, "__name__ not found");
     err = 1;
     goto out;
   }
   strncpy(class_name, obj_name, CLASS_NAME_MAX_LEN);
+  class_name[CLASS_NAME_MAX_LEN - 1] = '\0';
   if (strlen(class_name) == 0) {
     PyErr_SetString(PyExc_AttributeError, "__name__ not found");
     err = 1;
     goto out;
   }
 
   sprintf(cls_def_buf, "class %s: pass", class_name);
@@ -205,15 +206,15 @@
   // change setattr and getattr to PySchema_ClassDefSetAttr and
   // PySchema_ClassDefGetAttr
   class_type->tp_setattro = PySchema_ClassDefSetAttr;
   class_type->tp_getattro = PySchema_ClassDefGetAttr;
   class_type->tp_init = PySchema_ClassInit;
   class_type->tp_as_number = &PySchema_NumberMethods;
 
-  if (PySchema_SetAnnotations(class, annotations) < 0) {
+  if (PySchema_SetAnnotations(class, annotations) == NULL) {
     PyErr_SetString(PyExc_RuntimeError, "Failed to set annotations");
     err = 1;
     goto out;
   }
 
   // if any of the values in annotation is also set in the class, then
   // set the value to the class
```

### Comparing `betterschema-0.1.1/baselib/src/utils.c` & `betterschema-0.1.6/baselib/src/utils.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 #include "utils.h"
 #include "schema.h"
 
 // Get the current thread frame global and local
 int PySys_GetGlobalLocal(PyObject **pGlobal, PyObject **pLocal) {
-  // Get the current frame
-  PyFrameObject *currentFrame = PyEval_GetFrame();
-  if (currentFrame == NULL) {
-    PyErr_SetString(PyExc_RuntimeError, "Failed to get the current frame");
-    return 0;
-  }
-
   // Access the global and local dictionaries
-  *pGlobal = PyFrame_GetGlobals(currentFrame);
-  *pLocal = PyFrame_GetLocals(currentFrame);
+  *pGlobal = PyEval_GetGlobals();
+  *pLocal = PyEval_GetLocals();
   if (*pGlobal == NULL || *pLocal == NULL) {
     PyErr_SetString(PyExc_RuntimeError,
                     "Failed to get the global and local dictionaries");
     return 0;
   }
   return 1;
 }
```

### Comparing `betterschema-0.1.1/baselib/src/watch.c` & `betterschema-0.1.6/baselib/src/watch.c`

 * *Files identical despite different names*

### Comparing `betterschema-0.1.1/setup.py` & `betterschema-0.1.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,64 @@
-from setuptools import setup, find_packages, Extension
+"""Setup script for the betterschema package."""
+
 import os
+import sys
 
+from setuptools import Extension, find_packages, setup
 
 module = Extension(
     "betterschema.baselib",
     # all c files in the lib/src directory
     sources=[
         os.path.join("baselib", "src", f)
         for f in os.listdir("baselib/src")
         if f.endswith(".c")
     ],
     include_dirs=["baselib/include"],
-    extra_compile_args=["-O3", "-Wall", "-Wextra", "-Werror", "-std=c11"],
-    extra_link_args=["-O3", "-Wall", "-Wextra", "-Werror", "-std=c11"],
+    extra_compile_args=["-O3", "-Wall", "-Werror", "-std=c11"],
+    extra_link_args=["-O3", "-Wall", "-Werror", "-std=c11"],
 )
 
+# Add compiler-specific options
+if sys.platform == "win32":
+    module.extra_compile_args = ["/W4"]
+else:
+    module.extra_compile_args = ["-Wextra"]
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
 
 setup(
     name="betterschema",
-    version="0.1.1",
+    version="0.1.6",
     author="Wilson Wang",
     project_urls={
-        'Source': 'https://github.com/wilsonwang371/betterschema',
+        "Source": "https://github.com/wilsonwang371/betterschema",
     },
     author_email="wilsonny371@gmail.com",
-    description="A library for schema support in Python",
+    description="A Python schema library that supports type checking and validation",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=["tests"]),
     setup_requires=[
         "build",
     ],
     install_requires=[
-        "pyyaml",
+        "PyYAML",
     ],
     extras_require={
         "dev": [
             "unittest",
             "black",
             "build",
+            "isort",
+            "pylint",
         ]
     },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+    ],
     # only include from source directory
     package_dir={"": "src"},
     ext_modules=[module],
 )
```

### Comparing `betterschema-0.1.1/src/betterschema/core.py` & `betterschema-0.1.6/src/betterschema/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+""" core module """
+
+# pylint: disable=E0401, E0611
 import logging
-import betterschema.baselib as baselib
 from typing import Optional
 
+from betterschema.baselib import __schemas__, __watches__
+from betterschema.baselib import schema as baseschema
+from betterschema.baselib import watch as basewatch
+
 logger = logging.getLogger(__name__)
 
 
 optional = Optional
-__watches__ = baselib.__watches__
-__schemas__ = baselib.__schemas__
 
 
 def is_schema_instance(schema_instance):
+    """Check if the schema instance is a schema instance."""
     if type(schema_instance).__name__ not in __schemas__:
         return False
     return type(schema_instance).__name__ in __schemas__
 
 
 def _schema(cls):
     # make sure the cls is a class with __annotations__
     if not isinstance(cls, type):
         raise ValueError("schema must be a class")
     if not hasattr(cls, "__annotations__"):
         raise ValueError("schema must be a class with __annotations__")
-    res = baselib.schema(cls)
+    res = baseschema(cls)
     return res
 
 
 def _watch(*args):
     # make sure the args is a list of tuples
     for arg in args:
         if not isinstance(arg, tuple):
@@ -39,15 +44,15 @@
         # make sure the second element of the tuple is a string
         if not isinstance(arg[1], str):
             raise ValueError(
                 "args must be a list of tuples with the second element as a string"
             )
 
     def wrapper(func):
-        return baselib.watch(list(args), func)
+        return basewatch(list(args), func)
 
     return wrapper
 
 
 schema = _schema
 watch = _watch
```

### Comparing `betterschema-0.1.1/tests/testlib.py` & `betterschema-0.1.6/tests/testlib.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-import unittest
-import betterschema.core as core
-import typing as t
+""" Test the core module """
 
-# import faulthandler
+# pylint: disable=E1101, R0903, W0201
+import unittest
 
-# faulthandler.enable()
+from betterschema import core
 
 
 @core.schema
 class DEF:
+    """DEF schema"""
+
     x: int
     y: str
     z: bool
 
 
 @core.schema
 class ABC:
+    """ABC schema"""
+
     a: int
     b: str = 1
     c: bool
     # d: t.Optional[int]  # not supported yet
     e: DEF
 
 
 class TestCore(unittest.TestCase):
+    """Test core module"""
+
     def test_libmodule(self):
+        """Test lib module"""
         print(str(ABC.__annotations__))
 
         a = ABC(
             {
                 "a": 10,
                 "b": "hello",
                 "c": True,
@@ -37,19 +43,19 @@
                     "y": "hello",
                     "z": True,
                 },
             }
         )
         assert a.a == 10
         assert a.b == "hello"
-        assert a.c == True
+        assert a.c is True
         print(a.e)
         assert a.e.x == 10
         assert a.e.y == "hello"
-        assert a.e.z == True
+        assert a.e.z is True
 
         print(a.__annotations__)
         a.a = 10
         a.b = "hello"
         a.c = True
 
         try:
```

