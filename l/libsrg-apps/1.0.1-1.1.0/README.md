# Comparing `tmp/libsrg_apps-1.0.1.tar.gz` & `tmp/libsrg_apps-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsrg_apps-1.0.1.tar", max compression
+gzip compressed data, was "libsrg_apps-1.1.0.tar", max compression
```

## Comparing `libsrg_apps-1.0.1.tar` & `libsrg_apps-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1242 2024-05-02 23:43:19.113008 libsrg_apps-1.0.1/README.md
--rwxr-xr-x   0        0        0     6028 2024-04-09 15:09:14.512097 libsrg_apps-1.0.1/libsrg_apps/DiskInfo.py
--rwxr-xr-x   0        0        0    15705 2024-04-09 15:09:14.551097 libsrg_apps-1.0.1/libsrg_apps/ReZFS.py
--rwxr-xr-x   0        0        0     7024 2023-10-05 17:56:35.188332 libsrg_apps-1.0.1/libsrg_apps/Stage0.py
--rw-r--r--   0        0        0        0 2024-05-02 19:09:02.278580 libsrg_apps-1.0.1/libsrg_apps/__init__.py
--rwxr-xr-x   0        0        0    26598 2024-04-09 15:09:14.543097 libsrg_apps-1.0.1/libsrg_apps/ztool.py
--rw-r--r--   0        0        0      944 2024-05-02 23:53:49.178373 libsrg_apps-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 libsrg_apps-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1242 2024-05-02 23:43:19.113008 libsrg_apps-1.1.0/README.md
+-rwxr-xr-x   0        0        0     6266 2024-05-19 14:57:54.770021 libsrg_apps-1.1.0/libsrg_apps/DiskInfo.py
+-rwxr-xr-x   0        0        0    15943 2024-05-19 14:57:54.773021 libsrg_apps-1.1.0/libsrg_apps/ReZFS.py
+-rwxr-xr-x   0        0        0     7262 2024-05-19 14:57:54.766021 libsrg_apps-1.1.0/libsrg_apps/Stage0.py
+-rw-r--r--   0        0        0      239 2024-05-19 14:57:54.768021 libsrg_apps-1.1.0/libsrg_apps/__init__.py
+-rwxr-xr-x   0        0        0    26837 2024-05-19 14:57:54.763022 libsrg_apps-1.1.0/libsrg_apps/ztool.py
+-rw-r--r--   0        0        0      944 2024-05-19 14:59:53.009387 libsrg_apps-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2100 1970-01-01 00:00:00.000000 libsrg_apps-1.1.0/PKG-INFO
```

### Comparing `libsrg_apps-1.0.1/README.md` & `libsrg_apps-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `libsrg_apps-1.0.1/libsrg_apps/DiskInfo.py` & `libsrg_apps-1.1.0/libsrg_apps/DiskInfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #! /usr/bin/env python3
+# libsrg_apps (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 """
 A reference copy of this program is maintained at /GNAS/PROJ/PycharmProjects/libsrg/DiskInfo.py
 
 Active copy is /GNAS/PROJ/PycharmProjects/ANS_PROJECT/scripts/DiskInfo.py
 
 See also QT version at /GNAS/PROJ/PycharmProjects/ANS_PROJECT/scripts/DiskInfo.py
```

### Comparing `libsrg_apps-1.0.1/libsrg_apps/ReZFS.py` & `libsrg_apps-1.1.0/libsrg_apps/ReZFS.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #! /usr/bin/env python3
+# libsrg_apps (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 # cd /GNAS/PROJ/PycharmProjects/libsrg
 # venvF/bin/python -m libsrg.ReZFS --source
 
 # noinspection PyPep8
 """
 Manual procedure to install from source:
```

### Comparing `libsrg_apps-1.0.1/libsrg_apps/Stage0.py` & `libsrg_apps-1.1.0/libsrg_apps/Stage0.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 #!/usr/bin/env  python3
+# libsrg_apps (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 import configparser
 import platform
 from importlib.metadata import version
 from pathlib import Path
 
 from libsrg.LoggingAppBase import LoggingAppBase
```

### Comparing `libsrg_apps-1.0.1/libsrg_apps/ztool.py` & `libsrg_apps-1.1.0/libsrg_apps/ztool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 #!/usr/bin/env python3
+# libsrg_apps (Code and Documentation) is published under an MIT License
+# Copyright (c) 2024 Steven Goncalo
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 import logging
 import sys
 
 from libsrg.LoggingAppBase import LoggingAppBase
 from libsrg.Runner import Runner
 from libsrg.Runner2 import Runner2
```

### Comparing `libsrg_apps-1.0.1/pyproject.toml` & `libsrg_apps-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libsrg-apps"
-version = "1.0.1"
+version = "1.1.0"
 description = "This is a handful of applications migrated out of lilbsrg."
 authors = ["Steve Goncalo <steven@goncalo.us>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -13,15 +13,15 @@
     "Natural Language :: English",
     "Topic :: Utilities",
     "Topic :: System :: Systems Administration"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-libsrg = "^4.3.2"
+libsrg = "^5.2.2"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.3.7"
 sphinx-rtd-theme = "^2.0.0"
 sphinxcontrib-napoleon = "^0.7"
```

### Comparing `libsrg_apps-1.0.1/PKG-INFO` & `libsrg_apps-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg-apps
-Version: 1.0.1
+Version: 1.1.0
 Summary: This is a handful of applications migrated out of lilbsrg.
 Author: Steve Goncalo
 Author-email: steven@goncalo.us
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
-Requires-Dist: libsrg (>=4.3.2,<5.0.0)
+Requires-Dist: libsrg (>=5.2.2,<6.0.0)
 Description-Content-Type: text/markdown
 
 # libsrg_apps
 
 This library provides three python applications
 
 * DiskInfo - displays disks, aliases, formatting and ZFS pool membership
```

