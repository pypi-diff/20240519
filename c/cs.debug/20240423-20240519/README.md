# Comparing `tmp/cs.debug-20240423.tar.gz` & `tmp/cs.debug-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.debug-20240423.tar", last modified: Tue Apr 23 07:58:49 2024, max compression
+gzip compressed data, was "cs.debug-20240519.tar", last modified: Sun May 19 02:27:06 2024, max compression
```

## Comparing `cs.debug-20240423.tar` & `cs.debug-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.129033 cs.debug-20240423/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-23 07:58:34.000000 cs.debug-20240423/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     4591 2024-04-23 07:58:49.128766 cs.debug-20240423/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     3802 2024-04-23 07:58:38.000000 cs.debug-20240423/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.125067 cs.debug-20240423/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.125351 cs.debug-20240423/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.126602 cs.debug-20240423/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    20486 2024-04-23 07:58:20.000000 cs.debug-20240423/lib/python/cs/debug.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.128322 cs.debug-20240423/lib/python/cs.debug.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     4591 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-04-23 07:58:49.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      216 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     5209 2024-04-23 07:58:47.000000 cs.debug-20240423/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-23 07:58:49.129152 cs.debug-20240423/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:27:06.041805 cs.debug-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:26:50.000000 cs.debug-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4554 2024-05-19 02:27:06.041519 cs.debug-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3765 2024-05-19 02:26:55.000000 cs.debug-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:27:06.037181 cs.debug-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:27:06.037490 cs.debug-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:27:06.038959 cs.debug-20240519/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    20515 2024-05-19 02:26:30.000000 cs.debug-20240519/lib/python/cs/debug.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:27:06.041062 cs.debug-20240519/lib/python/cs.debug.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4554 2024-05-19 02:27:05.000000 cs.debug-20240519/lib/python/cs.debug.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-05-19 02:27:05.000000 cs.debug-20240519/lib/python/cs.debug.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:27:05.000000 cs.debug-20240519/lib/python/cs.debug.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      216 2024-05-19 02:27:05.000000 cs.debug-20240519/lib/python/cs.debug.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:27:05.000000 cs.debug-20240519/lib/python/cs.debug.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5170 2024-05-19 02:27:04.000000 cs.debug-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:27:06.041906 cs.debug-20240519/setup.cfg
```

### Comparing `cs.debug-20240423/PKG-INFO` & `cs.debug-20240519/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20240423
+Version: 20240519
 Summary: Assorted debugging facilities.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,17 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20240423*:
-* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
-* @trace: include the elapsed time on the return/exception log message.
+*Latest release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
@@ -72,14 +71,17 @@
 
 Decorator to report the call and return of a function.
 
 # Release Log
 
 
 
+*Release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
+
 *Release 20240423*:
 * Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
 * @trace: include the elapsed time on the return/exception log message.
 
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
```

### Comparing `cs.debug-20240423/README.md` & `cs.debug-20240519/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Assorted debugging facilities.
 
-*Latest release 20240423*:
-* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
-* @trace: include the elapsed time on the return/exception log message.
+*Latest release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
@@ -53,14 +52,17 @@
 
 Decorator to report the call and return of a function.
 
 # Release Log
 
 
 
+*Release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
+
 *Release 20240423*:
 * Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
 * @trace: include the elapsed time on the return/exception log message.
 
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
```

### Comparing `cs.debug-20240423/lib/python/cs/debug.py` & `cs.debug-20240519/lib/python/cs/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from cs.py.func import funccite, func_a_kw_fmt
 from cs.py.stack import caller
 from cs.py3 import Queue, Queue_Empty, exec_code
 from cs.seq import seq
 from cs.upd import breakpoint, print  # pylint: disable=redefined-builtin
 from cs.x import X
 
-__version__ = '20240423'
+__version__ = '20240519'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
@@ -484,17 +484,21 @@
 def trace_caller(func):
   ''' Decorator to report the caller of a function when called.
   '''
 
   def subfunc(*a, **kw):
     frame = caller()
     D(
-        "CALL %s()<%s:%d> FROM %s()<%s:%d>", func.__name__,
-        func.__code__.co_filename, func.__code__.co_firstlineno,
-        frame.funcname, frame.filename, frame.lineno
+        "CALL %s()<%s:%d> FROM %s()<%s:%d>",
+        func.__name__,
+        func.__code__.co_filename,
+        func.__code__.co_firstlineno,
+        frame.name,
+        frame.filename,
+        frame.lineno,
     )
     return func(*a, **kw)
 
   subfunc.__name__ = "trace_caller/subfunc/" + func.__name__
   return subfunc
 
 class TracingObject(Proxy):
```

### Comparing `cs.debug-20240423/lib/python/cs.debug.egg-info/PKG-INFO` & `cs.debug-20240519/lib/python/cs.debug.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20240423
+Version: 20240519
 Summary: Assorted debugging facilities.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,17 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20240423*:
-* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
-* @trace: include the elapsed time on the return/exception log message.
+*Latest release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
@@ -72,14 +71,17 @@
 
 Decorator to report the call and return of a function.
 
 # Release Log
 
 
 
+*Release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
+
 *Release 20240423*:
 * Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
 * @trace: include the elapsed time on the return/exception log message.
 
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
```

### Comparing `cs.debug-20240423/pyproject.toml` & `cs.debug-20240519/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
     "cs.deco>=20240412",
     "cs.fs>=20240422",
-    "cs.lex>=20240316",
+    "cs.lex>=20240519",
     "cs.logutils>=20230212",
     "cs.obj>=20220918",
     "cs.pfx>=20240412",
     "cs.py.func>=20230331",
-    "cs.py.stack>=20240412",
+    "cs.py.stack>=20240519",
     "cs.py3>=20220523",
     "cs.seq>=20221118",
     "cs.upd>=20240412",
     "cs.x>=20240316",
 ]
 classifiers = [
     "Programming Language :: Python",
@@ -28,29 +28,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240423"
+version = "20240519"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted debugging facilities.
 
-*Latest release 20240423*:
-* Support \"import *\" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
-* @trace: include the elapsed time on the return/exception log message.
+*Latest release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
 The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
@@ -97,14 +96,17 @@
 
 Decorator to report the call and return of a function.
 
 # Release Log
 
 
 
+*Release 20240519*:
+trace_caller: access frame.name instead of frame.funcname.
+
 *Release 20240423*:
 * Support \"import *\" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
 * @trace: include the elapsed time on the return/exception log message.
 
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
```

