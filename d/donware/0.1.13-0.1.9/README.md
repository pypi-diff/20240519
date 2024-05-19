# Comparing `tmp/donware-0.1.13.tar.gz` & `tmp/donware-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donware-0.1.13.tar", last modified: Sun May 19 06:08:50 2024, max compression
+gzip compressed data, was "donware-0.1.9.tar", last modified: Sun May 19 04:31:32 2024, max compression
```

## Comparing `donware-0.1.13.tar` & `donware-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:50.107875 donware-0.1.13/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 06:08:30.000000 donware-0.1.13/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-19 06:08:30.000000 donware-0.1.13/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 06:08:50.107875 donware-0.1.13/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:30.000000 donware-0.1.13/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:50.107875 donware-0.1.13/donware/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-19 06:08:30.000000 donware-0.1.13/donware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:50.107875 donware-0.1.13/donware/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:30.000000 donware-0.1.13/donware/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:50.107875 donware-0.1.13/donware/src/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:30.000000 donware-0.1.13/donware/src/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:50.107875 donware-0.1.13/donware/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:30.000000 donware-0.1.13/donware/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-19 06:08:30.000000 donware-0.1.13/donware/src/utils/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 06:08:30.000000 donware-0.1.13/donware/src/utils/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-19 06:08:30.000000 donware-0.1.13/donware/src/utils/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 06:08:50.107875 donware-0.1.13/donware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-19 06:08:50.000000 donware-0.1.13/donware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-19 06:08:50.000000 donware-0.1.13/donware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 06:08:50.000000 donware-0.1.13/donware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 06:08:50.000000 donware-0.1.13/donware.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 06:08:50.000000 donware-0.1.13/donware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 06:08:50.107875 donware-0.1.13/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-19 06:08:30.000000 donware-0.1.13/setup.py
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

### Comparing `donware-0.1.13/LICENSE` & `donware-0.1.9/LICENSE`

 * *Files identical despite different names*

