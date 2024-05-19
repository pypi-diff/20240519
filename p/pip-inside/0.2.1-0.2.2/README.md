# Comparing `tmp/pip_inside-0.2.1.tar.gz` & `tmp/pip_inside-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_inside-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pip_inside-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pip_inside-0.2.1.tar` & `pip_inside-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    10174 2023-02-07 04:20:17.227923 pip_inside-0.2.1/LICENSE
--rw-r--r--   0        0        0     1320 2024-02-19 02:48:51.788078 pip_inside-0.2.1/README.md
--rw-r--r--   0        0        0      111 2024-02-28 04:42:20.611616 pip_inside-0.2.1/pip_inside/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 03:11:37.270743 pip_inside-0.2.1/pip_inside/commands/__init__.py
--rw-r--r--   0        0        0      968 2023-07-21 08:08:33.698647 pip_inside-0.2.1/pip_inside/commands/add.py
--rw-r--r--   0        0        0     5092 2024-01-05 02:08:36.090057 pip_inside-0.2.1/pip_inside/commands/build.py
--rw-r--r--   0        0        0      253 2024-01-02 02:05:26.790485 pip_inside-0.2.1/pip_inside/commands/deps.py
--rw-r--r--   0        0        0     1028 2024-02-19 02:48:51.788253 pip_inside-0.2.1/pip_inside/commands/export.py
--rw-r--r--   0        0        0     9358 2024-02-28 04:36:46.996047 pip_inside-0.2.1/pip_inside/commands/init.py
--rw-r--r--   0        0        0     1980 2023-11-14 15:30:27.317098 pip_inside-0.2.1/pip_inside/commands/install.py
--rw-r--r--   0        0        0     5835 2023-02-14 10:16:47.945835 pip_inside-0.2.1/pip_inside/commands/publish.py
--rw-r--r--   0        0        0     1059 2023-07-21 08:19:39.898277 pip_inside-0.2.1/pip_inside/commands/remove.py
--rw-r--r--   0        0        0      183 2023-03-24 02:42:23.169726 pip_inside-0.2.1/pip_inside/commands/resources/.dockerignore
--rw-r--r--   0        0        0      526 2023-03-24 02:42:23.169885 pip_inside-0.2.1/pip_inside/commands/resources/.gitignore
--rw-r--r--   0        0        0     2211 2024-01-02 02:05:26.791464 pip_inside-0.2.1/pip_inside/commands/shell.py
--rw-r--r--   0        0        0      470 2023-08-14 05:57:54.632569 pip_inside-0.2.1/pip_inside/commands/upgrade.py
--rw-r--r--   0        0        0      832 2023-07-27 04:17:27.198266 pip_inside-0.2.1/pip_inside/commands/version.py
--rw-r--r--   0        0        0     9069 2024-02-19 02:48:51.788478 pip_inside-0.2.1/pip_inside/main.py
--rw-r--r--   0        0        0        0 2023-02-01 06:44:34.894743 pip_inside-0.2.1/pip_inside/utils/__init__.py
--rw-r--r--   0        0        0    11608 2024-01-05 02:08:36.091101 pip_inside-0.2.1/pip_inside/utils/dependencies.py
--rw-r--r--   0        0        0      480 2023-03-21 03:58:30.083911 pip_inside-0.2.1/pip_inside/utils/licenses.py
--rw-r--r--   0        0        0    10174 2023-02-06 03:45:43.826519 pip_inside-0.2.1/pip_inside/utils/licenses/Apache-2.0.txt
--rw-r--r--   0        0        0    35149 2023-02-07 06:36:31.902883 pip_inside-0.2.1/pip_inside/utils/licenses/GPL-3.0-or-later.txt
--rw-r--r--   0        0        0     7652 2023-02-06 04:08:59.022825 pip_inside-0.2.1/pip_inside/utils/licenses/LGPL-3.0-or-later.txt
--rw-r--r--   0        0        0     1067 2023-02-06 07:11:54.140706 pip_inside-0.2.1/pip_inside/utils/licenses/MIT.txt
--rw-r--r--   0        0        0     9185 2023-02-07 06:40:50.811920 pip_inside-0.2.1/pip_inside/utils/licenses/MulanPSL-2.0.txt
--rw-r--r--   0        0        0     3605 2024-01-05 02:08:36.091771 pip_inside-0.2.1/pip_inside/utils/markers.py
--rw-r--r--   0        0        0     1515 2023-11-14 15:30:27.319022 pip_inside-0.2.1/pip_inside/utils/misc.py
--rw-r--r--   0        0        0     9317 2024-02-28 04:40:36.858719 pip_inside-0.2.1/pip_inside/utils/packages.py
--rw-r--r--   0        0        0     5890 2024-01-05 02:08:36.092370 pip_inside-0.2.1/pip_inside/utils/pyproject.py
--rw-r--r--   0        0        0     2418 2023-11-21 11:08:34.893422 pip_inside-0.2.1/pip_inside/utils/spinner.py
--rw-r--r--   0        0        0     1765 2023-07-27 04:20:21.025285 pip_inside-0.2.1/pip_inside/utils/versions.py
--rw-r--r--   0        0        0     1881 2024-02-28 04:48:08.238918 pip_inside-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 pip_inside-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-03-26 01:15:31.222687 pip_inside-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1320 2024-05-19 01:13:11.924856 pip_inside-0.2.2/README.md
+-rw-r--r--   0        0        0      111 2024-05-19 10:33:33.873995 pip_inside-0.2.2/pip_inside/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 01:15:31.223144 pip_inside-0.2.2/pip_inside/commands/__init__.py
+-rw-r--r--   0        0        0      968 2023-07-21 23:54:55.400440 pip_inside-0.2.2/pip_inside/commands/add.py
+-rw-r--r--   0        0        0     5092 2024-05-19 01:13:11.925757 pip_inside-0.2.2/pip_inside/commands/build.py
+-rw-r--r--   0        0        0      253 2023-12-09 01:49:33.091728 pip_inside-0.2.2/pip_inside/commands/deps.py
+-rw-r--r--   0        0        0     1028 2024-05-19 01:13:11.925921 pip_inside-0.2.2/pip_inside/commands/export.py
+-rw-r--r--   0        0        0     9358 2024-05-19 01:13:11.926361 pip_inside-0.2.2/pip_inside/commands/init.py
+-rw-r--r--   0        0        0     1980 2023-12-09 01:49:33.092370 pip_inside-0.2.2/pip_inside/commands/install.py
+-rw-r--r--   0        0        0     5835 2023-03-26 01:15:31.223727 pip_inside-0.2.2/pip_inside/commands/publish.py
+-rw-r--r--   0        0        0     1059 2023-07-21 23:54:55.401209 pip_inside-0.2.2/pip_inside/commands/remove.py
+-rw-r--r--   0        0        0      183 2023-03-26 01:15:31.223934 pip_inside-0.2.2/pip_inside/commands/resources/.dockerignore
+-rw-r--r--   0        0        0      526 2023-03-26 01:15:31.224014 pip_inside-0.2.2/pip_inside/commands/resources/.gitignore
+-rw-r--r--   0        0        0     2211 2023-12-09 01:49:33.093386 pip_inside-0.2.2/pip_inside/commands/shell.py
+-rw-r--r--   0        0        0      470 2023-09-24 11:48:24.667063 pip_inside-0.2.2/pip_inside/commands/upgrade.py
+-rw-r--r--   0        0        0      832 2023-08-13 11:00:16.775904 pip_inside-0.2.2/pip_inside/commands/version.py
+-rw-r--r--   0        0        0     9069 2024-05-19 01:13:11.926600 pip_inside-0.2.2/pip_inside/main.py
+-rw-r--r--   0        0        0        0 2023-03-26 01:15:31.224448 pip_inside-0.2.2/pip_inside/utils/__init__.py
+-rw-r--r--   0        0        0    11608 2024-05-19 01:13:11.926850 pip_inside-0.2.2/pip_inside/utils/dependencies.py
+-rw-r--r--   0        0        0      480 2023-03-26 01:15:31.224652 pip_inside-0.2.2/pip_inside/utils/licenses.py
+-rw-r--r--   0        0        0    10174 2023-03-26 01:15:31.224795 pip_inside-0.2.2/pip_inside/utils/licenses/Apache-2.0.txt
+-rw-r--r--   0        0        0    35149 2023-03-26 01:15:31.225044 pip_inside-0.2.2/pip_inside/utils/licenses/GPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     7652 2023-03-26 01:15:31.225168 pip_inside-0.2.2/pip_inside/utils/licenses/LGPL-3.0-or-later.txt
+-rw-r--r--   0        0        0     1067 2023-03-26 01:15:31.225250 pip_inside-0.2.2/pip_inside/utils/licenses/MIT.txt
+-rw-r--r--   0        0        0     9185 2023-03-26 01:15:31.225361 pip_inside-0.2.2/pip_inside/utils/licenses/MulanPSL-2.0.txt
+-rw-r--r--   0        0        0     3807 2024-05-19 10:27:15.017286 pip_inside-0.2.2/pip_inside/utils/markers.py
+-rw-r--r--   0        0        0     1515 2023-12-09 01:49:33.094531 pip_inside-0.2.2/pip_inside/utils/misc.py
+-rw-r--r--   0        0        0     9317 2024-05-19 01:13:11.927291 pip_inside-0.2.2/pip_inside/utils/packages.py
+-rw-r--r--   0        0        0     5890 2024-05-19 01:13:11.927518 pip_inside-0.2.2/pip_inside/utils/pyproject.py
+-rw-r--r--   0        0        0     3125 2024-05-19 10:31:58.813449 pip_inside-0.2.2/pip_inside/utils/spinner.py
+-rw-r--r--   0        0        0     1765 2023-08-13 11:00:16.777477 pip_inside-0.2.2/pip_inside/utils/versions.py
+-rw-r--r--   0        0        0     1881 2024-05-19 01:13:11.928014 pip_inside-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 pip_inside-0.2.2/PKG-INFO
```

### Comparing `pip_inside-0.2.1/LICENSE` & `pip_inside-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/README.md` & `pip_inside-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/add.py` & `pip_inside-0.2.2/pip_inside/commands/add.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/build.py` & `pip_inside-0.2.2/pip_inside/commands/build.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/export.py` & `pip_inside-0.2.2/pip_inside/commands/export.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/init.py` & `pip_inside-0.2.2/pip_inside/commands/init.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/install.py` & `pip_inside-0.2.2/pip_inside/commands/install.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/publish.py` & `pip_inside-0.2.2/pip_inside/commands/publish.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/remove.py` & `pip_inside-0.2.2/pip_inside/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/resources/.gitignore` & `pip_inside-0.2.2/pip_inside/commands/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/shell.py` & `pip_inside-0.2.2/pip_inside/commands/shell.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/commands/version.py` & `pip_inside-0.2.2/pip_inside/commands/version.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/main.py` & `pip_inside-0.2.2/pip_inside/main.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/dependencies.py` & `pip_inside-0.2.2/pip_inside/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/licenses/Apache-2.0.txt` & `pip_inside-0.2.2/pip_inside/utils/licenses/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/licenses/GPL-3.0-or-later.txt` & `pip_inside-0.2.2/pip_inside/utils/licenses/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/licenses/LGPL-3.0-or-later.txt` & `pip_inside-0.2.2/pip_inside/utils/licenses/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/licenses/MIT.txt` & `pip_inside-0.2.2/pip_inside/utils/licenses/MIT.txt`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/licenses/MulanPSL-2.0.txt` & `pip_inside-0.2.2/pip_inside/utils/licenses/MulanPSL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/markers.py` & `pip_inside-0.2.2/pip_inside/utils/markers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # https://peps.python.org/pep-0496/
 # https://peps.python.org/pep-0508/
 import logging
 import os
 from typing import List, Union
 
 from pkg_resources import Requirement as _Requirement
-from pkg_resources._vendor.packaging.markers import InvalidMarker
+from pkg_resources._vendor.packaging.markers import InvalidMarker, default_environment, _format_marker
 from pkg_resources._vendor.packaging.markers import Marker as _Marker
 from pkg_resources._vendor.packaging.markers import Op, UndefinedComparison, UndefinedEnvironmentName, Variable, _evaluate_markers
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Marker(_Marker):
     def __init__(self) -> None:
         self._markers = []
 
     def evaluate(self, environment=None):
         def strip_doller_sign(item):
-            if not isinstance(item, Variable):
+            if item.__class__.__name__ != 'Variable':
                 return item
             return Variable(item.value.strip('$'))
 
-        current_environment = os.environ
+        builtin_environment = default_environment()
+        current_environment = {**os.environ, **builtin_environment}
         if environment is not None:
             current_environment.update(environment)
         markers = [(strip_doller_sign(lhs), op, strip_doller_sign(rhs)) for lhs, op, rhs in self._markers]
         return _evaluate_markers(markers, current_environment)
+    
+    def __str__(self):
+        return _format_marker(self._markers or [])
 
 
 class Requirement(_Requirement):
     def __init__(self, requirement_string: str) -> None:
         requirement_string = self._parse_requirements(requirement_string)
         super().__init__(requirement_string)
         if self.marker:
```

### Comparing `pip_inside-0.2.1/pip_inside/utils/misc.py` & `pip_inside-0.2.2/pip_inside/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/packages.py` & `pip_inside-0.2.2/pip_inside/utils/packages.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/pyproject.py` & `pip_inside-0.2.2/pip_inside/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pip_inside/utils/versions.py` & `pip_inside-0.2.2/pip_inside/utils/versions.py`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/pyproject.toml` & `pip_inside-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pip_inside-0.2.1/PKG-INFO` & `pip_inside-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-inside
-Version: 0.2.1
+Version: 0.2.2
 Summary: Like poetry, but it's pip
 Home-page: https://github.com/orctom/pip-inside
 License: Apache-2.0
 Author: orctom
 Author-email: orctom <orctom@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

