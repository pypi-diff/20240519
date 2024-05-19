# Comparing `tmp/ytmusic_deleter-2.3.2.tar.gz` & `tmp/ytmusic_deleter-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytmusic_deleter-2.3.2.tar", last modified: Sun May 12 01:14:49 2024, max compression
+gzip compressed data, was "ytmusic_deleter-2.3.3.tar", last modified: Sun May 19 03:21:03 2024, max compression
```

## Comparing `ytmusic_deleter-2.3.2.tar` & `ytmusic_deleter-2.3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2024-05-12 01:14:31.813149 ytmusic_deleter-2.3.2/LICENSE
--rw-r--r--   0        0        0     1447 2024-05-12 01:14:49.901264 ytmusic_deleter-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     6578 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/tests/conftest.py
--rw-r--r--   0        0        0     1304 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/tests/resources/test.example.cfg
--rw-r--r--   0        0        0     4090 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/tests/test_cli.py
--rw-r--r--   0        0        0     5475 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/ytmusic_deleter/README.md
--rw-r--r--   0        0        0       22 2024-05-12 01:14:49.901264 ytmusic_deleter-2.3.2/ytmusic_deleter/_version.py
--rw-r--r--   0        0        0     1142 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/ytmusic_deleter/auth.py
--rw-r--r--   0        0        0    20465 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/ytmusic_deleter/cli.py
--rw-r--r--   0        0        0      168 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/ytmusic_deleter/constants.py
--rw-r--r--   0        0        0      319 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/ytmusic_deleter/progress.py
--rw-r--r--   0        0        0     9521 2024-05-12 01:14:31.817149 ytmusic_deleter-2.3.2/ytmusic_deleter/uploads.py
--rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-19 03:20:48.206808 ytmusic_deleter-2.3.3/LICENSE
+-rw-r--r--   0        0        0     1447 2024-05-19 03:21:03.438807 ytmusic_deleter-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     7641 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      691 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/tests/resources/test.example.cfg
+-rw-r--r--   0        0        0     7277 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/tests/test_cli.py
+-rw-r--r--   0        0        0     5475 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/ytmusic_deleter/README.md
+-rw-r--r--   0        0        0       22 2024-05-19 03:21:03.438807 ytmusic_deleter-2.3.3/ytmusic_deleter/_version.py
+-rw-r--r--   0        0        0     1142 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/ytmusic_deleter/auth.py
+-rw-r--r--   0        0        0    21097 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/ytmusic_deleter/cli.py
+-rw-r--r--   0        0        0      168 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/ytmusic_deleter/constants.py
+-rw-r--r--   0        0        0      319 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/ytmusic_deleter/progress.py
+-rw-r--r--   0        0        0     9512 2024-05-19 03:20:48.210808 ytmusic_deleter-2.3.3/ytmusic_deleter/uploads.py
+-rw-r--r--   0        0        0     5846 1970-01-01 00:00:00.000000 ytmusic_deleter-2.3.3/PKG-INFO
```

### Comparing `ytmusic_deleter-2.3.2/LICENSE` & `ytmusic_deleter-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.2/pyproject.toml` & `ytmusic_deleter-2.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "click>=8.1.7",
     "enlighten>=1.12.4",
     "thefuzz>=0.22.1",
     "ytmusicapi>=1.7.0",
 ]
 requires-python = "<3.13,>=3.8.1"
 readme = "ytmusic_deleter/README.md"
-version = "2.3.2"
+version = "2.3.3"
 
 [project.license]
 text = "GPL-3.0"
 
 [project.scripts]
 ytmusic-deleter = "ytmusic_deleter.cli:cli"
```

### Comparing `ytmusic_deleter-2.3.2/tests/conftest.py` & `ytmusic_deleter-2.3.3/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import configparser
 import time
 from pathlib import Path
 from typing import Dict
+from typing import List
 
 import pytest
 from ytmusic_deleter import constants
 from ytmusicapi import YTMusic
 
 
 def get_resource(file: str) -> str:
@@ -38,14 +39,19 @@
 
 @pytest.fixture(name="sample_video")
 def fixture_sample_video() -> str:
     """Oasis - Wonderwall"""
     return "hpSrLjc5SMs"
 
 
+@pytest.fixture(name="sample_song_list")
+def fixture_sample_song_list() -> List[str]:
+    return ["hpSrLjc5SMs", "PIuAFrLeXfY", "9gi4WwQcPW8", "beX-9wW5rL0", "8ay_BkRuv-o", "HGorCGszxZU", "t2rsf8SiMJY"]
+
+
 @pytest.fixture(name="sample_public_playlist")
 def fixture_sample_playlist() -> str:
     """'00s Metal"""
     return "RDCLAK5uy_kx0d2-VPr69KAkIQOTVFq04hCBsJE9LaI"
 
 
 @pytest.fixture(name="sample_podcast")
@@ -90,45 +96,47 @@
     return YTMusic(config["auth"]["headers_empty"], config["auth"]["brand_account_empty"])
 
 
 @pytest.fixture(name="upload_song")
 def fixture_upload_song(config, yt_browser: YTMusic) -> Dict | None:
     """
     Upload a song and wait for it to finish processing.
-    Return the song object or None if it did not upload successfully.
     """
     upload_response = yt_browser.upload_song(get_resource(config["uploads"]["file"]))
     if not isinstance(upload_response, str) and upload_response.status_code == 409:
         # Song is already in uploads. Delete it and re-upload.
         # Although this app is not responsible for verifying that upload works properly,
         # we still want to verify that no errors happen if we try to delete a song right
         # after it was uploaded, since this was an issue previously https://github.com/sigma67/ytmusicapi/issues/578.
         songs = yt_browser.get_library_upload_songs()
-        delete_response = None
-        for song in songs:
-            if song.get("title") in config["uploads"]["file"]:
-                delete_response = yt_browser.delete_upload_entity(song["entityId"])
-        assert delete_response == "STATUS_SUCCEEDED"
+        if songs:
+            delete_response = None
+            for song in songs:
+                if song.get("title") in config["uploads"]["file"]:
+                    delete_response = yt_browser.delete_upload_entity(song["entityId"])
+            assert delete_response == "STATUS_SUCCEEDED"
         # Need to wait for song to be fully deleted
         time.sleep(10)
         # Now re-upload
         upload_response = yt_browser.upload_song(get_resource(config["uploads"]["file"]))
 
     assert upload_response == "STATUS_SUCCEEDED" or upload_response.status_code == 200
 
     # Wait for upload to finish processing
     retries_remaining = 20
     while retries_remaining:
-        time.sleep(2)
+        time.sleep(3)
         songs = yt_browser.get_library_upload_songs(limit=None)
         for song in songs:
             if song.get("title") in config["uploads"]["file"]:
                 return song
         retries_remaining -= 1
 
+    raise AssertionError("Failed to verify uploaded song exists in library.")
+
 
 @pytest.fixture(name="add_library_album")
 def fixture_add_library_album(yt_oauth: YTMusic, sample_album_as_playlist):
     response = yt_oauth.rate_playlist(sample_album_as_playlist, constants.LIKE)
     assert "actions" in response
 
     # Wait for album to finish processing
@@ -137,30 +145,34 @@
         albums = yt_oauth.get_library_albums(limit=None)
         for album in albums:
             if album.get("title") == "Revival":
                 return album
         retries_remaining -= 1
         time.sleep(2)
 
+    raise AssertionError("Failed to confirm that album was added to library")
+
 
 @pytest.fixture(name="add_podcast")
-def fixtrue_add_podcast(yt_oauth: YTMusic, sample_podcast):
+def fixture_add_podcast(yt_oauth: YTMusic, sample_podcast):
     response = yt_oauth.rate_playlist(sample_podcast, constants.LIKE)
     assert "actions" in response
 
     # Wait for podcast to be in library
     retries_remaining = 5
     while retries_remaining:
         podcasts = yt_oauth.get_library_podcasts(limit=None)
         for podcast in podcasts:
             if podcast.get("title") == "JRE Archive - Episodes #701 - 1000":
                 return podcast
         retries_remaining -= 1
         time.sleep(2)
 
+    raise AssertionError("Failed to confirm that podcast was added to library")
+
 
 @pytest.fixture(name="like_song")
 def fixture_like_song(yt_oauth: YTMusic, sample_video):
     response = yt_oauth.rate_song(sample_video, constants.LIKE)
     assert "actions" in response
 
     # Wait for song to finish processing
@@ -177,24 +189,42 @@
         time.sleep(2)
 
     # Remove song from library to clean up
     yt_oauth.rate_playlist("OLAK5uy_lZ90LvUqQdKrByCbk99v54d8XpUOmFavo", constants.INDIFFERENT)
 
 
 @pytest.fixture(name="create_playlist")
-def fixture_playlist(yt_oauth: YTMusic, sample_public_playlist) -> str:
+def fixture_create_playlist(yt_oauth: YTMusic, sample_public_playlist) -> str:
     playlist_id = yt_oauth.create_playlist("Test Playlist", "a test playlist", source_playlist=sample_public_playlist)
+    assert isinstance(playlist_id, str)
 
     return playlist_id
 
 
+@pytest.fixture(name="create_playlist_and_delete_after")
+def fixture_create_playlist_and_delete_after(yt_oauth: YTMusic, create_playlist):
+    playlist_id = create_playlist
+    yield playlist_id
+
+    yt_oauth.delete_playlist(playlist_id)
+
+
 @pytest.fixture(name="playlist_with_dupes")
 def fixture_playlist_with_dupes(yt_oauth: YTMusic, create_playlist):
     playlist_id = create_playlist
     playlist = yt_oauth.get_playlist(playlist_id)
     sample_video_id = playlist.get("tracks")[0].get("videoId")
     items_to_add = [sample_video_id]
     yt_oauth.add_playlist_items(playlist_id, items_to_add, duplicates=True)
 
     yield playlist_id
 
     yt_oauth.delete_playlist(playlist_id)
+
+
+@pytest.fixture(name="add_history_items")
+def fixture_add_history_items(yt_oauth: YTMusic, sample_song_list):
+    timestamp = yt_oauth.get_signatureTimestamp()
+    for song in sample_song_list:
+        song = yt_oauth.get_song(song, timestamp)
+        response = yt_oauth.add_history_item(song)
+        assert response.status_code == 204
```

### Comparing `ytmusic_deleter-2.3.2/ytmusic_deleter/README.md` & `ytmusic_deleter-2.3.3/ytmusic_deleter/README.md`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.2/ytmusic_deleter/auth.py` & `ytmusic_deleter-2.3.3/ytmusic_deleter/auth.py`

 * *Files identical despite different names*

### Comparing `ytmusic_deleter-2.3.2/ytmusic_deleter/cli.py` & `ytmusic_deleter-2.3.3/ytmusic_deleter/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging.handlers
 import os
 import re
 import sys
+import time
 from itertools import groupby
 from operator import itemgetter
 from pathlib import Path
 from random import shuffle as unsort
 from time import strftime
 
 import click
@@ -292,56 +293,66 @@
             response = yt_auth.delete_playlist(playlist["playlistId"])
             if response:
                 logging.info(f"\tRemoved playlist {playlist['title']!r} from your library.")
                 playlists_deleted += 1
             else:
                 logging.error(f"\tFailed to remove playlist {playlist['title']!r} from your library.")
         except Exception:
-            logging.error(f"\tCould not delete playlist {playlist['title']}. It might be a YT Music curated playlist.")
+            logging.error(
+                f"\tCould not delete playlist {playlist['title']!r}. It might be a YT Music curated playlist."
+            )
         update_progress()
     logging.info(f"Deleted {playlists_deleted} out of {len(library_playlists)} from your library.")
     return (playlists_deleted, len(library_playlists))
 
 
 @cli.command()
 @click.pass_context
-def delete_history(ctx: click.Context):
+def delete_history(ctx: click.Context, items_deleted: int = 0):
     """
     Delete your play history. This does not currently work with brand accounts.
     The API can only retrieve 200 history items at a time, so the process will appear to
     start over and repeat multiple times if necessary until all history is deleted.
     """
     yt_auth: YTMusic = ctx.obj["YT_AUTH"]
     logging.info("Begin deleting history...")
     try:
         history_items = yt_auth.get_history()
     except Exception as e:
         if str(e) == "None":
-            logging.info("History is empty, nothing to delete.")
+            logging.info("History is empty, nothing left to delete.")
         else:
             logging.exception(e)
-        return False
+        logging.info(f"Deleted {items_deleted} history items.")
+        return items_deleted
     global progress_bar
     progress_bar = manager.counter(
         total=len(history_items),
         desc="History Items Deleted",
         unit="items",
         enabled=not ctx.obj["STATIC_PROGRESS"],
     )
     logging.info(f"Found {len(history_items)} history items to delete.")
     for item in history_items:
         artist = (
             item["artists"][0]["name"]
             if item.get("artists")  # Using `get` ensures key exists and isn't []
             else const.UNKNOWN_ARTIST
         )
-        logging.info(f"Processing {artist} - {item['title']}")
-        yt_auth.remove_history_items(item["feedbackToken"])
+        logging.info(f"\tProcessing history item: {artist} - {item['title']!r}")
+        response = yt_auth.remove_history_items(item["feedbackToken"])
+        if response.get("feedbackResponses")[0].get("isProcessed"):
+            logging.info(f"\tDeleted history item: {artist} - {item['title']!r}")
+            items_deleted += 1
+        else:
+            logging.info(f"\tFailed to delete history item: {response}")
         update_progress()
-    ctx.invoke(delete_history)  # repeat until history is empty
+    logging.info("Restarting history deletion to ensure all songs are deleted.")
+    time.sleep(5)  # Wait before checking for new items as they take time to disappear
+    return ctx.invoke(delete_history, items_deleted)  # repeat until history is empty
 
 
 @cli.command()
 @click.pass_context
 def delete_all(ctx: click.Context):
     """Executes delete-uploads, remove-library, delete-playlists, unlike-all, and delete-history"""
     ctx.invoke(delete_uploads)
```

### Comparing `ytmusic_deleter-2.3.2/ytmusic_deleter/uploads.py` & `ytmusic_deleter-2.3.3/ytmusic_deleter/uploads.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 if artist == const.UNKNOWN_ARTIST:
                     logging.warn("\tSong is missing artist metadata.")
                 if album_title == const.UNKNOWN_ALBUM:
                     logging.warn("\tSong is missing album metadata.")
                 logging.warn("\tSkipping match search and will not delete.")
                 update_progress(progress_bar)
                 continue
-            elif not add_album_to_library(yt_auth, artist, album_title):
+            elif not add_album_to_library(artist, album_title):
                 logging.warn(
                     f"\tNo album was added to library for '{artist} - {album_title}'. Will not delete from uploads."
                 )
                 update_progress(progress_bar)
                 continue
         response = yt_auth.delete_upload_entity(song["album"]["id"] if song.get("album") else song["entityId"])
         if response == "STATUS_SUCCEEDED":
```

### Comparing `ytmusic_deleter-2.3.2/PKG-INFO` & `ytmusic_deleter-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytmusic-deleter
-Version: 2.3.2
+Version: 2.3.3
 Summary: Easily delete your YouTube Music library
 Author-Email: apastel <alex.r.pastel@gmail.com>
 License: GPL-3.0
 Requires-Python: <3.13,>=3.8.1
 Requires-Dist: click>=8.1.7
 Requires-Dist: enlighten>=1.12.4
 Requires-Dist: thefuzz>=0.22.1
```

