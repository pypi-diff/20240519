# Comparing `tmp/pytubefix-5.5rc3.tar.gz` & `tmp/pytubefix-5.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.5rc3.tar", last modified: Tue May 14 00:59:34 2024, max compression
+gzip compressed data, was "pytubefix-5.6rc1.tar", last modified: Sun May 19 14:16:35 2024, max compression
```

## Comparing `pytubefix-5.5rc3.tar` & `pytubefix-5.6rc1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-14 00:59:34.134936 pytubefix-5.5rc3/
--rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/LICENSE
--rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/MANIFEST.in
--rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-14 00:59:34.134936 pytubefix-5.5rc3/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     3011 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/README.md
--rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-05-14 00:56:03.000000 pytubefix-5.5rc3/pyproject.toml
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-14 00:59:34.126936 pytubefix-5.5rc3/pytubefix/
--rw-rw-r--   0 juan      (1000) juan      (1000)      657 2024-05-14 00:55:54.000000 pytubefix-5.5rc3/pytubefix/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    22728 2024-05-14 00:55:54.000000 pytubefix-5.5rc3/pytubefix/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6593 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/chapters.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16972 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      781 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/colors.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-14 00:59:34.130936 pytubefix-5.5rc3/pytubefix/contrib/
--rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/contrib/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/contrib/channel.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/contrib/playlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/contrib/search.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4099 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18343 2024-05-14 00:55:54.000000 pytubefix-5.5rc3/pytubefix/extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     9943 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    17742 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/innertube.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     4276 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/jsinterp.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1339 2024-05-14 00:55:54.000000 pytubefix-5.5rc3/pytubefix/keymoments.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/monostate.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5948 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    14359 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     8736 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16049 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/pytubefix/streams.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-05-14 00:56:10.000000 pytubefix-5.5rc3/pytubefix/version.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-14 00:59:34.134936 pytubefix-5.5rc3/pytubefix.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-14 00:59:34.000000 pytubefix-5.5rc3/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     1053 2024-05-14 00:59:34.000000 pytubefix-5.5rc3/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-14 00:59:34.000000 pytubefix-5.5rc3/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-05-14 00:59:34.000000 pytubefix-5.5rc3/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-05-14 00:59:34.000000 pytubefix-5.5rc3/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-14 00:59:34.134936 pytubefix-5.5rc3/setup.cfg
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-14 00:59:34.130936 pytubefix-5.5rc3/tests/
--rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_captions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_cipher.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_extract.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_helpers.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_itags.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_main.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_metadata.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_parser.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_query.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_request.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-05-14 00:46:42.000000 pytubefix-5.5rc3/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-19 14:16:35.853046 pytubefix-5.6rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-19 14:16:35.853046 pytubefix-5.6rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3011 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-05-19 14:07:18.000000 pytubefix-5.6rc1/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-19 14:16:35.841047 pytubefix-5.6rc1/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      657 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    22728 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6593 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16972 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      781 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-19 14:16:35.845047 pytubefix-5.6rc1/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4099 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18343 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9943 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17743 2024-05-19 14:05:49.000000 pytubefix-5.6rc1/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4276 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1339 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/keymoments.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5948 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14359 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8736 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16049 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-05-19 14:06:46.000000 pytubefix-5.6rc1/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-19 14:16:35.853046 pytubefix-5.6rc1/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-19 14:16:35.000000 pytubefix-5.6rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1053 2024-05-19 14:16:35.000000 pytubefix-5.6rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-19 14:16:35.000000 pytubefix-5.6rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-05-19 14:16:35.000000 pytubefix-5.6rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-05-19 14:16:35.000000 pytubefix-5.6rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-19 14:16:35.853046 pytubefix-5.6rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-19 14:16:35.849047 pytubefix-5.6rc1/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-05-19 14:03:48.000000 pytubefix-5.6rc1/tests/test_streams.py
```

### Comparing `pytubefix-5.5rc3/LICENSE` & `pytubefix-5.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/PKG-INFO` & `pytubefix-5.6rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.5rc3
+Version: 5.6rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc3 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.6rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.5rc3/README.md` & `pytubefix-5.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pyproject.toml` & `pytubefix-5.6rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.5-rc3"
+version = "5.6-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.5rc3/pytubefix/__init__.py` & `pytubefix-5.6rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/__main__.py` & `pytubefix-5.6rc1/pytubefix/__main__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/captions.py` & `pytubefix-5.6rc1/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/chapters.py` & `pytubefix-5.6rc1/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/cipher.py` & `pytubefix-5.6rc1/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/cli.py` & `pytubefix-5.6rc1/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/colors.py` & `pytubefix-5.6rc1/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/contrib/channel.py` & `pytubefix-5.6rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/contrib/playlist.py` & `pytubefix-5.6rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/contrib/search.py` & `pytubefix-5.6rc1/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/exceptions.py` & `pytubefix-5.6rc1/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/extract.py` & `pytubefix-5.6rc1/pytubefix/extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/helpers.py` & `pytubefix-5.6rc1/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/innertube.py` & `pytubefix-5.6rc1/pytubefix/innertube.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
         'header': {
             'User-Agent': 'com.google.android.youtube/',
         },
         'api_key': 'AIzaSyAO_FJ2SlqU8Q4STEHLGCilw_Y9_11qcW8',
         'require_js_player': False
     },
     'MWEB': {
-        'inertube_context': {
+        'innertube_context': {
             'context': {
                 'client': {
                     'clientName': 'MWEB',
                     'clientVersion': '2.20220801.00.00',
                 }
             }
         },
```

### Comparing `pytubefix-5.5rc3/pytubefix/itags.py` & `pytubefix-5.6rc1/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/jsinterp.py` & `pytubefix-5.6rc1/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/keymoments.py` & `pytubefix-5.6rc1/pytubefix/keymoments.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/metadata.py` & `pytubefix-5.6rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/parser.py` & `pytubefix-5.6rc1/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/query.py` & `pytubefix-5.6rc1/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/request.py` & `pytubefix-5.6rc1/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix/streams.py` & `pytubefix-5.6rc1/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.6rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.5rc3
+Version: 5.6rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc3 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.6rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.5rc3/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.6rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_captions.py` & `pytubefix-5.6rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_cipher.py` & `pytubefix-5.6rc1/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_cli.py` & `pytubefix-5.6rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_exceptions.py` & `pytubefix-5.6rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_extract.py` & `pytubefix-5.6rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_helpers.py` & `pytubefix-5.6rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_main.py` & `pytubefix-5.6rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_parser.py` & `pytubefix-5.6rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_query.py` & `pytubefix-5.6rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_request.py` & `pytubefix-5.6rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.5rc3/tests/test_streams.py` & `pytubefix-5.6rc1/tests/test_streams.py`

 * *Files identical despite different names*

