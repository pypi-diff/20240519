# Comparing `tmp/wol_api-0.1.6.tar.gz` & `tmp/wol_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wol_api-0.1.6.tar", last modified: Sun Nov  6 13:42:14 2022, max compression
+gzip compressed data, was "wol_api-1.0.0.tar", last modified: Sun May 19 12:43:52 2024, max compression
```

## Comparing `wol_api-0.1.6.tar` & `wol_api-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:14.533747 wol_api-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-11-06 13:42:14.533747 wol_api-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-11-06 13:42:04.000000 wol_api-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-06 13:42:14.533747 wol_api-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-11-06 13:42:04.000000 wol_api-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:14.533747 wol_api-0.1.6/wol_api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:04.000000 wol_api-0.1.6/wol_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-11-06 13:42:04.000000 wol_api-0.1.6/wol_api/web.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:14.533747 wol_api-0.1.6/wol_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-06 13:42:14.000000 wol_api-0.1.6/wol_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 12:43:45.000000 wol_api-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 12:43:45.000000 wol_api-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 12:43:52.323850 wol_api-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-19 12:43:45.000000 wol_api-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:43:52.323850 wol_api-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-19 12:43:45.000000 wol_api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/wol_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/wol_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-19 12:43:45.000000 wol_api-1.0.0/wol_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:43:52.323850 wol_api-1.0.0/wol_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 12:43:52.000000 wol_api-1.0.0/wol_api.egg-info/top_level.txt
```

### Comparing `wol_api-0.1.6/README.md` & `wol_api-1.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 #  WakeOnLAN-API
 
 [![PyPI version](https://badge.fury.io/py/wol-api.svg)](https://badge.fury.io/py/wol-api)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
-A simple flask interface to send wake on LAN commands. Just send a `POST` to `/wol/FF:FF:FF:FF:FF:FF` where `FF:FF:FF:FF:FF:FF` is the desired MAC address of the device to be woken up.
-
-The official docker image is available at [Docker Hub](https://hub.docker.com/r/rix1337/docker-wol_api).
+A simple http interface to send wake on LAN commands. Just send a `POST` to `/FF:FF:FF:FF:FF:FF` where `FF:FF:FF:FF:FF:FF` is the desired MAC address of the device to be woken up.
 
 # Setup
 
 `pip install wol_api`
 
 # Run
 
-` wol_api --port=8080` 
+` wol_api --port=8080`
 
+# Docker
+```
+docker run -d \
+  --name="WakeOnLAN-API" \
+  -p port:8080 \
+  rix1337/docker-wol-api:latest
+  ```
```

### Comparing `wol_api-0.1.6/setup.py` & `wol_api-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 # -*- coding: utf-8 -*-
 # WakeOnLAN-API
-# Project by https://github.com/rix1337
+# Projekt by https://github.com/rix1337
 
 import setuptools
 
+from wol_api.providers.version import get_version
+
 try:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 except:
     import io
 
     long_description = io.open('README.md', encoding='utf-8').read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="wol_api",
-    version="0.1.6",
+    version=get_version(),
     author="rix1337",
     author_email="",
-    description="A simple wake on LAN interface that accepts post commands",
+    description="Full template for python web projects with Docker, Github Actions, PyPI, and more.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/rix1337/docker-wakeonlan",
+    url="https://github.com/rix1337/WakeOnLAN-API",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=required,
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'wol_api = wol_api.web:main',
+            'wol_api = wol_api.run:main',
         ],
     },
 )
```

