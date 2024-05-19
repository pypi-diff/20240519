# Comparing `tmp/donware-0.1.12.tar.gz` & `tmp/donware-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donware-0.1.12.tar", last modified: Sun May 19 05:52:40 2024, max compression
+gzip compressed data, was "donware-0.1.9.tar", last modified: Sun May 19 04:31:32 2024, max compression
```

## Comparing `donware-0.1.12.tar` & `donware-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:40.644390 donware-0.1.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 05:52:21.000000 donware-0.1.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 05:52:21.000000 donware-0.1.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 05:52:40.644390 donware-0.1.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:21.000000 donware-0.1.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:40.644390 donware-0.1.12/donware/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-19 05:52:21.000000 donware-0.1.12/donware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:40.644390 donware-0.1.12/donware/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:21.000000 donware-0.1.12/donware/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:40.644390 donware-0.1.12/donware/src/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:21.000000 donware-0.1.12/donware/src/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:40.644390 donware-0.1.12/donware/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:21.000000 donware-0.1.12/donware/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-19 05:52:21.000000 donware-0.1.12/donware/src/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-19 05:52:21.000000 donware-0.1.12/donware/src/utils/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 05:52:40.644390 donware-0.1.12/donware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 05:52:40.000000 donware-0.1.12/donware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-19 05:52:40.000000 donware-0.1.12/donware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 05:52:40.000000 donware-0.1.12/donware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 05:52:40.000000 donware-0.1.12/donware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 05:52:40.644390 donware-0.1.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-19 05:52:21.000000 donware-0.1.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:32.353406 donware-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 04:31:13.000000 donware-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 04:31:13.000000 donware-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-19 04:31:32.353406 donware-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:13.000000 donware-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:32.349405 donware-0.1.9/donware/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 04:31:27.000000 donware-0.1.9/donware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:32.349405 donware-0.1.9/donware/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 04:31:13.000000 donware-0.1.9/donware/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:32.353406 donware-0.1.9/donware/src/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:13.000000 donware-0.1.9/donware/src/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:32.353406 donware-0.1.9/donware/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 04:31:13.000000 donware-0.1.9/donware/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-19 04:31:13.000000 donware-0.1.9/donware/src/utils/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 04:31:32.353406 donware-0.1.9/donware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-19 04:31:32.000000 donware-0.1.9/donware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-19 04:31:32.000000 donware-0.1.9/donware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 04:31:32.000000 donware-0.1.9/donware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 04:31:32.000000 donware-0.1.9/donware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 04:31:32.353406 donware-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-19 04:31:13.000000 donware-0.1.9/setup.py
```

### Comparing `donware-0.1.12/LICENSE` & `donware-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `donware-0.1.12/setup.py` & `donware-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="donware",
-    version="0.1.12",
+    version="0.1.9",
     author="Don Yin",
     author_email="Don_Yin@outlook.com",
     description="Don's personal toolkits for data science and machine learning.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Don-Yin/donware",
     packages=find_packages(),
```

