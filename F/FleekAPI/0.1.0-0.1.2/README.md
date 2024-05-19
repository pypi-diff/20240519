# Comparing `tmp/fleekapi-0.1.0.tar.gz` & `tmp/fleekapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.1.0.tar", last modified: Sun May 19 07:18:59 2024, max compression
+gzip compressed data, was "fleekapi-0.1.2.tar", last modified: Sun May 19 12:13:59 2024, max compression
```

## Comparing `fleekapi-0.1.0.tar` & `fleekapi-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:18:59.689878 fleekapi-0.1.0/
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:18:59.685878 fleekapi-0.1.0/FleekAPI/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:05:58.000000 fleekapi-0.1.0/FleekAPI/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.0/FleekAPI/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.0/FleekAPI/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.0/FleekAPI/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:18:59.689878 fleekapi-0.1.0/FleekAPI.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)      872 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 07:18:59.000000 fleekapi-0.1.0/FleekAPI.egg-info/top_level.txt
--rw-r--r--   0 hasan     (1002) hasan     (1002)      872 2024-05-19 07:18:59.689878 fleekapi-0.1.0/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       11 2024-05-18 10:33:36.000000 fleekapi-0.1.0/README.md
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 07:18:59.693878 fleekapi-0.1.0/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3979 2024-05-19 07:18:56.000000 fleekapi-0.1.0/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:13:59.560019 fleekapi-0.1.2/
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:13:59.548019 fleekapi-0.1.2/FleekAPI/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        0 2024-05-19 07:05:58.000000 fleekapi-0.1.2/FleekAPI/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.2/FleekAPI/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.2/FleekAPI/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.2/FleekAPI/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 12:13:59.556019 fleekapi-0.1.2/FleekAPI.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7725 2024-05-19 12:13:59.000000 fleekapi-0.1.2/FleekAPI.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 12:13:59.000000 fleekapi-0.1.2/FleekAPI.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 12:13:59.000000 fleekapi-0.1.2/FleekAPI.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 12:13:59.000000 fleekapi-0.1.2/FleekAPI.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 12:13:59.000000 fleekapi-0.1.2/FleekAPI.egg-info/top_level.txt
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7725 2024-05-19 12:13:59.556019 fleekapi-0.1.2/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     6863 2024-05-19 12:10:49.000000 fleekapi-0.1.2/README.md
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 12:13:59.560019 fleekapi-0.1.2/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3979 2024-05-19 12:13:37.000000 fleekapi-0.1.2/setup.py
```

### Comparing `fleekapi-0.1.0/FleekAPI/app.py` & `fleekapi-0.1.2/FleekAPI/app.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.0/FleekAPI/middleware.py` & `fleekapi-0.1.2/FleekAPI/middleware.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.0/FleekAPI/response.py` & `fleekapi-0.1.2/FleekAPI/response.py`

 * *Files identical despite different names*

### Comparing `fleekapi-0.1.0/setup.py` & `fleekapi-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'FleekAPI'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.0'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
```

