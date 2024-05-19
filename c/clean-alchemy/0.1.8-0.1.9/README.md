# Comparing `tmp/clean-alchemy-0.1.8.tar.gz` & `tmp/clean-alchemy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean-alchemy-0.1.8.tar", last modified: Sat May 18 13:41:21 2024, max compression
+gzip compressed data, was "clean-alchemy-0.1.9.tar", last modified: Sat May 18 13:52:39 2024, max compression
```

## Comparing `clean-alchemy-0.1.8.tar` & `clean-alchemy-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.742069 clean-alchemy-0.1.8/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     1452 2024-05-18 13:41:21.741943 clean-alchemy-0.1.8/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/README.md
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.740516 clean-alchemy-0.1.8/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     1452 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      430 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)        4 2024-05-18 13:41:21.000000 clean-alchemy-0.1.8/clean_alchemy.egg-info/top_level.txt
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-18 13:41:21.742119 clean-alchemy-0.1.8/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)     1641 2024-05-18 13:40:55.000000 clean-alchemy-0.1.8/setup.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.740642 clean-alchemy-0.1.8/src/
--rw-r--r--   0 swords     (501) staff       (20)        0 2024-05-18 13:39:42.000000 clean-alchemy-0.1.8/src/__init__.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:41:21.741606 clean-alchemy-0.1.8/src/clean_alchemy/
--rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.8/src/clean_alchemy/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      449 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base.py
--rw-r--r--   0 swords     (501) staff       (20)      786 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_dao.py
--rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_ent.py
--rw-r--r--   0 swords     (501) staff       (20)     3653 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_rpo.py
--rw-r--r--   0 swords     (501) staff       (20)     2004 2024-05-18 13:39:56.000000 clean-alchemy-0.1.8/src/clean_alchemy/base_srv.py
--rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.8/src/clean_alchemy/config.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:52:39.382519 clean-alchemy-0.1.9/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.9/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     1452 2024-05-18 13:52:39.382374 clean-alchemy-0.1.9/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      883 2024-05-15 18:56:06.000000 clean-alchemy-0.1.9/README.md
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-18 13:52:39.382572 clean-alchemy-0.1.9/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)     1714 2024-05-18 13:52:18.000000 clean-alchemy-0.1.9/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:52:39.378633 clean-alchemy-0.1.9/src/
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:52:39.381354 clean-alchemy-0.1.9/src/clean_alchemy/
+-rw-r--r--   0 swords     (501) staff       (20)      195 2024-05-17 08:13:25.000000 clean-alchemy-0.1.9/src/clean_alchemy/__init__.py
+-rw-r--r--   0 swords     (501) staff       (20)      449 2024-05-18 13:39:56.000000 clean-alchemy-0.1.9/src/clean_alchemy/base.py
+-rw-r--r--   0 swords     (501) staff       (20)      786 2024-05-18 13:39:56.000000 clean-alchemy-0.1.9/src/clean_alchemy/base_dao.py
+-rw-r--r--   0 swords     (501) staff       (20)      500 2024-05-15 18:56:06.000000 clean-alchemy-0.1.9/src/clean_alchemy/base_ent.py
+-rw-r--r--   0 swords     (501) staff       (20)     3653 2024-05-18 13:39:56.000000 clean-alchemy-0.1.9/src/clean_alchemy/base_rpo.py
+-rw-r--r--   0 swords     (501) staff       (20)     2004 2024-05-18 13:39:56.000000 clean-alchemy-0.1.9/src/clean_alchemy/base_srv.py
+-rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean-alchemy-0.1.9/src/clean_alchemy/config.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-18 13:52:39.382174 clean-alchemy-0.1.9/src/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     1452 2024-05-18 13:52:39.000000 clean-alchemy-0.1.9/src/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      434 2024-05-18 13:52:39.000000 clean-alchemy-0.1.9/src/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-18 13:52:39.000000 clean-alchemy-0.1.9/src/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      516 2024-05-18 13:52:39.000000 clean-alchemy-0.1.9/src/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-18 13:52:39.000000 clean-alchemy-0.1.9/src/clean_alchemy.egg-info/top_level.txt
```

### Comparing `clean-alchemy-0.1.8/LICENSE` & `clean-alchemy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.8/PKG-INFO` & `clean-alchemy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.8/README.md` & `clean-alchemy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.8/clean_alchemy.egg-info/PKG-INFO` & `clean-alchemy-0.1.9/src/clean_alchemy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.8
+Version: 0.1.9
 Summary: A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clean-alchemy-0.1.8/clean_alchemy.egg-info/requires.txt` & `clean-alchemy-0.1.9/src/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.8/setup.py` & `clean-alchemy-0.1.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clean-alchemy",
-    version="0.1.8",
-    packages=find_packages(exclude=["tests*", "build*"]),
+    version="0.1.9",
+    packages=find_packages(where='src', exclude=["tests*", "build*"]),
+    package_dir={'': 'src'},
+    include_package_data=True,
     install_requires=[
         "annotated-types==0.6.0",
         "black==24.4.2",
         "click==8.1.7",
         "exceptiongroup==1.2.1",
         "factory-boy==3.3.0",
         "Faker==25.0.1",
```

### Comparing `clean-alchemy-0.1.8/src/clean_alchemy/base_dao.py` & `clean-alchemy-0.1.9/src/clean_alchemy/base_dao.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.8/src/clean_alchemy/base_rpo.py` & `clean-alchemy-0.1.9/src/clean_alchemy/base_rpo.py`

 * *Files identical despite different names*

### Comparing `clean-alchemy-0.1.8/src/clean_alchemy/base_srv.py` & `clean-alchemy-0.1.9/src/clean_alchemy/base_srv.py`

 * *Files identical despite different names*

