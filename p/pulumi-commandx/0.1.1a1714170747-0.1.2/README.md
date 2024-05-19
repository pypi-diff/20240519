# Comparing `tmp/pulumi_commandx-0.1.1a1714170747.tar.gz` & `tmp/pulumi_commandx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_commandx-0.1.1a1714170747.tar", last modified: Fri Apr 26 22:33:57 2024, max compression
+gzip compressed data, was "pulumi_commandx-0.1.2.tar", last modified: Sun May 19 03:14:25 2024, max compression
```

## Comparing `pulumi_commandx-0.1.1a1714170747.tar` & `pulumi_commandx-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:33:57.479577 pulumi_commandx-0.1.1a1714170747/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-26 22:33:57.479577 pulumi_commandx-0.1.1a1714170747/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:33:57.475577 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/
--rw-------   0 runner    (1001) docker     (127)     1253 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/_utilities.py
--rw-------   0 runner    (1001) docker     (127)     2738 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/provider.py
--rw-------   0 runner    (1001) docker     (127)      101 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:33:57.479577 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/
--rw-------   0 runner    (1001) docker     (127)      590 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108421 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14943 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14962 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/curl.py
--rw-------   0 runner    (1001) docker     (127)    15035 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15175 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14943 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14978 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14838 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/mv.py
--rw-------   0 runner    (1001) docker     (127)    91760 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14838 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/rm.py
--rw-------   0 runner    (1001) docker     (127)    14873 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/sed.py
--rw-------   0 runner    (1001) docker     (127)    15105 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14873 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/tar.py
--rw-------   0 runner    (1001) docker     (127)    14893 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/tee.py
--rw-------   0 runner    (1001) docker     (127)    14908 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 22:33:57.479577 pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-26 22:33:57.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-26 22:33:57.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 22:33:57.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 22:33:57.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 22:33:57.000000 pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      745 2024-04-26 22:33:51.000000 pulumi_commandx-0.1.1a1714170747/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 22:33:57.479577 pulumi_commandx-0.1.1a1714170747/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:14:25.688719 pulumi_commandx-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-19 03:14:25.688719 pulumi_commandx-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:14:25.684719 pulumi_commandx-0.1.2/pulumi_commandx/
+-rw-------   0 runner    (1001) docker     (127)     1253 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)     2738 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/provider.py
+-rw-------   0 runner    (1001) docker     (127)      123 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:14:25.688719 pulumi_commandx-0.1.2/pulumi_commandx/remote/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108421 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14943 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14962 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15035 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15175 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14943 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14978 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14838 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91760 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14838 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14873 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15105 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14873 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14893 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14908 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pulumi_commandx/remote/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:14:25.688719 pulumi_commandx-0.1.2/pulumi_commandx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-19 03:14:25.000000 pulumi_commandx-0.1.2/pulumi_commandx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 03:14:25.000000 pulumi_commandx-0.1.2/pulumi_commandx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:14:25.000000 pulumi_commandx-0.1.2/pulumi_commandx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 03:14:25.000000 pulumi_commandx-0.1.2/pulumi_commandx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 03:14:25.000000 pulumi_commandx-0.1.2/pulumi_commandx.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      734 2024-05-19 03:14:18.000000 pulumi_commandx-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 03:14:25.688719 pulumi_commandx-0.1.2/setup.cfg
```

### Comparing `pulumi_commandx-0.1.1a1714170747/PKG-INFO` & `pulumi_commandx-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pulumi_commandx
-Version: 0.1.1a1714170747
+Version: 0.1.2
 Summary: A Pulumi component provider for creating statically typed `Command` resources.
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-commandx
 Keywords: pulumi,command,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
-Requires-Dist: pulumi-command<1.0.0,>=0.10.0
+Requires-Dist: pulumi-command<1.0.0,>=0.11.1
 Requires-Dist: semver>=2.8.1
 
 # Pulumi Commandx
 
 Mostly helper functions for creating statically typed `Command` resources.
 
 ## Development
```

### Comparing `pulumi_commandx-0.1.1a1714170747/README.md` & `pulumi_commandx-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/__init__.py` & `pulumi_commandx-0.1.2/pulumi_commandx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/_utilities.py` & `pulumi_commandx-0.1.2/pulumi_commandx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/provider.py` & `pulumi_commandx-0.1.2/pulumi_commandx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/__init__.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/_enums.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/_inputs.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/chmod.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/curl.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/etcdctl.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/hostnamectl.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/mkdir.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/mktemp.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/mv.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/outputs.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/rm.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/sed.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/systemctl.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/tar.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/tee.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx/remote/wget.py` & `pulumi_commandx-0.1.2/pulumi_commandx/remote/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/PKG-INFO` & `pulumi_commandx-0.1.2/pulumi_commandx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pulumi_commandx
-Version: 0.1.1a1714170747
+Version: 0.1.2
 Summary: A Pulumi component provider for creating statically typed `Command` resources.
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-commandx
 Keywords: pulumi,command,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.91.1
-Requires-Dist: pulumi-command<1.0.0,>=0.10.0
+Requires-Dist: pulumi-command<1.0.0,>=0.11.1
 Requires-Dist: semver>=2.8.1
 
 # Pulumi Commandx
 
 Mostly helper functions for creating statically typed `Command` resources.
 
 ## Development
```

### Comparing `pulumi_commandx-0.1.1a1714170747/pulumi_commandx.egg-info/SOURCES.txt` & `pulumi_commandx-0.1.2/pulumi_commandx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_commandx-0.1.1a1714170747/pyproject.toml` & `pulumi_commandx-0.1.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_commandx"
   description = "A Pulumi component provider for creating statically typed `Command` resources."
-  dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "semver>=2.8.1"]
+  dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.1.1a1714170747"
+  version = "0.1.2"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-commandx"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

