# Comparing `tmp/flet_route_static-0.0.1.tar.gz` & `tmp/flet_route_static-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_route_static-0.0.1.tar", last modified: Sun May 19 10:51:35 2024, max compression
+gzip compressed data, was "flet_route_static-0.0.2.tar", last modified: Sun May 19 14:05:38 2024, max compression
```

## Comparing `flet_route_static-0.0.1.tar` & `flet_route_static-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 10:51:35.533227 flet_route_static-0.0.1/
--rw-rw-rw-   0        0        0     1093 2024-05-19 09:40:28.000000 flet_route_static-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1597 2024-05-19 10:51:35.533227 flet_route_static-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1108 2024-05-19 10:51:32.000000 flet_route_static-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 10:51:35.520261 flet_route_static-0.0.1/flet_route_static/
--rw-rw-rw-   0        0        0      131 2024-05-19 09:40:28.000000 flet_route_static-0.0.1/flet_route_static/__init__.py
--rw-rw-rw-   0        0        0      676 2024-05-19 09:40:28.000000 flet_route_static-0.0.1/flet_route_static/basket.py
--rw-rw-rw-   0        0        0      907 2024-05-19 09:40:28.000000 flet_route_static-0.0.1/flet_route_static/not_found_view.py
--rw-rw-rw-   0        0        0      747 2024-05-19 09:40:28.000000 flet_route_static-0.0.1/flet_route_static/params.py
--rw-rw-rw-   0        0        0     7582 2024-05-19 09:50:02.000000 flet_route_static-0.0.1/flet_route_static/routing.py
-drwxrwxrwx   0        0        0        0 2024-05-19 10:51:35.532229 flet_route_static-0.0.1/flet_route_static.egg-info/
--rw-rw-rw-   0        0        0     1597 2024-05-19 10:51:35.000000 flet_route_static-0.0.1/flet_route_static.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-05-19 10:51:35.000000 flet_route_static-0.0.1/flet_route_static.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 10:51:35.000000 flet_route_static-0.0.1/flet_route_static.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-19 10:51:35.000000 flet_route_static-0.0.1/flet_route_static.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-19 10:51:35.000000 flet_route_static-0.0.1/flet_route_static.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 10:51:35.533227 flet_route_static-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      821 2024-05-19 09:51:20.000000 flet_route_static-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:05:38.218770 flet_route_static-0.0.2/
+-rw-rw-rw-   0        0        0     1093 2024-05-19 09:40:28.000000 flet_route_static-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5968 2024-05-19 14:05:38.217774 flet_route_static-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5479 2024-05-19 14:04:54.000000 flet_route_static-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 14:05:38.195832 flet_route_static-0.0.2/flet_route_static/
+-rw-rw-rw-   0        0        0      131 2024-05-19 09:40:28.000000 flet_route_static-0.0.2/flet_route_static/__init__.py
+-rw-rw-rw-   0        0        0      676 2024-05-19 09:40:28.000000 flet_route_static-0.0.2/flet_route_static/basket.py
+-rw-rw-rw-   0        0        0      907 2024-05-19 09:40:28.000000 flet_route_static-0.0.2/flet_route_static/not_found_view.py
+-rw-rw-rw-   0        0        0      747 2024-05-19 09:40:28.000000 flet_route_static-0.0.2/flet_route_static/params.py
+-rw-rw-rw-   0        0        0     7582 2024-05-19 09:50:02.000000 flet_route_static-0.0.2/flet_route_static/routing.py
+drwxrwxrwx   0        0        0        0 2024-05-19 14:05:38.216776 flet_route_static-0.0.2/flet_route_static.egg-info/
+-rw-rw-rw-   0        0        0     5968 2024-05-19 14:05:38.000000 flet_route_static-0.0.2/flet_route_static.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-05-19 14:05:38.000000 flet_route_static-0.0.2/flet_route_static.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 14:05:38.000000 flet_route_static-0.0.2/flet_route_static.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 14:05:38.000000 flet_route_static-0.0.2/flet_route_static.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-19 14:05:38.000000 flet_route_static-0.0.2/flet_route_static.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 14:05:38.218770 flet_route_static-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      821 2024-05-19 14:05:34.000000 flet_route_static-0.0.2/setup.py
```

### Comparing `flet_route_static-0.0.1/LICENSE` & `flet_route_static-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_route_static-0.0.1/flet_route_static/basket.py` & `flet_route_static-0.0.2/flet_route_static/basket.py`

 * *Files identical despite different names*

### Comparing `flet_route_static-0.0.1/flet_route_static/not_found_view.py` & `flet_route_static-0.0.2/flet_route_static/not_found_view.py`

 * *Files identical despite different names*

### Comparing `flet_route_static-0.0.1/flet_route_static/params.py` & `flet_route_static-0.0.2/flet_route_static/params.py`

 * *Files identical despite different names*

### Comparing `flet_route_static-0.0.1/flet_route_static/routing.py` & `flet_route_static-0.0.2/flet_route_static/routing.py`

 * *Files identical despite different names*

### Comparing `flet_route_static-0.0.1/setup.py` & `flet_route_static-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name = "flet_route_static",
-    version = "0.0.1",
+    version = "0.0.2",
     author="Saurabh Wadekar, SmokyAce",
     packages=find_packages(),
     license="MIT",
     maintainer="SmokyAce",
     maintainer_email="smokyacetv@gmail.com",
     keywords=["flet","routing","flet_route_static","routes","flet app","flet-route","flet simple routing"],
     description="This makes it easy to manage multiple views with dynamic routing.",
```

