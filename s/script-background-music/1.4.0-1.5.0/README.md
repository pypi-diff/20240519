# Comparing `tmp/script-background-music-1.4.0.tar.gz` & `tmp/script-background-music-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "script-background-music-1.4.0.tar", last modified: Thu Aug 11 16:50:16 2022, max compression
+gzip compressed data, was "script-background-music-1.5.0.tar", last modified: Sun May 19 16:40:10 2024, max compression
```

## Comparing `script-background-music-1.4.0.tar` & `script-background-music-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:16.744289 script-background-music-1.4.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1068 2022-08-11 16:50:06.000000 script-background-music-1.4.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       44 2022-08-11 16:50:06.000000 script-background-music-1.4.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2367 2022-08-11 16:50:16.744289 script-background-music-1.4.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1941 2022-08-11 16:50:06.000000 script-background-music-1.4.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:16.736289 script-background-music-1.4.0/script_background_music/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      197 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      893 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1579 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/play.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:16.744289 script-background-music-1.4.0/script_background_music/songs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      305 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/songs/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)  4543531 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/songs/local-forecast.mp3
--rw-r--r--   0 circleci  (3434) circleci  (3434)   959678 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/songs/lofi.mp3
--rw-r--r--   0 circleci  (3434) circleci  (3434)   914864 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/songs/overcast.mp3
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:16.744289 script-background-music-1.4.0/script_background_music/vendor/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/vendor/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:16.744289 script-background-music-1.4.0/script_background_music/vendor/playsound/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6459 2022-08-11 16:50:06.000000 script-background-music-1.4.0/script_background_music/vendor/playsound/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-08-11 16:50:16.740289 script-background-music-1.4.0/script_background_music.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2367 2022-08-11 16:50:15.000000 script-background-music-1.4.0/script_background_music.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      598 2022-08-11 16:50:16.000000 script-background-music-1.4.0/script_background_music.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-08-11 16:50:16.000000 script-background-music-1.4.0/script_background_music.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-08-11 16:50:16.000000 script-background-music-1.4.0/script_background_music.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-08-11 16:50:16.744289 script-background-music-1.4.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2022-08-11 16:50:06.000000 script-background-music-1.4.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-19 16:40:10.134491 script-background-music-1.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1068 2024-05-19 16:39:59.000000 script-background-music-1.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2024-05-19 16:39:59.000000 script-background-music-1.5.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7133 2024-05-19 16:40:10.134491 script-background-music-1.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6707 2024-05-19 16:39:59.000000 script-background-music-1.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-19 16:40:10.126491 script-background-music-1.5.0/script_background_music/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      958 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1751 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/play.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-19 16:40:10.130491 script-background-music-1.5.0/script_background_music/songs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      383 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/songs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  4543531 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/songs/local-forecast.mp3
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   959678 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/songs/lofi.mp3
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   914864 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/songs/overcast.mp3
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-19 16:40:10.130491 script-background-music-1.5.0/script_background_music/vendor/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       56 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/vendor/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-19 16:40:10.130491 script-background-music-1.5.0/script_background_music/vendor/playsound/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6459 2024-05-19 16:39:59.000000 script-background-music-1.5.0/script_background_music/vendor/playsound/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-19 16:40:10.134491 script-background-music-1.5.0/script_background_music.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7133 2024-05-19 16:40:10.000000 script-background-music-1.5.0/script_background_music.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-19 16:40:10.000000 script-background-music-1.5.0/script_background_music.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-19 16:40:10.000000 script-background-music-1.5.0/script_background_music.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2024-05-19 16:40:10.000000 script-background-music-1.5.0/script_background_music.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-19 16:40:10.134491 script-background-music-1.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      830 2024-05-19 16:39:59.000000 script-background-music-1.5.0/setup.py
```

### Comparing `script-background-music-1.4.0/LICENSE` & `script-background-music-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `script-background-music-1.4.0/script_background_music/context.py` & `script-background-music-1.5.0/script_background_music/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from typing import Callable
+"""
+Use the elevator music as a context
+"""
+from typing import Callable, Union
 
 from script_background_music.play import play_random_music_in_background, PlayThread
 
 
 class BackgroundMusicContext(object):
     """
     Run background music in a given context
 
     <b>WARNING: Not verified to work on macOS! Should work there as well, since also creates a subprocess under the hood.</b>
     """
-    __thread: PlayThread = None
+    __thread: Union[PlayThread, None] = None
 
     def __init__(self, player_callback: Callable[[], PlayThread] = play_random_music_in_background):
         """
         Create new background music context
+
         :param player_callback: Callback to run the music, defaults to<i>script_background_music.play.play_random_music_in_background</i>
         """
         self.__thread = player_callback()
 
     def __enter__(self):
         return self
```

### Comparing `script-background-music-1.4.0/script_background_music/play.py` & `script-background-music-1.5.0/script_background_music/play.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+"""
+Infrastructure to facilitate playing songs
+"""
 import logging
 from multiprocessing import Process
 from typing import Union
 import psutil
 from script_background_music.songs import get_random_song
 from script_background_music.vendor.playsound import get_play_sound
 
 
 class PlayThread(Process):
+    """
+    Thread to be used for playing songs
+    """
     def kill_children(self):
+        """
+        Ensures all player child threads are terminated properly
+        """
         process = psutil.Process(self.pid)
         for child in process.children(recursive=True):
             child.kill()
 
 
 def __music(song_title):
     try:
@@ -20,32 +29,34 @@
     except:
         logging.debug("Could not start music, exiting.")
 
 
 def play_music_in_background(song_file: Union[str, None] = None) -> PlayThread:
     """
     Play music in background if no song is provided, a random will be picked
+
     :param song_file: Song to play, set to None or omit to use a random one
     :return: Underlying thread for playing music
     """
     song_to_play = get_random_song() if song_file is None else song_file
     thread = PlayThread(target=__music, args=(song_to_play,))
-    # thread.daemon = True
     thread.start()
     return thread
 
 
 def play_random_music_in_background() -> PlayThread:
     """
     Play random music from the available songs in the background
+
     :return: Underlying thread for playing music
     """
     return play_music_in_background(None)
 
 
 def play_song_in_background(file_name: str) -> PlayThread:
     """
     Play song from given file in background
+
     :param file_name: Filename of song to play in background
     :return: Underlying thread for playing music
     """
     return play_music_in_background(file_name)
```

### Comparing `script-background-music-1.4.0/script_background_music/songs/local-forecast.mp3` & `script-background-music-1.5.0/script_background_music/songs/local-forecast.mp3`

 * *Files identical despite different names*

### Comparing `script-background-music-1.4.0/script_background_music/songs/lofi.mp3` & `script-background-music-1.5.0/script_background_music/songs/lofi.mp3`

 * *Files identical despite different names*

### Comparing `script-background-music-1.4.0/script_background_music/songs/overcast.mp3` & `script-background-music-1.5.0/script_background_music/songs/overcast.mp3`

 * *Files identical despite different names*

### Comparing `script-background-music-1.4.0/script_background_music/vendor/playsound/__init__.py` & `script-background-music-1.5.0/script_background_music/vendor/playsound/__init__.py`

 * *Files identical despite different names*

### Comparing `script-background-music-1.4.0/script_background_music.egg-info/SOURCES.txt` & `script-background-music-1.5.0/script_background_music.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `script-background-music-1.4.0/setup.py` & `script-background-music-1.5.0/setup.py`

 * *Files identical despite different names*

