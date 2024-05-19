# Comparing `tmp/youtubedlez-1.0.0.tar.gz` & `tmp/youtubedlez-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtubedlez-1.0.0.tar", max compression
+gzip compressed data, was "youtubedlez-1.0.1.tar", max compression
```

## Comparing `youtubedlez-1.0.0.tar` & `youtubedlez-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    13827 2024-05-19 17:58:32.518191 youtubedlez-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0      376 2024-05-19 17:55:55.010179 youtubedlez-1.0.0/README.md
--rw-r--r--   0        0        0     4437 2024-05-19 17:59:44.209197 youtubedlez-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2697 2024-05-19 17:47:09.686137 youtubedlez-1.0.0/youtubedlez/__main__.py
--rw-r--r--   0        0        0       48 2024-05-19 17:47:09.686137 youtubedlez-1.0.0/youtubedlez/sample_input.txt
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 youtubedlez-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    13827 2024-05-19 17:58:32.518191 youtubedlez-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      376 2024-05-19 17:55:55.010179 youtubedlez-1.0.1/README.md
+-rw-r--r--   0        0        0     4437 2024-05-19 18:01:05.970204 youtubedlez-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2685 2024-05-19 18:00:51.239203 youtubedlez-1.0.1/youtubedlez/__main__.py
+-rw-r--r--   0        0        0       48 2024-05-19 17:47:09.686137 youtubedlez-1.0.1/youtubedlez/sample_input.txt
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 youtubedlez-1.0.1/PKG-INFO
```

### Comparing `youtubedlez-1.0.0/LICENSE.txt` & `youtubedlez-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youtubedlez-1.0.0/pyproject.toml` & `youtubedlez-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # See https://python-poetry.org/docs/pyproject/ for more details!
 
 # The name of your project.
 # Ensure that it is available on PyPI: https://pypi.org/
 name = "youtubedlez"
 
 # The version of the package.
-version = "1.0.0"
+version = "1.0.1"
 
 # A brief, one-sentence description about your project.
 description = "Super simple terminal interface for yt-dlp"
 
 # A list of the authors of the project.
 authors = [
     "Stefano Pigozzi <me@steffo.eu>",
```

### Comparing `youtubedlez-1.0.0/youtubedlez/__main__.py` & `youtubedlez-1.0.1/youtubedlez/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 video_formats = ['mp4', 'flv', 'webm', 'ogg', 'mkv', 'avi']
 audio_formats = ['best', 'aac', 'flac', 'mp3', 'm4a', 'opus', 'vorbis', 'wav']
 
 def main():
     print(f"Easy Youtube Downloader")
     print("(c) Stefano Pigozzi")
-    print("Licensed under the GNU-GPL-3.0-or-later")
+    print("Licensed under the EUPL-1.2")
     print("-" * 80)
     print()
 
     dl_location = pathlib.Path.home().joinpath("Downloads")
     os.makedirs(name=dl_location, exist_ok=True)
     print(f"Downloads will be saved in: {dl_location}")
     print("-" * 80)
```

### Comparing `youtubedlez-1.0.0/PKG-INFO` & `youtubedlez-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtubedlez
-Version: 1.0.0
+Version: 1.0.1
 Summary: Super simple terminal interface for yt-dlp
 Home-page: https://github.com/steffo99/youtubedlez
 License: EUPL-1.2
 Keywords: youtube,downloader,ytdlp,tui,easy
 Author: Stefano Pigozzi
 Author-email: me@steffo.eu
 Maintainer: Stefano Pigozzi
```

