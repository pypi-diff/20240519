# Comparing `tmp/donware-0.1.7.tar.gz` & `tmp/donware-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donware-0.1.7.tar", last modified: Tue May 14 08:24:27 2024, max compression
+gzip compressed data, was "donware-0.1.8.tar", last modified: Sun May 19 04:22:49 2024, max compression
```

## Comparing `donware-0.1.7.tar` & `donware-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:27.280161 donware-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 08:23:58.000000 donware-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-14 08:23:58.000000 donware-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 08:24:27.276161 donware-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:23:58.000000 donware-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:27.276161 donware-0.1.7/donware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:23:58.000000 donware-0.1.7/donware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:27.276161 donware-0.1.7/donware/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:23:58.000000 donware-0.1.7/donware/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:27.276161 donware-0.1.7/donware/src/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:23:58.000000 donware-0.1.7/donware/src/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:27.276161 donware-0.1.7/donware/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 08:23:58.000000 donware-0.1.7/donware/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-14 08:23:58.000000 donware-0.1.7/donware/src/utils/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 08:24:27.276161 donware-0.1.7/donware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-14 08:24:27.000000 donware-0.1.7/donware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-14 08:24:27.000000 donware-0.1.7/donware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 08:24:27.000000 donware-0.1.7/donware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 08:24:27.000000 donware-0.1.7/donware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 08:24:27.280161 donware-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-14 08:23:58.000000 donware-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:49.370684 donware-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 04:22:31.000000 donware-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 04:22:31.000000 donware-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-19 04:22:49.366684 donware-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:31.000000 donware-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:49.366684 donware-0.1.8/donware/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 04:22:44.000000 donware-0.1.8/donware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:49.366684 donware-0.1.8/donware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 04:22:44.000000 donware-0.1.8/donware/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:49.366684 donware-0.1.8/donware/src/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:31.000000 donware-0.1.8/donware/src/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:49.366684 donware-0.1.8/donware/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 04:22:31.000000 donware-0.1.8/donware/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-19 04:22:31.000000 donware-0.1.8/donware/src/utils/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:22:49.366684 donware-0.1.8/donware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-19 04:22:49.000000 donware-0.1.8/donware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-19 04:22:49.000000 donware-0.1.8/donware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:22:49.000000 donware-0.1.8/donware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 04:22:49.000000 donware-0.1.8/donware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:22:49.370684 donware-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-19 04:22:31.000000 donware-0.1.8/setup.py
```

### Comparing `donware-0.1.7/LICENSE` & `donware-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `donware-0.1.7/setup.py` & `donware-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="donware",
-    version="0.1.7",
+    version="0.1.8",
     author="Don Yin",
     author_email="Don_Yin@outlook.com",
     description="Don's personal toolkits for data science and machine learning.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Don-Yin/donware",
     packages=find_packages(),
```
