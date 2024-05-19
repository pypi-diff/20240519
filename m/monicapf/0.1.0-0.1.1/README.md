# Comparing `tmp/monicapf-0.1.0.tar.gz` & `tmp/monicapf-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monicapf-0.1.0.tar", last modified: Sat May 18 11:25:03 2024, max compression
+gzip compressed data, was "monicapf-0.1.1.tar", last modified: Sun May 19 07:00:33 2024, max compression
```

## Comparing `monicapf-0.1.0.tar` & `monicapf-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-18 11:25:03.500386 monicapf-0.1.0/
--rw-r--r--   0 bilol     (1000) bilol     (1000)      708 2024-05-18 11:25:03.499386 monicapf-0.1.0/PKG-INFO
-drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-18 11:25:03.499386 monicapf-0.1.0/monicapf.egg-info/
--rw-r--r--   0 bilol     (1000) bilol     (1000)      708 2024-05-18 11:25:03.000000 monicapf-0.1.0/monicapf.egg-info/PKG-INFO
--rw-r--r--   0 bilol     (1000) bilol     (1000)      167 2024-05-18 11:25:03.000000 monicapf-0.1.0/monicapf.egg-info/SOURCES.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-18 11:25:03.000000 monicapf-0.1.0/monicapf.egg-info/dependency_links.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)      122 2024-05-18 11:25:03.000000 monicapf-0.1.0/monicapf.egg-info/requires.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-18 11:25:03.000000 monicapf-0.1.0/monicapf.egg-info/top_level.txt
--rw-r--r--   0 bilol     (1000) bilol     (1000)       38 2024-05-18 11:25:03.500386 monicapf-0.1.0/setup.cfg
--rw-r--r--   0 bilol     (1000) bilol     (1000)     3946 2024-05-18 11:22:50.000000 monicapf-0.1.0/setup.py
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:00:33.731516 monicapf-0.1.1/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     4337 2024-05-19 07:00:33.730516 monicapf-0.1.1/PKG-INFO
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3678 2024-05-19 07:00:18.000000 monicapf-0.1.1/README.md
+drwxr-xr-x   0 bilol     (1000) bilol     (1000)        0 2024-05-19 07:00:33.729516 monicapf-0.1.1/monicapf.egg-info/
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     4337 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/PKG-INFO
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      177 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/SOURCES.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/dependency_links.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)      122 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/requires.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)        1 2024-05-19 07:00:33.000000 monicapf-0.1.1/monicapf.egg-info/top_level.txt
+-rw-r--r--   0 bilol     (1000) bilol     (1000)       38 2024-05-19 07:00:33.731516 monicapf-0.1.1/setup.cfg
+-rw-r--r--   0 bilol     (1000) bilol     (1000)     3946 2024-05-19 07:00:09.000000 monicapf-0.1.1/setup.py
```

### Comparing `monicapf-0.1.0/setup.py` & `monicapf-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'monicapf'
 DESCRIPTION = 'Python Web Frmaework built for learning purposes. '
 URL = 'https://github.com/me/myproject'
 EMAIL = 'bilolabdumalikov1@gmail.com'
 AUTHOR = 'Abdumalikov Bilolbek'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "gunicorn==19.9.0",
     "Jinja2==3.1.4",
     "whitenoise==6.6.0",
     "WebOb==1.8.5",
```

