# Comparing `tmp/microchain_python-0.3.6.tar.gz` & `tmp/microchain_python-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microchain_python-0.3.6.tar", last modified: Fri May  3 14:33:06 2024, max compression
+gzip compressed data, was "microchain_python-0.3.7.tar", last modified: Sun May 19 10:29:12 2024, max compression
```

## Comparing `microchain_python-0.3.6.tar` & `microchain_python-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.847809 microchain_python-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-03 14:32:58.000000 microchain_python-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-03 14:33:06.843809 microchain_python-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-03 14:32:58.000000 microchain_python-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/engine/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-03 14:32:58.000000 microchain_python-0.3.6/microchain/models/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/microchain_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 14:33:06.000000 microchain_python-0.3.6/microchain_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 14:33:06.847809 microchain_python-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-03 14:32:58.000000 microchain_python-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 14:33:06.843809 microchain_python-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-03 14:32:58.000000 microchain_python-0.3.6/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-03 14:32:58.000000 microchain_python-0.3.6/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-03 14:32:58.000000 microchain_python-0.3.6/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.136514 microchain_python-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-19 10:29:04.000000 microchain_python-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-19 10:29:12.136514 microchain_python-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-19 10:29:04.000000 microchain_python-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.132514 microchain_python-0.3.7/microchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.132514 microchain_python-0.3.7/microchain/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/engine/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.132514 microchain_python-0.3.7/microchain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-19 10:29:04.000000 microchain_python-0.3.7/microchain/models/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.136514 microchain_python-0.3.7/microchain_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 10:29:12.000000 microchain_python-0.3.7/microchain_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 10:29:12.136514 microchain_python-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-19 10:29:04.000000 microchain_python-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 10:29:12.136514 microchain_python-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 10:29:04.000000 microchain_python-0.3.7/tests/test_str_args.py
```

### Comparing `microchain_python-0.3.6/LICENSE` & `microchain_python-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/PKG-INFO` & `microchain_python-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.6
+Version: 0.3.7
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain_python-0.3.6/README.md` & `microchain_python-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/microchain/engine/agent.py` & `microchain_python-0.3.7/microchain/engine/agent.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/microchain/engine/engine.py` & `microchain_python-0.3.7/microchain/engine/engine.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/microchain/engine/function.py` & `microchain_python-0.3.7/microchain/engine/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     def example(self):
         if not isinstance(self.example_args, list):
             raise ValueError("example_args must be a list")
         if len(self.example_args) != len(self.call_parameters):
             raise ValueError(f"example_args must have the same length as call_parameters ({len(self.call_parameters)})")
 
         bound = self.call_signature.bind(*self.example_args)
-        
-        return f"{self.name}({', '.join([f'{name}={value}' for name, value in bound.arguments.items()])})"
+        return f"{self.name}({', '.join([f'{name}={repr(value)}' for name, value in bound.arguments.items()])})"
     
     @property
     def signature(self):
         arguments = [f"{parameter['name']}: {parameter['annotation'].__name__}" for parameter in self.call_parameters]
         return f"{self.name}({', '.join(arguments)})"
 
     @property
```

### Comparing `microchain_python-0.3.6/microchain/functions.py` & `microchain_python-0.3.7/microchain/functions.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/microchain/models/generators.py` & `microchain_python-0.3.7/microchain/models/generators.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/microchain/models/templates.py` & `microchain_python-0.3.7/microchain/models/templates.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/microchain_python.egg-info/PKG-INFO` & `microchain_python-0.3.7/microchain_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microchain-python
-Version: 0.3.6
+Version: 0.3.7
 Home-page: 
 Author: Federico A. Galatolo
 Author-email: federico.galatolo@unipi.it
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `microchain_python-0.3.6/microchain_python.egg-info/SOURCES.txt` & `microchain_python-0.3.7/microchain_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 microchain_python.egg-info/PKG-INFO
 microchain_python.egg-info/SOURCES.txt
 microchain_python.egg-info/dependency_links.txt
 microchain_python.egg-info/requires.txt
 microchain_python.egg-info/top_level.txt
 tests/test_agent.py
 tests/test_engine.py
-tests/test_openai.py
+tests/test_openai.py
+tests/test_str_args.py
```

### Comparing `microchain_python-0.3.6/setup.py` & `microchain_python-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "README.md"), "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="microchain-python",
-    version="0.3.6",
+    version="0.3.7",
     author="Federico A. Galatolo",
     author_email="federico.galatolo@unipi.it",
     description="",
     url="",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["microchain", "microchain.models", "microchain.engine"],
```

### Comparing `microchain_python-0.3.6/tests/test_agent.py` & `microchain_python-0.3.7/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/tests/test_engine.py` & `microchain_python-0.3.7/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `microchain_python-0.3.6/tests/test_openai.py` & `microchain_python-0.3.7/tests/test_openai.py`

 * *Files identical despite different names*

