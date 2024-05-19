# Comparing `tmp/evernote2-1.0.2.tar.gz` & `tmp/evernote2-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evernote2-1.0.2.tar", last modified: Sun May 19 10:25:33 2024, max compression
+gzip compressed data, was "dist/evernote2-1.9.1.tar", last modified: Sun Nov 15 15:36:56 2020, max compression
```

## Comparing `evernote2-1.0.2.tar` & `evernote2-1.9.1.tar`

### file list

```diff
@@ -1,57 +1,16 @@
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.733952 evernote2-1.0.2/
--rw-r--r--   0 jackon     (501) staff       (20)     1455 2024-05-19 10:13:25.000000 evernote2-1.0.2/LICENSE
--rw-r--r--   0 jackon     (501) staff       (20)      167 2024-05-19 10:13:25.000000 evernote2-1.0.2/NOTICE
--rw-r--r--   0 jackon     (501) staff       (20)     4530 2024-05-19 10:25:33.733789 evernote2-1.0.2/PKG-INFO
--rw-r--r--   0 jackon     (501) staff       (20)     4242 2024-05-19 10:18:35.000000 evernote2-1.0.2/README.md
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.723381 evernote2-1.0.2/evernote2/
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.725257 evernote2-1.0.2/evernote2/api/
--rw-r--r--   0 jackon     (501) staff       (20)        0 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/api/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)     6513 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/api/client.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.725408 evernote2-1.0.2/evernote2/edam/
--rw-r--r--   0 jackon     (501) staff       (20)        0 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/__init__.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.725869 evernote2-1.0.2/evernote2/edam/error/
--rw-r--r--   0 jackon     (501) staff       (20)       34 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/error/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)      376 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/error/constants.py
--rw-r--r--   0 jackon     (501) staff       (20)    22931 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/error/ttypes.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.726417 evernote2-1.0.2/evernote2/edam/limits/
--rw-r--r--   0 jackon     (501) staff       (20)       34 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/limits/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)    10125 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/limits/constants.py
--rw-r--r--   0 jackon     (501) staff       (20)      450 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/limits/ttypes.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.728785 evernote2-1.0.2/evernote2/edam/notestore/
--rw-r--r--   0 jackon     (501) staff       (20)   927133 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/notestore/NoteStore.py
--rw-r--r--   0 jackon     (501) staff       (20)       47 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/notestore/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)      376 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/notestore/constants.py
--rw-r--r--   0 jackon     (501) staff       (20)   233152 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/notestore/ttypes.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.729941 evernote2-1.0.2/evernote2/edam/type/
--rw-r--r--   0 jackon     (501) staff       (20)       34 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/type/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)      687 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/type/constants.py
--rw-r--r--   0 jackon     (501) staff       (20)   339308 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/type/ttypes.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.731817 evernote2-1.0.2/evernote2/edam/userstore/
--rw-r--r--   0 jackon     (501) staff       (20)   178942 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/userstore/UserStore.py
--rw-r--r--   0 jackon     (501) staff       (20)       47 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/userstore/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)      424 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/userstore/constants.py
--rw-r--r--   0 jackon     (501) staff       (20)    43200 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/edam/userstore/ttypes.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.732030 evernote2-1.0.2/evernote2/nlp/
--rw-r--r--   0 jackon     (501) staff       (20)        0 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/nlp/__init__.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.732257 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/
--rw-r--r--   0 jackon     (501) staff       (20)        0 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/__init__.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.732790 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/algorithms/
--rw-r--r--   0 jackon     (501) staff       (20)        0 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/algorithms/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)      575 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/algorithms/html_cleaner.py
--rw-r--r--   0 jackon     (501) staff       (20)     1447 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/algorithms/space.py
--rw-r--r--   0 jackon     (501) staff       (20)     1471 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/nlp/text_cleansing_pipe/api.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.733278 evernote2-1.0.2/evernote2/tools/
--rw-r--r--   0 jackon     (501) staff       (20)        0 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/tools/__init__.py
--rw-r--r--   0 jackon     (501) staff       (20)     2233 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/tools/cleanse_notes_for_nlp.py
--rw-r--r--   0 jackon     (501) staff       (20)    11646 2024-05-19 10:13:25.000000 evernote2-1.0.2/evernote2/tools/export_notes.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.725019 evernote2-1.0.2/evernote2.egg-info/
--rw-r--r--   0 jackon     (501) staff       (20)     4530 2024-05-19 10:25:33.000000 evernote2-1.0.2/evernote2.egg-info/PKG-INFO
--rw-r--r--   0 jackon     (501) staff       (20)     1305 2024-05-19 10:25:33.000000 evernote2-1.0.2/evernote2.egg-info/SOURCES.txt
--rw-r--r--   0 jackon     (501) staff       (20)        1 2024-05-19 10:25:33.000000 evernote2-1.0.2/evernote2.egg-info/dependency_links.txt
--rw-r--r--   0 jackon     (501) staff       (20)        1 2024-05-19 10:25:33.000000 evernote2-1.0.2/evernote2.egg-info/not-zip-safe
--rw-r--r--   0 jackon     (501) staff       (20)       16 2024-05-19 10:25:33.000000 evernote2-1.0.2/evernote2.egg-info/requires.txt
--rw-r--r--   0 jackon     (501) staff       (20)       10 2024-05-19 10:25:33.000000 evernote2-1.0.2/evernote2.egg-info/top_level.txt
--rw-r--r--   0 jackon     (501) staff       (20)       38 2024-05-19 10:25:33.733994 evernote2-1.0.2/setup.cfg
--rw-r--r--   0 jackon     (501) staff       (20)     2101 2024-05-19 10:23:25.000000 evernote2-1.0.2/setup.py
-drwxr-xr-x   0 jackon     (501) staff       (20)        0 2024-05-19 10:25:33.733458 evernote2-1.0.2/tests/
--rw-r--r--   0 jackon     (501) staff       (20)      136 2024-05-19 10:13:25.000000 evernote2-1.0.2/tests/test_versions.py
+drwxrwxr-x   0 jackon    (1000) jackon    (1000)        0 2020-11-15 15:36:56.000000 evernote2-1.9.1/
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)       18 2020-11-15 10:44:20.000000 evernote2-1.9.1/MANIFEST.in
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)     1644 2020-11-15 15:36:56.000000 evernote2-1.9.1/PKG-INFO
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)     1038 2020-11-15 15:19:10.000000 evernote2-1.9.1/README.md
+drwxrwxr-x   0 jackon    (1000) jackon    (1000)        0 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2/
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)      217 2020-11-15 15:14:55.000000 evernote2-1.9.1/evernote2/__init__.py
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)      308 2020-11-15 15:36:36.000000 evernote2-1.9.1/evernote2/__version__.py
+drwxrwxr-x   0 jackon    (1000) jackon    (1000)        0 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)     1644 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/PKG-INFO
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)      273 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)        1 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)        1 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/not-zip-safe
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)       14 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/requires.txt
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)       10 2020-11-15 15:36:56.000000 evernote2-1.9.1/evernote2.egg-info/top_level.txt
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)       38 2020-11-15 15:36:56.000000 evernote2-1.9.1/setup.cfg
+-rw-rw-r--   0 jackon    (1000) jackon    (1000)     2062 2020-11-15 15:33:52.000000 evernote2-1.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `evernote2-1.0.2/setup.py` & `evernote2-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 
 from codecs import open
 
-from setuptools import setup, find_packages
+from setuptools import setup
+
 from setuptools.command.test import test as TestCommand
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 class PyTest(TestCommand):
     user_options = [('pytest-args=', 'a', "Arguments to pass into py.test")]
@@ -40,15 +41,15 @@
     readme = f.read()
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-packages = find_packages(include=['evernote2.*'])
+packages = ['evernote2']
 requires = read('requirements.txt')
 test_requirements = read('requirements-dev.txt')
 
 
 setup(
     name=about['__title__'],
     version=about['__version__'],
```

