# Comparing `tmp/baosight-0.0.8.tar.gz` & `tmp/baosight-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baosight-0.0.8.tar", last modified: Sun May 19 03:15:31 2024, max compression
+gzip compressed data, was "baosight-0.0.9.tar", last modified: Sun May 19 03:35:36 2024, max compression
```

## Comparing `baosight-0.0.8.tar` & `baosight-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.822232 baosight-0.0.8/
--rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1380 2024-05-19 03:15:31.821238 baosight-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      767 2024-05-18 18:57:41.000000 baosight-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.729754 baosight-0.0.8/baosight/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.8/baosight/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.786000 baosight-0.0.8/baosight/cli/
--rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.8/baosight/cli/__init__.py
--rw-rw-rw-   0        0        0     1409 2024-05-18 18:56:55.000000 baosight-0.0.8/baosight/cli/gl_runner.py
--rw-rw-rw-   0        0        0     1418 2024-05-18 18:01:43.000000 baosight-0.0.8/baosight/cli/main.py
-drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.817218 baosight-0.0.8/baosight/tools/
--rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.8/baosight/tools/__init__.py
--rw-rw-rw-   0        0        0     4609 2024-05-19 03:13:28.000000 baosight-0.0.8/baosight/tools/gitlab_runner.py
--rw-rw-rw-   0        0        0     1593 2024-05-18 18:56:44.000000 baosight-0.0.8/baosight/tools/gitlab_runner_config_generator.py
--rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.8/baosight/tools/gitlab_runner_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-19 03:15:31.819233 baosight-0.0.8/baosight.egg-info/
--rw-rw-rw-   0        0        0     1380 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-19 03:15:30.000000 baosight-0.0.8/baosight.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-19 03:15:31.000000 baosight-0.0.8/baosight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2024-05-19 03:15:31.826237 baosight-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:35:36.167258 baosight-0.0.9/
+-rw-rw-rw-   0        0        0     1064 2023-10-25 05:23:47.000000 baosight-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      126 2024-05-18 18:14:34.000000 baosight-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1380 2024-05-19 03:35:36.167258 baosight-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-05-18 18:57:41.000000 baosight-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 03:35:36.131259 baosight-0.0.9/baosight/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:41:58.000000 baosight-0.0.9/baosight/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:35:36.158258 baosight-0.0.9/baosight/cli/
+-rw-rw-rw-   0        0        0        0 2023-10-25 05:23:47.000000 baosight-0.0.9/baosight/cli/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-05-19 03:34:30.000000 baosight-0.0.9/baosight/cli/cmd_admin.py
+-rw-rw-rw-   0        0        0     1409 2024-05-18 18:56:55.000000 baosight-0.0.9/baosight/cli/gl_runner.py
+-rw-rw-rw-   0        0        0     1457 2024-05-19 03:24:02.000000 baosight-0.0.9/baosight/cli/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:35:36.163259 baosight-0.0.9/baosight/tools/
+-rw-rw-rw-   0        0        0        0 2024-05-18 17:42:50.000000 baosight-0.0.9/baosight/tools/__init__.py
+-rw-rw-rw-   0        0        0     4609 2024-05-19 03:13:28.000000 baosight-0.0.9/baosight/tools/gitlab_runner.py
+-rw-rw-rw-   0        0        0     1593 2024-05-18 18:56:44.000000 baosight-0.0.9/baosight/tools/gitlab_runner_config_generator.py
+-rw-rw-rw-   0        0        0     7201 2024-05-18 18:24:21.000000 baosight-0.0.9/baosight/tools/gitlab_runner_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:35:36.165261 baosight-0.0.9/baosight.egg-info/
+-rw-rw-rw-   0        0        0     1380 2024-05-19 03:35:36.000000 baosight-0.0.9/baosight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2024-05-19 03:35:36.000000 baosight-0.0.9/baosight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 03:35:36.000000 baosight-0.0.9/baosight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-19 03:35:36.000000 baosight-0.0.9/baosight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 03:35:35.000000 baosight-0.0.9/baosight.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-05-19 03:35:36.000000 baosight-0.0.9/baosight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 03:35:36.000000 baosight-0.0.9/baosight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      666 2024-05-19 03:35:36.170260 baosight-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      171 2024-05-18 18:10:58.000000 baosight-0.0.9/setup.py
```

### Comparing `baosight-0.0.8/LICENSE` & `baosight-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `baosight-0.0.8/PKG-INFO` & `baosight-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baosight
-Version: 0.0.8
+Version: 0.0.9
 Summary: baosight tools
 Home-page: https://cuddlebugs.asia
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `baosight-0.0.8/README.md` & `baosight-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `baosight-0.0.8/baosight/cli/gl_runner.py` & `baosight-0.0.9/baosight/cli/gl_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.8/baosight/cli/main.py` & `baosight-0.0.9/baosight/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import importlib
 import textwrap
 
 subcommands = [
     ("gl-runner", "baosight.cli.gl_runner"),
+    ("cmd", "baosight.cli.cmd_admin"),
 ]
 
 
 def main():
     parser = argparse.ArgumentParser(prog="baosight", description="常用工具包")
     subparsers = parser.add_subparsers(title="subcommand", dest="subcommand")
     subparser_help = subparsers.add_parser("help", description="Help", help="子命令帮助")
```

### Comparing `baosight-0.0.8/baosight/tools/gitlab_runner.py` & `baosight-0.0.9/baosight/tools/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.8/baosight/tools/gitlab_runner_config_generator.py` & `baosight-0.0.9/baosight/tools/gitlab_runner_config_generator.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.8/baosight/tools/gitlab_runner_gui.py` & `baosight-0.0.9/baosight/tools/gitlab_runner_gui.py`

 * *Files identical despite different names*

### Comparing `baosight-0.0.8/baosight.egg-info/PKG-INFO` & `baosight-0.0.9/baosight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baosight
-Version: 0.0.8
+Version: 0.0.9
 Summary: baosight tools
 Home-page: https://cuddlebugs.asia
 Author: Hao Zhao
 Author-email: 601095001@qq.com
 License: OSI Approved :: MIT License
 Platform: Linux/Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `baosight-0.0.8/setup.cfg` & `baosight-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 616f 7369 6768 740d 0a76 6572   = baosight..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6465  sion = 0.0.8..de
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6465  sion = 0.0.9..de
 00000030: 7363 7269 7074 696f 6e20 3d20 6261 6f73  scription = baos
 00000040: 6967 6874 2074 6f6f 6c73 0d0a 6c6f 6e67  ight tools..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a61  text/markdown..a
```

