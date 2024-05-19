# Comparing `tmp/tarina-0.5.1.tar.gz` & `tmp/tarina-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.5.1.tar", last modified: Sun May 19 08:16:39 2024, max compression
+gzip compressed data, was "tarina-0.5.2.tar", last modified: Sun May 19 13:28:01 2024, max compression
```

## Comparing `tarina-0.5.1.tar` & `tarina-0.5.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.031603 tarina-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 08:16:21.000000 tarina-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-19 08:16:21.000000 tarina-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 08:16:39.031603 tarina-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-19 08:16:21.000000 tarina-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-19 08:16:21.000000 tarina-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 08:16:39.031603 tarina-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 08:16:21.000000 tarina-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.023603 tarina-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.027603 tarina-0.5.1/src/tarina/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_lru_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_lru_c.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_lru_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_op.h
--rw-r--r--   0 runner    (1001) docker     (127)   213169 2024-05-19 08:16:33.000000 tarina-0.5.1/src/tarina/_string_c.c
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_string_c.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_string_c.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/_string_py.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/guard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.027603 tarina-0.5.1/src/tarina/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/.config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/.lang.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/.template.json
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/.template.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/en-US.json
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/i18n/zh-CN.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.031603 tarina-0.5.1/src/tarina/lang/
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/lang/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/lang/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/lang/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/lru.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/lru.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    68734 2024-05-19 08:16:21.000000 tarina-0.5.1/src/tarina/trie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.031603 tarina-0.5.1/src/tarina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 08:16:39.000000 tarina-0.5.1/src/tarina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-19 08:16:39.000000 tarina-0.5.1/src/tarina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 08:16:39.000000 tarina-0.5.1/src/tarina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 08:16:39.000000 tarina-0.5.1/src/tarina.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 08:16:39.000000 tarina-0.5.1/src/tarina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 08:16:39.000000 tarina-0.5.1/src/tarina.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 08:16:39.031603 tarina-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-19 08:16:21.000000 tarina-0.5.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.951621 tarina-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 13:27:46.000000 tarina-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-19 13:27:46.000000 tarina-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 13:28:01.951621 tarina-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-19 13:27:46.000000 tarina-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-19 13:27:46.000000 tarina-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:28:01.951621 tarina-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 13:27:46.000000 tarina-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.943621 tarina-0.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.947621 tarina-0.5.2/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_op.h
+-rw-r--r--   0 runner    (1001) docker     (127)   213169 2024-05-19 13:27:55.000000 tarina-0.5.2/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/guard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.951621 tarina-0.5.2/src/tarina/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/.config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/.lang.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/.template.json
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/.template.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/en-US.json
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/i18n/zh-CN.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.951621 tarina-0.5.2/src/tarina/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/lang/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/lang/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/lang/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68734 2024-05-19 13:27:46.000000 tarina-0.5.2/src/tarina/trie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.951621 tarina-0.5.2/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-19 13:28:01.000000 tarina-0.5.2/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-19 13:28:01.000000 tarina-0.5.2/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:28:01.000000 tarina-0.5.2/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-19 13:28:01.000000 tarina-0.5.2/src/tarina.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 13:28:01.000000 tarina-0.5.2/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 13:28:01.000000 tarina-0.5.2/src/tarina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:28:01.951621 tarina-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-19 13:27:46.000000 tarina-0.5.2/tests/test_main.py
```

### Comparing `tarina-0.5.1/LICENSE` & `tarina-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/PKG-INFO` & `tarina-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.5.1
+Version: 0.5.2
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions>=4.4.0
```

### Comparing `tarina-0.5.1/pyproject.toml` & `tarina-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tarina"
-version = "0.5.1"
+version = "0.5.2"
 description = "A collection of common utils for Arclet"
 authors = [
     {name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com"},
 ]
 dependencies = [
     "typing-extensions>=4.4.0",
 ]
```

### Comparing `tarina-0.5.1/setup.py` & `tarina-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/__init__.py` & `tarina-0.5.2/src/tarina/__init__.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_lru_c.c` & `tarina-0.5.2/src/tarina/_lru_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_lru_c.pyi` & `tarina-0.5.2/src/tarina/_lru_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_lru_py.py` & `tarina-0.5.2/src/tarina/_lru_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_op.h` & `tarina-0.5.2/src/tarina/_op.h`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_string_c.c` & `tarina-0.5.2/src/tarina/_string_c.c`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_string_c.pyi` & `tarina-0.5.2/src/tarina/_string_c.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_string_c.pyx` & `tarina-0.5.2/src/tarina/_string_c.pyx`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/_string_py.py` & `tarina-0.5.2/src/tarina/_string_py.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/context.py` & `tarina-0.5.2/src/tarina/context.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/date.py` & `tarina-0.5.2/src/tarina/date.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/generic.py` & `tarina-0.5.2/src/tarina/generic.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/guard.py` & `tarina-0.5.2/src/tarina/guard.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/i18n/.lang.schema.json` & `tarina-0.5.2/src/tarina/i18n/.lang.schema.json`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/i18n/.template.schema.json` & `tarina-0.5.2/src/tarina/i18n/.template.schema.json`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/lang/__init__.py` & `tarina-0.5.2/src/tarina/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/lang/__main__.py` & `tarina-0.5.2/src/tarina/lang/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from argparse import ArgumentParser
 from tarina.lang.schema import write_lang_schema
 from tarina.lang.model import write_model
 from pathlib import Path
 import json
 
-CONFIG_TEMPLATE = """
+CONFIG_TEMPLATE = """\
 {
   "default": "zh-CN",
   "frozen": [],
   "require": []
 }
 """
 
-CONFIG_INIT = """
+CONFIG_INIT = """\
 # This file is @generated by tarina.lang CLI tool
 # It is not intended for manual editing.
 
 from pathlib import Path
 
 from tarina.lang import lang
 
 
 lang.load(Path(__file__).parent)
 """
 
 
-TEMPLATE_SCHEMA = """
+TEMPLATE_SCHEMA = """\
 {
   "title": "Template",
   "description": "Template for lang items to generate schema for lang files",
   "type": "object",
   "properties": {
     "scopes": {
       "title": "Scopes",
@@ -57,24 +57,24 @@
         }
       }
     }
   }
 }
 """
 
-TEMPLATE_TEMPLATE = """
+TEMPLATE_TEMPLATE = """\
 {
-  "$schema": "./.template.schema.json",
+  "$schema": ".template.schema.json",
   "scopes": []
 }
 """
 
-LANG_TEMPLATE = """
+LANG_TEMPLATE = """\
 {
-  "$schema": "./.lang.schema.json"
+  "$schema": ".lang.schema.json"
 }
 """
 
 def new(*_):
     i18n_dir = Path.cwd() / "i18n"
     if i18n_dir.exists():
         print("i18n directory already exists")
```

### Comparing `tarina-0.5.1/src/tarina/lang/model.py` & `tarina-0.5.2/src/tarina/lang/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from pathlib import Path
 from tarina.lang import lang
 from tarina.lang.schema import _TemplateDict, get_template
+from tarina.tools import pascal_case
 import keyword
 
 
 class LangItem:
     def __init__(self, scope: str, type: str):
         self.scope = scope
         self.type = type
@@ -23,23 +24,23 @@
 MODEL_TEMPLATE = """\
 # This file is @generated by tarina.lang CLI tool
 # It is not intended for manual editing.
 
 from tarina.lang.model import LangModel, LangItem
 
 
-{scope_classes}
-class Lang(LangModel):
-{scopes}
+{scope_classes}class Lang(LangModel):
+{scopes}\
 """
 
 
 SCOPE_TEMPLATE = """\
 class {scope}:
 {types}
+
 """
 
 TYPE_TEMPLATE = """\
     {name}: LangItem = LangItem("{scope}", "{type}")
 """
 
 
@@ -51,23 +52,23 @@
     scopes: list[_TemplateDict] = template["scopes"]
     scopes_classes = ""
     scopes_str = ""
     for s in scopes:
         scope = re.sub(r"[\W\s]+", "_", s["scope"])
         if scope in keyword.kwlist:
             scope += "_"
-        scope_class = scope.capitalize()
+        scope_class = pascal_case(scope)
         if scope_class == "Lang":
             scope_class += "_"
         types_str = ""
         for t in s["types"]:
             name = re.sub(r"[\W\s]+", "_", t)
             if name in keyword.kwlist:
                 name += "_"
-            types_str += TYPE_TEMPLATE.format(name=t, scope=s["scope"], type=t)
+            types_str += TYPE_TEMPLATE.format(name=name, scope=s["scope"], type=t)
         scopes_classes += SCOPE_TEMPLATE.format(scope=scope_class, types=types_str)
         scopes_str += f"    {scope} = {scope_class}\n"
     return MODEL_TEMPLATE.format(scope_classes=scopes_classes, scopes=scopes_str)
 
 
 def write_model(root: Path):
     model = generate_model(root)
```

### Comparing `tarina-0.5.1/src/tarina/lang/schema.py` & `tarina-0.5.2/src/tarina/lang/schema.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/lru.pyi` & `tarina-0.5.2/src/tarina/lru.pyi`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/signature.py` & `tarina-0.5.2/src/tarina/signature.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/string.py` & `tarina-0.5.2/src/tarina/string.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina/tools.py` & `tarina-0.5.2/src/tarina/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -118,7 +118,31 @@
                         if _part[0] in ("'", '"') and _part[-1] in ("'", '"'):
                             _part = _part[1:-1]
                         _args.append(_part)
                 res = res(*_args, **_kwargs)
         else:
             res = getattr(res, part)
     return res
+
+
+def uncapitalize(source: str) -> str:
+    return source[0].lower() + source[1:]
+
+
+def camel_case(source: str) -> str:
+    return re.sub("[_-][a-z]", lambda mat: mat[0][1:].upper(), source)
+
+
+def pascal_case(source: str) -> str:
+    return re.sub("[_-][a-z]", lambda mat: mat[0][1:].upper(), source.capitalize())
+
+
+def param_case(source: str) -> str:
+    return re.sub(
+        ".[A-Z]+", lambda mat: mat[0][0] + "-" + mat[0][1:].lower(), uncapitalize(source).replace("_", "-")
+    )
+
+
+def snake_case(source: str) -> str:
+    return re.sub(
+        ".[A-Z]", lambda mat: mat[0][0] + "_" + mat[0][1:].lower(), uncapitalize(source).replace("-", "_")
+    )
```

### Comparing `tarina-0.5.1/src/tarina/trie.py` & `tarina-0.5.2/src/tarina/trie.py`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/src/tarina.egg-info/PKG-INFO` & `tarina-0.5.2/src/tarina.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tarina
-Version: 0.5.1
+Version: 0.5.2
 Summary: A collection of common utils for Arclet
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing-extensions>=4.4.0
```

### Comparing `tarina-0.5.1/src/tarina.egg-info/SOURCES.txt` & `tarina-0.5.2/src/tarina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tarina-0.5.1/tests/test_main.py` & `tarina-0.5.2/tests/test_main.py`

 * *Files identical despite different names*

