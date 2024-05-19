# Comparing `tmp/Mopidy_WebM3U-0.1.2-py3-none-any.whl.zip` & `tmp/Mopidy_WebM3U-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9869 bytes, number of entries: 11
--rw-r--r--  2.0 unx      947 b- defN 24-Mar-06 02:21 mopidy_webm3u/__init__.py
--rw-r--r--  2.0 unx     2886 b- defN 24-Mar-06 02:21 mopidy_webm3u/backend.py
--rw-r--r--  2.0 unx      246 b- defN 24-Mar-06 02:21 mopidy_webm3u/ext.conf
--rw-r--r--  2.0 unx     1575 b- defN 24-Mar-06 02:21 mopidy_webm3u/m3u.py
--rw-r--r--  2.0 unx      135 b- defN 24-Mar-06 02:21 mopidy_webm3u/types.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Mar-06 02:21 Mopidy_WebM3U-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3110 b- defN 24-Mar-06 02:21 Mopidy_WebM3U-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-06 02:21 Mopidy_WebM3U-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 24-Mar-06 02:21 Mopidy_WebM3U-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-06 02:21 Mopidy_WebM3U-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      913 b- defN 24-Mar-06 02:21 Mopidy_WebM3U-0.1.2.dist-info/RECORD
-11 files, 21322 bytes uncompressed, 8315 bytes compressed:  61.0%
+Zip file size: 9989 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      947 b- defN 24-May-19 02:15 mopidy_webm3u/__init__.py
+-rw-r--r--  2.0 unx     3285 b- defN 24-May-19 02:15 mopidy_webm3u/backend.py
+-rw-r--r--  2.0 unx      242 b- defN 24-May-19 02:15 mopidy_webm3u/ext.conf
+-rw-r--r--  2.0 unx     1575 b- defN 24-May-19 02:15 mopidy_webm3u/m3u.py
+-rw-r--r--  2.0 unx      135 b- defN 24-May-19 02:15 mopidy_webm3u/types.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-19 02:15 Mopidy_WebM3U-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3105 b- defN 24-May-19 02:15 Mopidy_WebM3U-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 02:15 Mopidy_WebM3U-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 24-May-19 02:15 Mopidy_WebM3U-0.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-May-19 02:15 Mopidy_WebM3U-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      913 b- defN 24-May-19 02:15 Mopidy_WebM3U-0.1.3.dist-info/RECORD
+11 files, 21712 bytes uncompressed, 8435 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: mopidy_webm3u/m3u.py
 Comment: 
 
 Filename: mopidy_webm3u/types.py
 Comment: 
 
-Filename: Mopidy_WebM3U-0.1.2.dist-info/LICENSE
+Filename: Mopidy_WebM3U-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: Mopidy_WebM3U-0.1.2.dist-info/METADATA
+Filename: Mopidy_WebM3U-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: Mopidy_WebM3U-0.1.2.dist-info/WHEEL
+Filename: Mopidy_WebM3U-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: Mopidy_WebM3U-0.1.2.dist-info/entry_points.txt
+Filename: Mopidy_WebM3U-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: Mopidy_WebM3U-0.1.2.dist-info/top_level.txt
+Filename: Mopidy_WebM3U-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: Mopidy_WebM3U-0.1.2.dist-info/RECORD
+Filename: Mopidy_WebM3U-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mopidy_webm3u/__init__.py

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 
 from mopidy import config, ext
 
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 # If you need to log, use loggers named after the current Python module
 logger = logging.getLogger(__name__)
 
 
 class Extension(ext.Extension):
```

## mopidy_webm3u/backend.py

```diff
@@ -1,10 +1,13 @@
 import pykka
+import hashlib
 import logging
 import typing
+from pathlib import Path
+from urllib.parse import urlparse
 from mopidy import backend, models
 from .m3u import parse_playlist
 from .types import WebM3UConfig
 from typing import cast, ClassVar
 
 logger = logging.getLogger('mopidy_webm3u')
 
@@ -12,70 +15,79 @@
     def __init__(self, config, audio):
         super().__init__()
         ext_config = cast(WebM3UConfig, config['webm3u'])
         uri_scheme = ext_config['uri_scheme']
         self.uri_schemes = [uri_scheme]
         self.playlists = WebM3UPlaylistsProvider(self, ext_config['seed_m3u'], uri_scheme)
 
-# TODO: Protected URI against server-side request forgery - by enforcing hostname and path prefix for playlist URLs?!
-
 class WebM3UPlaylistsProvider(backend.PlaylistsProvider):
     def __init__(self, backend, seed_m3u_url, uri_scheme):
         super().__init__(backend)
         self._seed_m3u_url = seed_m3u_url
         self._uri_scheme = uri_scheme
-        self._playlist_refs = []
+        self._playlist_refs = {}
         self.refresh()
 
     def as_list(self):
         logger.debug('Listing playlists')
-        return self._playlist_refs
+        l = [p.ref for p in self._playlist_refs.values()]
+        l.sort(key=lambda p: (p.name, p.uri))
+        return l
 
     def get_items(self, uri):
         logger.debug('Getting playlist ltems')
         url = self._uri2url(uri)
         return [_item2ref(item) for item in parse_playlist(url)]
 
     def lookup(self, uri):
         logger.debug(f"Looking up playlist {uri}")
-        pl = self._uri2playlistref(uri)
+        pl = self._uri2playlistref(uri).ref
         url = self._uri2url(uri)
         tracks = [_item2track(item) for item in parse_playlist(url)]
         return models.Playlist(uri=uri, name=pl.name, tracks=tracks)
 
     def _uri2playlistref(self, uri):
-        for pl in self._playlist_refs:
-            if pl.uri == uri:
-                return pl
-        raise Exception(f"playlist {uri} not found")
+        p = self._playlist_refs.get(uri)
+        if not p:
+            raise Exception(f"playlist {uri} not found")
+        return p
 
     def refresh(self):
         logger.info(f"Loading M3U playlists from {self._seed_m3u_url}...")
         playlists = [self._playlistref(pl) for pl in parse_playlist(self._seed_m3u_url)]
         logger.info(f"Loaded {len(playlists)} M3U playlists from server")
-        self._playlist_refs = playlists
+        self._playlist_refs = {p.uri: p for p in playlists}
 
     def create(self, name):
         logger.warning('Playlist creation is not supported by this provider')
 
     def delete(self, uri):
         logger.warning('Playlist deletion is not supported by this provider')
         return False
 
     def save(self, uri):
         logger.warning('Playlist manipulation is not supported by this provider')
 
     def _uri2url(self, uri):
-        assert uri.startswith(f"{self._uri_scheme}:"), 'unsupported URI format provided'
-        return uri[len(self._uri_scheme)+1:]
+        assert uri.startswith(f"{self._uri_scheme}:playlist:"), 'unsupported URI format provided'
+        return self._uri2playlistref(uri).url
 
     def _playlistref(self, item):
-        uri = f"{self._uri_scheme}:{item.uri}"
-        return models.Ref(uri=uri, name=item.title, type=models.Ref.PLAYLIST)
+        filename = Path(urlparse(item.uri).path).stem
+        urlhash = hashlib.sha256(item.uri.encode('utf-8')).hexdigest()[:7]
+        id = f"{filename}-{urlhash}".strip('-.')
+        uri = f"{self._uri_scheme}:playlist:{id}"
+        return PlaylistRef(uri, item.uri, item.title)
 
 def _item2track(item):
     return models.Track(
         uri=item.uri,
         name=item.title,
         genre=item.attrs.get('genre'),
         length=item.duration*1000,
     )
+
+class PlaylistRef:
+    def __init__(self, uri, url, name):
+        self.uri = uri
+        self.url = url
+        self.ref = models.Ref(uri=uri, name=name, type=models.Ref.PLAYLIST)
```

## mopidy_webm3u/ext.conf

```diff
@@ -1,7 +1,6 @@
 [webm3u]
 enabled = false
-#seed_m3u = http://beets:8337/m3u/playlists/index.m3u8
-seed_m3u = http://localhost:8337/m3u/playlists/index.m3u8
-#seed_m3u = http://localhost:8337/m3u/playlists/index.m3u8?uri-format=subidy:song:3$id
+#seed_m3u = http://beets:8337/m3u/playlists/index.m3u
+seed_m3u = http://localhost:8337/m3u/playlists/index.m3u
+#seed_m3u = http://localhost:8337/m3u/playlists/index.m3u?uri-format=subidy:song:3$id
 uri_scheme = webm3u
-
```

## Comparing `Mopidy_WebM3U-0.1.2.dist-info/LICENSE` & `Mopidy_WebM3U-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Mopidy_WebM3U-0.1.2.dist-info/METADATA` & `Mopidy_WebM3U-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-WebM3U
-Version: 0.1.2
+Version: 0.1.3
 Summary: Mopidy plugin to play M3U playlists that are hosted on a web server
 Home-page: https://github.com/mgoltzsche/mopidy-webm3u
 Author: Max Goltzsche
 Author-email: max.goltzsche@gmail.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: No Input/Output (Daemon)
@@ -42,33 +42,33 @@
 
 Before starting Mopidy, you must configure it as follows, enabling the webm3u extension and specifying the URL to the M3U playlist of playlists::
 
     [m3u]
     enabled = false
     [webm3u]
     enabled = true
-    seed_m3u = http://beets:8337/playlists/index.m3u8
+    seed_m3u = http://beets:8337/playlists/index.m3u
     uri_scheme = m3u
 
 
 (Mopidy's built-in m3u extension must be disabled in order to be able to use the ``m3u`` URI scheme with the webm3u extension which is required to make playlists show up within the Iris web GUI, see `here <https://github.com/jaedb/Iris/blob/62c4e063f855896d2b4de8dcc024a43f967d5b67/src/js/util/helpers.js#L144>`_.)
 
-The playlist of playlists URL specified by the ``seed_m3u`` option is expected to return an `EXTM3U-formatted <https://datatracker.ietf.org/doc/html/rfc8216#section-4.3.1.1>`_ list of `tagged <https://datatracker.ietf.org/doc/html/rfc8216#section-4.3.2.1>`_ `*.m3u8` HTTP URLs, e.g.::
+The playlist of playlists URL specified by the ``seed_m3u`` option is expected to return an `EXTM3U-formatted <https://datatracker.ietf.org/doc/html/rfc8216#section-4.3.1.1>`_ list of `tagged <https://datatracker.ietf.org/doc/html/rfc8216#section-4.3.2.1>`_ `*.m3u` HTTP URLs, e.g.::
 
     #EXTM3U
     #EXTINF:0,Playlist 1
-    http://localhost:8337/playlists/playlist1.m3u8
+    http://localhost:8337/playlists/playlist1.m3u
     #EXTINF:0,Playlist 2
-    http://localhost:8337/playlists/playlist2.m3u8
+    http://localhost:8337/playlists/playlist2.m3u
 
 
 Development
 ===========
 
-First make sure an example M3U playlist of playlists is served at ``http://localhost:8337/m3u/playlists/index.m3u8``, e.g. by running the `beets-webm3u development server <https://github.com/mgoltzsche/beets-container?tab=readme-ov-file#run-the-beets-web-server>`_.
+First make sure an example M3U playlist of playlists is served at ``http://localhost:8337/m3u/playlists/index.m3u``, e.g. by running the `beets-webm3u development server <https://github.com/mgoltzsche/beets-container?tab=readme-ov-file#run-the-beets-web-server>`_.
 
 Then you can run a mopidy container with the extension installed (including your local changes) as follows (requires `docker <https://docs.docker.com/engine/install/>`_)::
 
     make run
 
 
 Once Mopidy started, you can browse the playlists within the Iris UI at `http://localhost:6680/iris/library/playlists <http://localhost:6680/iris/library/playlists>`_.
```

## Comparing `Mopidy_WebM3U-0.1.2.dist-info/RECORD` & `Mopidy_WebM3U-0.1.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-mopidy_webm3u/__init__.py,sha256=-NV3kDGx5yWlgvHXH27QAFS__CIr0VCiruJvE1SmeaQ,947
-mopidy_webm3u/backend.py,sha256=0A-xY9gHoQoCQGchELO3hPF5uzJoeIgP6gXnq0ZeM_4,2886
-mopidy_webm3u/ext.conf,sha256=7KX91F_q3slAukOFo7JMLAig75w5QnhhlbIR1O93j1c,246
+mopidy_webm3u/__init__.py,sha256=Hcqos7Eid1Cfej5j4CQ-nzw3fm46Wzl9d5xnqOQPspQ,947
+mopidy_webm3u/backend.py,sha256=5jI_JqNjwsxzlRQmQVu8Q9Yo-nUCFfnllzseIEU76mU,3285
+mopidy_webm3u/ext.conf,sha256=56vhsZH-k_83ACnIzh6irdgl6wVw_fUAUsdNWWbzKgg,242
 mopidy_webm3u/m3u.py,sha256=5QXlfh5kR9qpcybkku3YjLfjuc4Ib62DmqxRfJ7NBTY,1575
 mopidy_webm3u/types.py,sha256=Cfo4XVEd3gE1GUtjw8axXxAQFuwIsdnxsDzwXkUcFuc,135
-Mopidy_WebM3U-0.1.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-Mopidy_WebM3U-0.1.2.dist-info/METADATA,sha256=NFTFy6q5teK5Ilnwmt4Qv94JMLRt0JclqOiErKWOu3M,3110
-Mopidy_WebM3U-0.1.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-Mopidy_WebM3U-0.1.2.dist-info/entry_points.txt,sha256=HfE-Dj3-7UHTfAWOFABWz_xp6ndg1TfWQpGLPx4W6oI,47
-Mopidy_WebM3U-0.1.2.dist-info/top_level.txt,sha256=DcUJ5HTeo6UT8TPBU7w05hQwiukyO8p8v3JzPXsrtdY,14
-Mopidy_WebM3U-0.1.2.dist-info/RECORD,,
+Mopidy_WebM3U-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+Mopidy_WebM3U-0.1.3.dist-info/METADATA,sha256=8jPTTySD7yKyxUM19GDLBDX_QTCc-exV0VBpA_aJv4c,3105
+Mopidy_WebM3U-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Mopidy_WebM3U-0.1.3.dist-info/entry_points.txt,sha256=HfE-Dj3-7UHTfAWOFABWz_xp6ndg1TfWQpGLPx4W6oI,47
+Mopidy_WebM3U-0.1.3.dist-info/top_level.txt,sha256=DcUJ5HTeo6UT8TPBU7w05hQwiukyO8p8v3JzPXsrtdY,14
+Mopidy_WebM3U-0.1.3.dist-info/RECORD,,
```

