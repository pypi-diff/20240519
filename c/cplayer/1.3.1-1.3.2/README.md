# Comparing `tmp/cplayer-1.3.1.tar.gz` & `tmp/cplayer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cplayer-1.3.1.tar", max compression
+gzip compressed data, was "cplayer-1.3.2.tar", max compression
```

## Comparing `cplayer-1.3.1.tar` & `cplayer-1.3.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1063 2024-04-26 02:03:51.400567 cplayer-1.3.1/LICENSE
--rw-r--r--   0        0        0    10461 2024-04-27 14:23:16.363419 cplayer-1.3.1/README.md
--rw-r--r--   0        0        0       85 2024-04-26 02:03:51.350567 cplayer-1.3.1/cplayer/__init__.py
--rw-r--r--   0        0        0     4703 2024-04-27 03:08:32.620792 cplayer-1.3.1/cplayer/__main__.py
--rw-r--r--   0        0        0     2015 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/documentation/help.md
--rw-r--r--   0        0        0     1592 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/resources/config/default.yaml
--rw-r--r--   0        0        0      696 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/resources/styles/application.css
--rw-r--r--   0        0        0       19 2024-04-27 03:09:30.104127 cplayer-1.3.1/cplayer/src/__init__.py
--rw-r--r--   0        0        0       26 2024-04-27 03:05:32.414118 cplayer-1.3.1/cplayer/src/components/__init__.py
--rw-r--r--   0        0        0     2776 2024-04-27 14:19:49.060078 cplayer-1.3.1/cplayer/src/components/file_explorer/__init__.py
--rw-r--r--   0        0        0      142 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/file_explorer/styles.css
--rw-r--r--   0        0        0     1293 2024-04-27 03:06:33.267454 cplayer-1.3.1/cplayer/src/components/hidden_widget/__init__.py
--rw-r--r--   0        0        0     2797 2024-04-27 03:04:15.317449 cplayer-1.3.1/cplayer/src/components/input_label/__init__.py
--rw-r--r--   0        0        0       87 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/input_label/styles.css
--rw-r--r--   0        0        0     1911 2024-04-27 03:04:30.137449 cplayer-1.3.1/cplayer/src/components/notification/__init__.py
--rw-r--r--   0        0        0       54 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/notification/styles.css
--rw-r--r--   0        0        0     5633 2024-04-27 03:07:42.567456 cplayer-1.3.1/cplayer/src/components/options_list/__init__.py
--rw-r--r--   0        0        0      145 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/options_list/styles.css
--rw-r--r--   0        0        0     2551 2024-04-27 03:08:03.607457 cplayer-1.3.1/cplayer/src/components/progress_bar/__init__.py
--rw-r--r--   0        0        0      146 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/progress_bar/styles.css
--rw-r--r--   0        0        0     1626 2024-04-27 03:03:16.404114 cplayer-1.3.1/cplayer/src/components/status_song/__init__.py
--rw-r--r--   0        0        0       50 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/status_song/styles.css
--rw-r--r--   0        0        0    12933 2024-04-26 02:15:38.463925 cplayer-1.3.1/cplayer/src/components/tracklist/__init__.py
--rw-r--r--   0        0        0      235 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/tracklist/styles.css
--rw-r--r--   0        0        0     2309 2024-04-27 03:08:45.910792 cplayer-1.3.1/cplayer/src/components/volume_bar/__init__.py
--rw-r--r--   0        0        0      143 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/components/volume_bar/styles.css
--rw-r--r--   0        0        0      253 2024-04-27 03:05:47.750786 cplayer-1.3.1/cplayer/src/elements/__init__.py
--rw-r--r--   0        0        0     4209 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/elements/config.py
--rw-r--r--   0        0        0     2221 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/elements/downloader.py
--rw-r--r--   0        0        0     1674 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/elements/playlist.py
--rw-r--r--   0        0        0       21 2024-04-27 03:05:00.737450 cplayer-1.3.1/cplayer/src/pages/__init__.py
--rw-r--r--   0        0        0      916 2024-04-27 03:02:32.087445 cplayer-1.3.1/cplayer/src/pages/base/__init__.py
--rw-r--r--   0        0        0       44 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/pages/base/styles.css
--rw-r--r--   0        0        0     1133 2024-04-27 03:02:12.167445 cplayer-1.3.1/cplayer/src/pages/help/__init__.py
--rw-r--r--   0        0        0      128 2024-04-26 02:03:51.347234 cplayer-1.3.1/cplayer/src/pages/help/styles.css
--rw-r--r--   0        0        0    25311 2024-04-26 02:07:08.857241 cplayer-1.3.1/cplayer/src/pages/home/__init__.py
--rw-r--r--   0        0        0       62 2024-04-26 02:03:51.350567 cplayer-1.3.1/cplayer/src/pages/home/styles.css
--rw-r--r--   0        0        0     1724 2024-04-27 02:49:25.994084 cplayer-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    11751 1970-01-01 00:00:00.000000 cplayer-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-26 02:03:51.400567 cplayer-1.3.2/LICENSE
+-rw-r--r--   0        0        0     8737 2024-05-17 02:36:23.510706 cplayer-1.3.2/README.md
+-rw-r--r--   0        0        0       85 2024-05-18 23:10:01.847745 cplayer-1.3.2/cplayer/__init__.py
+-rw-r--r--   0        0        0     4703 2024-05-17 02:32:09.980697 cplayer-1.3.2/cplayer/__main__.py
+-rw-r--r--   0        0        0     2015 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/documentation/help.md
+-rw-r--r--   0        0        0     1592 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/resources/config/default.yaml
+-rw-r--r--   0        0        0      696 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/resources/styles/application.css
+-rw-r--r--   0        0        0       19 2024-04-27 03:09:30.104127 cplayer-1.3.2/cplayer/src/__init__.py
+-rw-r--r--   0        0        0       26 2024-04-27 03:05:32.414118 cplayer-1.3.2/cplayer/src/components/__init__.py
+-rw-r--r--   0        0        0     2776 2024-04-27 14:19:49.060078 cplayer-1.3.2/cplayer/src/components/file_explorer/__init__.py
+-rw-r--r--   0        0        0      142 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/file_explorer/styles.css
+-rw-r--r--   0        0        0     1293 2024-04-27 03:06:33.267454 cplayer-1.3.2/cplayer/src/components/hidden_widget/__init__.py
+-rw-r--r--   0        0        0     2797 2024-04-27 03:04:15.317449 cplayer-1.3.2/cplayer/src/components/input_label/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/input_label/styles.css
+-rw-r--r--   0        0        0     1911 2024-04-27 03:04:30.137449 cplayer-1.3.2/cplayer/src/components/notification/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/notification/styles.css
+-rw-r--r--   0        0        0     5633 2024-04-27 03:07:42.567456 cplayer-1.3.2/cplayer/src/components/options_list/__init__.py
+-rw-r--r--   0        0        0      145 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/options_list/styles.css
+-rw-r--r--   0        0        0     2551 2024-04-27 03:08:03.607457 cplayer-1.3.2/cplayer/src/components/progress_bar/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/progress_bar/styles.css
+-rw-r--r--   0        0        0     1626 2024-04-27 03:03:16.404114 cplayer-1.3.2/cplayer/src/components/status_song/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/status_song/styles.css
+-rw-r--r--   0        0        0    12933 2024-04-26 02:15:38.463925 cplayer-1.3.2/cplayer/src/components/tracklist/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/tracklist/styles.css
+-rw-r--r--   0        0        0     2309 2024-04-27 03:08:45.910792 cplayer-1.3.2/cplayer/src/components/volume_bar/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/components/volume_bar/styles.css
+-rw-r--r--   0        0        0      253 2024-04-27 03:05:47.750786 cplayer-1.3.2/cplayer/src/elements/__init__.py
+-rw-r--r--   0        0        0     4209 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/elements/config.py
+-rw-r--r--   0        0        0     2221 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/elements/downloader.py
+-rw-r--r--   0        0        0     1674 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/elements/playlist.py
+-rw-r--r--   0        0        0       21 2024-04-27 03:05:00.737450 cplayer-1.3.2/cplayer/src/pages/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-27 03:02:32.087445 cplayer-1.3.2/cplayer/src/pages/base/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/pages/base/styles.css
+-rw-r--r--   0        0        0     1133 2024-04-27 03:02:12.167445 cplayer-1.3.2/cplayer/src/pages/help/__init__.py
+-rw-r--r--   0        0        0      128 2024-04-26 02:03:51.347234 cplayer-1.3.2/cplayer/src/pages/help/styles.css
+-rw-r--r--   0        0        0    25513 2024-05-18 23:19:14.777764 cplayer-1.3.2/cplayer/src/pages/home/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-26 02:03:51.350567 cplayer-1.3.2/cplayer/src/pages/home/styles.css
+-rw-r--r--   0        0        0     1702 2024-05-18 23:08:39.791075 cplayer-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10027 1970-01-01 00:00:00.000000 cplayer-1.3.2/PKG-INFO
```

### Comparing `cplayer-1.3.1/LICENSE` & `cplayer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/README.md` & `cplayer-1.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1
+Name: cplayer
+Version: 1.3.2
+Summary: Minimalist song player implemented with Python
+Home-page: https://github.com/eccanto/cplayer
+License: MIT
+Keywords: music,songs player,command line
+Author: Erik Ccanto
+Author-email: ccanto.erik@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: dotmap (>=1.3.30,<2.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pip (>=24.0,<25.0)
+Requires-Dist: pydub (>=0.25.1,<0.26.0)
+Requires-Dist: pygame (>=2.5.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: textual (>=0.58.0,<0.59.0)
+Requires-Dist: tox (>=4.14.1,<5.0.0)
+Requires-Dist: yt-dlp (>=2024.3.10,<2025.0.0)
+Project-URL: Repository, https://github.com/eccanto/cplayer
+Description-Content-Type: text/markdown
+
 # CPlayer
 
 ![](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![](https://img.shields.io/pypi/v/cplayer)
 ![](https://img.shields.io/badge/license-MIT-green)
 ![](https://img.shields.io/github/stars/eccanto)
 
@@ -259,59 +293,17 @@
   * [dodgy](https://github.com/landscapeio/dodgy): It is a series of simple regular expressions designed to detect
     things such as accidental SCM diff checkins, or passwords or secret keys hard coded into files.
   * [mypy](https://github.com/python/mypy): Mypy is an optional static type checker for Python.
   * [pyroma](https://github.com/regebro/pyroma): Pyroma is a product aimed at giving a rating of how well a Python
     project complies with the best practices of the Python packaging ecosystem, primarily PyPI, pip, Distribute etc,
     as well as a list of issues that could be improved.
 
-* [detect-secrets](https://github.com/Yelp/detect-secrets): Detect secrets in your code.
-
 ### Run manually
 
 ```bash
-poetry run tox -e check_code
+bash .githooks/pre-commit
 ```
 
 ## License
 
 [MIT](./LICENSE)
 
-## Changelog
-
-* 1.0.0 - Initial version.
-* 1.0.1:
-    * `refactor`: Updates documentation.
-    * `fix`: Default playlist loading.
-    * `feat`: Adds `--version` command line argument.
-* 1.0.2:
-    * `feat`: Download song from a YouTube URL (`--url`).
-* 1.1.0:
-    * `fix`: Updates the application when a song is broken.
-    * `feat`: Adds log details when downloading a song.
-* 1.1.1:
-    * `fix`: Stores absolute paths of the songs in the playlist file.
-    * `refactor`: Changes keyboard shortcuts (`vim` style).
-* 1.1.2:
-    * `fix`: Handle error when song files are not found.
-    * `documentation`: Adds development documentation.
-    * `refactor`: Enables log file.
-* 1.1.3:
-    * `refactor`: Updates requirements compatibility.
-* 1.1.4:
-    * `refactor`: Updates application compatibility.
-* 1.1.5:
-    * `fix`: Apply background and primary color from local configuration file.
-* 1.2.0:
-    * `feat`: Adds displacement to the last position with `:$`.
-    * `feat`: Adds synchronization feature to take a directory path and synchronize its files with the current playlist,
-      if the directory contains previously deleted songs they are not re-added.
-* 1.2.1:
-    * `feat`: Adds compatibility to python 3.10 and 3.12.
-    * `fix`: Fixes an error in the size of the layouts.
-    * `refactor`: Adds poetry as a dependency and packaging manager.
-    * `refactor`: General refactoring on static code analysis tools.
-* 1.3.0:
-    * `feat`: Adds support for wav song files.
-    * `documentation`: Refactor developers documentation.
-* 1.3.1:
-    * `fix`: Adds file explorer quit action.
-    * `refactor`: Update textual package.
```

### Comparing `cplayer-1.3.1/cplayer/__main__.py` & `cplayer-1.3.2/cplayer/__main__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/documentation/help.md` & `cplayer-1.3.2/cplayer/documentation/help.md`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/resources/config/default.yaml` & `cplayer-1.3.2/cplayer/resources/config/default.yaml`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/resources/styles/application.css` & `cplayer-1.3.2/cplayer/resources/styles/application.css`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/file_explorer/__init__.py` & `cplayer-1.3.2/cplayer/src/components/file_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/hidden_widget/__init__.py` & `cplayer-1.3.2/cplayer/src/components/hidden_widget/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/input_label/__init__.py` & `cplayer-1.3.2/cplayer/src/components/input_label/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/notification/__init__.py` & `cplayer-1.3.2/cplayer/src/components/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/options_list/__init__.py` & `cplayer-1.3.2/cplayer/src/components/options_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/progress_bar/__init__.py` & `cplayer-1.3.2/cplayer/src/components/progress_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/status_song/__init__.py` & `cplayer-1.3.2/cplayer/src/components/status_song/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/tracklist/__init__.py` & `cplayer-1.3.2/cplayer/src/components/tracklist/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/components/volume_bar/__init__.py` & `cplayer-1.3.2/cplayer/src/components/volume_bar/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/elements/config.py` & `cplayer-1.3.2/cplayer/src/elements/config.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/elements/downloader.py` & `cplayer-1.3.2/cplayer/src/elements/downloader.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/elements/playlist.py` & `cplayer-1.3.2/cplayer/src/elements/playlist.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/pages/base/__init__.py` & `cplayer-1.3.2/cplayer/src/pages/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/pages/help/__init__.py` & `cplayer-1.3.2/cplayer/src/pages/help/__init__.py`

 * *Files identical despite different names*

### Comparing `cplayer-1.3.1/cplayer/src/pages/home/__init__.py` & `cplayer-1.3.2/cplayer/src/pages/home/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         self.playlists_directory = Path(CONFIG.data.general.playlist.directory).expanduser()
         self.playlists_directory.mkdir(parents=True, exist_ok=True)
 
         self._start_position = 0
         self._playing = False
         self._volume = 0.75
 
+        self._song: mixer.Sound | None = None
+
         self.status_song_widget = StatusSong(self._volume, start_hidden=False)
         self.tracklist_widget = TracklistWidget(
             self.play_song,
             self.action_cursor_left,
             self.action_cursor_right,
             on_change_position=self.on_change_position,
             order=next(
@@ -177,16 +179,18 @@
         """Move the playback position `seconds` backward."""
         if mixer.music.get_busy():
             self._start_position = max(int(self._start_position + mixer.music.get_pos() / 1000.0 - seconds), 0)
             mixer.music.play(0, self._start_position)
 
     def action_cursor_right(self, seconds: int = 5) -> None:
         """Move the playback position `seconds` forward."""
-        if mixer.music.get_busy():
-            self._start_position += int(mixer.music.get_pos() / 1000.0) + seconds
+        if mixer.music.get_busy() and self._song:
+            self._start_position = min(
+                int(self._start_position + mixer.music.get_pos() / 1000.0 + seconds), int(self._song.get_length())
+            )
             mixer.music.play(0, self._start_position)
 
     def action_filter(self) -> None:
         """Opens a input text to filter songs in the current playlist."""
         self.status_song_widget.hide()
 
         self.filter_widget.show()
@@ -223,14 +227,16 @@
         """Plays the selected song.
 
         :param song: The song to be played.
         """
         if song.seconds:
             try:
                 self._start_position = 0
+                self._song = mixer.Sound(song.path)
+
                 mixer.music.load(song.path)
                 mixer.music.play()
 
                 self._playing = True
 
                 self.status_song_widget.progress.set_status(ProgressStatusWidget.Status.PLAYING)
                 self.status_song_widget.progress.total_seconds = (
```

### Comparing `cplayer-1.3.1/pyproject.toml` & `cplayer-1.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cplayer"
-version = "1.3.1"
+version = "1.3.2"
 description = "Minimalist song player implemented with Python"
 authors = ["Erik Ccanto <ccanto.erik@gmail.com>"]
 repository = "https://github.com/eccanto/cplayer"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "cplayer" },
@@ -52,15 +52,14 @@
 tox = "^4.14.1"
 pip = "^24.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 twine = "^5.0.0"
 assertpy = "^1.1"
-pre-commit = "^3.6.2"
 prospector = {extras = ["with-mypy", "with-pyroma"], version = "^1.10.3"}
 types-pyyaml = "^6.0.12.20240311"
 ruff = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cplayer-1.3.1/PKG-INFO` & `cplayer-1.3.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,7 @@
-Metadata-Version: 2.1
-Name: cplayer
-Version: 1.3.1
-Summary: Minimalist song player implemented with Python
-Home-page: https://github.com/eccanto/cplayer
-License: MIT
-Keywords: music,songs player,command line
-Author: Erik Ccanto
-Author-email: ccanto.erik@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: dotmap (>=1.3.30,<2.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pip (>=24.0,<25.0)
-Requires-Dist: pydub (>=0.25.1,<0.26.0)
-Requires-Dist: pygame (>=2.5.2,<3.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: textual (>=0.58.0,<0.59.0)
-Requires-Dist: tox (>=4.14.1,<5.0.0)
-Requires-Dist: yt-dlp (>=2024.3.10,<2025.0.0)
-Project-URL: Repository, https://github.com/eccanto/cplayer
-Description-Content-Type: text/markdown
-
 # CPlayer
 
 ![](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![](https://img.shields.io/pypi/v/cplayer)
 ![](https://img.shields.io/badge/license-MIT-green)
 ![](https://img.shields.io/github/stars/eccanto)
 
@@ -293,60 +259,16 @@
   * [dodgy](https://github.com/landscapeio/dodgy): It is a series of simple regular expressions designed to detect
     things such as accidental SCM diff checkins, or passwords or secret keys hard coded into files.
   * [mypy](https://github.com/python/mypy): Mypy is an optional static type checker for Python.
   * [pyroma](https://github.com/regebro/pyroma): Pyroma is a product aimed at giving a rating of how well a Python
     project complies with the best practices of the Python packaging ecosystem, primarily PyPI, pip, Distribute etc,
     as well as a list of issues that could be improved.
 
-* [detect-secrets](https://github.com/Yelp/detect-secrets): Detect secrets in your code.
-
 ### Run manually
 
 ```bash
-poetry run tox -e check_code
+bash .githooks/pre-commit
 ```
 
 ## License
 
 [MIT](./LICENSE)
-
-## Changelog
-
-* 1.0.0 - Initial version.
-* 1.0.1:
-    * `refactor`: Updates documentation.
-    * `fix`: Default playlist loading.
-    * `feat`: Adds `--version` command line argument.
-* 1.0.2:
-    * `feat`: Download song from a YouTube URL (`--url`).
-* 1.1.0:
-    * `fix`: Updates the application when a song is broken.
-    * `feat`: Adds log details when downloading a song.
-* 1.1.1:
-    * `fix`: Stores absolute paths of the songs in the playlist file.
-    * `refactor`: Changes keyboard shortcuts (`vim` style).
-* 1.1.2:
-    * `fix`: Handle error when song files are not found.
-    * `documentation`: Adds development documentation.
-    * `refactor`: Enables log file.
-* 1.1.3:
-    * `refactor`: Updates requirements compatibility.
-* 1.1.4:
-    * `refactor`: Updates application compatibility.
-* 1.1.5:
-    * `fix`: Apply background and primary color from local configuration file.
-* 1.2.0:
-    * `feat`: Adds displacement to the last position with `:$`.
-    * `feat`: Adds synchronization feature to take a directory path and synchronize its files with the current playlist,
-      if the directory contains previously deleted songs they are not re-added.
-* 1.2.1:
-    * `feat`: Adds compatibility to python 3.10 and 3.12.
-    * `fix`: Fixes an error in the size of the layouts.
-    * `refactor`: Adds poetry as a dependency and packaging manager.
-    * `refactor`: General refactoring on static code analysis tools.
-* 1.3.0:
-    * `feat`: Adds support for wav song files.
-    * `documentation`: Refactor developers documentation.
-* 1.3.1:
-    * `fix`: Adds file explorer quit action.
-    * `refactor`: Update textual package.
-
```

