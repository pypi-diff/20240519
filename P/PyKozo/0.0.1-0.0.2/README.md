# Comparing `tmp/pykozo-0.0.1.tar.gz` & `tmp/pykozo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykozo-0.0.1.tar", last modified: Sun May 19 19:06:02 2024, max compression
+gzip compressed data, was "pykozo-0.0.2.tar", last modified: Sun May 19 21:11:54 2024, max compression
```

## Comparing `pykozo-0.0.1.tar` & `pykozo-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mano      (1000) mano      (1001)        0 2024-05-19 19:06:02.564788 pykozo-0.0.1/
--rw-r--r--   0 mano      (1000) mano      (1001)     1110 2024-05-19 18:14:14.000000 pykozo-0.0.1/LICENSE
--rw-r--r--   0 mano      (1000) mano      (1001)      289 2024-05-19 19:06:02.564788 pykozo-0.0.1/PKG-INFO
-drwxr-xr-x   0 mano      (1000) mano      (1001)        0 2024-05-19 19:06:02.561454 pykozo-0.0.1/PyKozo.egg-info/
--rw-r--r--   0 mano      (1000) mano      (1001)      289 2024-05-19 19:06:02.000000 pykozo-0.0.1/PyKozo.egg-info/PKG-INFO
--rw-r--r--   0 mano      (1000) mano      (1001)      192 2024-05-19 19:06:02.000000 pykozo-0.0.1/PyKozo.egg-info/SOURCES.txt
--rw-r--r--   0 mano      (1000) mano      (1001)        1 2024-05-19 19:06:02.000000 pykozo-0.0.1/PyKozo.egg-info/dependency_links.txt
--rw-r--r--   0 mano      (1000) mano      (1001)        7 2024-05-19 19:06:02.000000 pykozo-0.0.1/PyKozo.egg-info/top_level.txt
--rw-r--r--   0 mano      (1000) mano      (1001)      231 2024-05-19 18:24:01.000000 pykozo-0.0.1/README.md
-drwxr-xr-x   0 mano      (1000) mano      (1001)        0 2024-05-19 19:06:02.561454 pykozo-0.0.1/pykozo/
--rw-r--r--   0 mano      (1000) mano      (1001)       30 2024-05-19 18:05:38.000000 pykozo-0.0.1/pykozo/__init__.py
--rw-r--r--   0 mano      (1000) mano      (1001)    19752 2024-05-19 17:52:36.000000 pykozo-0.0.1/pykozo/pykozo.py
--rw-r--r--   0 mano      (1000) mano      (1001)       79 2024-05-19 19:06:02.564788 pykozo-0.0.1/setup.cfg
--rw-r--r--   0 mano      (1000) mano      (1001)      366 2024-05-19 18:33:35.000000 pykozo-0.0.1/setup.py
+drwxr-xr-x   0 mano      (1000) mano      (1001)        0 2024-05-19 21:11:54.505307 pykozo-0.0.2/
+-rw-r--r--   0 mano      (1000) mano      (1001)     1110 2024-05-19 18:14:14.000000 pykozo-0.0.2/LICENSE
+-rw-r--r--   0 mano      (1000) mano      (1001)      747 2024-05-19 21:11:54.505307 pykozo-0.0.2/PKG-INFO
+drwxr-xr-x   0 mano      (1000) mano      (1001)        0 2024-05-19 21:11:54.501973 pykozo-0.0.2/PyKozo.egg-info/
+-rw-r--r--   0 mano      (1000) mano      (1001)      747 2024-05-19 21:11:54.000000 pykozo-0.0.2/PyKozo.egg-info/PKG-INFO
+-rw-r--r--   0 mano      (1000) mano      (1001)      192 2024-05-19 21:11:54.000000 pykozo-0.0.2/PyKozo.egg-info/SOURCES.txt
+-rw-r--r--   0 mano      (1000) mano      (1001)        1 2024-05-19 21:11:54.000000 pykozo-0.0.2/PyKozo.egg-info/dependency_links.txt
+-rw-r--r--   0 mano      (1000) mano      (1001)        7 2024-05-19 21:11:54.000000 pykozo-0.0.2/PyKozo.egg-info/top_level.txt
+-rw-r--r--   0 mano      (1000) mano      (1001)      374 2024-05-19 19:11:40.000000 pykozo-0.0.2/README.md
+drwxr-xr-x   0 mano      (1000) mano      (1001)        0 2024-05-19 21:11:54.501973 pykozo-0.0.2/pykozo/
+-rw-r--r--   0 mano      (1000) mano      (1001)       30 2024-05-19 18:05:38.000000 pykozo-0.0.2/pykozo/__init__.py
+-rw-r--r--   0 mano      (1000) mano      (1001)    19752 2024-05-19 17:52:36.000000 pykozo-0.0.2/pykozo/pykozo.py
+-rw-r--r--   0 mano      (1000) mano      (1001)       79 2024-05-19 21:11:54.505307 pykozo-0.0.2/setup.cfg
+-rw-r--r--   0 mano      (1000) mano      (1001)      523 2024-05-19 21:11:23.000000 pykozo-0.0.2/setup.py
```

### Comparing `pykozo-0.0.1/LICENSE` & `pykozo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pykozo-0.0.1/pykozo/pykozo.py` & `pykozo-0.0.2/pykozo/pykozo.py`

 * *Files identical despite different names*

