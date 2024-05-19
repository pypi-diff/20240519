# Comparing `tmp/pysubs2-1.6.0.tar.gz` & `tmp/pysubs2-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysubs2-1.6.0.tar", last modified: Sun Nov 27 23:22:38 2022, max compression
+gzip compressed data, was "pysubs2-1.6.1.tar", last modified: Sun Apr  2 14:18:21 2023, max compression
```

## Comparing `pysubs2-1.6.0.tar` & `pysubs2-1.6.1.tar`

### file list

```diff
@@ -1,32 +1,50 @@
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2022-11-27 23:22:38.162852 pysubs2-1.6.0/
--rw-rw-r--   0 azar      (1000) azar      (1000)     1063 2022-02-20 13:38:27.000000 pysubs2-1.6.0/LICENSE.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)     3001 2022-11-27 23:22:38.162852 pysubs2-1.6.0/PKG-INFO
--rw-rw-r--   0 azar      (1000) azar      (1000)     1705 2022-11-15 20:51:15.000000 pysubs2-1.6.0/README.rst
--rw-rw-r--   0 azar      (1000) azar      (1000)       85 2022-11-15 22:12:42.000000 pysubs2-1.6.0/pyproject.toml
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2022-11-27 23:22:38.158852 pysubs2-1.6.0/pysubs2/
--rw-rw-r--   0 azar      (1000) azar      (1000)      505 2022-11-27 20:24:46.000000 pysubs2-1.6.0/pysubs2/__init__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)      134 2021-10-02 16:04:45.000000 pysubs2-1.6.0/pysubs2/__main__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    10616 2022-03-02 19:32:52.000000 pysubs2-1.6.0/pysubs2/cli.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1479 2022-11-27 23:15:15.000000 pysubs2-1.6.0/pysubs2/common.py
--rw-rw-r--   0 azar      (1000) azar      (1000)      633 2021-10-02 16:04:45.000000 pysubs2-1.6.0/pysubs2/exceptions.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2893 2021-10-02 16:04:45.000000 pysubs2-1.6.0/pysubs2/formatbase.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2438 2021-10-02 16:04:45.000000 pysubs2-1.6.0/pysubs2/formats.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1862 2021-10-02 16:04:45.000000 pysubs2-1.6.0/pysubs2/jsonformat.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4365 2021-10-02 16:04:45.000000 pysubs2-1.6.0/pysubs2/microdvd.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1802 2021-10-02 16:52:06.000000 pysubs2-1.6.0/pysubs2/mpl2.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     5883 2021-10-02 17:11:23.000000 pysubs2-1.6.0/pysubs2/ssaevent.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    20476 2022-11-27 22:32:06.000000 pysubs2-1.6.0/pysubs2/ssafile.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     3995 2022-11-27 21:48:25.000000 pysubs2-1.6.0/pysubs2/ssastyle.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     7181 2022-11-27 23:06:07.000000 pysubs2-1.6.0/pysubs2/subrip.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    16124 2022-11-27 22:44:38.000000 pysubs2-1.6.0/pysubs2/substation.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4641 2022-10-31 22:32:04.000000 pysubs2-1.6.0/pysubs2/time.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     3962 2022-11-27 23:08:08.000000 pysubs2-1.6.0/pysubs2/tmp.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1237 2021-12-19 21:16:30.000000 pysubs2-1.6.0/pysubs2/webvtt.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1604 2022-11-15 20:42:03.000000 pysubs2-1.6.0/pysubs2/whisper.py
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2022-11-27 23:22:38.162852 pysubs2-1.6.0/pysubs2.egg-info/
--rw-rw-r--   0 azar      (1000) azar      (1000)     3001 2022-11-27 23:22:38.000000 pysubs2-1.6.0/pysubs2.egg-info/PKG-INFO
--rw-rw-r--   0 azar      (1000) azar      (1000)      566 2022-11-27 23:22:38.000000 pysubs2-1.6.0/pysubs2.egg-info/SOURCES.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)        1 2022-11-27 23:22:38.000000 pysubs2-1.6.0/pysubs2.egg-info/dependency_links.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)       49 2022-11-27 23:22:38.000000 pysubs2-1.6.0/pysubs2.egg-info/entry_points.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)        8 2022-11-27 23:22:38.000000 pysubs2-1.6.0/pysubs2.egg-info/top_level.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)     1358 2022-11-27 23:22:38.162852 pysubs2-1.6.0/setup.cfg
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2023-04-02 14:18:21.404512 pysubs2-1.6.1/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1063 2023-04-02 14:08:34.000000 pysubs2-1.6.1/LICENSE.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3281 2023-04-02 14:18:21.404512 pysubs2-1.6.1/PKG-INFO
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1985 2023-01-29 23:43:20.000000 pysubs2-1.6.1/README.rst
+-rw-rw-r--   0 azar      (1000) azar      (1000)       85 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pyproject.toml
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2023-04-02 14:18:21.396512 pysubs2-1.6.1/pysubs2/
+-rw-rw-r--   0 azar      (1000) azar      (1000)      505 2023-01-29 23:38:11.000000 pysubs2-1.6.1/pysubs2/__init__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      134 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/__main__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    10607 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/cli.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1479 2023-04-02 14:08:34.000000 pysubs2-1.6.1/pysubs2/common.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      633 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/exceptions.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2945 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/formatbase.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2438 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/formats.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1862 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/jsonformat.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4398 2023-01-29 23:38:11.000000 pysubs2-1.6.1/pysubs2/microdvd.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1802 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/mpl2.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     5883 2023-01-29 23:38:11.000000 pysubs2-1.6.1/pysubs2/ssaevent.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    20356 2023-01-29 23:38:11.000000 pysubs2-1.6.1/pysubs2/ssafile.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3995 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/ssastyle.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     7371 2023-04-02 14:02:19.000000 pysubs2-1.6.1/pysubs2/subrip.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    16170 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/substation.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4641 2023-01-29 23:38:11.000000 pysubs2-1.6.1/pysubs2/time.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3954 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/tmp.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1531 2023-04-02 14:02:19.000000 pysubs2-1.6.1/pysubs2/webvtt.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1604 2022-12-28 16:13:18.000000 pysubs2-1.6.1/pysubs2/whisper.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2023-04-02 14:18:21.400512 pysubs2-1.6.1/pysubs2.egg-info/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3281 2023-04-02 14:18:21.000000 pysubs2-1.6.1/pysubs2.egg-info/PKG-INFO
+-rw-rw-r--   0 azar      (1000) azar      (1000)      929 2023-04-02 14:18:21.000000 pysubs2-1.6.1/pysubs2.egg-info/SOURCES.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)        1 2023-04-02 14:18:21.000000 pysubs2-1.6.1/pysubs2.egg-info/dependency_links.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)       49 2023-04-02 14:18:21.000000 pysubs2-1.6.1/pysubs2.egg-info/entry_points.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)        8 2023-04-02 14:18:21.000000 pysubs2-1.6.1/pysubs2.egg-info/top_level.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1447 2023-04-02 14:18:21.404512 pysubs2-1.6.1/setup.cfg
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2023-04-02 14:18:21.404512 pysubs2-1.6.1/tests/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4282 2023-01-29 23:38:11.000000 pysubs2-1.6.1/tests/test_attachment.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    15832 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_cli.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      256 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_common.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      642 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_formats.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      500 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_json.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     5148 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_microdvd.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1819 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_mpl2.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1695 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_parse_tags.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2177 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_ssaevent.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3812 2023-01-29 23:38:11.000000 pysubs2-1.6.1/tests/test_ssafile.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1207 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_ssastyle.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     7608 2023-04-02 14:02:19.000000 pysubs2-1.6.1/tests/test_subrip.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    16303 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_substation.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     6961 2023-01-29 23:38:11.000000 pysubs2-1.6.1/tests/test_time.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2825 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_tmp.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2731 2023-04-02 14:02:19.000000 pysubs2-1.6.1/tests/test_vtt.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1894 2022-12-28 16:13:18.000000 pysubs2-1.6.1/tests/test_whisper.py
```

### Comparing `pysubs2-1.6.0/LICENSE.txt` & `pysubs2-1.6.1/LICENSE.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2014-2022 Tomas Karabela
+Copyright (c) 2014-2023 Tomas Karabela
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pysubs2-1.6.0/PKG-INFO` & `pysubs2-1.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubs2
-Version: 1.6.0
+Version: 1.6.1
 Summary: A library for editing subtitle files
 Home-page: https://github.com/tkarabela/pysubs2
 Author: Tomas Karabela
 Author-email: tkarabela@seznam.cz
 License: MIT
 Project-URL: Documentation, https://pysubs2.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/tkarabela/pysubs2/issues
@@ -29,20 +29,23 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 pysubs2
 =======
 
 
-.. image:: https://circleci.com/gh/tkarabela/pysubs2.svg?style=shield
+.. image:: https://img.shields.io/github/actions/workflow/status/tkarabela/pysubs2/main.yml?branch=master
     :alt: pysubs2 build master branch
-    :target: https://circleci.com/gh/tkarabela/pysubs2
+    :target: https://github.com/tkarabela/pysubs2/actions
+.. image:: https://img.shields.io/codecov/c/github/tkarabela/pysubs2
+    :alt: pysubs2 test code coverage
+    :target: https://app.codecov.io/github/tkarabela/pysubs2
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :alt: MyPy checked
-    :target: https://circleci.com/gh/tkarabela/pysubs2
+    :target: https://github.com/tkarabela/pysubs2/actions
 .. image:: https://img.shields.io/pypi/v/pysubs2.svg?style=flat-square
     :alt: PyPI - Version
     :target: https://pypi.org/project/pysubs2/
 .. image:: https://img.shields.io/pypi/status/pysubs2.svg?style=flat-square
     :alt: PyPI - Status
     :target: https://pypi.org/project/pysubs2/
 .. image:: https://img.shields.io/pypi/pyversions/pysubs2.svg?style=flat-square
@@ -72,9 +75,10 @@
     subs = pysubs2.load("my_subtitles.ass", encoding="utf-8")
     subs.shift(s=2.5)
     for line in subs:
         line.text = "{\\be1}" + line.text
     subs.save("my_subtitles_edited.ass")
 
 To learn more, please `see the documentation <http://pysubs2.readthedocs.io>`_.
+If you'd like to contribute, see `CONTRIBUTING.md <CONTRIBUTING.md>`_.
 
 pysubs2 is licensed under the MIT license (see `LICENSE.txt <LICENSE.txt>`_).
```

### Comparing `pysubs2-1.6.0/README.rst` & `pysubs2-1.6.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 pysubs2
 =======
 
 
-.. image:: https://circleci.com/gh/tkarabela/pysubs2.svg?style=shield
+.. image:: https://img.shields.io/github/actions/workflow/status/tkarabela/pysubs2/main.yml?branch=master
     :alt: pysubs2 build master branch
-    :target: https://circleci.com/gh/tkarabela/pysubs2
+    :target: https://github.com/tkarabela/pysubs2/actions
+.. image:: https://img.shields.io/codecov/c/github/tkarabela/pysubs2
+    :alt: pysubs2 test code coverage
+    :target: https://app.codecov.io/github/tkarabela/pysubs2
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :alt: MyPy checked
-    :target: https://circleci.com/gh/tkarabela/pysubs2
+    :target: https://github.com/tkarabela/pysubs2/actions
 .. image:: https://img.shields.io/pypi/v/pysubs2.svg?style=flat-square
     :alt: PyPI - Version
     :target: https://pypi.org/project/pysubs2/
 .. image:: https://img.shields.io/pypi/status/pysubs2.svg?style=flat-square
     :alt: PyPI - Status
     :target: https://pypi.org/project/pysubs2/
 .. image:: https://img.shields.io/pypi/pyversions/pysubs2.svg?style=flat-square
@@ -41,9 +44,10 @@
     subs = pysubs2.load("my_subtitles.ass", encoding="utf-8")
     subs.shift(s=2.5)
     for line in subs:
         line.text = "{\\be1}" + line.text
     subs.save("my_subtitles_edited.ass")
 
 To learn more, please `see the documentation <http://pysubs2.readthedocs.io>`_.
+If you'd like to contribute, see `CONTRIBUTING.md <CONTRIBUTING.md>`_.
 
 pysubs2 is licensed under the MIT license (see `LICENSE.txt <LICENSE.txt>`_).
```

### Comparing `pysubs2-1.6.0/pysubs2/cli.py` & `pysubs2-1.6.1/pysubs2/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 from .common import VERSION
 import logging
 
 
 def positive_float(s: str) -> float:
     x = float(s)
     if not x > 0:
-        raise argparse.ArgumentTypeError("%r is not a positive number" % s)
+        raise argparse.ArgumentTypeError(f"{s!r} is not a positive number")
     return x
 
+
 def character_encoding(s: str) -> str:
     try:
         codecs.lookup(s)
         return s
     except LookupError:
-        raise argparse.ArgumentError(None, "unknown character encoding: {}".format(s))
+        raise argparse.ArgumentError(None, f"unknown character encoding: {s}")
 
 
 def time(s: str) -> int:
     d = {}
     for v, k in re.findall(r"(\d*\.?\d*)(ms|m|s|h)", s):
         d[k] = float(v)
     return make_time(**d)  # type: ignore  # Argument 1 has incomp. type "**Dict[Any, float]"; expected "Optional[int]"
@@ -59,15 +60,15 @@
                                                          python -m pysubs2 --transform-framerate 25 23.976 *.srt"""))
 
         parser.add_argument("files", nargs="*", metavar="FILE",
                             help="Input subtitle files. Can be in SubStation Alpha (*.ass, *.ssa), SubRip (*.srt), "
                                  "MicroDVD (*.sub) or other supported format. When no files are specified, "
                                  "pysubs2 will work as a pipe, reading from standard input and writing to standard output.")
 
-        parser.add_argument("-v", "--version", action="version", version="pysubs2 %s" % VERSION)
+        parser.add_argument("-v", "--version", action="version", version=f"pysubs2 {VERSION}")
 
         parser.add_argument("-f", "--from", choices=FORMAT_IDENTIFIERS, dest="input_format",
                             help="By default, subtitle format is detected from the file. This option can be used to "
                                  "skip autodetection and force specific format. Generally, it should never be needed.")
         parser.add_argument("-t", "--to", choices=FORMAT_IDENTIFIERS, dest="output_format",
                             help="Convert subtitle files to given format. By default, each file is saved in its "
                                  "original format.")
```

### Comparing `pysubs2-1.6.0/pysubs2/common.py` & `pysubs2-1.6.1/pysubs2/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,11 +54,11 @@
         return SSA_ALIGNMENT[self.value - 1]
 
 
 SSA_ALIGNMENT = (1, 2, 3, 9, 10, 11, 5, 6, 7)
 
 
 #: Version of the pysubs2 library.
-VERSION = "1.6.0"
+VERSION = "1.6.1"
 
 
 IntOrFloat = Union[int, float]
```

### Comparing `pysubs2-1.6.0/pysubs2/exceptions.py` & `pysubs2-1.6.1/pysubs2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.6.0/pysubs2/formatbase.py` & `pysubs2-1.6.1/pysubs2/formatbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional
 import io
+import pysubs2
 
 
 class FormatBase:
     """
     Base class for subtitle format implementations.
 
     How to implement a new subtitle format:
@@ -14,15 +15,15 @@
     4. (optional) Add your file extension and class to :data:`pysubs2.formats.FILE_EXTENSION_TO_FORMAT_IDENTIFIER`.
 
     After finishing these steps, you can call :meth:`SSAFile.load()` and :meth:`SSAFile.save()` with your
     format, including autodetection from content and file extension (if you provided these).
 
     """
     @classmethod
-    def from_file(cls, subs, fp: io.TextIOBase, format_: str, **kwargs):
+    def from_file(cls, subs: "pysubs2.SSAFile", fp: io.TextIOBase, format_: str, **kwargs):
         """
         Load subtitle file into an empty SSAFile.
 
         If the parser autodetects framerate, set it as ``subs.fps``.
 
         Arguments:
             subs (SSAFile): An empty :class:`SSAFile`.
@@ -37,15 +38,15 @@
         Raises:
             pysubs2.exceptions.UnknownFPSError: Framerate was not provided and cannot
                 be detected.
         """
         raise NotImplementedError("Parsing is not supported for this format")
 
     @classmethod
-    def to_file(cls, subs, fp: io.TextIOBase, format_: str, **kwargs):
+    def to_file(cls, subs: "pysubs2.SSAFile", fp: io.TextIOBase, format_: str, **kwargs):
         """
         Write SSAFile into a file.
 
         If you need framerate and it is not passed in keyword arguments,
         use ``subs.fps``.
 
         Arguments:
@@ -62,15 +63,15 @@
         Raises:
             pysubs2.exceptions.UnknownFPSError: Framerate was not provided and
                 ``subs.fps is None``.
         """
         raise NotImplementedError("Writing is not supported for this format")
 
     @classmethod
-    def guess_format(self, text: str) -> Optional[str]:
+    def guess_format(cls, text: str) -> Optional[str]:
         """
         Return format identifier of recognized format, or None.
 
         Arguments:
             text (str): Content of subtitle file. When the file is long,
                 this may be only its first few thousand characters.
```

### Comparing `pysubs2-1.6.0/pysubs2/formats.py` & `pysubs2-1.6.1/pysubs2/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     if format_ not in FORMAT_IDENTIFIER_TO_FORMAT_CLASS:
         raise UnknownFormatIdentifierError(format_)
 
     for ext, f in FILE_EXTENSION_TO_FORMAT_IDENTIFIER.items():
         if f == format_:
             return ext
 
-    raise RuntimeError("No file extension for format %r" % format_)
+    raise RuntimeError(f"No file extension for format {format_!r}")
 
 
 def autodetect_format(content: str) -> str:
     """Return format identifier for given fragment or raise FormatAutodetectionError."""
     formats = set()
     for impl in FORMAT_IDENTIFIER_TO_FORMAT_CLASS.values():
         guess = impl.guess_format(content)
@@ -73,8 +73,8 @@
             formats.add(guess)
 
     if len(formats) == 1:
         return formats.pop()
     elif not formats:
         raise FormatAutodetectionError("No suitable formats")
     else:
-        raise FormatAutodetectionError("Multiple suitable formats (%r)" % formats)
+        raise FormatAutodetectionError(f"Multiple suitable formats ({formats!r})")
```

### Comparing `pysubs2-1.6.0/pysubs2/jsonformat.py` & `pysubs2-1.6.1/pysubs2/jsonformat.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.6.0/pysubs2/microdvd.py` & `pysubs2-1.6.1/pysubs2/microdvd.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
                                           "the MicroDVD file.")
 
             start, end = map(partial(frames_to_ms, fps=fps), (fstart, fend))
 
             def prepare_text(text):
                 text = text.replace("|", r"\N")
 
-                def style_replacer(match):
+                def style_replacer(match: re.Match) -> str:
                     tags = [c for c in "biu" if c in match.group(0)]
-                    return "{%s}" % "".join(r"\%s1" % c for c in tags)
+                    return "{%s}" % "".join(f"\\{c}1" for c in tags)
 
                 text = re.sub(r"\{[Yy]:[^}]+\}", style_replacer, text)
                 text = re.sub(r"\{[Ff]:([^}]+)\}", r"{\\fn\1}", text)
                 text = re.sub(r"\{[Ss]:([^}]+)\}", r"{\\fs\1}", text)
                 text = re.sub(r"\{P:(\d+),(\d+)\}", r"{\\pos(\1,\2)}", text)
 
                 return text.strip()
@@ -78,15 +78,15 @@
         if fps is None:
             fps = subs.fps
 
         if fps is None:
             raise UnknownFPSError("Framerate must be specified when writing MicroDVD.")
         to_frames = partial(ms_to_frames, fps=fps)
 
-        def is_entirely_italic(line):
+        def is_entirely_italic(line: SSAEvent) -> bool:
             style = subs.styles.get(line.style, SSAStyle.DEFAULT_STYLE)
             for fragment, sty in parse_tags(line.text, style, subs.styles):
                 fragment = fragment.replace(r"\h", " ")
                 fragment = fragment.replace(r"\n", "\n")
                 fragment = fragment.replace(r"\N", "\n")
                 if not sty.italic and fragment and not fragment.isspace():
                     return False
```

### Comparing `pysubs2-1.6.0/pysubs2/mpl2.py` & `pysubs2-1.6.1/pysubs2/mpl2.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.6.0/pysubs2/ssaevent.py` & `pysubs2-1.6.1/pysubs2/ssaevent.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.6.0/pysubs2/ssafile.py` & `pysubs2-1.6.1/pysubs2/ssafile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-try:
-    from collections import abc
-except ImportError:
-    import collections as abc  # type: ignore[no-redef]
+from collections.abc import MutableSequence
 import io
 from io import open
 from itertools import chain
 import os.path
 import logging
 from typing import Optional, List, Dict, Iterable, Any, overload, Iterator
 
@@ -13,16 +10,15 @@
 from .formats import autodetect_format, get_format_class, get_format_identifier
 from .substation import is_valid_field_content
 from .ssaevent import SSAEvent
 from .ssastyle import SSAStyle
 from .time import make_time, ms_to_str
 
 
-# TODO fix mypy errors regarding SSAFile
-class SSAFile(abc.MutableSequence):
+class SSAFile(MutableSequence):
     """
     Subtitle file in SubStation Alpha format.
 
     This class has a list-like interface which exposes :attr:`SSAFile.events`,
     list of subtitles in the file::
 
         subs = SSAFile.load("subtitles.srt")
@@ -283,15 +279,15 @@
             out_fps (float)
 
         Raises:
             ValueError: Non-positive framerate given.
 
         """
         if in_fps <= 0 or out_fps <= 0:
-            raise ValueError("Framerates must be positive, cannot transform %f -> %f" % (in_fps, out_fps))
+            raise ValueError(f"Framerates must be positive, cannot transform {in_fps} -> {out_fps}")
 
         ratio = in_fps / out_fps
         for line in self:
             line.start = int(round(line.start * ratio))
             line.end = int(round(line.end * ratio))
 
     # ------------------------------------------------------------------------
@@ -309,19 +305,19 @@
         Raises:
             KeyError: No style named old_name.
             ValueError: new_name is not a legal name (cannot use commas)
                 or new_name is taken.
 
         """
         if old_name not in self.styles:
-            raise KeyError("Style %r not found" % old_name)
+            raise KeyError(f"Style {old_name!r} not found")
         if new_name in self.styles:
-            raise ValueError("There is already a style called %r" % new_name)
+            raise ValueError(f"There is already a style called {new_name!r}")
         if not is_valid_field_content(new_name):
-            raise ValueError("%r is not a valid name" % new_name)
+            raise ValueError(f"{new_name!r} is not a valid name")
 
         self.styles[new_name] = self.styles[old_name]
         del self.styles[old_name]
 
         for line in self:
             # XXX also handle \r override tag
             if line.style == old_name:
```

### Comparing `pysubs2-1.6.0/pysubs2/ssastyle.py` & `pysubs2-1.6.1/pysubs2/ssastyle.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.6.0/pysubs2/subrip.py` & `pysubs2-1.6.1/pysubs2/subrip.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 import warnings
+from typing import List
 
+import pysubs2
 from .formatbase import FormatBase
 from .ssaevent import SSAEvent
 from .ssastyle import SSAStyle
 from .substation import parse_tags
 from .exceptions import ContentNotUsable
 from .time import ms_to_times, make_time, TIMESTAMP, timestamp_to_ms
 
@@ -21,15 +23,15 @@
         """Convert ms to 'HH:MM:SS,mmm'"""
         if ms < 0:
             ms = 0
         if ms > MAX_REPRESENTABLE_TIME:
             warnings.warn("Overflow in SubRip timestamp, clamping to MAX_REPRESENTABLE_TIME", RuntimeWarning)
             ms = MAX_REPRESENTABLE_TIME
         h, m, s, ms = ms_to_times(ms)
-        return "%02d:%02d:%02d,%03d" % (h, m, s, ms)
+        return f"{h:02d}:{m:02d}:{s:02d},{ms:03d}"
 
     @staticmethod
     def timestamp_to_ms(groups):
         return timestamp_to_ms(groups)
 
     @classmethod
     def guess_format(cls, text):
@@ -139,30 +141,35 @@
 
             body = []
             if keep_ssa_tags:
                 body.append(text)
             else:
                 for fragment, sty in parse_tags(text, style, subs.styles):
                     if apply_styles:
-                        if sty.italic: fragment = "<i>%s</i>" % fragment
-                        if sty.underline: fragment = "<u>%s</u>" % fragment
-                        if sty.strikeout: fragment = "<s>%s</s>" % fragment
+                        if sty.italic: fragment = f"<i>{fragment}</i>"
+                        if sty.underline: fragment = f"<u>{fragment}</u>"
+                        if sty.strikeout: fragment = f"<s>{fragment}</s>"
                     if sty.drawing: raise ContentNotUsable
                     body.append(fragment)
 
             return re.sub("\n+", "\n", "".join(body).strip())
 
-        visible_lines = (line for line in subs if not line.is_comment)
+        visible_lines = cls._get_visible_lines(subs)
 
         lineno = 1
         for line in visible_lines:
             start = cls.ms_to_timestamp(line.start)
             end = cls.ms_to_timestamp(line.end)
             try:
                 text = prepare_text(line.text, subs.styles.get(line.style, SSAStyle.DEFAULT_STYLE))
             except ContentNotUsable:
                 continue
 
-            print("%d" % lineno, file=fp) # Python 2.7 compat
+            print(lineno, file=fp)
             print(start, "-->", end, file=fp)
             print(text, end="\n\n", file=fp)
             lineno += 1
+
+    @classmethod
+    def _get_visible_lines(cls, subs: "pysubs2.SSAFile") -> List["pysubs2.SSAEvent"]:
+        visible_lines = [line for line in subs if not line.is_comment]
+        return visible_lines
```

### Comparing `pysubs2-1.6.0/pysubs2/substation.py` & `pysubs2-1.6.1/pysubs2/substation.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,18 @@
     "ssa": ["marked", "start", "end", "style", "name", "marginl", "marginr", "marginv", "effect", "text"]
 }
 
 #: Largest timestamp allowed in SubStation, ie. 9:59:59.99.
 MAX_REPRESENTABLE_TIME = make_time(h=10) - 10
 
 def color_to_ass_rgba(c: Color) -> str:
-    return "&H%08X" % ((c.a << 24) | (c.b << 16) | (c.g << 8) | c.r)
+    return f"&H{((c.a << 24) | (c.b << 16) | (c.g << 8) | c.r):08X}"
 
 def color_to_ssa_rgb(c: Color) -> str:
-    return "%d" % ((c.b << 16) | (c.g << 8) | c.r)
+    return f"{((c.b << 16) | (c.g << 8) | c.r)}"
 
 def rgba_to_color(s: str) -> Color:
     if s[0] == '&':
         x = int(s[2:], base=16)
     else:
         x = int(s)
     r = x & 0xff
@@ -106,23 +106,24 @@
     if styles is None:
         styles = {}
     
     fragments = SSAEvent.OVERRIDE_SEQUENCE.split(text)
     if len(fragments) == 1:
         return [(text, style)]
     
-    def apply_overrides(all_overrides):
+    def apply_overrides(all_overrides: str) -> SSAStyle:
         s = style.copy()
         for tag in re.findall(r"\\[ibusp][0-9]|\\r[a-zA-Z_0-9 ]*", all_overrides):
             if tag == r"\r":
                 s = style.copy() # reset to original line style
             elif tag.startswith(r"\r"):
                 name = tag[2:]
-                if name in styles:
-                    s = styles[name].copy() # reset to named style
+                if name in styles:  # type: ignore[operator]
+                    # reset to named style
+                    s = styles[name].copy()  # type: ignore[index]
             else:
                 if "i" in tag: s.italic = "1" in tag
                 elif "b" in tag: s.bold = "1" in tag
                 elif "u" in tag: s.underline = "1" in tag
                 elif "s" in tag: s.strikeout = "1" in tag
                 elif "p" in tag:
                     try:
@@ -154,15 +155,15 @@
             ms = MAX_REPRESENTABLE_TIME
 
         h, m, s, ms = ms_to_times(ms)
 
         # Aegisub does rounding, see https://github.com/Aegisub/Aegisub/blob/6f546951b4f004da16ce19ba638bf3eedefb9f31/libaegisub/include/libaegisub/ass/time.h#L32
         cs = ((ms + 5) - (ms + 5) % 10) // 10
 
-        return "%01d:%02d:%02d.%02d" % (h, m, s, cs)
+        return f"{h:01d}:{m:02d}:{s:02d}.{cs:02d}"
 
     @classmethod
     def guess_format(cls, text):
         """See :meth:`pysubs2.formats.FormatBase.guess_format()`"""
         if re.search(r"V4\+ Styles", text, re.IGNORECASE):
             return "ass"
         elif re.search(r"V4 Styles", text, re.IGNORECASE):
@@ -187,15 +188,15 @@
                 else:
                     sign = 1
 
                 m = TIMESTAMP.match(v)
                 if m is None:
                     m = TIMESTAMP_SHORT.match(v)
                     if m is None:
-                        raise ValueError("Failed to parse timestamp: {!r}".format(v))
+                        raise ValueError(f"Failed to parse timestamp: {v!r}")
 
                 return sign * timestamp_to_ms(m.groups())
             elif "color" in f:
                 v = v.strip()
                 return rgba_to_color(v)
             elif f in {"bold", "underline", "italic", "strikeout"}:
                 return v == "-1"
@@ -321,15 +322,15 @@
             for k, v in subs.aegisub_project.items():
                 print(k, v, sep=": ", file=fp)
 
         def field_to_string(f: str, v: Any, line: Union[SSAEvent, SSAStyle]):
             if f in {"start", "end"}:
                 return cls.ms_to_timestamp(v)
             elif f == "marked":
-                return "Marked=%d" % v
+                return f"Marked={v:d}"
             elif f == "alignment":
                 if isinstance(v, Alignment):
                     alignment = v
                 else:
                     warnings.warn("The 'alignment' attribute of SSAStyle should be an Alignment instance, using plain int is deprecated", DeprecationWarning)
                     alignment = Alignment(v)
 
@@ -343,34 +344,34 @@
                 return str(v)
             elif isinstance(v, Color):
                 if format_ == "ass":
                     return color_to_ass_rgba(v)
                 else:
                     return color_to_ssa_rgb(v)
             else:
-                raise TypeError("Unexpected type when writing a SubStation field {!r} for line {!r}".format(f, line))
+                raise TypeError(f"Unexpected type when writing a SubStation field {f!r} for line {line!r}")
 
         print("\n[V4+ Styles]" if format_ == "ass" else "\n[V4 Styles]", file=fp)
         print(STYLE_FORMAT_LINE[format_], file=fp)
         for name, sty in subs.styles.items():
             fields = [field_to_string(f, getattr(sty, f), sty) for f in STYLE_FIELDS[format_]]
-            print("Style: %s" % name, *fields, sep=",", file=fp)
+            print(f"Style: {name}", *fields, sep=",", file=fp)
 
         if subs.fonts_opaque:
             print("\n[Fonts]", file=fp)
             for font_name, font_lines in sorted(subs.fonts_opaque.items()):
-                print("fontname: {}".format(font_name), file=fp)
+                print(f"fontname: {font_name}", file=fp)
                 for line in font_lines:
                     print(line, file=fp)
                 print(file=fp)
 
         if subs.graphics_opaque:
             print("\n[Graphics]", file=fp)
             for picture_name, picture_lines in sorted(subs.graphics_opaque.items()):
-                print("filename: {}".format(picture_name), file=fp)
+                print(f"filename: {picture_name}", file=fp)
                 for line in picture_lines:
                     print(line, file=fp)
                 print(file=fp)
 
         print("\n[Events]", file=fp)
         print(EVENT_FORMAT_LINE[format_], file=fp)
         for ev in subs.events:
```

### Comparing `pysubs2-1.6.0/pysubs2/time.py` & `pysubs2-1.6.1/pysubs2/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         Number of milliseconds (rounded to int).
         
     Raises:
         ValueError: fps was negative or zero.
     
     """
     if fps <= 0:
-        raise ValueError("Framerate must be positive number (%f)." % fps)
+        raise ValueError(f"Framerate must be a positive number ({fps}).")
 
     return int(round(frames * (1000 / fps)))
 
 
 def ms_to_frames(ms: IntOrFloat, fps: float) -> int:
     """
     Convert milliseconds to number of frames.
@@ -115,15 +115,15 @@
         Number of frames (int).
         
     Raises:
         ValueError: fps was negative or zero.
     
     """
     if fps <= 0:
-        raise ValueError("Framerate must be positive number (%f)." % fps)
+        raise ValueError(f"Framerate must be a positive number ({fps}).")
 
     return int(round((ms / 1000) * fps))
 
 
 def ms_to_times(ms: IntOrFloat) -> Tuple[int, int, int, int]:
     """
     Convert milliseconds to normalized tuple (h, m, s, ms).
```

### Comparing `pysubs2-1.6.0/pysubs2/tmp.py` & `pysubs2-1.6.1/pysubs2/tmp.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """Convert ms to 'HH:MM:SS'"""
         if ms < 0:
             ms = 0
         if ms > MAX_REPRESENTABLE_TIME:
             warnings.warn("Overflow in TMP timestamp, clamping to MAX_REPRESENTABLE_TIME", RuntimeWarning)
             ms = MAX_REPRESENTABLE_TIME
         h, m, s, _ = ms_to_times(ms)
-        return "%02d:%02d:%02d" % (h, m, s)
+        return f"{h:02d}:{m:02d}:{s:02d}"
 
     @classmethod
     def guess_format(cls, text):
         """See :meth:`pysubs2.formats.FormatBase.guess_format()`"""
         if "[Script Info]" in text or "[V4+ Styles]" in text:
             # disambiguation vs. SSA/ASS
             return None
@@ -86,17 +86,17 @@
             body = []
             skip = False
             for fragment, sty in parse_tags(text, style, subs.styles):
                 fragment = fragment.replace(r"\h", " ")
                 fragment = fragment.replace(r"\n", "\n")
                 fragment = fragment.replace(r"\N", "\n")
                 if apply_styles:
-                    if sty.italic: fragment = "<i>%s</i>" % fragment
-                    if sty.underline: fragment = "<u>%s</u>" % fragment
-                    if sty.strikeout: fragment = "<s>%s</s>" % fragment
+                    if sty.italic: fragment = f"<i>{fragment}</i>"
+                    if sty.underline: fragment = f"<u>{fragment}</u>"
+                    if sty.strikeout: fragment = f"<s>{fragment}</s>"
                 if sty.drawing: skip = True
                 body.append(fragment)
 
             if skip:
                 return ""
             else:
                 return re.sub("\n+", "\n", "".join(body).strip())
```

### Comparing `pysubs2-1.6.0/pysubs2/webvtt.py` & `pysubs2-1.6.1/pysubs2/webvtt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import re
+from typing import List
+
+import pysubs2
 from .subrip import SubripFormat
 from .time import make_time
 
 
 class WebVTTFormat(SubripFormat):
     """
     Web Video Text Tracks (WebVTT) subtitle format implementation
@@ -36,7 +39,13 @@
     def to_file(cls, subs, fp, format_, **kwargs):
         """
         See :meth:`pysubs2.formats.FormatBase.to_file()`
         """
         print("WEBVTT\n", file=fp)
         return super(WebVTTFormat, cls).to_file(
             subs=subs, fp=fp, format_=format_, **kwargs)
+
+    @classmethod
+    def _get_visible_lines(cls, subs: "pysubs2.SSAFile") -> List["pysubs2.SSAEvent"]:
+        visible_lines = [line for line in subs if not line.is_comment]
+        visible_lines.sort(key=lambda e: e.start)
+        return visible_lines
```

### Comparing `pysubs2-1.6.0/pysubs2/whisper.py` & `pysubs2-1.6.1/pysubs2/whisper.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.6.0/pysubs2.egg-info/PKG-INFO` & `pysubs2-1.6.1/pysubs2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubs2
-Version: 1.6.0
+Version: 1.6.1
 Summary: A library for editing subtitle files
 Home-page: https://github.com/tkarabela/pysubs2
 Author: Tomas Karabela
 Author-email: tkarabela@seznam.cz
 License: MIT
 Project-URL: Documentation, https://pysubs2.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/tkarabela/pysubs2/issues
@@ -29,20 +29,23 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 pysubs2
 =======
 
 
-.. image:: https://circleci.com/gh/tkarabela/pysubs2.svg?style=shield
+.. image:: https://img.shields.io/github/actions/workflow/status/tkarabela/pysubs2/main.yml?branch=master
     :alt: pysubs2 build master branch
-    :target: https://circleci.com/gh/tkarabela/pysubs2
+    :target: https://github.com/tkarabela/pysubs2/actions
+.. image:: https://img.shields.io/codecov/c/github/tkarabela/pysubs2
+    :alt: pysubs2 test code coverage
+    :target: https://app.codecov.io/github/tkarabela/pysubs2
 .. image:: http://www.mypy-lang.org/static/mypy_badge.svg
     :alt: MyPy checked
-    :target: https://circleci.com/gh/tkarabela/pysubs2
+    :target: https://github.com/tkarabela/pysubs2/actions
 .. image:: https://img.shields.io/pypi/v/pysubs2.svg?style=flat-square
     :alt: PyPI - Version
     :target: https://pypi.org/project/pysubs2/
 .. image:: https://img.shields.io/pypi/status/pysubs2.svg?style=flat-square
     :alt: PyPI - Status
     :target: https://pypi.org/project/pysubs2/
 .. image:: https://img.shields.io/pypi/pyversions/pysubs2.svg?style=flat-square
@@ -72,9 +75,10 @@
     subs = pysubs2.load("my_subtitles.ass", encoding="utf-8")
     subs.shift(s=2.5)
     for line in subs:
         line.text = "{\\be1}" + line.text
     subs.save("my_subtitles_edited.ass")
 
 To learn more, please `see the documentation <http://pysubs2.readthedocs.io>`_.
+If you'd like to contribute, see `CONTRIBUTING.md <CONTRIBUTING.md>`_.
 
 pysubs2 is licensed under the MIT license (see `LICENSE.txt <LICENSE.txt>`_).
```

### Comparing `pysubs2-1.6.0/setup.cfg` & `pysubs2-1.6.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -37,11 +37,18 @@
 [options.entry_points]
 console_scripts = 
 	pysubs2 = pysubs2.cli:__main__
 
 [mypy]
 files = pysubs2, tests/test_*.py
 
+[coverage:run]
+branch = True
+
+[coverage:report]
+show_missing = True
+skip_covered = True
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

