# Comparing `tmp/myjd_api-1.1.1.tar.gz` & `tmp/myjd_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myjd_api-1.1.1.tar", last modified: Sat Jan  6 08:38:48 2024, max compression
+gzip compressed data, was "myjd_api-1.2.0.tar", last modified: Sun May 19 11:25:51 2024, max compression
```

## Comparing `myjd_api-1.1.1.tar` & `myjd_api-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:38:48.254718 myjd_api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-06 08:38:42.000000 myjd_api-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-01-06 08:38:48.254718 myjd_api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-01-06 08:38:42.000000 myjd_api-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:38:48.254718 myjd_api-1.1.1/myjd_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    23318 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/myjd.py
--rw-r--r--   0 runner    (1001) docker     (127)    39854 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/myjdapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14223 2024-01-06 08:38:42.000000 myjd_api-1.1.1/myjd_api/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 08:38:48.254718 myjd_api-1.1.1/myjd_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-06 08:38:48.000000 myjd_api-1.1.1/myjd_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 08:38:48.254718 myjd_api-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-01-06 08:38:42.000000 myjd_api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:25:51.875368 myjd_api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 11:25:46.000000 myjd_api-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-19 11:25:51.875368 myjd_api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-19 11:25:46.000000 myjd_api-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:25:51.871369 myjd_api-1.2.0/myjd_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:25:51.875368 myjd_api-1.2.0/myjd_api/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/myjd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39864 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/myjdapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-05-19 11:25:46.000000 myjd_api-1.2.0/myjd_api/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:25:51.871369 myjd_api-1.2.0/myjd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 11:25:51.000000 myjd_api-1.2.0/myjd_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:25:51.875368 myjd_api-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-19 11:25:46.000000 myjd_api-1.2.0/setup.py
```

### Comparing `myjd_api-1.1.1/LICENSE.md` & `myjd_api-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `myjd_api-1.1.1/PKG-INFO` & `myjd_api-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: myjd_api
-Version: 1.1.1
-Summary: A simple json interface for the MyJDownloader API to be used with Organizr
-Home-page: https://github.com/rix1337/MyJD-API
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 #  MyJD-API
 
 [![PyPI version](https://badge.fury.io/py/myjd-api.svg)](https://badge.fury.io/py/myjd-api)
 [![Github Sponsorship](https://img.shields.io/badge/support-me-red.svg)](https://github.com/users/rix1337/sponsorship)
 
 This is a standalone version of [FeedCrawler](https://github.com/rix1337/FeedCrawler)'s MyJDownloader API for use with projects like [Organizr](https://github.com/causefx/Organizr).
 
@@ -26,20 +11,36 @@
 
 `pip install myjd-api`
 
 # Run
 
 `myjd_api`
 
-# Parameters
+## Parameters
 * `--jd-user` Set your My JDownloader username 
 * `--jd-pass` Set your My JDownloader password 
 * `--jd-device` Set your My JDownloader device name 
 * `--port` _Optional:_ Set desired Port to serve the API 
 * `--username` _Optional:_ Set desired username for the API 
 * `--password` _Optional:_ Set desired username for the API 
 
-## Credits
+# Docker
+```
+docker run -d \
+  --name="MyJD-API" \
+  -p port:8080 \
+  -v /path/to/config/:/config:rw \
+  -e USER=USERNAME \ 
+  -e PASS=PASSWORD \
+  -e DEVICE=DEVICENAME \
+  rix1337/docker-myjd-api
+  ```
+  
+## Optional Parameters
+ - `-e USER` (after first run, if unchanged)
+ - `-e PASS` (after first run, if unchanged)
+ - `-e DEVICE` (always, if only one device is present at MyJD-Account, otherwise after first run, if unchanged)
 
-* [mmarquezs](https://github.com/mmarquezs/)
 
+## Credits
 
+* [mmarquezs](https://github.com/mmarquezs/)
```

### Comparing `myjd_api-1.1.1/myjd_api/common.py` & `myjd_api-1.2.0/myjd_api/providers/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # MyJD
 # Project by https://github.com/rix1337
 
 
 import base64
 import socket
 
-from myjd_api import myjdapi
+from myjd_api.providers import myjdapi
 
 
 def check_ip():
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         s.connect(('10.255.255.255', 0))
         ip = s.getsockname()[0]
```

### Comparing `myjd_api-1.1.1/myjd_api/config.py` & `myjd_api-1.2.0/myjd_api/providers/config.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.1.1/myjd_api/files.py` & `myjd_api-1.2.0/myjd_api/providers/files.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 # MyJD
 # Project by https://github.com/rix1337
 
 import os
 import sys
 
-from myjd_api.config import Config
-from myjd_api.myjd import get_device
-from myjd_api.myjd import get_if_one_device
+from myjd_api.providers.config import Config
+from myjd_api.providers.myjd import get_device
+from myjd_api.providers.myjd import get_if_one_device
 
 
 def config():
     configfile = "MyJD.conf"
     configpath = ""
     if os.path.exists(configfile):
         f = open(configfile, "r")
```

### Comparing `myjd_api-1.1.1/myjd_api/myjd.py` & `myjd_api-1.2.0/myjd_api/providers/myjd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 # -*- coding: utf-8 -*-
 # MyJD
 # Project by https://github.com/rix1337
 
-import myjd_api.myjdapi
-from myjd_api.common import is_device
-from myjd_api.common import readable_size
-from myjd_api.common import readable_time
-from myjd_api.config import Config
+import myjd_api.providers.myjdapi
+from myjd_api.providers.common import is_device
+from myjd_api.providers.common import readable_size
+from myjd_api.providers.common import readable_time
+from myjd_api.providers.config import Config
 
 
 def get_device(configfile):
     conf = Config('MyJD', configfile)
     myjd_user = str(conf.get('myjd_user'))
     myjd_pass = str(conf.get('myjd_pass'))
     myjd_device = str(conf.get('myjd_device'))
 
-    jd = myjd_api.myjdapi.Myjdapi()
+    jd = myjd_api.providers.myjdapi.Myjdapi()
     jd.set_app_key('MyJD')
 
     if myjd_user and myjd_pass and myjd_device:
         try:
             try:
                 jd.connect(myjd_user, myjd_pass)
                 jd.update_devices()
                 device = jd.get_device(myjd_device)
-            except myjd_api.myjdapi.RequestTimeoutException:
+            except myjd_api.providers.myjdapi.RequestTimeoutException:
                 device = jd.get_device(myjd_device)
-        except myjd_api.myjdapi.MYJDException as e:
+        except myjd_api.providers.myjdapi.MYJDException as e:
             print(u"Error connection to MyJDownloader: " + str(e))
             return False
         if not device or not is_device(device):
             return False
         return device
     elif myjd_user and myjd_pass:
         myjd_device = get_if_one_device(myjd_user, myjd_pass)
         if myjd_device:
             Config('MyJD', configfile).save("myjd_device", myjd_device)
         try:
             jd.connect(myjd_user, myjd_pass)
             jd.update_devices()
             device = jd.get_device(myjd_device)
-        except myjd_api.myjdapi.MYJDException as e:
+        except myjd_api.providers.myjdapi.MYJDException as e:
             print(u"Error connection to MyJDownloader: " + str(e))
             return False
         if not device or not is_device(device):
             return False
         return device
     else:
         return False
 
 
 def check_device(myjd_user, myjd_pass, myjd_device):
-    jd = myjd_api.myjdapi.Myjdapi()
+    jd = myjd_api.providers.myjdapi.Myjdapi()
     jd.set_app_key('MyJD')
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         device = jd.get_device(myjd_device)
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
     return device
 
 
 def get_if_one_device(myjd_user, myjd_pass):
-    jd = myjd_api.myjdapi.Myjdapi()
+    jd = myjd_api.providers.myjdapi.Myjdapi()
     jd.set_app_key('MyJD')
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         devices = jd.list_devices()
         if len(devices) == 1:
             return devices[0].get('name')
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def get_packages_in_downloader(device):
     links = device.downloads.query_links()
 
@@ -245,24 +245,24 @@
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 downloader_state = device.downloadcontroller.get_current_state()
                 grabber_collecting = device.linkgrabber.is_collecting()
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 downloader_state = device.downloadcontroller.get_current_state()
                 grabber_collecting = device.linkgrabber.is_collecting()
             return [device, downloader_state, grabber_collecting]
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def get_info(configfile, device):
     try:
         if not device or not is_device(device):
@@ -279,15 +279,15 @@
                 packages_in_downloader_offline = packages_in_downloader[1]
                 packages_in_downloader_decrypted = packages_in_downloader[2]
 
                 packages_in_linkgrabber = get_packages_in_linkgrabber(device)
                 packages_in_linkgrabber_failed = packages_in_linkgrabber[0]
                 packages_in_linkgrabber_offline = packages_in_linkgrabber[1]
                 packages_in_linkgrabber_decrypted = packages_in_linkgrabber[2]
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 downloader_state = device.downloadcontroller.get_current_state()
                 grabber_collecting = device.linkgrabber.is_collecting()
                 device.update.run_update_check()
                 update_ready = device.update.is_update_available()
@@ -318,57 +318,57 @@
 
             return [device, downloader_state, grabber_collecting, update_ready,
                     [packages_in_downloader_decrypted, packages_in_linkgrabber_decrypted,
                      packages_offline,
                      packages_failed]]
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def move_to_downloads(configfile, device, linkids, uuid):
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 device.linkgrabber.move_to_downloadlist(linkids, uuid)
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 device.linkgrabber.move_to_downloadlist(linkids, uuid)
             return device
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def remove_from_linkgrabber(configfile, device, linkids, uuid):
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 device.linkgrabber.remove_links(linkids, uuid)
                 device.downloads.remove_links(linkids, uuid)
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 device.linkgrabber.remove_links(linkids, uuid)
                 device.downloads.remove_links(linkids, uuid)
             return device
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def download(configfile, device, title, subdir, links, password, full_path=None):
     try:
         if not device or not is_device(device):
@@ -398,15 +398,15 @@
                     "packageName": title,
                     "extractPassword": password,
                     "priority": priority,
                     "downloadPassword": password,
                     "destinationFolder": path,
                     "overwritePackagizerRules": False
                 }])
-        except myjd_api.myjdapi.TokenExpiredException:
+        except myjd_api.providers.myjdapi.TokenExpiredException:
             device = get_device(configfile)
             if not device or not is_device(device):
                 return False
             device.linkgrabber.add_links(params=[
                 {
                     "autostart": autostart,
                     "links": links,
@@ -414,15 +414,15 @@
                     "extractPassword": password,
                     "priority": priority,
                     "downloadPassword": password,
                     "destinationFolder": path,
                     "overwritePackagizerRules": False
                 }])
         return device
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def retry_decrypt(configfile, device, linkids, uuid, links):
     try:
         if not device or not is_device(device):
@@ -443,15 +443,15 @@
                         "maxResults": -1,
                         "packageUUIDs": uuid,
                         "priority": True,
                         "saveTo": True,
                         "startAt": 0,
                         "status": True
                     }])
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 package = device.linkgrabber.query_packages(params=[
                     {
                         "availableOfflineCount": True,
                         "availableOnlineCount": True,
@@ -486,15 +486,15 @@
                             "childCount": True,
                             "hosts": True,
                             "saveTo": True,
                             "maxResults": -1,
                             "packageUUIDs": uuid,
                             "startAt": 0,
                         }])
-                except myjd_api.myjdapi.TokenExpiredException:
+                except myjd_api.providers.myjdapi.TokenExpiredException:
                     device = get_device(configfile)
                     if not device or not is_device(device):
                         return False
                     package = device.downloads.query_packages(params=[
                         {
                             "bytesLoaded": True,
                             "bytesTotal": True,
@@ -519,95 +519,95 @@
                 full_path = package[0].get('saveTo')
                 download(configfile, device, title, None, links, None, full_path)
                 return device
             else:
                 return False
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def update_jdownloader(configfile, device):
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 device.update.restart_and_update()
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 device.update.restart_and_update()
             return device
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def jdownloader_start(configfile, device):
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 device.downloadcontroller.start_downloads()
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 device.downloadcontroller.start_downloads()
             return device
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def jdownloader_pause(configfile, device, bl):
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 device.downloadcontroller.pause_downloads(bl)
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 device.downloadcontroller.pause_downloads(bl)
             return device
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def jdownloader_stop(configfile, device):
     try:
         if not device or not is_device(device):
             device = get_device(configfile)
         if device:
             try:
                 device.downloadcontroller.stop_downloads()
-            except myjd_api.myjdapi.TokenExpiredException:
+            except myjd_api.providers.myjdapi.TokenExpiredException:
                 device = get_device(configfile)
                 if not device or not is_device(device):
                     return False
                 device.downloadcontroller.stop_downloads()
             return device
         else:
             return False
-    except myjd_api.myjdapi.MYJDException as e:
+    except myjd_api.providers.myjdapi.MYJDException as e:
         print(u"Error connection to MyJDownloader: " + str(e))
         return False
 
 
 def myjd_download(configfile, device, title, subdir, links, password):
     if device:
         device = download(configfile, device, title, subdir, links, password)
```

### Comparing `myjd_api-1.1.1/myjd_api/myjdapi.py` & `myjd_api-1.2.0/myjd_api/providers/myjdapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import json
 import time
 from urllib.error import URLError
 from urllib.parse import quote
 
 from Cryptodome.Cipher import AES
 
-from myjd_api.requests import request
+from myjd_api.providers.requests import request
 
 BS = 16
 
 
 class MYJDException(BaseException):
     pass
```

### Comparing `myjd_api-1.1.1/myjd_api/requests.py` & `myjd_api-1.2.0/myjd_api/providers/requests.py`

 * *Files identical despite different names*

### Comparing `myjd_api-1.1.1/myjd_api/web.py` & `myjd_api-1.2.0/myjd_api/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 from functools import wraps
 from socketserver import ThreadingMixIn
 from wsgiref.simple_server import make_server, WSGIServer, WSGIRequestHandler
 
 from Cryptodome.Protocol.KDF import scrypt
 from Cryptodome.Random import get_random_bytes
 from bottle import Bottle, request, redirect, abort, HTTPError
-from myjd_api.common import check_ip
-from myjd_api.common import decode_base64
-from myjd_api.config import Config
-from myjd_api.files import config
-from myjd_api.files import myjd_input
-from myjd_api.myjd import get_device
-from myjd_api.myjd import get_if_one_device
-from myjd_api.myjd import get_info
-from myjd_api.myjd import get_state
-from myjd_api.myjd import jdownloader_pause
-from myjd_api.myjd import jdownloader_start
-from myjd_api.myjd import jdownloader_stop
-from myjd_api.myjd import move_to_downloads
-from myjd_api.myjd import remove_from_linkgrabber
-from myjd_api.myjd import retry_decrypt
-from myjd_api.myjd import update_jdownloader
-from myjd_api.version import get_version
+from myjd_api.providers.common import check_ip
+from myjd_api.providers.common import decode_base64
+from myjd_api.providers.config import Config
+from myjd_api.providers.files import config
+from myjd_api.providers.files import myjd_input
+from myjd_api.providers.myjd import get_device
+from myjd_api.providers.myjd import get_if_one_device
+from myjd_api.providers.myjd import get_info
+from myjd_api.providers.myjd import get_state
+from myjd_api.providers.myjd import jdownloader_pause
+from myjd_api.providers.myjd import jdownloader_start
+from myjd_api.providers.myjd import jdownloader_stop
+from myjd_api.providers.myjd import move_to_downloads
+from myjd_api.providers.myjd import remove_from_linkgrabber
+from myjd_api.providers.myjd import retry_decrypt
+from myjd_api.providers.myjd import update_jdownloader
+from myjd_api.providers.version import get_version
 
 
 class ThreadingWSGIServer(ThreadingMixIn, WSGIServer):
     daemon_threads = True
 
 
 class NoLoggingWSGIRequestHandler(WSGIRequestHandler):
@@ -385,7 +385,10 @@
         else:
             print(u'MyJD-API (v.' + get_version() + ') is available and connected with: ' + _device.name)
         app_container(port, configfile, _device)
     else:
         print(u'Could not connect to My JDownloader! Exiting...')
         time.sleep(10)
         sys.exit(1)
+
+if __name__ == "__main__":
+    main()
```

### Comparing `myjd_api-1.1.1/myjd_api.egg-info/PKG-INFO` & `myjd_api-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: myjd-api
-Version: 1.1.1
+Name: myjd_api
+Version: 1.2.0
 Summary: A simple json interface for the MyJDownloader API to be used with Organizr
 Home-page: https://github.com/rix1337/MyJD-API
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -26,20 +26,38 @@
 
 `pip install myjd-api`
 
 # Run
 
 `myjd_api`
 
-# Parameters
+## Parameters
 * `--jd-user` Set your My JDownloader username 
 * `--jd-pass` Set your My JDownloader password 
 * `--jd-device` Set your My JDownloader device name 
 * `--port` _Optional:_ Set desired Port to serve the API 
 * `--username` _Optional:_ Set desired username for the API 
 * `--password` _Optional:_ Set desired username for the API 
 
+# Docker
+```
+docker run -d \
+  --name="MyJD-API" \
+  -p port:8080 \
+  -v /path/to/config/:/config:rw \
+  -e USER=USERNAME \ 
+  -e PASS=PASSWORD \
+  -e DEVICE=DEVICENAME \
+  rix1337/docker-myjd-api
+  ```
+  
+## Optional Parameters
+ - `-e USER` (after first run, if unchanged)
+ - `-e PASS` (after first run, if unchanged)
+ - `-e DEVICE` (always, if only one device is present at MyJD-Account, otherwise after first run, if unchanged)
+
+
 ## Credits
 
 * [mmarquezs](https://github.com/mmarquezs/)
```

### Comparing `myjd_api-1.1.1/setup.py` & `myjd_api-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # MyJD
 # Project by https://github.com/rix1337
 
 import setuptools
 
-from myjd_api.version import get_version
+from myjd_api.providers.version import get_version
 
 try:
     with open('README.md', encoding='utf-8') as f:
         long_description = f.read()
 except:
     import io
 
@@ -33,11 +33,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'myjd_api = myjd_api.web:main',
+            'myjd_api = myjd_api.run:main',
         ],
     },
 )
```

