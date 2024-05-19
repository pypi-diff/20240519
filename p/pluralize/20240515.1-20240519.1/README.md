# Comparing `tmp/pluralize-20240515.1.tar.gz` & `tmp/pluralize-20240519.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluralize-20240515.1.tar", last modified: Thu May 16 06:48:55 2024, max compression
+gzip compressed data, was "pluralize-20240519.1.tar", last modified: Sun May 19 18:33:10 2024, max compression
```

## Comparing `pluralize-20240515.1.tar` & `pluralize-20240519.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.580986 pluralize-20240515.1/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-05-16 06:48:55.580986 pluralize-20240515.1/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20240515.1/README.md
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.577653 pluralize-20240515.1/pluralize/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     5719 2024-05-16 06:42:17.000000 pluralize-20240515.1/pluralize/__init__.py
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.580986 pluralize-20240515.1/pluralize.egg-info/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/PKG-INFO
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      199 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/SOURCES.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/dependency_links.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       10 2024-05-16 06:48:55.000000 pluralize-20240515.1/pluralize.egg-info/top_level.txt
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      563 2024-05-16 06:42:06.000000 pluralize-20240515.1/pyproject.toml
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-16 06:48:55.580986 pluralize-20240515.1/setup.cfg
-drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-16 06:48:55.580986 pluralize-20240515.1/tests/
--rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1355 2021-07-16 07:50:13.000000 pluralize-20240515.1/tests/test_simple.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-19 18:33:10.102252 pluralize-20240519.1/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-05-19 18:33:10.102252 pluralize-20240519.1/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2195 2021-07-16 07:51:13.000000 pluralize-20240519.1/README.md
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-19 18:33:10.102252 pluralize-20240519.1/pluralize/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     6081 2024-05-19 18:32:00.000000 pluralize-20240519.1/pluralize/__init__.py
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-19 18:33:10.102252 pluralize-20240519.1/pluralize.egg-info/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     2748 2024-05-19 18:33:10.000000 pluralize-20240519.1/pluralize.egg-info/PKG-INFO
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      199 2024-05-19 18:33:10.000000 pluralize-20240519.1/pluralize.egg-info/SOURCES.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)        1 2024-05-19 18:33:10.000000 pluralize-20240519.1/pluralize.egg-info/dependency_links.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       10 2024-05-19 18:33:10.000000 pluralize-20240519.1/pluralize.egg-info/top_level.txt
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)      563 2024-05-19 18:32:06.000000 pluralize-20240519.1/pyproject.toml
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)       38 2024-05-19 18:33:10.102252 pluralize-20240519.1/setup.cfg
+drwxr-xr-x   0 mdipierro  (1000) mdipierro  (1000)        0 2024-05-19 18:33:10.102252 pluralize-20240519.1/tests/
+-rw-r--r--   0 mdipierro  (1000) mdipierro  (1000)     1697 2024-05-19 18:31:02.000000 pluralize-20240519.1/tests/test_simple.py
```

### Comparing `pluralize-20240515.1/PKG-INFO` & `pluralize-20240519.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralize
-Version: 20240515.1
+Version: 20240519.1
 Summary: i18n + pluralization library with multi-plural form support and thread safe for web apps
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pluralize
 Project-URL: Bug Tracker, https://github.com/web2py/yatl/pluralize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pluralize-20240515.1/README.md` & `pluralize-20240519.1/README.md`

 * *Files identical despite different names*

### Comparing `pluralize-20240515.1/pluralize/__init__.py` & `pluralize-20240519.1/pluralize/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import ast
+import json
 import os
 import re
-import json
 import threading
-import ast
 
-__version__ = "20240515.1"
+__version__ = "20240519.1"
 
 re_language = re.compile(r"^\w\w(-\w+)*.json$")
 
 
 class lazyT(object):
 
     """accesssory object used to represent a T("string")"""
@@ -42,47 +42,58 @@
 
     def xml(self):
         """same as str but for interoperability with yatl helpers"""
         return self.translator(self.text, **self.kwargs)
 
 
 class Translator(object):
-    def __init__(self, folder=None, encoding="utf-8"):
+    def __init__(self, folder=None, encoding="utf-8", comment_marker=None):
         """
         creates a translator object loading languages and pluralizations from translations/en-US.py files
         usage:
 
             T =  Translator('translations')
             print(T('dog'))
         """
         self.local = threading.local()
         self.languages = {}
         self.local.tag = None
         self.local.language = None
         self.missing = set()
         self.folder = folder
         self.encoding = encoding
+        self.comment_marker = comment_marker
         if folder:
             self.load(folder)
 
     def load(self, folder):
         """loads languages and pluralizations from folder/en-US.json files"""
         self.languages = {}
         for filename in os.listdir(folder):
             if re_language.match(filename):
-                with open(os.path.join(folder, filename), "r", encoding=self.encoding) as fp:
+                with open(
+                    os.path.join(folder, filename), "r", encoding=self.encoding
+                ) as fp:
                     self.languages[filename[:-5].lower()] = json.load(fp)
 
     def save(self, folder=None, ensure_ascii=True):
         """save the loaded translation files"""
         folder = folder or self.folder
         for key in self.languages:
             filename = "%s.json" % key
-            with open(os.path.join(folder, filename), "w", encoding=self.encoding) as fp:
-                json.dump(self.languages[key], fp, sort_keys=True, indent=4, ensure_ascii=ensure_ascii)
+            with open(
+                os.path.join(folder, filename), "w", encoding=self.encoding
+            ) as fp:
+                json.dump(
+                    self.languages[key],
+                    fp,
+                    sort_keys=True,
+                    indent=4,
+                    ensure_ascii=ensure_ascii,
+                )
 
     def select(self, accepted_languages="fr-CH, fr;q=0.9, en;q=0.8, de;q=0.7, *;q=0.5"):
         """given appected_langauges string from HTTP header, picks the best match"""
         if isinstance(accepted_languages, str):
             accepted_languages = [
                 tag.split(";")[0].replace("_", "-").strip()
                 for tag in accepted_languages.split(",")
@@ -114,18 +125,22 @@
             n = kwargs.get("n", 1)
             translations = self.local.language.get(text)
             if translations is None:
                 self.missing.add(text)
             elif isinstance(translations, dict) and translations:
                 k = max(int(i) for i in translations.keys() if int(i) <= n)
                 text = translations[str(k)].format(**kwargs)
+        if text and self.comment_marker:
+            text = text.split(self.comment_marker)[0]
         return text.format(**kwargs)
 
     @staticmethod
-    def find_matches(folder, name="T", extensions=["py", "js", "html"], encoding="utf-8"):
+    def find_matches(
+        folder, name="T", extensions=["py", "js", "html"], encoding="utf-8"
+    ):
         """finds all strings in files in folder needing translations"""
         matches_found = set()
         re_string_t = (
             r"(?<=[^\w]%s\()(?P<name>"
             r"[uU]?[rR]?(?:'''(?:[^']|'{1,2}(?!'))*''')"
             r"|(?:'(?:[^'\\]|\\.)*')"
             r'|(?:"""(?:[^"]|"{1,2}(?!"))*""")'
```

### Comparing `pluralize-20240515.1/pluralize.egg-info/PKG-INFO` & `pluralize-20240519.1/pluralize.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluralize
-Version: 20240515.1
+Version: 20240519.1
 Summary: i18n + pluralization library with multi-plural form support and thread safe for web apps
 Author-email: Massimo Di Pierro <massimo.dipierro@gmail.com>
 Project-URL: Homepage, https://github.com/web2py/pluralize
 Project-URL: Bug Tracker, https://github.com/web2py/yatl/pluralize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pluralize-20240515.1/pyproject.toml` & `pluralize-20240519.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pluralize"
-version = "20240515.1"
+version = "20240519.1"
 authors = [{ name="Massimo Di Pierro", email="massimo.dipierro@gmail.com" },]
 description = "i18n + pluralization library with multi-plural form support and thread safe for web apps"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
       "Programming Language :: Python :: 3",
       "License :: OSI Approved :: BSD License",
```

### Comparing `pluralize-20240515.1/tests/test_simple.py` & `pluralize-20240519.1/tests/test_simple.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import unittest
+
 from pluralize import Translator
 
 
 class TestPluralization(unittest.TestCase):
     def setUp(self):
-        T = Translator()
+        T = Translator(comment_marker="##")
         T.update_languages(T.find_matches("./"))
         T.languages = {
             "it": {
                 "dog": {
                     "0": "no cane",
                     "1": "un cane",
                     "2": "due cani",
                     "3": "alcuni cani",
                     "10": "tanti cani",
-                }
+                },
+                "dog##dialect": {
+                    "0": "nisciuno cane",
+                },
             }
         }
         T.select("en;q=0.9,it-IT;q=0.1")
         self.T = T
 
     def test_simple(self):
         T = self.T
@@ -32,14 +36,21 @@
 
         plus = T("plus")
         T.languages["it"]["plus"] = {"0": "piu'"}
         self.assertEqual(
             dog + " " + plus + " " + dog.format(n=2), "un cane piu' due cani"
         )
 
+    def test_comments(self):
+        T = self.T
+        dog = T("dog")
+        self.assertEqual(str(dog.format(n=0)), "no cane")
+        dog = T("dog##dialect")
+        self.assertEqual(str(dog.format(n=0)), "nisciuno cane")
+
     def test_idempotency(self):
         T = self.T
         text = "dog"
         a = T(text)
         b = T(a)
         c = T(b)
         self.assertEqual(str(c.format(n=1)), "un cane")
```

