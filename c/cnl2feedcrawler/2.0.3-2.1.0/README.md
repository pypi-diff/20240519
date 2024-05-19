# Comparing `tmp/cnl2feedcrawler-2.0.3.tar.gz` & `tmp/cnl2feedcrawler-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnl2feedcrawler-2.0.3.tar", last modified: Sun Nov  6 13:42:37 2022, max compression
+gzip compressed data, was "cnl2feedcrawler-2.1.0.tar", last modified: Sun May 19 12:23:50 2024, max compression
```

## Comparing `cnl2feedcrawler-2.0.3.tar` & `cnl2feedcrawler-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:37.039404 cnl2feedcrawler-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-11-06 13:42:37.035404 cnl2feedcrawler-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-11-06 13:42:30.000000 cnl2feedcrawler-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:37.035404 cnl2feedcrawler-2.0.3/cnl2feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:30.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9178 2022-11-06 13:42:30.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler/cnl2feedcrawler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:37.035404 cnl2feedcrawler-2.0.3/cnl2feedcrawler/http_requests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:30.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6994 2022-11-06 13:42:30.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler/http_requests/request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 13:42:37.035404 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2086 2022-11-06 13:42:36.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-11-06 13:42:37.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 13:42:36.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-06 13:42:36.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 13:42:36.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-06 13:42:36.000000 cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-06 13:42:37.039404 cnl2feedcrawler-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-11-06 13:42:30.000000 cnl2feedcrawler-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.153802 cnl2feedcrawler-2.1.0/cnl2feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.153802 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9256 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 12:23:50.153802 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-19 12:23:50.000000 cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 12:23:50.157802 cnl2feedcrawler-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-19 12:23:44.000000 cnl2feedcrawler-2.1.0/setup.py
```

### Comparing `cnl2feedcrawler-2.0.3/PKG-INFO` & `cnl2feedcrawler-2.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: cnl2feedcrawler
-Version: 2.0.3
+Version: 2.1.0
 Summary: Intercept, decrypt and forward CnL to FeedCrawler
 Home-page: https://github.com/rix1337/ClickNLoad2FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
-Description: # Click'n'Load2FeedCrawler
-        Click'n'Load2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
-        
-        [![PyPI version](https://badge.fury.io/py/cnl2feedcrawler.svg)](https://badge.fury.io/py/cnl2feedcrawler)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/cnl2feedcrawler)](https://img.shields.io/pypi/dm/cnl2feedcrawler)
-        [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
-        
-        ####  Voraussetzungen
-        * Linux basierte Laufzeitumgebung (inkompatibel mit Windows)
-        * [Python 3.6](https://www.python.org/downloads/) oder neuer
-        * [pip](https://pip.pypa.io/en/stable/installing/)
-        * [openssl](https://www.openssl.org/)
-        * [Node.js](https://nodejs.org/)
-        * [FeedCrawler](https://github.com/rix1337/FeedCrawler)
-        
-        #### Update
-        
-        ```pip install -U cnl2feedcrawler```
-        
-        #### Starten
-        
-        ```cnl2feedcrawler --url=192.168.1.1:9090``` in der Konsole (Python muss im System-PATH hinterlegt sein)
-        
-        
-        #### Pflichtparameter
-        
-        | Parameter         | Erläuterung                                                        |
-        |-------------------|--------------------------------------------------------------------|
-        | ```--url=<URL>``` | Die lokale URL des FeedCrawlers - bspw. `http://192.168.1.1:9090`) |
-        
-        ***
-        
-        ## Credits
-        
-        * [drwilly](https://github.com/drwilly)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Click'n'Load2FeedCrawler
+Click'n'Load2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
+
+[![PyPI version](https://badge.fury.io/py/cnl2feedcrawler.svg)](https://badge.fury.io/py/cnl2feedcrawler)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/cnl2feedcrawler)](https://img.shields.io/pypi/dm/cnl2feedcrawler)
+[![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
+
+####  Voraussetzungen
+* Linux basierte Laufzeitumgebung (inkompatibel mit Windows)
+* [Python 3.6](https://www.python.org/downloads/) oder neuer
+* [pip](https://pip.pypa.io/en/stable/installing/)
+* [openssl](https://www.openssl.org/)
+* [Node.js](https://nodejs.org/)
+* [FeedCrawler](https://github.com/rix1337/FeedCrawler)
+
+#### Update
+
+```pip install -U cnl2feedcrawler```
+
+#### Starten
+
+```cnl2feedcrawler --url=192.168.1.1:9090``` in der Konsole (Python muss im System-PATH hinterlegt sein)
+
+
+#### Pflichtparameter
+
+| Parameter         | Erläuterung                                                        |
+|-------------------|--------------------------------------------------------------------|
+| ```--url=<URL>``` | Die lokale URL des FeedCrawlers - bspw. `http://192.168.1.1:9090`) |
+
+***
+
+## Credits
+
+* [drwilly](https://github.com/drwilly)
+
+
```

### Comparing `cnl2feedcrawler-2.0.3/README.md` & `cnl2feedcrawler-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cnl2feedcrawler-2.0.3/cnl2feedcrawler/cnl2feedcrawler.py` & `cnl2feedcrawler-2.1.0/cnl2feedcrawler/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # ClickNLoad2FeedCrawler
-# Projekt von https://github.com/rix1337
+# Projekt by https://github.com/rix1337
 #
 # Enthält Code von https://github.com/drwilly/clicknload2text
 # Lizenz: https://github.com/drwilly/clicknload2text/blob/master/LICENSE
 
 """FeedCrawler.
 
 Usage:
@@ -21,15 +21,16 @@
 import http.server
 import json
 import socket
 import subprocess
 import sys
 from io import StringIO
 
-from cnl2feedcrawler.http_requests.request_handler import request
+from cnl2feedcrawler.providers.http_requests.request_handler import request
+from cnl2feedcrawler.providers.version import get_version
 
 feedcrawler_url = ""
 
 
 class URLMap:
     def __init__(self, pattern, get_fn=None, post_fn=None):
         self.pattern = pattern
@@ -228,18 +229,18 @@
         s.close()
     return ip
 
 
 def main():
     global feedcrawler_url
 
-    print(u"┌──────────────────────────────────────────────────┐")
-    print(u"  Click'n'Load2FeedCrawler von RiX")
-    print(u"  https://github.com/rix1337/ClickNLoad2FeedCrawler")
-    print(u"└──────────────────────────────────────────────────┘")
+    print("┌──────────────────────────────────────────────────┐")
+    print(f"  Click'n'Load2FeedCrawler v.{get_version()} von RiX")
+    print("  https://github.com/rix1337/ClickNLoad2FeedCrawler")
+    print("└──────────────────────────────────────────────────┘")
     local_address = 'http://' + check_ip() + ':' + str(9666)
 
     # Test if NodeJS is available
     try:
         node_version = call(["node", "-v"])
     except FileNotFoundError:
         print("NodeJS ist nicht verfügbar!")
@@ -265,28 +266,28 @@
     url = arguments.url.replace("http://", "").replace("https://", "")
     if url.endswith("/"):
         url = url[:-1]
     feedcrawler_url = "http://" + url + "/"
     try:
         feedcrawler_version = request(feedcrawler_url + "api/version/")
     except:
-        print(u"Fehler beim Verbinden mit " + feedcrawler_url + "!")
+        print("Fehler beim Verbinden mit " + feedcrawler_url + "!")
         sys.exit(1)
     if feedcrawler_version.status_code == 200:
         try:
             feedcrawler_version = json.loads(feedcrawler_version.text)["version"]["ver"].replace("v.", "").strip()
-            print(u"Nutze FeedCrawler " + feedcrawler_version + " zur Übergabe der Links an My JDownloader")
+            print("Nutze FeedCrawler " + feedcrawler_version + " zur Übergabe der Links an My JDownloader")
         except:
             pass
     if not feedcrawler_version:
-        print(u"FeedCrawler Version nicht ermittelbar!")
+        print("FeedCrawler Version nicht ermittelbar!")
         sys.exit(1)
 
     httpd = http.server.HTTPServer(("0.0.0.0", 9666), CNLHandler)
-    print(u"Click'n'Load ist verfügbar unter http://127.0.0.1:9666 und " + local_address)
+    print("Click'n'Load ist verfügbar unter http://127.0.0.1:9666 und " + local_address)
     try:
         httpd.serve_forever()
     except KeyboardInterrupt:
         pass
     finally:
         httpd.server_close()
```

### Comparing `cnl2feedcrawler-2.0.3/cnl2feedcrawler/http_requests/request_handler.py` & `cnl2feedcrawler-2.1.0/cnl2feedcrawler/providers/http_requests/request_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # FeedCrawler
-# Projekt von https://github.com/rix1337
+# Projekt by https://github.com/rix1337
 #
 # Dieses Modul realisiert HTTP-Requests auf Basis der Python-eigenen urllib-Bibliothek
 #
 # Enthält Code von:
 # https://github.com/sesh/thttp
 #
 # This is free and unencumbered software released into the public domain.
```

### Comparing `cnl2feedcrawler-2.0.3/cnl2feedcrawler.egg-info/PKG-INFO` & `cnl2feedcrawler-2.1.0/cnl2feedcrawler.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 Metadata-Version: 2.1
 Name: cnl2feedcrawler
-Version: 2.0.3
+Version: 2.1.0
 Summary: Intercept, decrypt and forward CnL to FeedCrawler
 Home-page: https://github.com/rix1337/ClickNLoad2FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
-Description: # Click'n'Load2FeedCrawler
-        Click'n'Load2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
-        
-        [![PyPI version](https://badge.fury.io/py/cnl2feedcrawler.svg)](https://badge.fury.io/py/cnl2feedcrawler)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/cnl2feedcrawler)](https://img.shields.io/pypi/dm/cnl2feedcrawler)
-        [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
-        
-        ####  Voraussetzungen
-        * Linux basierte Laufzeitumgebung (inkompatibel mit Windows)
-        * [Python 3.6](https://www.python.org/downloads/) oder neuer
-        * [pip](https://pip.pypa.io/en/stable/installing/)
-        * [openssl](https://www.openssl.org/)
-        * [Node.js](https://nodejs.org/)
-        * [FeedCrawler](https://github.com/rix1337/FeedCrawler)
-        
-        #### Update
-        
-        ```pip install -U cnl2feedcrawler```
-        
-        #### Starten
-        
-        ```cnl2feedcrawler --url=192.168.1.1:9090``` in der Konsole (Python muss im System-PATH hinterlegt sein)
-        
-        
-        #### Pflichtparameter
-        
-        | Parameter         | Erläuterung                                                        |
-        |-------------------|--------------------------------------------------------------------|
-        | ```--url=<URL>``` | Die lokale URL des FeedCrawlers - bspw. `http://192.168.1.1:9090`) |
-        
-        ***
-        
-        ## Credits
-        
-        * [drwilly](https://github.com/drwilly)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Click'n'Load2FeedCrawler
+Click'n'Load2FeedCrawler fängt Click'n'Load ab, entschlüsselt die Payload und übergibt diese dem FeedCrawler.
+
+[![PyPI version](https://badge.fury.io/py/cnl2feedcrawler.svg)](https://badge.fury.io/py/cnl2feedcrawler)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/cnl2feedcrawler)](https://img.shields.io/pypi/dm/cnl2feedcrawler)
+[![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
+
+####  Voraussetzungen
+* Linux basierte Laufzeitumgebung (inkompatibel mit Windows)
+* [Python 3.6](https://www.python.org/downloads/) oder neuer
+* [pip](https://pip.pypa.io/en/stable/installing/)
+* [openssl](https://www.openssl.org/)
+* [Node.js](https://nodejs.org/)
+* [FeedCrawler](https://github.com/rix1337/FeedCrawler)
+
+#### Update
+
+```pip install -U cnl2feedcrawler```
+
+#### Starten
+
+```cnl2feedcrawler --url=192.168.1.1:9090``` in der Konsole (Python muss im System-PATH hinterlegt sein)
+
+
+#### Pflichtparameter
+
+| Parameter         | Erläuterung                                                        |
+|-------------------|--------------------------------------------------------------------|
+| ```--url=<URL>``` | Die lokale URL des FeedCrawlers - bspw. `http://192.168.1.1:9090`) |
+
+***
+
+## Credits
+
+* [drwilly](https://github.com/drwilly)
+
+
```

### Comparing `cnl2feedcrawler-2.0.3/setup.py` & `cnl2feedcrawler-2.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 # ClickNLoad2FeedCrawler
-# Projekt von https://github.com/rix1337
+# Projekt by https://github.com/rix1337
 
 import setuptools
 
+from cnl2feedcrawler.providers.version import get_version
+
 try:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 except:
     import io
 
     long_description = io.open('README.md', encoding='utf-8').read()
 
 setuptools.setup(
     name="cnl2feedcrawler",
-    version="2.0.3",
+    version=get_version(),
     author="rix1337",
     author_email="",
     description="Intercept, decrypt and forward CnL to FeedCrawler",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rix1337/ClickNLoad2FeedCrawler",
     packages=setuptools.find_packages(),
@@ -27,11 +29,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
     ],
     entry_points={
         'console_scripts': [
-            'cnl2feedcrawler = cnl2feedcrawler.cnl2feedcrawler:main',
+            'cnl2feedcrawler = cnl2feedcrawler.run:main',
         ],
     },
 )
```

