# Comparing `tmp/pymenu_cli-1.0.4.tar.gz` & `tmp/pymenu_cli-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymenu_cli-1.0.4.tar", last modified: Sun May 19 18:07:16 2024, max compression
+gzip compressed data, was "pymenu_cli-1.0.5.tar", last modified: Sun May 19 18:13:25 2024, max compression
```

## Comparing `pymenu_cli-1.0.4.tar` & `pymenu_cli-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:07:16.011323 pymenu_cli-1.0.4/
--rw-r--r--   0 moraneus   (501) staff       (20)     3023 2024-05-19 18:07:16.011036 pymenu_cli-1.0.4/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)     2753 2024-05-19 18:06:42.000000 pymenu_cli-1.0.4/README.md
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:07:16.008799 pymenu_cli-1.0.4/pymenu_cli/
--rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.4/pymenu_cli/__init__.py
--rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.4/pymenu_cli/menu.py
-drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:07:16.010025 pymenu_cli-1.0.4/pymenu_cli.egg-info/
--rw-r--r--   0 moraneus   (501) staff       (20)     3023 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/PKG-INFO
--rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/SOURCES.txt
--rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/dependency_links.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/entry_points.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-19 18:07:15.000000 pymenu_cli-1.0.4/pymenu_cli.egg-info/top_level.txt
--rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-19 18:07:16.011372 pymenu_cli-1.0.4/setup.cfg
--rw-r--r--   0 moraneus   (501) staff       (20)      644 2024-05-19 18:01:22.000000 pymenu_cli-1.0.4/setup.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:13:25.783700 pymenu_cli-1.0.5/
+-rw-r--r--   0 moraneus   (501) staff       (20)     3013 2024-05-19 18:13:25.783496 pymenu_cli-1.0.5/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)     2743 2024-05-19 18:11:26.000000 pymenu_cli-1.0.5/README.md
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:13:25.782007 pymenu_cli-1.0.5/pymenu_cli/
+-rw-r--r--   0 moraneus   (501) staff       (20)        0 2024-05-17 18:45:03.000000 pymenu_cli-1.0.5/pymenu_cli/__init__.py
+-rw-r--r--   0 moraneus   (501) staff       (20)     5117 2024-05-17 18:51:29.000000 pymenu_cli-1.0.5/pymenu_cli/menu.py
+drwxr-xr-x   0 moraneus   (501) staff       (20)        0 2024-05-19 18:13:25.783280 pymenu_cli-1.0.5/pymenu_cli.egg-info/
+-rw-r--r--   0 moraneus   (501) staff       (20)     3013 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/PKG-INFO
+-rw-r--r--   0 moraneus   (501) staff       (20)      233 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)        1 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       52 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/entry_points.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       11 2024-05-19 18:13:25.000000 pymenu_cli-1.0.5/pymenu_cli.egg-info/top_level.txt
+-rw-r--r--   0 moraneus   (501) staff       (20)       38 2024-05-19 18:13:25.783743 pymenu_cli-1.0.5/setup.cfg
+-rw-r--r--   0 moraneus   (501) staff       (20)      644 2024-05-19 18:12:37.000000 pymenu_cli-1.0.5/setup.py
```

### Comparing `pymenu_cli-1.0.4/PKG-INFO` & `pymenu_cli-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pymenu-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for creating interactive CLI menus
 Home-page: https://github.com/moraneus/pymenu-cli
 Author: Moraneus
 Author-email: moraneus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pymenu-cli
 
-![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi%20package)
+![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
 ## Features
```

### Comparing `pymenu_cli-1.0.4/README.md` & `pymenu_cli-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pymenu-cli
 
-![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi%20package)
+![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
 ## Features
```

### Comparing `pymenu_cli-1.0.4/pymenu_cli/menu.py` & `pymenu_cli-1.0.5/pymenu_cli/menu.py`

 * *Files identical despite different names*

### Comparing `pymenu_cli-1.0.4/pymenu_cli.egg-info/PKG-INFO` & `pymenu_cli-1.0.5/pymenu_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pymenu-cli
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python library for creating interactive CLI menus
 Home-page: https://github.com/moraneus/pymenu-cli
 Author: Moraneus
 Author-email: moraneus@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # pymenu-cli
 
-![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi%20package)
+![PyPI](https://img.shields.io/pypi/v/pymenu-cli?label=pypi)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pymenu-cli)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 pymenu-cli is a Python library that simplifies the creation of interactive command-line interface (CLI) menus. It provides a convenient way to define hierarchical menu structures and associate actions with menu items.
 
 ## Features
```

### Comparing `pymenu_cli-1.0.4/setup.py` & `pymenu_cli-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymenu-cli',
-    version='1.0.4',
+    version='1.0.5',
     description='A Python library for creating interactive CLI menus',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Moraneus',
     author_email='moraneus@gmail.com',
     url='https://github.com/moraneus/pymenu-cli',
     packages=find_packages(),
```

