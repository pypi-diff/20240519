# Comparing `tmp/translator_uabthehack-0.3.0.tar.gz` & `tmp/translator_uabthehack-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translator_uabthehack-0.3.0.tar", max compression
+gzip compressed data, was "translator_uabthehack-0.4.0.tar", max compression
```

## Comparing `translator_uabthehack-0.3.0.tar` & `translator_uabthehack-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-19 07:59:55.909363 translator_uabthehack-0.3.0/README.md
--rw-r--r--   0        0        0      304 2024-05-19 08:06:05.629360 translator_uabthehack-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 07:59:57.622696 translator_uabthehack-0.3.0/translator_uabthehack/__init__.py
--rw-r--r--   0        0        0     4116 2024-05-19 07:59:57.622696 translator_uabthehack-0.3.0/translator_uabthehack/main.py
--rw-r--r--   0        0        0      728 2024-05-19 07:59:57.622696 translator_uabthehack-0.3.0/translator_uabthehack/traductor.py
--rw-r--r--   0        0        0     1078 2024-05-19 07:59:57.622696 translator_uabthehack-0.3.0/translator_uabthehack/variable_seeker.py
--rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 translator_uabthehack-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-19 07:59:55.909363 translator_uabthehack-0.4.0/README.md
+-rw-r--r--   0        0        0      304 2024-05-19 08:19:46.342688 translator_uabthehack-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 07:59:57.622696 translator_uabthehack-0.4.0/translator_uabthehack/__init__.py
+-rw-r--r--   0        0        0     4123 2024-05-19 08:19:25.089355 translator_uabthehack-0.4.0/translator_uabthehack/main.py
+-rw-r--r--   0        0        0      728 2024-05-19 07:59:57.622696 translator_uabthehack-0.4.0/translator_uabthehack/traductor.py
+-rw-r--r--   0        0        0     1078 2024-05-19 07:59:57.622696 translator_uabthehack-0.4.0/translator_uabthehack/variable_seeker.py
+-rw-r--r--   0        0        0      344 1970-01-01 00:00:00.000000 translator_uabthehack-0.4.0/PKG-INFO
```

### Comparing `translator_uabthehack-0.3.0/translator_uabthehack/main.py` & `translator_uabthehack-0.4.0/translator_uabthehack/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-import variable_seeker
+from . import variable_seeker
 from deep_translator import GoogleTranslator
 import sys
 
 
 
 def process_line (token, toggle, traductor, output):
     if '#' in token:
```

### Comparing `translator_uabthehack-0.3.0/translator_uabthehack/traductor.py` & `translator_uabthehack-0.4.0/translator_uabthehack/traductor.py`

 * *Files identical despite different names*

### Comparing `translator_uabthehack-0.3.0/translator_uabthehack/variable_seeker.py` & `translator_uabthehack-0.4.0/translator_uabthehack/variable_seeker.py`

 * *Files identical despite different names*

