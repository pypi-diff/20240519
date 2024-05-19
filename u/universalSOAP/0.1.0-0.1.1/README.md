# Comparing `tmp/universalsoap-0.1.0.tar.gz` & `tmp/universalsoap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universalsoap-0.1.0.tar", last modified: Thu May 16 18:18:14 2024, max compression
+gzip compressed data, was "universalsoap-0.1.1.tar", last modified: Sun May 19 00:14:02 2024, max compression
```

## Comparing `universalsoap-0.1.0.tar` & `universalsoap-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:18:14.567987 universalsoap-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-16 18:18:10.000000 universalsoap-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-16 18:18:14.567987 universalsoap-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-16 18:18:10.000000 universalsoap-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:18:14.567987 universalsoap-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 18:18:10.000000 universalsoap-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:18:14.567987 universalsoap-0.1.0/universalSOAP/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 18:18:10.000000 universalsoap-0.1.0/universalSOAP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-16 18:18:10.000000 universalsoap-0.1.0/universalSOAP/hypers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:18:14.567987 universalsoap-0.1.0/universalSOAP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-16 18:18:14.000000 universalsoap-0.1.0/universalSOAP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-16 18:18:14.000000 universalsoap-0.1.0/universalSOAP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:18:14.000000 universalsoap-0.1.0/universalSOAP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 18:18:14.000000 universalsoap-0.1.0/universalSOAP.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 18:18:14.000000 universalsoap-0.1.0/universalSOAP.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:14:02.078663 universalsoap-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-19 00:13:58.000000 universalsoap-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-19 00:14:02.074663 universalsoap-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-19 00:13:58.000000 universalsoap-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-19 00:13:58.000000 universalsoap-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 00:14:02.078663 universalsoap-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:14:02.074663 universalsoap-0.1.1/universalSOAP/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-19 00:13:58.000000 universalsoap-0.1.1/universalSOAP/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:14:02.074663 universalsoap-0.1.1/universalSOAP/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-19 00:13:58.000000 universalsoap-0.1.1/universalSOAP/cli/write_descriptor_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-19 00:13:58.000000 universalsoap-0.1.1/universalSOAP/hypers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 00:14:02.074663 universalsoap-0.1.1/universalSOAP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2024-05-19 00:14:02.000000 universalsoap-0.1.1/universalSOAP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-19 00:14:02.000000 universalsoap-0.1.1/universalSOAP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 00:14:02.000000 universalsoap-0.1.1/universalSOAP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-19 00:14:02.000000 universalsoap-0.1.1/universalSOAP.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 00:14:02.000000 universalsoap-0.1.1/universalSOAP.egg-info/top_level.txt
```

### Comparing `universalsoap-0.1.0/LICENSE` & `universalsoap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `universalsoap-0.1.0/PKG-INFO` & `universalsoap-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: universalSOAP
-Version: 0.1.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # universal-soap
 scripts to create SOAP descriptors for arbitrary elements and combinations
 
 Heuristics:
   * Length scales
     * Atomic (inputs)
       * typical bond length (from equilibrium bond length in lowest energy 2D or 3D structure)
```

### Comparing `universalsoap-0.1.0/universalSOAP/hypers.py` & `universalsoap-0.1.1/universalSOAP/hypers.py`

 * *Files identical despite different names*

