# Comparing `tmp/altstore_proxy-1.1.2.tar.gz` & `tmp/altstore_proxy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altstore_proxy-1.1.2.tar", last modified: Sat May 18 19:05:37 2024, max compression
+gzip compressed data, was "altstore_proxy-1.2.0.tar", last modified: Sun May 19 09:37:38 2024, max compression
```

## Comparing `altstore_proxy-1.1.2.tar` & `altstore_proxy-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/altstore_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/altstore_proxy/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/altstore_proxy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/altstore_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 19:05:37.000000 altstore_proxy-1.1.2/altstore_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 19:05:37.357455 altstore_proxy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-18 19:05:32.000000 altstore_proxy-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/altstore_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/altstore_proxy/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/altstore_proxy/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/altstore_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 09:37:38.000000 altstore_proxy-1.2.0/altstore_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:37:38.120103 altstore_proxy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-19 09:37:32.000000 altstore_proxy-1.2.0/setup.py
```

### Comparing `altstore_proxy-1.1.2/PKG-INFO` & `altstore_proxy-1.2.0/altstore_proxy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: altstore_proxy
-Version: 1.1.2
+Name: altstore-proxy
+Version: 1.2.0
 Summary: A simple proxy for slow AltStore servers
-Home-page: https://github.com/rix1337/docker-altstore-proxy
+Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 #  AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 A simple proxy for slow AltStore servers.
@@ -24,27 +25,24 @@
 `pip install altstore_proxy`
 
 # Run
 
 ```
 altstore_proxy
   --port=8080
-  --baseurl=https://example.com/
+  --baseurl=https://example.com
   --cache=/tmp/altstore_cache
   --repos=https://fake.tld/apps.json,https://foo.bar/altstore.json
 ```
 
 # Docker
 ```
 docker run -d \
   --name="AltStore-Proxy" \
   -p port:8080 \
   -v /path/to/cache/:/cache:rw \
-  rix1337/docker-altstore-proxy
+  -e 'BASEURL'='https://example.com'
+  -e 'REPOS'='https://fake.tld/apps.json,https://foo.bar/altstore.json'
+  rix1337/docker-altstore-proxy:latest
   ```
-## Optional Environment Variables
- - `-e BASEURL` Base URL for the AltStore-Proxy (for reverse proxy usage)
- - `-e REPOS` Desired apps.json Repositories to Cache - comma separated
-
-
```

### Comparing `altstore_proxy-1.1.2/README.md` & `altstore_proxy-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -10,25 +10,22 @@
 `pip install altstore_proxy`
 
 # Run
 
 ```
 altstore_proxy
   --port=8080
-  --baseurl=https://example.com/
+  --baseurl=https://example.com
   --cache=/tmp/altstore_cache
   --repos=https://fake.tld/apps.json,https://foo.bar/altstore.json
 ```
 
 # Docker
 ```
 docker run -d \
   --name="AltStore-Proxy" \
   -p port:8080 \
   -v /path/to/cache/:/cache:rw \
-  rix1337/docker-altstore-proxy
+  -e 'BASEURL'='https://example.com'
+  -e 'REPOS'='https://fake.tld/apps.json,https://foo.bar/altstore.json'
+  rix1337/docker-altstore-proxy:latest
   ```
-## Optional Environment Variables
- - `-e BASEURL` Base URL for the AltStore-Proxy (for reverse proxy usage)
- - `-e REPOS` Desired apps.json Repositories to Cache - comma separated
-
-
```

### Comparing `altstore_proxy-1.1.2/altstore_proxy/proxy.py` & `altstore_proxy-1.2.0/altstore_proxy/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 # AltStore-Proxy
-# Projekt by https://github.com/rix1337
+# Project by https://github.com/rix1337
 
 import argparse
 import multiprocessing
 import os
 import sys
 import time
 from socketserver import ThreadingMixIn
 from wsgiref.simple_server import make_server, WSGIServer, WSGIRequestHandler
 
 import requests
 from bottle import Bottle, abort, static_file
 from tqdm import tqdm
 
-from altstore_proxy.providers import shared_state
-from altstore_proxy.version import get_version
+from altstore_proxy.providers import shared_state, version
 
 
 class ThreadingWSGIServer(ThreadingMixIn, WSGIServer):
     daemon_threads = True
 
 
 class NoLoggingWSGIRequestHandler(WSGIRequestHandler):
@@ -44,42 +43,43 @@
     total_size_in_bytes = int(response.headers.get('content-length', 0))
 
     # Resolve the actual URL if the provided URL is a shortened URL
     if "tinyurl.com" in url:
         url = response.url
 
     filename = os.path.join(shared_state.values["cache"], os.path.basename(url))
-
-    print(f"Downloading {url} to {filename}")
     os.makedirs(os.path.dirname(filename), exist_ok=True)
 
     # Check if file already exists and compare sizes
     if os.path.exists(filename):
         existing_file_size = os.path.getsize(filename)
         if existing_file_size == total_size_in_bytes:
             print(f"File {filename} already exists with the same size. Skipping download.")
             return filename
 
+    print(f"Downloading {url} to {filename}")
     progress_bar = tqdm(total=total_size_in_bytes, unit='iB', unit_scale=True)
     with open(filename, 'wb') as f:
         for data in response.iter_content(chunk_size=1024):
             progress_bar.update(len(data))
             f.write(data)
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong")
 
     return filename
 
 
-def merge_jsons(shared_state_dict, shared_state_lock):
+def update_json_proxy(shared_state_dict, shared_state_lock):
     shared_state.set_state(shared_state_dict, shared_state_lock)
 
     try:
         while True:
+            print("[AltStore-Proxy] Updating cache...")
+
             merged_json = {
                 "name": "AltStore-Proxy",
                 "subtitle": "A simple proxy for slow AltStore servers.",
                 "iconURL": "https://altstore.io/images/AltStore_AppIcon.png",
                 "website": "https://github.com/rix1337/AltStore-Proxy",
                 "apps": [],
                 "news": []
@@ -107,15 +107,15 @@
 
 def main():
     with multiprocessing.Manager() as manager:
         shared_state_dict = manager.dict()
         shared_state_lock = manager.Lock()
         shared_state.set_state(shared_state_dict, shared_state_lock)
 
-        print("[AltStore-Proxy] Version " + get_version() + " by rix1337")
+        print("[AltStore-Proxy] Version " + version.get_version() + " by rix1337")
         shared_state.update("ready", False)
 
         parser = argparse.ArgumentParser()
         parser.add_argument("--port", help="Desired Port, defaults to 8080")
         parser.add_argument("--baseurl", help="Base URL for the AltStore-Proxy (for reverse proxy usage)")
         parser.add_argument("--cache", help="Desired Cache Directory, defaults to ./cache")
         parser.add_argument("--repos", help="Desired apps.json Repositories to Cache - comma separated")
@@ -130,14 +130,15 @@
         else:
             shared_state.update("port", 8080)
 
         if arguments.cache:
             shared_state.update("cache", arguments.cache)
         else:
             shared_state.update("cache", "./cache")
+
         if arguments.baseurl:
             shared_state.update("baseurl", arguments.baseurl)
         else:
             shared_state.update("baseurl", "http://127.0.0.1:" + str(shared_state.values["port"]))
 
         if shared_state.values["baseurl"][-1] == "/":
             shared_state.update("baseurl", shared_state.values["baseurl"][:-1])
@@ -224,15 +225,15 @@
         def status():
             try:
                 return shared_state.values["merged_json"]
             except Exception as e:
                 print("[AntiGateHandler] status - Error: " + str(e))
             return abort(503, "Cache not initialized. Please try again later.")
 
-        hourly_update = multiprocessing.Process(target=merge_jsons, args=(shared_state_dict, shared_state_lock,))
+        hourly_update = multiprocessing.Process(target=update_json_proxy, args=(shared_state_dict, shared_state_lock,))
         hourly_update.start()
 
         while not shared_state.values["ready"]:
             time.sleep(1)
 
         print(
             "[AltStore-Proxy] Add this source to AltStore by opening " + shared_state.values[
```

### Comparing `altstore_proxy-1.1.2/altstore_proxy.egg-info/PKG-INFO` & `altstore_proxy-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: altstore-proxy
-Version: 1.1.2
+Name: altstore_proxy
+Version: 1.2.0
 Summary: A simple proxy for slow AltStore servers
-Home-page: https://github.com/rix1337/docker-altstore-proxy
+Home-page: https://github.com/rix1337/AltStore-Proxy
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 #  AltStore-Proxy
 
 [![PyPI version](https://badge.fury.io/py/altstore-proxy.svg)](https://badge.fury.io/py/altstore-proxy)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 A simple proxy for slow AltStore servers.
@@ -24,27 +25,24 @@
 `pip install altstore_proxy`
 
 # Run
 
 ```
 altstore_proxy
   --port=8080
-  --baseurl=https://example.com/
+  --baseurl=https://example.com
   --cache=/tmp/altstore_cache
   --repos=https://fake.tld/apps.json,https://foo.bar/altstore.json
 ```
 
 # Docker
 ```
 docker run -d \
   --name="AltStore-Proxy" \
   -p port:8080 \
   -v /path/to/cache/:/cache:rw \
-  rix1337/docker-altstore-proxy
+  -e 'BASEURL'='https://example.com'
+  -e 'REPOS'='https://fake.tld/apps.json,https://foo.bar/altstore.json'
+  rix1337/docker-altstore-proxy:latest
   ```
-## Optional Environment Variables
- - `-e BASEURL` Base URL for the AltStore-Proxy (for reverse proxy usage)
- - `-e REPOS` Desired apps.json Repositories to Cache - comma separated
-
-
```

### Comparing `altstore_proxy-1.1.2/setup.py` & `altstore_proxy-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # AltStore-Proxy
 # Projekt by https://github.com/rix1337
 
 import setuptools
 
-from altstore_proxy.version import get_version
+from altstore_proxy.providers.version import get_version
 
 try:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 except:
     import io
 
@@ -21,23 +21,23 @@
     name="altstore_proxy",
     version=get_version(),
     author="rix1337",
     author_email="",
     description="A simple proxy for slow AltStore servers",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/rix1337/docker-altstore-proxy",
+    url="https://github.com/rix1337/AltStore-Proxy",
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
-            'altstore_proxy = altstore_proxy.proxy:main',
+            'altstore_proxy = altstore_proxy.run:main',
         ],
     },
 )
```

