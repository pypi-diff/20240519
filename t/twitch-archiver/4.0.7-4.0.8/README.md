# Comparing `tmp/twitch_archiver-4.0.7.tar.gz` & `tmp/twitch_archiver-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_archiver-4.0.7.tar", last modified: Tue May  7 03:18:42 2024, max compression
+gzip compressed data, was "twitch_archiver-4.0.8.tar", last modified: Sat May 18 22:39:08 2024, max compression
```

## Comparing `twitch_archiver-4.0.7.tar` & `twitch_archiver-4.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/twitch_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 03:18:42.000000 twitch_archiver-4.0.7/twitch_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/twitcharchiver/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 03:18:42.338221 twitch_archiver-4.0.7/twitcharchiver/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/realtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    32460 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/downloaders/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/twitch.py
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23657 2024-05-07 03:18:37.000000 twitch_archiver-4.0.7/twitcharchiver/vod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.383136 twitch_archiver-4.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-18 22:39:08.383136 twitch_archiver-4.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:39:08.383136 twitch_archiver-4.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.379136 twitch_archiver-4.0.8/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 22:39:08.000000 twitch_archiver-4.0.8/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.379136 twitch_archiver-4.0.8/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:39:08.379136 twitch_archiver-4.0.8/twitcharchiver/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32460 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/downloaders/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-05-18 22:38:57.000000 twitch_archiver-4.0.8/twitcharchiver/vod.py
```

### Comparing `twitch_archiver-4.0.7/LICENSE` & `twitch_archiver-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/PKG-INFO` & `twitch_archiver-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 4.0.7
+Version: 4.0.8
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch_archiver-4.0.7/README.md` & `twitch_archiver-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/pyproject.toml` & `twitch_archiver-4.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "twitch-archiver"
-version = "4.0.7"
+version = "4.0.8"
 dependencies = [
     "requests>=2.28.0",
     "m3u8>=0.3.12",
 ]
 authors = [
   { name="Brisppy", email="brisppy@protonmail.com" },
 ]
```

### Comparing `twitch_archiver-4.0.7/twitch_archiver.egg-info/PKG-INFO` & `twitch_archiver-4.0.8/twitch_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-archiver
-Version: 4.0.7
+Version: 4.0.8
 Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
 Author-email: Brisppy <brisppy@protonmail.com>
 Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
 Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `twitch_archiver-4.0.7/twitch_archiver.egg-info/SOURCES.txt` & `twitch_archiver-4.0.8/twitch_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/__init__.py` & `twitch_archiver-4.0.8/twitcharchiver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from twitcharchiver.utils import (
     getenv,
     check_update_available,
     get_latest_version,
     get_temp_dir,
 )
 
-__version__ = "4.0.7"
+__version__ = "4.0.8"
 
 from twitcharchiver.vod import Vod, ArchivedVod
 
 
 def main():
     """
     Main processing for twitch-archiver.
```

### Comparing `twitch_archiver-4.0.7/twitcharchiver/api.py` & `twitch_archiver-4.0.8/twitcharchiver/api.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/arguments.py` & `twitch_archiver-4.0.8/twitcharchiver/arguments.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/channel.py` & `twitch_archiver-4.0.8/twitcharchiver/channel.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/configuration.py` & `twitch_archiver-4.0.8/twitcharchiver/configuration.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/database.py` & `twitch_archiver-4.0.8/twitcharchiver/database.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/downloader.py` & `twitch_archiver-4.0.8/twitcharchiver/downloader.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/downloaders/chat.py` & `twitch_archiver-4.0.8/twitcharchiver/downloaders/chat.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/downloaders/realtime.py` & `twitch_archiver-4.0.8/twitcharchiver/downloaders/realtime.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/downloaders/stream.py` & `twitch_archiver-4.0.8/twitcharchiver/downloaders/stream.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/downloaders/video.py` & `twitch_archiver-4.0.8/twitcharchiver/downloaders/video.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/exceptions.py` & `twitch_archiver-4.0.8/twitcharchiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/logger.py` & `twitch_archiver-4.0.8/twitcharchiver/logger.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/processing.py` & `twitch_archiver-4.0.8/twitcharchiver/processing.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/twitch.py` & `twitch_archiver-4.0.8/twitcharchiver/twitch.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/utils.py` & `twitch_archiver-4.0.8/twitcharchiver/utils.py`

 * *Files identical despite different names*

### Comparing `twitch_archiver-4.0.7/twitcharchiver/vod.py` & `twitch_archiver-4.0.8/twitcharchiver/vod.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,31 +485,19 @@
         Gets a playback access token for the VOD.
 
         :return: dictionary of playback access token values if any
         :rtype: dict
         """
         # only accepts the default client ID for non-authenticated clients
         _h = {"Client-Id": "ue6666qo983tsx6so1t0vnawi233wa"}
-        _q = """
-        {{
-            videoPlaybackAccessToken(
-                id: {vod_id},
-                params: {{
-                    platform: "web",
-                    playerBackend: "mediaplayer",
-                    playerType: "site"
-                }}
-            ) {{
-                signature
-                value
-            }}
-        }}
-        """.format(
-            vod_id=self.v_id
+        _q = (
+            f'{{videoPlaybackAccessToken(id: "{self.v_id}", params: {{platform: "web", playerBackend: "mediaplayer", '
+            f'playerType: "site"}}) {{signature value}} }}'
         )
+
         _r = self._api.post_request("https://gql.twitch.tv/gql", j={"query": _q}, h=_h)
 
         _token = _r.json()["data"]["videoPlaybackAccessToken"]
 
         if _token:
             self._log.debug("Token retrieved for VOD %s: %s", self.v_id, _token)
             return _token
```

