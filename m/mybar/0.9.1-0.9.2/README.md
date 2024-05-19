# Comparing `tmp/mybar-0.9.1.tar.gz` & `tmp/mybar-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mybar-0.9.1.tar", last modified: Sun Nov 26 09:05:41 2023, max compression
+gzip compressed data, was "mybar-0.9.2.tar", last modified: Sun Nov 26 09:19:49 2023, max compression
```

## Comparing `mybar-0.9.1.tar` & `mybar-0.9.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-11-26 09:05:41.406718 mybar-0.9.1/
--rw-r--r--   0 sam       (1000) sam       (1000)     1077 2022-12-15 03:39:16.000000 mybar-0.9.1/LICENSE
--rw-r--r--   0 sam       (1000) sam       (1000)     6901 2023-11-26 09:05:41.406718 mybar-0.9.1/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)     5999 2023-11-26 09:05:25.000000 mybar-0.9.1/README.rst
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-11-26 09:05:41.404718 mybar-0.9.1/mybar/
--rw-r--r--   0 sam       (1000) sam       (1000)     1956 2023-11-24 15:15:58.000000 mybar-0.9.1/mybar/__init__.py
--rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-07-01 04:06:09.000000 mybar-0.9.1/mybar/__main__.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-07-01 04:06:09.000000 mybar-0.9.1/mybar/_setups.py
--rw-r--r--   0 sam       (1000) sam       (1000)     3963 2023-11-06 06:37:21.000000 mybar-0.9.1/mybar/_types.py
--rw-r--r--   0 sam       (1000) sam       (1000)    47790 2023-11-21 11:53:16.000000 mybar-0.9.1/mybar/bar.py
--rw-r--r--   0 sam       (1000) sam       (1000)    18234 2023-11-24 13:05:53.000000 mybar-0.9.1/mybar/cli.py
--rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-11-06 06:37:21.000000 mybar-0.9.1/mybar/constants.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2942 2023-11-06 06:37:21.000000 mybar-0.9.1/mybar/errors.py
--rw-r--r--   0 sam       (1000) sam       (1000)    28801 2023-11-21 11:15:58.000000 mybar-0.9.1/mybar/field.py
--rw-r--r--   0 sam       (1000) sam       (1000)    14130 2023-11-06 06:37:21.000000 mybar-0.9.1/mybar/field_funcs.py
--rw-r--r--   0 sam       (1000) sam       (1000)    27898 2023-11-06 06:37:21.000000 mybar-0.9.1/mybar/formatting.py
--rw-r--r--   0 sam       (1000) sam       (1000)      214 2023-01-13 00:44:41.000000 mybar-0.9.1/mybar/icon.py
--rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-07-01 04:06:09.000000 mybar-0.9.1/mybar/log.py
--rw-r--r--   0 sam       (1000) sam       (1000)     2380 2023-11-14 20:02:50.000000 mybar-0.9.1/mybar/namespaces.py
--rw-r--r--   0 sam       (1000) sam       (1000)    59496 2023-11-09 03:52:31.000000 mybar-0.9.1/mybar/parse_conf.py
--rw-r--r--   0 sam       (1000) sam       (1000)     8157 2023-11-14 18:33:46.000000 mybar-0.9.1/mybar/utils.py
-drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-11-26 09:05:41.406718 mybar-0.9.1/mybar.egg-info/
--rw-r--r--   0 sam       (1000) sam       (1000)     6901 2023-11-26 09:05:41.000000 mybar-0.9.1/mybar.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) sam       (1000)      472 2023-11-26 09:05:41.000000 mybar-0.9.1/mybar.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-11-26 09:05:41.000000 mybar-0.9.1/mybar.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-11-26 09:05:41.000000 mybar-0.9.1/mybar.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-11-26 09:05:41.000000 mybar-0.9.1/mybar.egg-info/top_level.txt
--rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-11-24 15:11:19.000000 mybar-0.9.1/pyproject.toml
--rw-r--r--   0 sam       (1000) sam       (1000)        7 2022-12-15 03:39:16.000000 mybar-0.9.1/requirements.txt
--rw-r--r--   0 sam       (1000) sam       (1000)     1004 2023-11-26 09:05:41.407718 mybar-0.9.1/setup.cfg
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-11-26 09:19:49.133834 mybar-0.9.2/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1077 2022-12-15 03:39:16.000000 mybar-0.9.2/LICENSE
+-rw-r--r--   0 sam       (1000) sam       (1000)     6907 2023-11-26 09:19:49.133834 mybar-0.9.2/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)     5999 2023-11-26 09:05:25.000000 mybar-0.9.2/README.rst
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-11-26 09:19:49.132834 mybar-0.9.2/mybar/
+-rw-r--r--   0 sam       (1000) sam       (1000)     1956 2023-11-26 09:17:58.000000 mybar-0.9.2/mybar/__init__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      336 2023-07-01 04:06:09.000000 mybar-0.9.2/mybar/__main__.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1863 2023-07-01 04:06:09.000000 mybar-0.9.2/mybar/_setups.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     3963 2023-11-06 06:37:21.000000 mybar-0.9.2/mybar/_types.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    47790 2023-11-21 11:53:16.000000 mybar-0.9.2/mybar/bar.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    18234 2023-11-24 13:05:53.000000 mybar-0.9.2/mybar/cli.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     1000 2023-11-06 06:37:21.000000 mybar-0.9.2/mybar/constants.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2942 2023-11-06 06:37:21.000000 mybar-0.9.2/mybar/errors.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    28801 2023-11-21 11:15:58.000000 mybar-0.9.2/mybar/field.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    14130 2023-11-06 06:37:21.000000 mybar-0.9.2/mybar/field_funcs.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    27898 2023-11-06 06:37:21.000000 mybar-0.9.2/mybar/formatting.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      214 2023-01-13 00:44:41.000000 mybar-0.9.2/mybar/icon.py
+-rw-r--r--   0 sam       (1000) sam       (1000)      361 2023-07-01 04:06:09.000000 mybar-0.9.2/mybar/log.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     2380 2023-11-14 20:02:50.000000 mybar-0.9.2/mybar/namespaces.py
+-rw-r--r--   0 sam       (1000) sam       (1000)    59496 2023-11-09 03:52:31.000000 mybar-0.9.2/mybar/parse_conf.py
+-rw-r--r--   0 sam       (1000) sam       (1000)     8157 2023-11-14 18:33:46.000000 mybar-0.9.2/mybar/utils.py
+drwxr-xr-x   0 sam       (1000) sam       (1000)        0 2023-11-26 09:19:49.133834 mybar-0.9.2/mybar.egg-info/
+-rw-r--r--   0 sam       (1000) sam       (1000)     6907 2023-11-26 09:19:49.000000 mybar-0.9.2/mybar.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) sam       (1000)      472 2023-11-26 09:19:49.000000 mybar-0.9.2/mybar.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        1 2023-11-26 09:19:49.000000 mybar-0.9.2/mybar.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2023-11-26 09:19:49.000000 mybar-0.9.2/mybar.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)        6 2023-11-26 09:19:49.000000 mybar-0.9.2/mybar.egg-info/top_level.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)       81 2023-11-24 15:11:19.000000 mybar-0.9.2/pyproject.toml
+-rw-r--r--   0 sam       (1000) sam       (1000)        7 2022-12-15 03:39:16.000000 mybar-0.9.2/requirements.txt
+-rw-r--r--   0 sam       (1000) sam       (1000)     1010 2023-11-26 09:19:49.134833 mybar-0.9.2/setup.cfg
```

### Comparing `mybar-0.9.1/LICENSE` & `mybar-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/PKG-INFO` & `mybar-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.9.1
-Summary: attr: mybar.__description__
+Version: 0.9.2
+Summary: Craft highly customizable status bars with ease.
 Home-page: https://github.com/akyuute/mybar
-Author: attr: mybar.__author__
+Author: akyuute
 License: MIT
 Project-URL: GitHub: repo, https://github.com/akyuute/mybar
 Keywords: status bar,bar,command line,i3,threads,async,API
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
```

### Comparing `mybar-0.9.1/README.rst` & `mybar-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/__init__.py` & `mybar-0.9.2/mybar/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 :copyright: (c) 2021-present by akyuute.
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'mybar'
 __description__ = "Craft highly customizable status bars with ease."
 __url__ = "https://github.com/akyuute/mybar"
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __author__ = "akyuute"
 __license__ = 'MIT'
 __copyright__ = "Copyright (c) 2021-present akyuute"
 
 
 __all__ = (
     'Bar',
```

### Comparing `mybar-0.9.1/mybar/_setups.py` & `mybar-0.9.2/mybar/_setups.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/_types.py` & `mybar-0.9.2/mybar/_types.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/bar.py` & `mybar-0.9.2/mybar/bar.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/cli.py` & `mybar-0.9.2/mybar/cli.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/constants.py` & `mybar-0.9.2/mybar/constants.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/errors.py` & `mybar-0.9.2/mybar/errors.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/field.py` & `mybar-0.9.2/mybar/field.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/field_funcs.py` & `mybar-0.9.2/mybar/field_funcs.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/formatting.py` & `mybar-0.9.2/mybar/formatting.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/namespaces.py` & `mybar-0.9.2/mybar/namespaces.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/parse_conf.py` & `mybar-0.9.2/mybar/parse_conf.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar/utils.py` & `mybar-0.9.2/mybar/utils.py`

 * *Files identical despite different names*

### Comparing `mybar-0.9.1/mybar.egg-info/PKG-INFO` & `mybar-0.9.2/mybar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mybar
-Version: 0.9.1
-Summary: attr: mybar.__description__
+Version: 0.9.2
+Summary: Craft highly customizable status bars with ease.
 Home-page: https://github.com/akyuute/mybar
-Author: attr: mybar.__author__
+Author: akyuute
 License: MIT
 Project-URL: GitHub: repo, https://github.com/akyuute/mybar
 Keywords: status bar,bar,command line,i3,threads,async,API
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
```

### Comparing `mybar-0.9.1/setup.cfg` & `mybar-0.9.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = mybar
 version = attr: mybar.__version__
-author = attr: mybar.__author__
-description = attr: mybar.__description__
+author = akyuute
+description = Craft highly customizable status bars with ease.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/akyuute/mybar
 copyright = Copyright (c) 2021-present by akyuute
 project_urls = 
 	GitHub: repo = https://github.com/akyuute/mybar
 classifiers =
```

