# Comparing `tmp/clean_alchemy-0.1.13.tar.gz` & `tmp/clean_alchemy-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_alchemy-0.1.13.tar", last modified: Sun May 19 09:26:37 2024, max compression
+gzip compressed data, was "clean_alchemy-0.1.14.tar", last modified: Sun May 19 20:29:34 2024, max compression
```

## Comparing `clean_alchemy-0.1.13.tar` & `clean_alchemy-0.1.14.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-19 09:26:37.675991 clean_alchemy-0.1.13/
--rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean_alchemy-0.1.13/LICENSE
--rw-r--r--   0 swords     (501) staff       (20)     3232 2024-05-19 09:26:37.675729 clean_alchemy-0.1.13/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      812 2024-05-18 14:19:28.000000 clean_alchemy-0.1.13/README.md
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-19 09:26:37.673219 clean_alchemy-0.1.13/clean_alchemy/
--rw-r--r--   0 swords     (501) staff       (20)      241 2024-05-19 07:17:55.000000 clean_alchemy-0.1.13/clean_alchemy/__init__.py
--rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-19 07:00:32.000000 clean_alchemy-0.1.13/clean_alchemy/base.py
--rw-r--r--   0 swords     (501) staff       (20)      782 2024-05-19 07:07:15.000000 clean_alchemy-0.1.13/clean_alchemy/base_dao.py
--rw-r--r--   0 swords     (501) staff       (20)      506 2024-05-18 18:40:28.000000 clean_alchemy-0.1.13/clean_alchemy/base_entity.py
--rw-r--r--   0 swords     (501) staff       (20)     3824 2024-05-19 07:37:24.000000 clean_alchemy-0.1.13/clean_alchemy/base_repo.py
--rw-r--r--   0 swords     (501) staff       (20)     2196 2024-05-19 07:31:40.000000 clean_alchemy-0.1.13/clean_alchemy/base_service.py
--rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean_alchemy-0.1.13/clean_alchemy/config.py
-drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-19 09:26:37.674571 clean_alchemy-0.1.13/clean_alchemy.egg-info/
--rw-r--r--   0 swords     (501) staff       (20)     3232 2024-05-19 09:26:37.000000 clean_alchemy-0.1.13/clean_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 swords     (501) staff       (20)      394 2024-05-19 09:26:37.000000 clean_alchemy-0.1.13/clean_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-19 09:26:37.000000 clean_alchemy-0.1.13/clean_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 swords     (501) staff       (20)      918 2024-05-19 09:26:37.000000 clean_alchemy-0.1.13/clean_alchemy.egg-info/requires.txt
--rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-19 09:26:37.000000 clean_alchemy-0.1.13/clean_alchemy.egg-info/top_level.txt
--rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-19 09:26:37.676100 clean_alchemy-0.1.13/setup.cfg
--rw-r--r--   0 swords     (501) staff       (20)      972 2024-05-19 09:26:24.000000 clean_alchemy-0.1.13/setup.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-19 20:29:34.717027 clean_alchemy-0.1.14/
+-rw-r--r--   0 swords     (501) staff       (20)    11357 2024-05-15 18:56:06.000000 clean_alchemy-0.1.14/LICENSE
+-rw-r--r--   0 swords     (501) staff       (20)     3232 2024-05-19 20:29:34.716775 clean_alchemy-0.1.14/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      812 2024-05-18 14:19:28.000000 clean_alchemy-0.1.14/README.md
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-19 20:29:34.714571 clean_alchemy-0.1.14/clean_alchemy/
+-rw-r--r--   0 swords     (501) staff       (20)      264 2024-05-19 18:49:22.000000 clean_alchemy-0.1.14/clean_alchemy/__init__.py
+-rw-r--r--   0 swords     (501) staff       (20)      445 2024-05-19 07:00:32.000000 clean_alchemy-0.1.14/clean_alchemy/base.py
+-rw-r--r--   0 swords     (501) staff       (20)      479 2024-05-19 19:37:01.000000 clean_alchemy-0.1.14/clean_alchemy/base_dao.py
+-rw-r--r--   0 swords     (501) staff       (20)      216 2024-05-19 19:42:00.000000 clean_alchemy-0.1.14/clean_alchemy/base_entity.py
+-rw-r--r--   0 swords     (501) staff       (20)     8280 2024-05-19 20:27:55.000000 clean_alchemy-0.1.14/clean_alchemy/base_repo.py
+-rw-r--r--   0 swords     (501) staff       (20)     6135 2024-05-19 19:30:01.000000 clean_alchemy-0.1.14/clean_alchemy/base_service.py
+-rw-r--r--   0 swords     (501) staff       (20)      357 2024-05-15 18:56:06.000000 clean_alchemy-0.1.14/clean_alchemy/config.py
+drwxr-xr-x   0 swords     (501) staff       (20)        0 2024-05-19 20:29:34.715629 clean_alchemy-0.1.14/clean_alchemy.egg-info/
+-rw-r--r--   0 swords     (501) staff       (20)     3232 2024-05-19 20:29:34.000000 clean_alchemy-0.1.14/clean_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 swords     (501) staff       (20)      394 2024-05-19 20:29:34.000000 clean_alchemy-0.1.14/clean_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 swords     (501) staff       (20)        1 2024-05-19 20:29:34.000000 clean_alchemy-0.1.14/clean_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 swords     (501) staff       (20)      918 2024-05-19 20:29:34.000000 clean_alchemy-0.1.14/clean_alchemy.egg-info/requires.txt
+-rw-r--r--   0 swords     (501) staff       (20)       14 2024-05-19 20:29:34.000000 clean_alchemy-0.1.14/clean_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 swords     (501) staff       (20)       38 2024-05-19 20:29:34.717098 clean_alchemy-0.1.14/setup.cfg
+-rw-r--r--   0 swords     (501) staff       (20)      975 2024-05-19 20:28:53.000000 clean_alchemy-0.1.14/setup.py
```

### Comparing `clean_alchemy-0.1.13/LICENSE` & `clean_alchemy-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_alchemy-0.1.13/PKG-INFO` & `clean_alchemy-0.1.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.13
+Version: 0.1.14
 Summary: A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `clean_alchemy-0.1.13/README.md` & `clean_alchemy-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `clean_alchemy-0.1.13/clean_alchemy.egg-info/PKG-INFO` & `clean_alchemy-0.1.14/clean_alchemy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-alchemy
-Version: 0.1.13
+Version: 0.1.14
 Summary: A framework for implementing Clean Architecture using SQLAlchemy for FastAPI.
 Home-page: https://github.com/davidswords/clean-alchemy
 Author: David Swords
 Author-email: furuer_svette.0k@icloud.com
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `clean_alchemy-0.1.13/clean_alchemy.egg-info/requires.txt` & `clean_alchemy-0.1.14/clean_alchemy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clean_alchemy-0.1.13/setup.py` & `clean_alchemy-0.1.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 
+
 def read_requirements(file_name):
     with open(file_name) as f:
         return f.read().splitlines()
 
+
 setup(
     name="clean-alchemy",
-    version="0.1.13",
+    version="0.1.14",
     packages=find_packages(exclude=["tests*", "build*"]),
     install_requires=read_requirements("requirements.txt"),
     extras_require={
         "dev": read_requirements("requirements-dev.txt"),
     },
     author="David Swords",
     author_email="furuer_svette.0k@icloud.com",
@@ -21,8 +23,8 @@
     url="https://github.com/davidswords/clean-alchemy",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.12.3",
-)
+)
```

