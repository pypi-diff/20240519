# Comparing `tmp/warp_python-1.2.8.tar.gz` & `tmp/warp_python-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warp_python-1.2.8.tar", last modified: Sat May 18 15:31:06 2024, max compression
+gzip compressed data, was "warp_python-1.2.9.tar", last modified: Sat May 18 15:35:57 2024, max compression
```

## Comparing `warp_python-1.2.8.tar` & `warp_python-1.2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.790283 warp_python-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:31:01.000000 warp_python-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:31:06.790283 warp_python-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:31:01.000000 warp_python-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:31:06.790283 warp_python-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-18 15:31:01.000000 warp_python-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.786283 warp_python-1.2.8/warp/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.786283 warp_python-1.2.8/warp/host/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/host/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/host/host.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:31:01.000000 warp_python-1.2.8/warp/set_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:31:06.790283 warp_python-1.2.8/warp_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:31:06.000000 warp_python-1.2.8/warp_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:35:57.258166 warp_python-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-18 15:35:53.000000 warp_python-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:35:57.258166 warp_python-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-18 15:35:53.000000 warp_python-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 15:35:57.258166 warp_python-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-18 15:35:53.000000 warp_python-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:35:57.254166 warp_python-1.2.9/warp/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 15:35:53.000000 warp_python-1.2.9/warp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:35:57.258166 warp_python-1.2.9/warp/host/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-18 15:35:53.000000 warp_python-1.2.9/warp/host/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-05-18 15:35:53.000000 warp_python-1.2.9/warp/host/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-18 15:35:53.000000 warp_python-1.2.9/warp/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-18 15:35:53.000000 warp_python-1.2.9/warp/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 15:35:53.000000 warp_python-1.2.9/warp/set_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 15:35:57.258166 warp_python-1.2.9/warp_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-18 15:35:57.000000 warp_python-1.2.9/warp_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-18 15:35:57.000000 warp_python-1.2.9/warp_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 15:35:57.000000 warp_python-1.2.9/warp_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 15:35:57.000000 warp_python-1.2.9/warp_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 15:35:57.000000 warp_python-1.2.9/warp_python.egg-info/top_level.txt
```

### Comparing `warp_python-1.2.8/LICENSE` & `warp_python-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.8/PKG-INFO` & `warp_python-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.8
+Version: 1.2.9
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project, Ryan_shamu
 Author-email: simon.c.gilde@gmail.com, ryanshamu418@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `warp_python-1.2.8/setup.py` & `warp_python-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import os
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '1.2.8'
+VERSION = '1.2.9'
 
 setup(
     name='warp-python',
     version=VERSION,
     author='warp-project, Ryan_shamu',
     author_email='simon.c.gilde@gmail.com, ryanshamu418@gmail.com',
     description='A python module for WARP',
```

### Comparing `warp_python-1.2.8/warp/host/host.py` & `warp_python-1.2.9/warp/host/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,27 +29,30 @@
         self.domains = domains or {}
         self.tlds = tlds or [tld]
         self.tlds = [_tld.strip(".") for _tld in self.tlds]
         try:
             assert tld or tlds
         except AssertionError:
             raise ValueError("Pass either tld or tlds")
+        def get_tld(domain_name):
+            return domain_name.split(".")[-1]
         @app.get("/resolve/<domain_name>/")
         def resolve_domain(domain_name : str):
-            if not domain_name.endswith("."+tld):
+            domain_tld = get_tld(domain_name)
+            if domain_tld not in self.tlds:
                 return jsonify({"success": False, "ip": None, "reason": "Wrong server"})
             try:
                 domain = domains[domain_name]
             except KeyError:
                 return jsonify({"success": False, "ip": None, "reason": "Domain doesn't exist"})
             return jsonify({"success": True, "ip": domain["ip"], "reason": "Found"})
         
         @app.post("/set_ip/<domain_name>/")
         def set_domain_ip(domain_name : str):
-            domain_tld = domain_name.split(".")[-1]
+            domain_tld = get_tld(domain_name)
             if domain_tld not in self.tlds:
                 return jsonify({"success": False, "ip": None, "reason": "Wrong server"})
             try:
                 domain = domains[domain_name]
             except KeyError:
                 return jsonify({"success": False, "ip": None, "reason": "Domain doesn't exist"})
             data = request.json
```

### Comparing `warp_python-1.2.8/warp/resolve.py` & `warp_python-1.2.9/warp/resolve.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.8/warp/set_ip.py` & `warp_python-1.2.9/warp/set_ip.py`

 * *Files identical despite different names*

### Comparing `warp_python-1.2.8/warp_python.egg-info/PKG-INFO` & `warp_python-1.2.9/warp_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warp-python
-Version: 1.2.8
+Version: 1.2.9
 Summary: A python module for WARP
 Home-page: https://github.com/warp-project/warp-python
 Author: warp-project, Ryan_shamu
 Author-email: simon.c.gilde@gmail.com, ryanshamu418@gmail.com
 Keywords: warp
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

