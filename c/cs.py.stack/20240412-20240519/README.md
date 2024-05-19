# Comparing `tmp/cs.py.stack-20240412.tar.gz` & `tmp/cs.py.stack-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.py.stack-20240412.tar", last modified: Fri Apr 12 02:36:05 2024, max compression
+gzip compressed data, was "cs.py.stack-20240519.tar", last modified: Sun May 19 02:16:12 2024, max compression
```

## Comparing `cs.py.stack-20240412.tar` & `cs.py.stack-20240519.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.439509 cs.py.stack-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 02:35:56.000000 cs.py.stack-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     3063 2024-04-12 02:36:05.439226 cs.py.stack-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     2248 2024-04-12 02:35:59.000000 cs.py.stack-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.435899 cs.py.stack-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.436197 cs.py.stack-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.436305 cs.py.stack-20240412/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.438792 cs.py.stack-20240412/lib/python/cs/py/
--rw-r--r--   0 cameron    (501) cameron    (502)     4253 2024-04-12 02:35:39.000000 cs.py.stack-20240412/lib/python/cs/py/stack.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.438467 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     3063 2024-04-12 02:36:04.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      246 2024-04-12 02:36:05.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 02:36:04.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 02:36:05.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     3373 2024-04-12 02:36:03.000000 cs.py.stack-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 02:36:05.439605 cs.py.stack-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:16:12.329123 cs.py.stack-20240519/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:16:01.000000 cs.py.stack-20240519/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3006 2024-05-19 02:16:12.328863 cs.py.stack-20240519/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2191 2024-05-19 02:16:04.000000 cs.py.stack-20240519/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:16:12.325624 cs.py.stack-20240519/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:16:12.325905 cs.py.stack-20240519/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:16:12.326010 cs.py.stack-20240519/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:16:12.328436 cs.py.stack-20240519/lib/python/cs/py/
+-rw-r--r--   0 cameron    (501) cameron    (502)     4100 2024-05-19 02:15:49.000000 cs.py.stack-20240519/lib/python/cs/py/stack.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:16:12.328110 cs.py.stack-20240519/lib/python/cs.py.stack.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3006 2024-05-19 02:16:11.000000 cs.py.stack-20240519/lib/python/cs.py.stack.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      246 2024-05-19 02:16:12.000000 cs.py.stack-20240519/lib/python/cs.py.stack.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:16:11.000000 cs.py.stack-20240519/lib/python/cs.py.stack.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:16:12.000000 cs.py.stack-20240519/lib/python/cs.py.stack.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3316 2024-05-19 02:16:10.000000 cs.py.stack-20240519/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:16:12.329236 cs.py.stack-20240519/setup.cfg
```

### Comparing `cs.py.stack-20240412/PKG-INFO` & `cs.py.stack-20240519/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.py.stack
-Version: 20240412
+Version: 20240519
 Summary: Convenience functions for the python execution stack.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -16,17 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20240412*:
-* stack_dump: new select parameter to pick interesting frames for the listing.
-* Provide StackSummary and FrameSummary if Python too old.
+*Latest release 20240519*:
+Drop Frame.funcname property.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
@@ -57,14 +56,17 @@
   if `select` is a `str` it must be present in the frame filename;
   otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240519*:
+Drop Frame.funcname property.
+
 *Release 20240412*:
 * stack_dump: new select parameter to pick interesting frames for the listing.
 * Provide StackSummary and FrameSummary if Python too old.
 
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
```

### Comparing `cs.py.stack-20240412/README.md` & `cs.py.stack-20240519/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20240412*:
-* stack_dump: new select parameter to pick interesting frames for the listing.
-* Provide StackSummary and FrameSummary if Python too old.
+*Latest release 20240519*:
+Drop Frame.funcname property.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
@@ -38,14 +37,17 @@
   if `select` is a `str` it must be present in the frame filename;
   otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240519*:
+Drop Frame.funcname property.
+
 *Release 20240412*:
 * stack_dump: new select parameter to pick interesting frames for the listing.
 * Provide StackSummary and FrameSummary if Python too old.
 
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
```

### Comparing `cs.py.stack-20240412/lib/python/cs/py/stack.py` & `cs.py.stack-20240519/lib/python/cs/py/stack.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 '''
 
 from __future__ import print_function
 from collections import namedtuple
 import sys
 from traceback import extract_stack
 
-__version__ = '20240412'
+__version__ = '20240519'
 
 DISTINFO = {
     'description':
     "Convenience functions for the python execution stack.",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -32,21 +32,14 @@
   class FrameSummary(namedtuple('FrameSummary', 'filename lineno name line')):
     ''' A `namedtuple` for stack frame contents.
     '''
 
     def __str__(self):
       return "%s:%d: %s" % (self.filename, self.lineno, self.line)
 
-    # compatibility with my prior Frame class
-    @property
-    def funcname(self):
-      ''' The frame function name.
-      '''
-      return self.name
-
     @property
     def linetext(self):
       ''' The line of source code.
       '''
       return self.line
 
   class StackSummary(list):
```

### Comparing `cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/PKG-INFO` & `cs.py.stack-20240519/lib/python/cs.py.stack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.py.stack
-Version: 20240412
+Version: 20240519
 Summary: Convenience functions for the python execution stack.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -16,17 +16,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20240412*:
-* stack_dump: new select parameter to pick interesting frames for the listing.
-* Provide StackSummary and FrameSummary if Python too old.
+*Latest release 20240519*:
+Drop Frame.funcname property.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
@@ -57,14 +56,17 @@
   if `select` is a `str` it must be present in the frame filename;
   otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240519*:
+Drop Frame.funcname property.
+
 *Release 20240412*:
 * stack_dump: new select parameter to pick interesting frames for the listing.
 * Provide StackSummary and FrameSummary if Python too old.
 
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
```

### Comparing `cs.py.stack-20240412/pyproject.toml` & `cs.py.stack-20240519/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,30 +15,29 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240412"
+version = "20240519"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20240412*:
-* stack_dump: new select parameter to pick interesting frames for the listing.
-* Provide StackSummary and FrameSummary if Python too old.
+*Latest release 20240519*:
+Drop Frame.funcname property.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
@@ -69,14 +68,17 @@
   if `select` is a `str` it must be present in the frame filename;
   otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240519*:
+Drop Frame.funcname property.
+
 *Release 20240412*:
 * stack_dump: new select parameter to pick interesting frames for the listing.
 * Provide StackSummary and FrameSummary if Python too old.
 
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
```

