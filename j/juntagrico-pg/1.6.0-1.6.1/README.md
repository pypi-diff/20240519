# Comparing `tmp/juntagrico_pg-1.6.0.tar.gz` & `tmp/juntagrico_pg-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juntagrico_pg-1.6.0.tar", last modified: Wed May 15 19:41:10 2024, max compression
+gzip compressed data, was "juntagrico_pg-1.6.1.tar", last modified: Sun May 19 17:45:57 2024, max compression
```

## Comparing `juntagrico_pg-1.6.0.tar` & `juntagrico_pg-1.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.526907 juntagrico_pg-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/migrations/0002_auto_20191007_1031.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.518907 juntagrico_pg-1.6.0/juntagrico_pg/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/templates/jpg/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/templates/jpg/home.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.518907 juntagrico_pg-1.6.0/juntagrico_pg/templates/juntagrico/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/templates/juntagrico/menu/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/templates/juntagrico/menu/admin.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/util/output.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/juntagrico_pg/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:41:10.522907 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 19:41:10.000000 juntagrico_pg-1.6.0/juntagrico_pg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 19:41:04.000000 juntagrico_pg-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:41:10.526907 juntagrico_pg-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.455809 juntagrico_pg-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-19 17:45:57.455809 juntagrico_pg-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.451809 juntagrico_pg-1.6.1/juntagrico_pg/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.451809 juntagrico_pg-1.6.1/juntagrico_pg/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/migrations/0002_auto_20191007_1031.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.447809 juntagrico_pg-1.6.1/juntagrico_pg/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.451809 juntagrico_pg-1.6.1/juntagrico_pg/templates/jpg/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/templates/jpg/home.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.447809 juntagrico_pg-1.6.1/juntagrico_pg/templates/juntagrico/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.451809 juntagrico_pg-1.6.1/juntagrico_pg/templates/juntagrico/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/templates/juntagrico/menu/admin.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.455809 juntagrico_pg-1.6.1/juntagrico_pg/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/util/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/juntagrico_pg/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:45:57.455809 juntagrico_pg-1.6.1/juntagrico_pg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-19 17:45:57.000000 juntagrico_pg-1.6.1/juntagrico_pg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-19 17:45:57.000000 juntagrico_pg-1.6.1/juntagrico_pg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:45:57.000000 juntagrico_pg-1.6.1/juntagrico_pg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 17:45:57.000000 juntagrico_pg-1.6.1/juntagrico_pg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 17:45:57.000000 juntagrico_pg-1.6.1/juntagrico_pg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 17:45:53.000000 juntagrico_pg-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:45:57.455809 juntagrico_pg-1.6.1/setup.cfg
```

### Comparing `juntagrico_pg-1.6.0/LICENSE` & `juntagrico_pg-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/PKG-INFO` & `juntagrico_pg-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juntagrico-pg
-Version: 1.6.0
+Version: 1.6.1
 Summary: postgres db editor for juntagrico
 Author-email: juntagrico <python@juntagrico.org>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,15 +185,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: juntagrico>=1.6.0
-Requires-Dist: pgspecial<2.0,>=1.12.1
+Requires-Dist: pgspecial<3.0,>=1.12.1
 Requires-Dist: texttable<2.0,>=1.6.3
 
 # juntagrico-pg
 
 
 [![juntagrico-ci](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/02bb5f131cc157fcc4b9/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-pg/maintainability)
```

### Comparing `juntagrico_pg-1.6.0/README.md` & `juntagrico_pg-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/juntagrico_pg/migrations/0001_initial.py` & `juntagrico_pg-1.6.1/juntagrico_pg/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/juntagrico_pg/templates/jpg/home.html` & `juntagrico_pg-1.6.1/juntagrico_pg/templates/jpg/home.html`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/juntagrico_pg/util/output.py` & `juntagrico_pg-1.6.1/juntagrico_pg/util/output.py`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/juntagrico_pg/views.py` & `juntagrico_pg-1.6.1/juntagrico_pg/views.py`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/juntagrico_pg.egg-info/PKG-INFO` & `juntagrico_pg-1.6.1/juntagrico_pg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juntagrico-pg
-Version: 1.6.0
+Version: 1.6.1
 Summary: postgres db editor for juntagrico
 Author-email: juntagrico <python@juntagrico.org>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -185,15 +185,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: juntagrico>=1.6.0
-Requires-Dist: pgspecial<2.0,>=1.12.1
+Requires-Dist: pgspecial<3.0,>=1.12.1
 Requires-Dist: texttable<2.0,>=1.6.3
 
 # juntagrico-pg
 
 
 [![juntagrico-ci](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml/badge.svg?branch=main&event=push)](https://github.com/juntagrico/juntagrico-pg/actions/workflows/juntagrico-ci.yml)
 [![Maintainability](https://api.codeclimate.com/v1/badges/02bb5f131cc157fcc4b9/maintainability)](https://codeclimate.com/github/juntagrico/juntagrico-pg/maintainability)
```

### Comparing `juntagrico_pg-1.6.0/juntagrico_pg.egg-info/SOURCES.txt` & `juntagrico_pg-1.6.1/juntagrico_pg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `juntagrico_pg-1.6.0/pyproject.toml` & `juntagrico_pg-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     {name = "juntagrico", email = "python@juntagrico.org"},
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 dependencies = [
     "juntagrico>=1.6.0",
-    "pgspecial>=1.12.1,<2.0",
+    "pgspecial>=1.12.1,<3.0",
     "texttable>=1.6.3,<2.0"
 ]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Environment :: Web Environment',
     'Framework :: Django',
     'Framework :: Django :: 4.2',
```

