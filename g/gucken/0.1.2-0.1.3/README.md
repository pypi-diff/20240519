# Comparing `tmp/gucken-0.1.2.tar.gz` & `tmp/gucken-0.1.3.tar.gz`

## Comparing `gucken-0.1.2.tar` & `gucken-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/__main__.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/aniskip.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/custom_widgets.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/default_settings.toml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/gucken.css
--rw-r--r--   0        0        0    23834 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/gucken.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/rome.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/settings.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/update.py
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/hoster/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/hoster/common.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/hoster/doodstream.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/hoster/streamtape.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/hoster/veo.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/hoster/vidoza.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/android.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/common.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/ffplay.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/flatpak.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/mpv.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/vlc.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/player/wmplayer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/__init__.py
--rw-r--r--   0        0        0    10145 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/burningseries.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/common.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/crunchyroll.py
--rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/serienstream.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/provider/streamcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/tracker/__init__.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/tracker/anilist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/tracker/aniworld.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/tracker/common.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/tracker/myanimelist.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.2/src/gucken/tracker/serienstream.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     7028 2020-02-02 00:00:00.000000 gucken-0.1.2/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 gucken-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/__main__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/aniskip.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/custom_widgets.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/default_settings.toml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/gucken.css
+-rw-r--r--   0        0        0    29922 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/gucken.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/rome.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/settings.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/skip.lua
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/update.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/_hosters.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/common.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/doodstream.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/streamtape.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/veo.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/hoster/vidoza.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/__init__.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/_players.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/android.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/common.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/ffplay.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/flatpak.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/mpv.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/vlc.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/player/wmplayer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/__init__.py
+-rw-r--r--   0        0        0    10781 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/burningseries.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/common.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/crunchyroll.py
+-rw-r--r--   0        0        0    10844 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/serienstream.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/provider/streamcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/tracker/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/tracker/anilist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/tracker/aniworld.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/tracker/common.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/tracker/myanimelist.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gucken-0.1.3/src/gucken/tracker/serienstream.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 gucken-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 gucken-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 gucken-0.1.3/README.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 gucken-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 gucken-0.1.3/PKG-INFO
```

### Comparing `gucken-0.1.2/src/gucken/aniskip.py` & `gucken-0.1.3/src/gucken/aniskip.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 from tempfile import NamedTemporaryFile
 from typing import Union
 
 from httpx import AsyncClient
 
 from .tracker.myanimelist import search
 
-
 # TODO: improve fuzzy
 
+
 def fuzzy_search(pattern, possibilities, threshold=0.6):
     matches = []
     for word in possibilities:
         ratio = SequenceMatcher(None, pattern, word).ratio()
         if ratio >= threshold:
             matches.append((word, ratio))
     return matches
 
 
 def fuzzy_sort(pattern, possibilities):
-    return sorted(possibilities, key=lambda x: SequenceMatcher(None, pattern, x).ratio(), reverse=True)
+    return sorted(
+        possibilities,
+        key=lambda x: SequenceMatcher(None, pattern, x).ratio(),
+        reverse=True,
+    )
 
 
-async def get_timings_from_id(anime_id: int, episode_number: int) -> Union[dict[str, float], None]:
+async def get_timings_from_id(
+    anime_id: int, episode_number: int
+) -> Union[dict[str, float], None]:
     async with AsyncClient(verify=False) as client:
         response = await client.get(
             f"https://api.aniskip.com/v1/skip-times/{anime_id}/{episode_number}?types=op&types=ed"
         )
         json = response.json()
         if json.get("found") is not True:
             return None
@@ -44,59 +50,65 @@
             if skip_type == "ed":
                 ed_start_time = start_time
                 ed_end_time = end_time
         return {
             "op_start_time": float(op_start_time),
             "op_end_time": float(op_end_time),
             "ed_start_time": float(ed_start_time),
-            "ed_end_time": float(ed_end_time)
+            "ed_end_time": float(ed_end_time),
         }
 
 
-async def get_timings_from_search(keyword: str, episode_number: int) -> Union[dict[str, float], None]:
+async def get_timings_from_search(
+    keyword: str, episode_number: int
+) -> Union[dict[str, float], None]:
     # TODO: improve search
     myanimelist_search_result = await search(keyword)
     animes = {}
     for anime in myanimelist_search_result["categories"][0]["items"]:
         animes[anime["name"]] = anime["id"]
     search_results = fuzzy_search(keyword, animes)
     if len(search_results) > 0:
         name = search_results[0][0]
         anime_id = animes[name]
         return await get_timings_from_id(anime_id, episode_number)
     return None
 
 
-def timings_to_mpv_options(timings=dict[str, float]) -> str:
+def opening_timings_to_mpv_option(timings=dict[str, float]) -> str:
     op_start_time = timings["op_start_time"]
     op_end_time = timings["op_end_time"]
+    return f"--script-opts-add=skip-op_start={op_start_time},skip-op_end={op_end_time}"
+
+
+def ending_timings_to_mpv_option(timings=dict[str, float]) -> str:
     ed_start_time = timings["ed_start_time"]
     ed_end_time = timings["ed_end_time"]
-    return f"--script-opts=skip-op_start={op_start_time},skip-op_end={op_end_time},skip-ed_start={ed_start_time},skip-ed_end={ed_end_time}"
+    return f"--script-opts-add=skip-ed_start={ed_start_time},skip-ed_end={ed_end_time}"
 
 
 def chapter(start: float, end: float, title: str) -> str:
     return f"\n[CHAPTER]\nTIMEBASE=1/1000\nSTART={int(start * 1000)}\nEND={int(end * 1000)}\nTITLE={title}\n"
 
 
 def get_chapters_file_content(timings=dict[str, float]) -> str:
     op_start_time = timings["op_start_time"]
     op_end_time = timings["op_end_time"]
     ed_start_time = timings["ed_start_time"]
     ed_end_time = timings["ed_end_time"]
     return (
-            ";FFMETADATA1" +
-            chapter(op_start_time, op_end_time, "Opening") +
-            chapter(ed_start_time, ed_end_time, "Ending") +
-            chapter(op_end_time, ed_start_time, "Episode")
+        ";FFMETADATA1"
+        + chapter(op_start_time, op_end_time, "Opening")
+        + chapter(ed_start_time, ed_end_time, "Ending")
+        + chapter(op_end_time, ed_start_time, "Episode")
     )
 
 
 def generate_chapters_file(timings=dict[str, float]) -> NamedTemporaryFile:
-    temp_file = NamedTemporaryFile(mode='w', prefix="gucken-", delete=False)
+    temp_file = NamedTemporaryFile(mode="w", prefix="gucken-", delete=False)
     temp_file.write(get_chapters_file_content(timings))
     temp_file.close()
     return temp_file
 
 
 def get_chapters_file_mpv_option(path: str) -> str:
     return f"--chapters-file={path}"
```

### Comparing `gucken-0.1.2/src/gucken/custom_widgets.py` & `gucken-0.1.3/src/gucken/custom_widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 
 class SortableTable(DataTable):
     """
     TODO: Add mouse support.
     TODO: Improve UX
     """
+
     class SortChanged(Message):
-        def __init__(self, sortable_table: "SortableTable", previous: int, now: int) -> None:
+        def __init__(
+            self, sortable_table: "SortableTable", previous: int, now: int
+        ) -> None:
             self.sortable_table = sortable_table
             self.previous = previous
             self.now = now
             super().__init__()
 
         @property
         def control(self) -> "SortableTable":
@@ -31,15 +34,17 @@
         previous = self.cursor_row
         now = previous + offset
 
         i1 = self._row_locations.get_key(previous)
         i2 = self._row_locations.get_key(now)
         self._row_locations[i1] = now
         self._row_locations[i2] = previous
-        self.cursor_coordinate = self.cursor_coordinate.down() if offset > 0 else self.cursor_coordinate.up()
+        self.cursor_coordinate = (
+            self.cursor_coordinate.down() if offset > 0 else self.cursor_coordinate.up()
+        )
         self._update_count += 1
         self.refresh()
         self.post_message(self.SortChanged(self, previous, now))
 
     def action_cursor_up(self) -> None:
         if not self.move_mode:
             super().action_cursor_up()
```

### Comparing `gucken-0.1.2/src/gucken/gucken.css` & `gucken-0.1.3/src/gucken/gucken.css`

 * *Files identical despite different names*

### Comparing `gucken-0.1.2/src/gucken/gucken.py` & `gucken-0.1.3/src/gucken/gucken.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,104 +1,102 @@
+import argparse
 import logging
-from atexit import register as register_atexit
 from asyncio import gather
-from os import name as os_name, remove
-from .settings import gucken_settings_manager
+from atexit import register as register_atexit
+from os import name as os_name
+from os import remove
+from pathlib import Path
 from random import choice
 from shutil import which
-from subprocess import PIPE, Popen, DEVNULL
+from subprocess import DEVNULL, PIPE, Popen
 from time import sleep, time
-from typing import Union, ClassVar, List
+from typing import ClassVar, List, Union
 
+from platformdirs import user_config_path, user_log_path
 from pypresence import AioPresence, DiscordNotFound
+from rich.markup import escape
 from textual import events, on, work
 from textual.app import App, ComposeResult
-from textual.binding import BindingType, Binding
+from textual.binding import Binding, BindingType
 from textual.containers import Center, Container, Horizontal, ScrollableContainer
 from textual.reactive import reactive
 from textual.screen import ModalScreen
 from textual.widgets import (
     Button,
     Checkbox,
+    Collapsible,
     DataTable,
     Footer,
     Header,
     Input,
     Label,
     ListItem,
     ListView,
     Markdown,
     RadioButton,
+    Select,
     TabbedContent,
     TabPane,
 )
 
-from .utils import detect_player, is_android
-from .custom_widgets import SortableTable
-from .update import check
 from .aniskip import (
-    get_timings_from_search,
-    timings_to_mpv_options,
     generate_chapters_file,
     get_chapters_file_mpv_option,
+    get_timings_from_search,
+    opening_timings_to_mpv_option,
+    ending_timings_to_mpv_option
 )
+from .custom_widgets import SortableTable
+from .hoster._hosters import hoster
 from .hoster.common import DirectLink, Hoster
-from .hoster.doodstream import DoodstreamHoster
-from .hoster.streamtape import StreamtapeHoster
-from .hoster.veo import VOEHoster
-from .hoster.vidoza import VidozaHoster
+from .player._players import all_players_keys, available_players_keys, player_map
 from .player.mpv import MPVPlayer
 from .player.vlc import VLCPlayer
 from .provider.aniworld import AniWorldProvider
 from .provider.common import Episode, Language, SearchResult, Series
 from .provider.serienstream import SerienStreamProvider
-from platformdirs import user_log_path, user_config_path
-
-logs_path = user_log_path("gucken", ensure_exists=True)
-logging.basicConfig(
-    filename=logs_path.joinpath("gucken.log"),
-    encoding="utf-8",
-    level=logging.INFO
-)
-
-register_atexit(gucken_settings_manager.save)
+from .settings import gucken_settings_manager
+from .update import check
+from .utils import detect_player, is_android
 
 
-def sort_favorite_lang(language_list: List[Language], pio_list: List[str]) -> List[Language]:
+def sort_favorite_lang(
+    language_list: List[Language], pio_list: List[str]
+) -> List[Language]:
     def lang_sort_key(hoster: Language) -> int:
         try:
             return pio_list.index(hoster.name)
         except ValueError:
             return len(pio_list)
 
     return sorted(language_list, key=lang_sort_key)
 
 
-"""
-def sort_favorite_hoster(hoster_list: List[Hoster], pio_list: List[Type[Hoster]]) -> List[Hoster]:
-    def hoster_sort_key(hoster: Hoster) -> int:
+def sort_favorite_hoster(
+    hoster_list: List[Hoster], pio_list: List[str]
+) -> List[Hoster]:
+    def hoster_sort_key(_hoster: Hoster) -> int:
         try:
-            return pio_list.index(type(hoster))
+            return pio_list.index(hoster.get_key(type(_hoster)))
         except ValueError:
             return len(pio_list)
 
     return sorted(hoster_list, key=hoster_sort_key)
-"""
 
 
-def sort_favorite_hoster(hoster_list: list[Hoster]) -> list[Hoster]:
-    return sorted(
-        hoster_list,
-        key=lambda x: (
-            not isinstance(x, StreamtapeHoster),
-            not isinstance(x, VOEHoster),
-            not isinstance(x, VidozaHoster),
-            not isinstance(x, DoodstreamHoster),
-        ),
-    )
+def sort_favorite_hoster_by_key(
+    hoster_list: List[str], pio_list: List[str]
+) -> List[str]:
+    def hoster_sort_key(_hoster: str) -> int:
+        try:
+            return pio_list.index(_hoster)
+        except ValueError:
+            return len(pio_list)
+
+    return sorted(hoster_list, key=hoster_sort_key)
 
 
 async def get_working_direct_link(hosters: list[Hoster]) -> Union[DirectLink, None]:
     for hoster in hosters:
         direct_link = await hoster.get_direct_link()
         is_working = await direct_link.check_is_working()
         logging.info(
@@ -187,14 +185,19 @@
 
 
 def remove_none_lang_keys(lst: list) -> list:
     valid_languages = {lang.name for lang in Language}
     return [item for item in lst if item in valid_languages]
 
 
+def remove_none_host_keys(lst: list) -> list:
+    valid_host = {h for h in hoster}
+    return [item for item in lst if item in valid_host]
+
+
 def move_item(lst: list, from_index: int, to_index: int) -> list:
     item = lst.pop(from_index)
     lst.insert(to_index, item)
     return lst
 
 
 client_id = "1238219157464416266"
@@ -208,84 +211,231 @@
     custom_css = user_config_path("gucken").joinpath("custom.css")
     if custom_css.exists():
         CSS_PATH.append(custom_css)
     BINDINGS: ClassVar[list[BindingType]] = [
         Binding("q", "quit", "Quit", show=True, priority=False),
     ]
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, debug: bool, search: str):
+        super().__init__(watch_css=debug)
+        self._debug = debug
+        self._search = search
+
         self.current: Union[list[SearchResult], None] = None
         self.current_info: Union[Series, None] = None
-        self.player = detect_player()
+        self.detected_player = detect_player()
         self.RPC: Union[AioPresence, None] = None
 
         language: list = gucken_settings_manager.settings["settings"]["language"]
         language = remove_none_lang_keys(language)
 
         for ll in Language:
             language.append(ll.name)
 
-        gucken_settings_manager.settings["settings"]["language"] = remove_duplicates(language)
+        gucken_settings_manager.settings["settings"]["language"] = remove_duplicates(
+            language
+        )
         self.language = gucken_settings_manager.settings["settings"]["language"]
 
+        _hoster: list = gucken_settings_manager.settings["settings"]["hoster"]
+        _hoster = remove_none_host_keys(_hoster)
+
+        for ll in hoster:
+            _hoster.append(ll)
+
+        gucken_settings_manager.settings["settings"]["hoster"] = remove_duplicates(
+            _hoster
+        )
+        self.hoster = gucken_settings_manager.settings["settings"]["hoster"]
+
     def compose(self) -> ComposeResult:
         settings = gucken_settings_manager.settings["settings"]
         providers = settings["providers"]
+
+        player = settings["player"]["player"]
+        if player not in all_players_keys:
+            player = "AutomaticPlayer"
+
         yield Header()
         with TabbedContent():
             with TabPane("Search", id="search"):  # Search "🔎"
                 with Horizontal(id="hosters"):
-                    yield Checkbox("AniWorld.to", value=providers["aniworld_to"], id="aniworld_to")
-                    yield Checkbox("SerienStream.to", value=providers["serienstream_to"], id="serienstream_to")
+                    yield Checkbox(
+                        "AniWorld.to",
+                        value=providers["aniworld_to"],
+                        id="aniworld_to",
+                        classes="provider"
+                    )
+                    yield Checkbox(
+                        "SerienStream.to",
+                        value=providers["serienstream_to"],
+                        id="serienstream_to",
+                        classes="provider"
+                    )
                 yield Input(id="input", placeholder="Search for a Anime")
                 yield ListView(id="results")
             with TabPane("Info", id="info", disabled=True):  # Info "ℹ"
                 with ScrollableContainer(id="res_con"):
                     yield Markdown(id="markdown")
                     yield ClickableDataTable(id="season_list")
             with TabPane("Settings", id="setting"):  # Settings "⚙"
                 # TODO: dont show unneeded on android
-                with Container():
+                with ScrollableContainer():
                     yield SortableTable(id="lang")
-                    yield RadioButton("Fullscreen", id="fullscreen", value=settings["fullscreen"])
-                    yield RadioButton("Syncplay", id="syncplay", value=settings["syncplay"])
-                    yield RadioButton("ani-skip", id="ani-skip", value=settings["ani-skip"])
-                    yield RadioButton("Discord Presence", id="discord_presence", value=settings["discord_presence"])
-            # with RadioSet():
-            #    yield RadioButton("VOE", id="voe", value=True)
-            #    yield RadioButton("Doodstream", id="doodstream")
-            #    yield RadioButton("Vidoza", id="vidoza")
-            #    yield RadioButton("Streamtape", id="streamtape")
+                    yield SortableTable(id="host")
+                    yield RadioButton(
+                        "Update checker",
+                        id="update_checker",
+                        value=settings["update_checker"],
+                    )
+                    yield RadioButton(
+                        "Discord Presence",
+                        id="discord_presence",
+                        value=settings["discord_presence"],
+                    )
+                    with Collapsible(title="Player", collapsed=False):
+                        yield RadioButton(
+                            "Fullscreen", id="fullscreen", value=settings["fullscreen"]
+                        )
+                        yield RadioButton(
+                            "Syncplay", id="syncplay", value=settings["syncplay"]
+                        )
+                        yield RadioButton(
+                            "Autoplay",
+                            id="autoplay",
+                            value=settings["autoplay"]["enabled"],
+                        )
+                        yield Select.from_values(
+                            available_players_keys,
+                            id="player",
+                            prompt="AutomaticPlayer",
+                            value=(
+                                Select.BLANK if player == "AutomaticPlayer" else player
+                            ),
+                        )
+                    with Collapsible(title="ani-skip (only for MPV)", collapsed=False):
+                        yield RadioButton(
+                            "Skip opening",
+                            id="ani_skip_opening",
+                            value=settings["ani_skip"]["skip_opening"],
+                        )
+                        yield RadioButton(
+                            "Skip ending",
+                            id="ani_skip_ending",
+                            value=settings["ani_skip"]["skip_ending"],
+                        )
+                        yield RadioButton(
+                            "Get chapters",
+                            id="ani_skip_chapters",
+                            value=settings["ani_skip"]["chapters"],
+                        )
         with Footer():
             with Center():
                 yield Label("Made by Commandcracker with [red]:heart:[/red]")
 
+    @on(Input.Changed)
+    async def input_changed(self, event: Input.Changed):
+        id = event.control.id
+        value = event.value
+
+        if id == "input":
+            if value:
+                self.lookup_anime(value)
+            else:
+                # TODO: fix sometimes wont clear
+                await self.query_one("#results", ListView).clear()
+
+    @on(SortableTable.SortChanged)
+    async def sortableTable_sortChanged(
+        self,
+        event: SortableTable.SortChanged
+    ):
+        id = event.control.id
+        if id == "lang":
+            move_item(self.language, event.previous, event.now)
+            return
+
+        if id == "host":
+            move_item(self.hoster, event.previous, event.now)
+            return
+
+    @on(Checkbox.Changed)
+    async def checkbox_changed(self, event: Checkbox.Changed):
+        id = event.control.id
+        settings = gucken_settings_manager.settings["settings"]
+
+        if event.control.has_class("provider"):
+            settings["providers"][id] = event.value
+            self.lookup_anime(self.query_one("#input", Input).value)
+
+    @on(RadioButton.Changed)
+    async def radio_button_changed(self, event: RadioButton.Changed):
+        id = event.control.id
+        settings = gucken_settings_manager.settings["settings"]
+
+        if id == "ani_skip_opening":
+            settings["ani_skip"]["skip_opening"] = event.value
+            return
+
+        if id == "ani_skip_ending":
+            settings["ani_skip"]["skip_ending"] = event.value
+            return
+
+        if id == "ani_skip_chapters":
+            settings["ani_skip"]["chapters"] = event.value
+            return
+
+        if id == "autoplay":
+            settings["autoplay"]["enabled"] = event.value
+            return
+
+        settings[id] = event.value
+
+        if id == "discord_presence":
+            if event.value is True:
+                await self.enable_RPC()
+            else:
+                await self.disable_RPC()
+
+    @on(Select.Changed)
+    def select_changed(self, event: Select.Changed) -> None:
+        id = event.control.id
+        settings = gucken_settings_manager.settings["settings"]
+
+        if id == "player":
+            if event.value == Select.BLANK:
+                settings["player"]["player"] = "AutomaticPlayer"
+            else:
+                settings["player"]["player"] = event.value
+
     # TODO: dont lock - no async
     async def on_mount(self) -> None:
         lang = self.query_one("#lang", DataTable)
         lang.add_columns("Language")
         for l in self.language:
             lang.add_row(l)
-        self.query_one(Input).focus()
-        # TODO: FIx sometimes not disabling loading
-        # TODO: dont lock
+
+        host = self.query_one("#host", DataTable)
+        host.add_columns("Host")
+        for h in self.hoster:
+            host.add_row(h)
+
+        input = self.query_one("#input", Input)
+        input.focus()
+        input.value = self._search
+
         self.query_one("#info", TabPane).loading = True
+
         table = self.query_one("#season_list", DataTable)
         table.cursor_type = "row"
-        # TODO: make them scale
         table.add_columns("FT", "S", "F", "Title", "Hoster", "Sprache")
-        if self.player is None:
-            self.notify(
-                "You wont be able to play videos.\n"
-                "Without an supported video player!",
-                title="No player found",
-                severity="warning",
-            )
-        self.update_check()
+
+        if self.query_one("#update_checker", RadioButton).value is True:
+            self.update_check()
+
         # TODO: dont lock
         if self.query_one("#discord_presence", RadioButton).value is True:
             await self.enable_RPC()
         else:
             await self.disable_RPC()
 
     async def enable_RPC(self):
@@ -300,36 +450,14 @@
         if self.RPC is not None:
             await self.RPC.clear()
             # close without closing event loop
             self.RPC.send_data(2, {"v": 1, "client_id": self.RPC.client_id})
             self.RPC.sock_writer.close()
             self.RPC = None
 
-    async def on_checkbox_changed(self, event: Checkbox.Changed):
-        gucken_settings_manager.settings["settings"]["providers"][event.control.id] = event.value
-        self.lookup_anime(self.query_one("#input", Input).value)
-
-    async def on_radio_button_changed(self, event: RadioButton.Changed):
-        gucken_settings_manager.settings["settings"][event.control.id] = event.value
-        if event.radio_button.id == "discord_presence":
-            if event.value is True:
-                await self.enable_RPC()
-            else:
-                await self.disable_RPC()
-
-    async def on_sortable_table_sort_changed(self, event: SortableTable.SortChanged) -> None:
-        move_item(self.language, event.previous, event.now)
-
-    async def on_input_changed(self, message: Input.Changed) -> None:
-        if message.value:
-            self.lookup_anime(message.value)
-        else:
-            # TODO: fix sometimes wont clear
-            await self.query_one("#results", ListView).clear()
-
     # TODO: https://textual.textualize.io/guide/workers/#thread-workers
     @work(exclusive=True)
     async def lookup_anime(self, keyword: str) -> None:
         search_providers = []
         if self.query_one("#aniworld_to", Checkbox).value:
             search_providers.append(AniWorldProvider.search(keyword))
 
@@ -347,17 +475,21 @@
                     final_results.append(e)
 
         # TODO: Sort final_results with fuzzy-sort
         if len(final_results) > 0:
             self.current = final_results
             for series in final_results:
                 # TODO: show provider
-                await results_list_view.append(ClickableListItem(Markdown(
-                    f"##### {series.name} {series.production_year}\n{series.description}"
-                )))
+                await results_list_view.append(
+                    ClickableListItem(
+                        Markdown(
+                            f"##### {series.name} {series.production_year}\n{series.description}"
+                        )
+                    )
+                )
         results_list_view.loading = False
         if len(final_results) > 0:
 
             def select_first_index():
                 try:
                     results_list_view.index = 0
                 except AssertionError:
@@ -397,20 +529,26 @@
     @work(exclusive=True)
     async def play_selected(self):
         dt = self.query_one("#season_list", DataTable)
         # TODO: show loading
         dt.loading = True
         index = self.app.query_one("#results", ListView).index
         series_search_result = self.current[index]
-        self.play(series_search_result=series_search_result, episodes=self.current_info.episodes, index=dt.cursor_row)
+        self.play(
+            series_search_result=series_search_result,
+            episodes=self.current_info.episodes,
+            index=dt.cursor_row,
+        )
         dt.loading = False
 
     @work(exclusive=True)
     async def open_info(self) -> None:
-        series_search_result: SearchResult = self.current[self.app.query_one("#results", ListView).index]
+        series_search_result: SearchResult = self.current[
+            self.app.query_one("#results", ListView).index
+        ]
         info_tab = self.query_one("#info", TabPane)
         info_tab.disabled = False
         info_tab.loading = True
         self.query_one(TabbedContent).active = "info"
         md = self.query_one("#markdown", Markdown)
         series = await series_search_result.get_series()
         self.current_info = series
@@ -418,35 +556,28 @@
 
         table = self.query_one("#season_list", DataTable)
         table.clear()
         c = 0
         for ep in series.episodes:
             hl = []
             for h in ep.available_hoster:
-                if h is VOEHoster:
-                    hl.append("VEO")
-                if h is DoodstreamHoster:
-                    hl.append("D")
-                if h is VidozaHoster:
-                    hl.append("VZ")
-                if h is StreamtapeHoster:
-                    hl.append("ST")
+                hl.append(hoster.get_key(h))
 
             ll = []
-            for l in ep.available_language:
+            for l in sort_favorite_lang(ep.available_language, self.language):
                 ll.append(l.name)
 
             c += 1
             table.add_row(
                 c,
                 ep.season,
                 ep.episode_number,
-                ep.title,
-                " ".join(hl),
-                " ".join(ll)
+                escape(ep.title),
+                " ".join(sort_favorite_hoster_by_key(hl, self.hoster)),
+                " ".join(ll),
             )
         table.focus(scroll_visible=False)
         info_tab.loading = False
 
     @work(exclusive=True, thread=True)
     async def update_check(self):
         res = await check()
@@ -455,55 +586,64 @@
                 f"{res.current} -> {res.latest}\npip install -U gucken",
                 title="Update available",
                 severity="information",
             )
 
     @work(thread=True)
     async def play(
-            self,
-            series_search_result: SearchResult,
-            episodes: list[Episode],
-            index: int
+        self, series_search_result: SearchResult, episodes: list[Episode], index: int
     ) -> None:
+        p = self.query_one("#player", Select).value
+        if p == Select.BLANK:
+            _player = self.detected_player
+        else:
+            _player = player_map[p]()
+
+        if _player is None:
+            self.notify(
+                "Please install a supported player!",
+                title="No player detected",
+                severity="error",
+            )
+            return
+
+        if p != Select.BLANK:
+            if not _player.is_available():
+                self.notify(
+                    "Your configured player has not been found!",
+                    title="Player not found",
+                    severity="error",
+                )
+                return
+
         episode: Episode = episodes[index]
         processed_hoster = await episode.process_hoster()
 
         if len(episode.available_language) <= 0:
             self.notify(
                 "The episode you are trying to watch has no stream available.",
                 title="No stream available",
                 severity="error",
             )
             return
 
         lang = sort_favorite_lang(episode.available_language, self.language)[0]
-        sorted_hoster = sort_favorite_hoster(processed_hoster.get(lang))
+        sorted_hoster = sort_favorite_hoster(processed_hoster.get(lang), self.hoster)
         direct_link = await get_working_direct_link(sorted_hoster)
 
         # TODO: check for header support
-
-        if self.player is None:
-            self.notify(
-                "You wont be able to play videos.\n"
-                "Without an supported video player!",
-                title="No player found",
-                severity="error",
-            )
-            return
-
-        # TODO: ani_skip, syncplay, fullscreen as cli arg
         # TODO: pass ani_skip as script
-        ani_skip = self.query_one("#ani-skip", RadioButton).value
         syncplay = self.query_one("#syncplay", RadioButton).value
         fullscreen = self.query_one("#fullscreen", RadioButton).value
 
-        title = f"{series_search_result.name} - {episode.title}"
-        args = self.player.play(direct_link.url, title, fullscreen, direct_link.headers)
+        title = f"{series_search_result.name} S{episode.season}E{episode.episode_number} - {episode.title}"
+        args = _player.play(direct_link.url, title, fullscreen, direct_link.headers)
 
         if self.RPC and self.RPC.sock_writer:
+
             async def update():
                 await self.RPC.update(
                     # state="00:20:00 / 00:25:00 57% complete",
                     details=title[:128],
                     large_text=title,
                     large_image=series_search_result.cover,
                     # small_image as playing or stopped ?
@@ -514,32 +654,49 @@
                 )
 
             self.app.call_later(update)
 
         chapters_file = None
 
         # TODO: cache more
-        if isinstance(self.player, MPVPlayer):
-            if ani_skip is True:
-                timings = await get_timings_from_search(series_search_result.name, index + 1)
+        # TODO: Support based on mpv
+        # TODO: recover start --start=00:56
+        if isinstance(_player, MPVPlayer):
+            ani_skip_opening = self.query_one("#ani_skip_opening", RadioButton).value
+            ani_skip_ending = self.query_one("#ani_skip_ending", RadioButton).value
+            ani_skip_chapters = self.query_one("#ani_skip_chapters", RadioButton).value
+
+            if ani_skip_opening or ani_skip_ending or ani_skip_chapters:
+                timings = await get_timings_from_search(
+                    series_search_result.name, index + 1
+                )
                 if timings:
-                    chapters_file = generate_chapters_file(timings)
+                    if ani_skip_chapters:
+                        chapters_file = generate_chapters_file(timings)
+
+                        def delete_chapters_file():
+                            try:
+                                remove(chapters_file.name)
+                            except FileNotFoundError:
+                                pass
+
+                        register_atexit(delete_chapters_file)
 
-                    def delete_chapters_file():
-                        try:
-                            remove(chapters_file.name)
-                        except FileNotFoundError:
-                            pass
-
-                    register_atexit(delete_chapters_file)
-                    # --start=00:56
-                    args += [
-                        timings_to_mpv_options(timings),
-                        get_chapters_file_mpv_option(chapters_file.name)
-                    ]
+                        args.append(get_chapters_file_mpv_option(chapters_file.name))
+
+                    if ani_skip_opening:
+                        args.append(opening_timings_to_mpv_option(timings))
+
+                    if ani_skip_ending:
+                        args.append(ending_timings_to_mpv_option(timings))
+
+                    args.append("--script=" + str(Path(__file__).parent.joinpath("skip.lua")))
+                    if self._debug:
+                        logs_path = user_log_path("gucken", ensure_exists=True)
+                        args.append("--log-file=" + str(logs_path.joinpath("mpv.log")))
 
         if syncplay:
             # TODO: make work with flatpak
             # TODO: make work with android
             syncplay_path = None
             if which("syncplay"):
                 syncplay_path = "syncplay"
@@ -551,20 +708,26 @@
                 self.notify(
                     "Syncplay not found",
                     title="Syncplay not found",
                     severity="error",
                 )
             else:
                 # TODO: add mpv.net, IINA, MPC-BE, MPC-HE, celluloid ?
-                if isinstance(self.player, MPVPlayer) or isinstance(self.player, VLCPlayer):
+                if isinstance(_player, MPVPlayer) or isinstance(_player, VLCPlayer):
                     player_path = which(args[0])
                     url = args[1]
                     args.pop(0)
                     args.pop(0)
-                    args = [syncplay_path, "--player-path", player_path, url, "--"] + args
+                    args = [
+                        syncplay_path,
+                        "--player-path",
+                        player_path,
+                        url,
+                        "--",
+                    ] + args
                 else:
                     self.notify(
                         "Your player is not supported by Syncplay",
                         title="Player not supported",
                         severity="warning",
                     )
 
@@ -611,34 +774,52 @@
                             self.play(
                                 series_search_result,
                                 episodes,
                                 index + 1,
                             )
 
                     await self.app.push_screen(
-                        Next("Playing next episode in", no_time=is_android), callback=play_next)
+                        Next("Playing next episode in", no_time=is_android),
+                        callback=play_next,
+                    )
 
+                autoplay = self.query_one("#autoplay", RadioButton).value
                 if not len(episodes) <= index + 1:
-                    self.app.call_later(push_next_screen)
+                    if autoplay is True:
+                        self.app.call_later(push_next_screen)
                 else:
                     # TODO: ask to mark as completed
                     pass
                 return
 
 
 exit_quotes = [
     "Closing one anime is just an invitation to open another.",
     "You finished one, now finish the next.",
     "Don't stop now, there's a whole universe waiting to be explored.",
     "The end of one journey is just the beginning of another.",
-    "Like a phoenix rising from the ashes, the end of one episode ignites the flames of anticipation for the next."
+    "Like a phoenix rising from the ashes, the end of one episode ignites the flames of anticipation for the next.",
 ]
 
 
 def main():
-    gucken_app = GuckenApp()
+    parser = argparse.ArgumentParser(
+        prog='Gucken',
+        description="Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style."
+    )
+    parser.add_argument("search", nargs='?')
+    parser.add_argument("--debug", "--dev", action="store_true")
+    args = parser.parse_args()
+    if args.debug:
+        logs_path = user_log_path("gucken", ensure_exists=True)
+        logging.basicConfig(
+            filename=logs_path.joinpath("gucken.log"), encoding="utf-8", level=logging.INFO
+        )
+
+    register_atexit(gucken_settings_manager.save)
+    gucken_app = GuckenApp(debug=args.debug, search=args.search)
     gucken_app.run()
     print(choice(exit_quotes))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `gucken-0.1.2/src/gucken/rome.py` & `gucken-0.1.3/src/gucken/rome.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from re import compile as re_compile
 
 ROMAN_PATTERN = re_compile(r"\b[IVXLCDM]+\b")
-ROMAN_NUMERALS = {'I': 1, 'V': 5, 'X': 10, 'L': 50, 'C': 100, 'D': 500, 'M': 1000}
+ROMAN_NUMERALS = {"I": 1, "V": 5, "X": 10, "L": 50, "C": 100, "D": 500, "M": 1000}
 
 
 def roman_to_int(roman: str) -> int:
     result = 0
     prev_value = 0
     for char in reversed(roman):
         value = ROMAN_NUMERALS[char]
```

### Comparing `gucken-0.1.2/src/gucken/settings.py` & `gucken-0.1.3/src/gucken/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Dict, Union
 from pathlib import Path
-from platformdirs import user_config_path
+from typing import Dict, Union
+
 import toml
+from platformdirs import user_config_path
 
 
 def _merge_dicts(dict1: Dict, dict2: Dict) -> Dict:
     """
     Deep merge
     """
     merged = dict1.copy()
@@ -18,44 +19,44 @@
         else:
             merged[key] = value
     return merged
 
 
 def _load_settings(file_path: Union[str, Path], default_settings: Dict) -> Dict:
     try:
-        with open(file_path, 'r') as file:
+        with open(file_path, "r") as file:
             loaded_settings = toml.load(file)
     except FileNotFoundError:
         loaded_settings = {}
     return _merge_dicts(default_settings, loaded_settings)
 
 
 def _save_settings(settings: Dict, file_path: Union[str, Path]) -> None:
-    with open(file_path, 'w') as file:
+    with open(file_path, "w") as file:
         toml.dump(settings, file)
 
 
 class SettingsManager:
     def __init__(
-            self,
-            default_settings_file: Path,
-            settings_file: Path,
-            load_on_init=True,
-            save_on_load=True
+        self,
+        default_settings_file: Path,
+        settings_file: Path,
+        load_on_init=True,
+        save_on_load=True,
     ):
         super().__init__()
         self.default_settings_file = default_settings_file
         self.settings_file = settings_file
         self.save_on_load = save_on_load
         self.settings: Union[Dict, None] = None
         if load_on_init:
             self.load()
 
     def load(self):
-        with open(self.default_settings_file, 'r') as file:
+        with open(self.default_settings_file, "r") as file:
             default_settings = toml.load(file)
 
         self.settings = _load_settings(self.settings_file, default_settings)
 
         if self.save_on_load:
             self.save()
 
@@ -75,9 +76,9 @@
 
 class GuckenSettingsManager(Singleton, SettingsManager):
     pass
 
 
 gucken_settings_manager = GuckenSettingsManager(
     default_settings_file=Path(__file__).parent.joinpath("default_settings.toml"),
-    settings_file=user_config_path("gucken").joinpath("settings.toml")
+    settings_file=user_config_path("gucken").joinpath("settings.toml"),
 )
```

### Comparing `gucken-0.1.2/src/gucken/update.py` & `gucken-0.1.3/src/gucken/hoster/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-from httpx import AsyncClient
-from packaging.version import Version
-from . import __version__ as current_version
-from typing import Union
+from abc import abstractmethod
 from dataclasses import dataclass
 
-
-PACKAGE_NAME = "gucken"
+from httpx import AsyncClient, HTTPError
 
 
 @dataclass
-class UpdateResult:
-    current: str
-    latest: str
-
-
-async def get_latest_version():
-    async with AsyncClient(verify=False) as client:
-        response = await client.get(f"https://pypi.org/pypi/{PACKAGE_NAME}/json")
-        return response.json().get("info").get("version")
-
+class DirectLink:
+    url: str
+    headers: dict[str, str] = None
+
+    async def check_is_working(self) -> bool:
+        try:
+            async with AsyncClient(verify=False) as client:
+                response = await client.head(
+                    self.url, follow_redirects=True, headers=self.headers
+                )
+                return response.is_success
+        except HTTPError:
+            return False
+
+    def __str__(self):
+        return self.url
+
+    def has_headers(self) -> bool:
+        if self.headers is not None:
+            return True
+        return False
 
-async def check() -> Union[UpdateResult, None]:
-    latest_version = await get_latest_version()
-    if Version(latest_version) > Version(current_version):
-        return UpdateResult(current_version, latest_version)
-    return None
 
-
-def main():
-    from asyncio import run
-    print(run(check()))
-
-
-if __name__ == "__main__":
-    main()
+@dataclass
+class Hoster:
+    url: str
+    requires_headers: bool = False
+
+    @abstractmethod
+    async def get_direct_link(self) -> DirectLink:
+        raise NotImplementedError
```

### Comparing `gucken-0.1.2/src/gucken/hoster/common.py` & `gucken-0.1.3/src/gucken/player/ffplay.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-from abc import abstractmethod
 from dataclasses import dataclass
+from shutil import which
 
-from httpx import AsyncClient, HTTPError
+from .common import Player, dict_to_string
 
 
 @dataclass
-class DirectLink:
-    url: str
-    headers: dict[str, str] = None
+class FFPlayPlayer(Player):
+    supports_headers: bool = True
 
-    async def check_is_working(self) -> bool:
-        try:
-            async with AsyncClient(verify=False) as client:
-                response = await client.head(self.url, follow_redirects=True, headers=self.headers)
-                return response.is_success
-        except HTTPError:
-            return False
-
-    def __str__(self):
-        return self.url
-
-    def has_headers(self) -> bool:
-        if self.headers is not None:
-            return True
-        return False
-
-
-@dataclass
-class Hoster:
-    url: str
-    requires_headers: bool = False
-
-    @abstractmethod
-    async def get_direct_link(self) -> DirectLink:
-        raise NotImplementedError
+    @staticmethod
+    def detect_executable() -> str:
+        if which("ffplay"):
+            return "ffplay"
+
+    def play(
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
+    ) -> list[str]:
+        args = [override_executable or self.detect_executable(), url]
+        if title:
+            args.append("-window_title")
+            args.append(title)
+        if headers:
+            args.append(f"-headers={dict_to_string(headers)}")
+        return args
```

### Comparing `gucken-0.1.2/src/gucken/hoster/doodstream.py` & `gucken-0.1.3/src/gucken/hoster/doodstream.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,35 +9,41 @@
 
 from .common import DirectLink, Hoster
 
 EXTRACT_DOODSTREAM_HLS_PATTERN = re_compile(r"/pass_md5/[\w-]+/[\w-]+")
 
 
 def random_str(length: int = 10) -> str:
-    return ''.join(choices(ascii_letters + digits, k=length))
+    return "".join(choices(ascii_letters + digits, k=length))
 
 
 def js_date_now() -> int:
     return int(time() * 1000)
 
 
-headers = {'Referer': 'https://d0000d.com/'}
+headers = {"Referer": "https://d0000d.com/"}
 
 
 @dataclass
 class DoodstreamHoster(Hoster):
     requires_headers = True
 
     async def get_direct_link(self) -> DirectLink:
-        async with (AsyncClient(verify=False) as client):
+        async with AsyncClient(verify=False) as client:
             response = await client.head(self.url)
             if response.has_redirect_location:
-                u2 = urlparse(response.headers.get("Location"))._replace(netloc="d000d.com").geturl()
+                u2 = (
+                    urlparse(response.headers.get("Location"))
+                    ._replace(netloc="d000d.com")
+                    .geturl()
+                )
                 response = await client.get(u2)
 
             pass_md5 = EXTRACT_DOODSTREAM_HLS_PATTERN.search(response.text)
-            response = await client.get(f"https://d0000d.com{pass_md5.group()}",
-                                        headers={'Referer': 'https://d0000d.com/'})
+            response = await client.get(
+                f"https://d0000d.com{pass_md5.group()}",
+                headers={"Referer": "https://d0000d.com/"},
+            )
             return DirectLink(
                 url=f"{response.text}{random_str()}?token={pass_md5.group().split('/')[-1]}&expiry={js_date_now()}",
-                headers=headers
+                headers=headers,
             )
```

### Comparing `gucken-0.1.2/src/gucken/hoster/streamtape.py` & `gucken-0.1.3/src/gucken/hoster/streamtape.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from re import compile as re_compile
 
 from httpx import AsyncClient
 
 from .common import DirectLink, Hoster
 
-STREAMTAPE_PATTERN = re_compile(r'botlink(.*?)innerHTML(.*?)\);')
-STREAMTAPE_PATTERN_SUBSTRING = re_compile(r'substring\(\d+')
-STREAMTAPE_PATTERN_DIGETS = re_compile(r'\d+')
+STREAMTAPE_PATTERN = re_compile(r"botlink(.*?)innerHTML(.*?)\);")
+STREAMTAPE_PATTERN_SUBSTRING = re_compile(r"substring\(\d+")
+STREAMTAPE_PATTERN_DIGETS = re_compile(r"\d+")
 
 
 class StreamtapeHoster(Hoster):
     async def get_direct_link(self) -> DirectLink:
         # TODO: Error checking
         async with AsyncClient(verify=False) as client:
             response = await client.get(self.url, follow_redirects=True)
             # TODO: Save html and error in order to investigate
             # with open("out.txt", "wb") as f:
             #    f.write(response.text.encode('utf-8'))
             video_src = STREAMTAPE_PATTERN.search(response.text)
             j1 = "".join(video_src.groups())
             u1 = j1.split(" ")[2][1:-2]
-            u2 = j1[j1.index("('") + 2:j1.rfind("')")]
+            u2 = j1[j1.index("('") + 2 : j1.rfind("')")]
 
             matches = STREAMTAPE_PATTERN_SUBSTRING.findall(j1)
             for match in matches:
                 sub = STREAMTAPE_PATTERN_DIGETS.search(match).group(0)
-                u2 = u2[int(sub):]
+                u2 = u2[int(sub) :]
 
             return DirectLink(f"https:{u1}{u2}")
```

### Comparing `gucken-0.1.2/src/gucken/hoster/veo.py` & `gucken-0.1.3/src/gucken/hoster/veo.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.2/src/gucken/hoster/vidoza.py` & `gucken-0.1.3/src/gucken/hoster/vidoza.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from re import compile as re_compile
 
 from httpx import AsyncClient
 
 from .common import DirectLink, Hoster
 
 # TODO: improve all patterns
-EXTRACT_VIDOZA_HLS_PATTERN = re_compile(r"sourcesCode:.*?\[.*?\{.*?src:.*?[\'|\"](?P<hls>.*?)[\'|\"],")
+EXTRACT_VIDOZA_HLS_PATTERN = re_compile(
+    r"sourcesCode:.*?\[.*?\{.*?src:.*?[\'|\"](?P<hls>.*?)[\'|\"],"
+)
 
 
 class VidozaHoster(Hoster):
     async def get_direct_link(self) -> DirectLink:
         async with AsyncClient(verify=False) as client:
             response = await client.get(self.url, follow_redirects=True)
             match_hls = EXTRACT_VIDOZA_HLS_PATTERN.search(response.text)
```

### Comparing `gucken-0.1.2/src/gucken/player/android.py` & `gucken-0.1.3/src/gucken/player/android.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,74 @@
 from .common import Player
 
 
 class AndroidChoosePlayer(Player):
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
         return [
             "am",
             "start",
             "--user",
             "0",
-            "-a"
-            "android.intent.action.VIEW",
+            "-a" "android.intent.action.VIEW",
             "-d",
             url,
             "-c",
-            "android.intent.category.BROWSABLE"
+            "android.intent.category.BROWSABLE",
         ]
 
 
 # http://mpv-android.github.io/mpv-android/intent.html
 class AndroidMPVPlayer(Player):
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
         return [
             "am",
             "start",
             "--user",
             "0",
-            "-a"
-            "android.intent.action.VIEW",
+            "-a" "android.intent.action.VIEW",
             "-d",
             url,
             "-n",
-            "is.xyz.mpv/.MPVActivity"
+            "is.xyz.mpv/.MPVActivity",
         ]
 
 
 # https://wiki.videolan.org/Android_Player_Intents/
 class AndroidVLCPlayer(Player):
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
         args = [
             "am",
             "start",
             "--user",
             "0",
-            "-a"
-            "android.intent.action.VIEW",
+            "-a" "android.intent.action.VIEW",
             "-d",
             url,
             "-n",
-            "org.videolan.vlc/org.videolan.vlc.gui.video.VideoPlayerActivity"
+            "org.videolan.vlc/org.videolan.vlc.gui.video.VideoPlayerActivity",
         ]
         if title:
             args.append("-e")
             args.append("title")
             args.append(title)
         return args
```

### Comparing `gucken-0.1.2/src/gucken/player/mpv.py` & `gucken-0.1.3/src/gucken/player/mpv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,89 @@
-from .common import Player, dict_to_string
 from dataclasses import dataclass
+from os import getenv
+from os import name as os_name
+from os.path import join
+from shutil import which
+
+from .common import Player, dict_to_string
 
 
 @dataclass
 class MPVPlayer(Player):
-    executable: str = "mpv"
     supports_headers: bool = True
 
+    @staticmethod
+    def detect_executable() -> str:
+        if os_name == "nt" and which("mpv.exe"):
+            return "mpv.exe"
+        if which("mpv"):
+            return "mpv"
+
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
-        args = [
-            override_executable or self.executable,
-            url
-        ]
+        args = [override_executable or self.executable, url]
         if full_screen:
             args.append("--fullscreen")
         if title:
             args.append(f"--force-media-title={title}")
         if headers:
             args.append(f"--http-header-fields={dict_to_string(headers)}")
         return args
 
 
 @dataclass
 class MPVNETPlayer(MPVPlayer):
-    executable: str = "mpvnet"
+    @staticmethod
+    def detect_executable() -> str:
+        if os_name == "nt":
+            if which("mpvnet.exe"):
+                return "mpvnet.exe"
+            if getenv("LOCALAPPDATA"):
+                mpvnet = join(
+                    getenv("LOCALAPPDATA"), "Programs", "mpv.net", "mpvnet.exe"
+                )
+                if which(mpvnet):
+                    return mpvnet
 
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
         return super().play(
-            url,
-            title,
-            full_screen,
-            headers,
-            override_executable or self.executable
+            url, title, full_screen, headers, override_executable or self.executable
         ) + ["--process-instance=multi"]
 
 
-@dataclass
 class CelluloidPlayer(MPVPlayer):
-    executable: str = "celluloid"
+    @staticmethod
+    def detect_executable() -> str:
+        if os_name == "posix":
+            if which("celluloid"):
+                return "celluloid"
 
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
         uf_args = super().play(
-            url,
-            title,
-            full_screen,
-            headers,
-            override_executable or self.executable
+            url, title, full_screen, headers, override_executable or self.executable
         )
         args = [uf_args[0], uf_args[1]]
         uf_args.pop(0)
         uf_args.pop(0)
         for arg in uf_args:
             args.append(f"--mpv-{arg.lstrip('-')}")
         return args + ["--new-window"]
```

### Comparing `gucken-0.1.2/src/gucken/player/vlc.py` & `gucken-0.1.3/src/gucken/player/vlc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-from dataclasses import dataclass
+from os import name as os_name
+from shutil import which
 
 from .common import Player
 
 
-@dataclass
 class VLCPlayer(Player):
-    executable: str = "vlc"
+
+    @staticmethod
+    def detect_executable() -> str:
+        if which("vlc"):
+            return "vlc"
+        if os_name == "nt":
+            path = r"C:\Program Files\VideoLAN\VLC\vlc.exe"
+            if which(path):
+                return path
 
     def play(
-            self,
-            url: str,
-            title: str,
-            full_screen: bool,
-            headers: dict[str, str] = None,
-            override_executable: str = None
+        self,
+        url: str,
+        title: str,
+        full_screen: bool,
+        headers: dict[str, str] = None,
+        override_executable: str = None,
     ) -> list[str]:
         args = [
             override_executable or self.executable,
             url,
             "--no-video-title-show",
             "--play-and-exit",
         ]
```

### Comparing `gucken-0.1.2/src/gucken/provider/aniworld.py` & `gucken-0.1.3/src/gucken/provider/aniworld.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,25 +39,27 @@
 
 @dataclass
 class AniWorldEpisode(Episode):
     url: str
 
     async def process_hoster(self) -> dict[Language, list[Hoster]]:
         async with AsyncClient(verify=False) as client:
-            response = await client.get(f"{self.url}/staffel-{self.season}/episode-{self.episode_number}")
+            response = await client.get(
+                f"{self.url}/staffel-{self.season}/episode-{self.episode_number}"
+            )
             soup = BeautifulSoup(response.text, "html.parser")
             watch_episode = soup.find_all(
                 "li",
                 class_=lambda value: value and value.startswith("episodeLink"),
                 attrs={
                     "data-lang-key": True,
                     "data-link-id": True,
                     "data-link-target": True,
-                    "data-external-embed": True
-                }
+                    "data-external-embed": True,
+                },
             )
             processed_hoster = {}
             for l in Language:
                 processed_hoster[l] = list()
 
             langs = soup.find("div", class_="changeLanguage").find_all("img")
             lang_map = {}
@@ -69,15 +71,17 @@
             for episode in watch_episode:
                 data_link_id = episode.attrs.get("data-link-id")
                 provider = episode.find_next("h4").text
 
                 data_lang_key = episode.attrs.get("data-lang-key")
                 lang = lang_map[data_lang_key]
 
-                hoster = provider_to_hoster(provider, f"https://{AniWorldProvider.host}/redirect/{data_link_id}")
+                hoster = provider_to_hoster(
+                    provider, f"https://{AniWorldProvider.host}/redirect/{data_link_id}"
+                )
 
                 processed_hoster[lang].append(hoster)
 
             return processed_hoster
 
 
 @dataclass
@@ -120,109 +124,135 @@
     host: str = "aniworld.to"
 
     @staticmethod
     async def search(keyword: str) -> Union[list[AniWorldSearchResult], None]:
         if keyword.strip() == "":
             return None
         async with AsyncClient(verify=False) as client:
-            response = await client.get(f"https://{AniWorldProvider.host}/ajax/seriesSearch?keyword={keyword}")
+            response = await client.get(
+                f"https://{AniWorldProvider.host}/ajax/seriesSearch?keyword={keyword}"
+            )
             results = response.json()
             search_results = []
             for series in results:
-                search_results.append(AniWorldSearchResult(
-                    name=unescape(series.get("name")).strip(),
-                    link=series.get("link"),
-                    description=unescape(series.get("description")),
-                    cover=f"https://{AniWorldProvider.host}{series.get('cover')}",
-                    production_year=series.get("productionYear"),
-                    host=AniWorldProvider.host
-                ))
+                search_results.append(
+                    AniWorldSearchResult(
+                        name=unescape(series.get("name")).strip(),
+                        link=series.get("link"),
+                        description=unescape(series.get("description")),
+                        cover=f"https://{AniWorldProvider.host}{series.get('cover')}",
+                        production_year=series.get("productionYear"),
+                        host=AniWorldProvider.host,
+                    )
+                )
             return search_results
 
     @staticmethod
     async def get_series(search_result: AniWorldSearchResult) -> AniWorldSeries:
-        async with (AsyncClient(verify=False) as client):
+        async with AsyncClient(verify=False) as client:
             response = await client.get(search_result.url)
             soup = BeautifulSoup(response.text, "html.parser")
 
             tags = []
-            for genre in soup.find_all("a", class_="genreButton clearbutton", attrs={"itemprop": "genre"}):
+            for genre in soup.find_all(
+                "a", class_="genreButton clearbutton", attrs={"itemprop": "genre"}
+            ):
                 tags.append(genre.text)
 
             actors = []
             for actor in soup.find_all("li", attrs={"itemprop": "actor"}):
                 actors.append(actor.find_next("span", attrs={"itemprop": "name"}).text)
 
             creators = []
             for creator in soup.find_all("li", attrs={"itemprop": "creator"}):
-                creators.append(creator.find_next("span", attrs={"itemprop": "name"}).text)
+                creators.append(
+                    creator.find_next("span", attrs={"itemprop": "name"}).text
+                )
 
             countrys = []
             for country in soup.find_all("li", attrs={"data-content-type": "country"}):
-                countrys.append(country.find_next("span", attrs={"itemprop": "name"}).text)
+                countrys.append(
+                    country.find_next("span", attrs={"itemprop": "name"}).text
+                )
 
             directors = []
             for director in soup.find_all("li", attrs={"itemprop": "director"}):
-                directors.append(director.find_next("span", attrs={"itemprop": "name"}).text)
+                directors.append(
+                    director.find_next("span", attrs={"itemprop": "name"}).text
+                )
 
             funcs = []
 
-            staffeln = soup.find("div", attrs={"id": "stream"}, class_="hosterSiteDirectNav").find("ul").find_all("a")
+            staffeln = (
+                soup.find("div", attrs={"id": "stream"}, class_="hosterSiteDirectNav")
+                .find("ul")
+                .find_all("a")
+            )
             count = 0
             for staffel in staffeln:
                 # TODO: Filme
                 if staffel.text != "Filme":
                     count += 1
                     if count > 1:
-                        funcs.append(
-                            get_episodes_from_url(count, search_result.url))
+                        funcs.append(get_episodes_from_url(count, search_result.url))
 
             eps = await gather(
-                get_episodes_from_soup(1, search_result.url, soup),
-                *funcs
+                get_episodes_from_soup(1, search_result.url, soup), *funcs
             )
 
             feps = []
             for e in eps:
                 for b in e:
                     feps.append(b)
 
             return AniWorldSeries(
                 # cover=f"https://{search_result.host}" + soup.find("div", class_="seriesCoverBox").find("img").attrs.get("data-src"),
-                name=unescape(soup.find("h1", attrs={"itemprop": "name"}).find("span").text).strip(),
-                production_year=unescape(soup.find("div", class_="series-title").find("small").text).strip(),
+                name=unescape(
+                    soup.find("h1", attrs={"itemprop": "name"}).find("span").text
+                ).strip(),
+                production_year=unescape(
+                    soup.find("div", class_="series-title").find("small").text
+                ).strip(),
                 # age=int(soup.find("div", class_="fsk").find("span").text),
                 # imdb_link=soup.find("a", class_="imdb-link").attrs.get("href"),
-                full_description=unescape(soup.find("p", class_="seri_des").attrs.get("data-full-description")),
+                full_description=unescape(
+                    soup.find("p", class_="seri_des").attrs.get("data-full-description")
+                ),
                 regisseure=directors,
                 schauspieler=actors,
                 produzent=creators,
                 land=countrys,
                 tags=tags,
                 # rating_value=int(soup.find("span", attrs={"itemprop": "ratingValue"}).text),
                 # rating_count=int(soup.find("span", attrs={"itemprop": "ratingCount"}).text),
                 # staffeln=count,
-                episodes=feps
+                episodes=feps,
             )
 
 
 async def get_episodes_from_url(staffel: int, url: str) -> list[Episode]:
     async with AsyncClient(verify=False) as client:
         response = await client.get(f"{url}/staffel-{staffel}")
         return await get_episodes_from_page(staffel, url, response.text)
 
 
 async def get_episodes_from_page(staffel: int, url: str, page: str) -> list[Episode]:
-    return await get_episodes_from_soup(staffel, url, BeautifulSoup(page, "html.parser"))
+    return await get_episodes_from_soup(
+        staffel, url, BeautifulSoup(page, "html.parser")
+    )
 
 
-async def get_episodes_from_soup(staffel: int, url: str, soup: BeautifulSoup) -> list[Episode]:
+async def get_episodes_from_soup(
+    staffel: int, url: str, soup: BeautifulSoup
+) -> list[Episode]:
     episodes = []
     e_count = 0
-    for episode in soup.find("table", class_="seasonEpisodesList").find("tbody").find_all("tr"):
+    for episode in (
+        soup.find("table", class_="seasonEpisodesList").find("tbody").find_all("tr")
+    ):
         title = episode.find_next("td", class_="seasonEpisodeTitle")
 
         language = set()
         for flag in episode.find_next("td", class_="editFunctions").find_all("img"):
             lang_name = flag.attrs.get("src").split("/")[-1].rsplit(".", 1)[0]
             language.add(lang_img_src_lang_name_to_lang(lang_name))
 
@@ -237,23 +267,29 @@
                 hoster.add(VidozaHoster)
             if t == "Streamtape":
                 hoster.add(StreamtapeHoster)
 
         e_count += 1
         title_en = title.find("span").text.strip()
         title_de = title.find("strong").text.strip()
-        title = f"{title_en} - {title_de}" if title_en and title_de else title_en or title_de
-        episodes.append(AniWorldEpisode(
-            url=url,
-            title=title,
-            season=staffel,
-            episode_number=e_count,
-            available_hoster=hoster,
-            available_language=language,
-            total_episode_number=None
-            # language=language,
-            # hoster=hoster,
-            # number=e_count,
-            # staffel=staffel
-        ))
+        title = (
+            f"{title_en} - {title_de}"
+            if title_en and title_de
+            else title_en or title_de
+        )
+        episodes.append(
+            AniWorldEpisode(
+                url=url,
+                title=title,
+                season=staffel,
+                episode_number=e_count,
+                available_hoster=hoster,
+                available_language=language,
+                total_episode_number=None,
+                # language=language,
+                # hoster=hoster,
+                # number=e_count,
+                # staffel=staffel
+            )
+        )
 
     return episodes
```

### Comparing `gucken-0.1.2/src/gucken/provider/common.py` & `gucken-0.1.3/src/gucken/provider/common.py`

 * *Files identical despite different names*

### Comparing `gucken-0.1.2/src/gucken/provider/serienstream.py` & `gucken-0.1.3/src/gucken/provider/serienstream.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,25 +39,27 @@
 
 @dataclass
 class SerienStreamEpisode(Episode):
     url: str
 
     async def process_hoster(self) -> dict[Language, list[Hoster]]:
         async with AsyncClient(verify=False) as client:
-            response = await client.get(f"{self.url}/staffel-{self.season}/episode-{self.episode_number}")
+            response = await client.get(
+                f"{self.url}/staffel-{self.season}/episode-{self.episode_number}"
+            )
             soup = BeautifulSoup(response.text, "html.parser")
             watch_episode = soup.find_all(
                 "li",
                 class_=lambda value: value and value.startswith("episodeLink"),
                 attrs={
                     "data-lang-key": True,
                     "data-link-id": True,
                     "data-link-target": True,
-                    "data-external-embed": True
-                }
+                    "data-external-embed": True,
+                },
             )
             processed_hoster = {}
             for l in Language:
                 processed_hoster[l] = list()
 
             langs = soup.find("div", class_="changeLanguage").find_all("img")
             lang_map = {}
@@ -69,15 +71,18 @@
             for episode in watch_episode:
                 data_link_id = episode.attrs.get("data-link-id")
                 provider = episode.find_next("h4").text
 
                 data_lang_key = episode.attrs.get("data-lang-key")
                 lang = lang_map[data_lang_key]
 
-                hoster = provider_to_hoster(provider, f"https://{SerienStreamProvider.host}/redirect/{data_link_id}")
+                hoster = provider_to_hoster(
+                    provider,
+                    f"https://{SerienStreamProvider.host}/redirect/{data_link_id}",
+                )
 
                 processed_hoster[lang].append(hoster)
 
             return processed_hoster
 
 
 @dataclass
@@ -120,109 +125,135 @@
     host: str = "186.2.175.5"
 
     @staticmethod
     async def search(keyword: str) -> Union[list[SerienStreamSearchResult], None]:
         if keyword.strip() == "":
             return None
         async with AsyncClient(verify=False) as client:
-            response = await client.get(f"https://{SerienStreamProvider.host}/ajax/seriesSearch?keyword={keyword}")
+            response = await client.get(
+                f"https://{SerienStreamProvider.host}/ajax/seriesSearch?keyword={keyword}"
+            )
             results = response.json()
             search_results = []
             for series in results:
-                search_results.append(SerienStreamSearchResult(
-                    name=unescape(series.get("name")).strip(),
-                    link=series.get("link"),
-                    description=unescape(series.get("description")),
-                    cover=f"https://s.to{series.get('cover')}",
-                    production_year=series.get("productionYear"),
-                    host=SerienStreamProvider.host
-                ))
+                search_results.append(
+                    SerienStreamSearchResult(
+                        name=unescape(series.get("name")).strip(),
+                        link=series.get("link"),
+                        description=unescape(series.get("description")),
+                        cover=f"https://s.to{series.get('cover')}",
+                        production_year=series.get("productionYear"),
+                        host=SerienStreamProvider.host,
+                    )
+                )
             return search_results
 
     @staticmethod
     async def get_series(search_result: SerienStreamSearchResult) -> SerienStreamSeries:
-        async with (AsyncClient(verify=False) as client):
+        async with AsyncClient(verify=False) as client:
             response = await client.get(search_result.url)
             soup = BeautifulSoup(response.text, "html.parser")
 
             tags = []
-            for genre in soup.find_all("a", class_="genreButton clearbutton", attrs={"itemprop": "genre"}):
+            for genre in soup.find_all(
+                "a", class_="genreButton clearbutton", attrs={"itemprop": "genre"}
+            ):
                 tags.append(genre.text)
 
             actors = []
             for actor in soup.find_all("li", attrs={"itemprop": "actor"}):
                 actors.append(actor.find_next("span", attrs={"itemprop": "name"}).text)
 
             creators = []
             for creator in soup.find_all("li", attrs={"itemprop": "creator"}):
-                creators.append(creator.find_next("span", attrs={"itemprop": "name"}).text)
+                creators.append(
+                    creator.find_next("span", attrs={"itemprop": "name"}).text
+                )
 
             countrys = []
             for country in soup.find_all("li", attrs={"data-content-type": "country"}):
-                countrys.append(country.find_next("span", attrs={"itemprop": "name"}).text)
+                countrys.append(
+                    country.find_next("span", attrs={"itemprop": "name"}).text
+                )
 
             directors = []
             for director in soup.find_all("li", attrs={"itemprop": "director"}):
-                directors.append(director.find_next("span", attrs={"itemprop": "name"}).text)
+                directors.append(
+                    director.find_next("span", attrs={"itemprop": "name"}).text
+                )
 
             funcs = []
 
-            staffeln = soup.find("div", attrs={"id": "stream"}, class_="hosterSiteDirectNav").find("ul").find_all("a")
+            staffeln = (
+                soup.find("div", attrs={"id": "stream"}, class_="hosterSiteDirectNav")
+                .find("ul")
+                .find_all("a")
+            )
             count = 0
             for staffel in staffeln:
                 # TODO: Filme
                 if staffel.text != "Filme":
                     count += 1
                     if count > 1:
-                        funcs.append(
-                            get_episodes_from_url(count, search_result.url))
+                        funcs.append(get_episodes_from_url(count, search_result.url))
 
             eps = await gather(
-                get_episodes_from_soup(1, search_result.url, soup),
-                *funcs
+                get_episodes_from_soup(1, search_result.url, soup), *funcs
             )
 
             feps = []
             for e in eps:
                 for b in e:
                     feps.append(b)
 
             return SerienStreamSeries(
                 # cover=f"https://{search_result.host}" + soup.find("div", class_="seriesCoverBox").find("img").attrs.get("data-src"),
-                name=unescape(soup.find("h1", attrs={"itemprop": "name"}).find("span").text).strip(),
-                production_year=unescape(soup.find("div", class_="series-title").find("small").text).strip(),
+                name=unescape(
+                    soup.find("h1", attrs={"itemprop": "name"}).find("span").text
+                ).strip(),
+                production_year=unescape(
+                    soup.find("div", class_="series-title").find("small").text
+                ).strip(),
                 # age=int(soup.find("div", class_="fsk").find("span").text),
                 # imdb_link=soup.find("a", class_="imdb-link").attrs.get("href"),
-                full_description=unescape(soup.find("p", class_="seri_des").attrs.get("data-full-description")),
+                full_description=unescape(
+                    soup.find("p", class_="seri_des").attrs.get("data-full-description")
+                ),
                 regisseure=directors,
                 schauspieler=actors,
                 produzent=creators,
                 land=countrys,
                 tags=tags,
                 # rating_value=int(soup.find("span", attrs={"itemprop": "ratingValue"}).text),
                 # rating_count=int(soup.find("span", attrs={"itemprop": "ratingCount"}).text),
                 # staffeln=count,
-                episodes=feps
+                episodes=feps,
             )
 
 
 async def get_episodes_from_url(staffel: int, url: str) -> list[Episode]:
     async with AsyncClient(verify=False) as client:
         response = await client.get(f"{url}/staffel-{staffel}")
         return await get_episodes_from_page(staffel, url, response.text)
 
 
 async def get_episodes_from_page(staffel: int, url: str, page: str) -> list[Episode]:
-    return await get_episodes_from_soup(staffel, url, BeautifulSoup(page, "html.parser"))
+    return await get_episodes_from_soup(
+        staffel, url, BeautifulSoup(page, "html.parser")
+    )
 
 
-async def get_episodes_from_soup(staffel: int, url: str, soup: BeautifulSoup) -> list[Episode]:
+async def get_episodes_from_soup(
+    staffel: int, url: str, soup: BeautifulSoup
+) -> list[Episode]:
     episodes = []
     e_count = 0
-    for episode in soup.find("table", class_="seasonEpisodesList").find("tbody").find_all("tr"):
+    for episode in (
+        soup.find("table", class_="seasonEpisodesList").find("tbody").find_all("tr")
+    ):
         title = episode.find_next("td", class_="seasonEpisodeTitle")
 
         language = set()
         for flag in episode.find_next("td", class_="editFunctions").find_all("img"):
             lang_name = flag.attrs.get("src").split("/")[-1].rsplit(".", 1)[0]
             language.add(lang_img_src_lang_name_to_lang(lang_name))
 
@@ -237,23 +268,29 @@
                 hoster.add(VidozaHoster)
             if t == "Streamtape":
                 hoster.add(StreamtapeHoster)
 
         e_count += 1
         title_en = title.find("span").text.strip()
         title_de = title.find("strong").text.strip()
-        title = f"{title_en} - {title_de}" if title_en and title_de else title_en or title_de
-        episodes.append(SerienStreamEpisode(
-            url=url,
-            title=title,
-            season=staffel,
-            episode_number=e_count,
-            available_hoster=hoster,
-            available_language=language,
-            total_episode_number=None
-            #language=language,
-            #hoster=hoster,
-            #number=e_count,
-            #staffel=staffel
-        ))
+        title = (
+            f"{title_en} - {title_de}"
+            if title_en and title_de
+            else title_en or title_de
+        )
+        episodes.append(
+            SerienStreamEpisode(
+                url=url,
+                title=title,
+                season=staffel,
+                episode_number=e_count,
+                available_hoster=hoster,
+                available_language=language,
+                total_episode_number=None,
+                # language=language,
+                # hoster=hoster,
+                # number=e_count,
+                # staffel=staffel
+            )
+        )
 
     return episodes
```

### Comparing `gucken-0.1.2/src/gucken/tracker/anilist.py` & `gucken-0.1.3/src/gucken/tracker/anilist.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 
 
 async def search(keyword: str) -> dict:
     async with AsyncClient(verify=False) as client:
         response = await client.post(
             f"https://graphql.anilist.co",
             headers={"Content-Type": "application/json"},
-            json={"query": SEARCH_QUERY, "variables": {"search": keyword}}
+            json={"query": SEARCH_QUERY, "variables": {"search": keyword}},
         )
         return response.json()
```

### Comparing `gucken-0.1.2/LICENSE.txt` & `gucken-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gucken-0.1.2/README.md` & `gucken-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,23 +80,23 @@
 
 </details>
 
 ## Features
 
 - [x] Update checker
 - [x] Language priority list
-- [ ] Hoster priority list
+- [x] Hoster priority list
 - [x] Automatically use working hoster
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
   - [x] Discord Presence **WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP** (need skip plugin)
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
     - [x] [Syncplay](https://github.com/Syncplay/syncplay) support (almost out of WIP)
     - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
@@ -194,57 +194,51 @@
 - [ ] Custom player
 - [ ] Colors themes
 - [ ] Installation helper
   - [ ] [MPV]
     - [ ] [Anime4k]
   - [ ] [VLC]
 - [ ] Create shortcut Windows & Linux
-- [ ] CLI args
 - [ ] CI Testing (Windows, Linux)
 - [ ] CD pip
 - [ ] [Anime4k] options
 - [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
 - [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
 - [ ] Image preview (Kitty protocol, iterm protocol, Sixel, textual-web)
 - [ ] Support textual-web
 - [ ] Blacklist detection & bypass
-- [ ] Syncplay on Android
 - [ ] Mac support
 - [ ] IOS support
-- [ ] Option to disable update checker
 - [ ] Update checker option to perform update
 - [ ] Snap support ?
 - [ ] 404 detection inside Hoster and don't crash whole program on http error + crash reports/logs
 - [ ] s.to, aniworld.to scrape episode description
 - [ ] search in episodes
 - [ ] Focus window when ask next
 - [ ] next and cancel hotkeys
 - [ ] show hotkeys in Footer
-- [ ] ani-skip load skip plugin from src
-- [ ] ani-skip only to get chapters
 - [ ] Window in settings menu to show where files are located (data, logs, config, downloads)
 - [ ] Utilize next and previous buttons in mpv
 - [ ] Nix
 - [ ] Docker
 - [ ] Flatpack ?
 - [ ] Merge anime's from SerienStream.to to AniWorld.to to get more langs
-- [ ] Fix title
 - [ ] Do unescape and stripe only on render
 - [ ] Dont coppy code from SerienStream.to to AniWorld.to
-- [ ] FIX TYPING SOMETIMES CAUSES CRASH
-- [ ] option to disable debug logging
 - [ ] BIG CODE CLEANUP
-- [ ] Player selection
-- [ ] Hoster prio list
 - [ ] Translation
 - [ ] detect existing chapters and use them for skip
+- [ ] Better settings design
+- [ ] FIX TYPING SOMETIMES CAUSES CRASH
+- [ ] Syncplay on Android
+- [ ] More CLI args
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
 [Python]: https://www.python.org/downloads/
```

### Comparing `gucken-0.1.2/pyproject.toml` & `gucken-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gucken-0.1.2/PKG-INFO` & `gucken-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gucken
-Version: 0.1.2
+Version: 0.1.3
 Summary: Gucken is a Terminal User Interface which allows you to browse and watch your favorite anime's with style.
 Project-URL: Repository, https://github.com/Commandcracker/gucken
 Author: Commandcracker
 Maintainer: Commandcracker
 License: MIT License
         
         Copyright (c) 2024 Commandcracker
@@ -135,23 +135,23 @@
 
 </details>
 
 ## Features
 
 - [x] Update checker
 - [x] Language priority list
-- [ ] Hoster priority list
+- [x] Hoster priority list
 - [x] Automatically use working hoster
 - [x] Browsing
   - [x] Descriptions
 - [x] Watching
   - [x] Automatically start next episode
   - [x] Discord Presence **WIP**
   - [MPV] only
-    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP** (need skip plugin)
+    - [X] [ani-skip](https://github.com/synacktraa/ani-skip) support **Very WIP**
     - [x] [Syncplay](https://github.com/Syncplay/syncplay) support (almost out of WIP)
     - [ ] Remember watch time **WIP**
     - [ ] Remember completed Episodes (and series)
   - [ ] Tracker support
     - [ ] [MyAnimeList](https://myanimelist.net/)
     - [ ] [AniList](https://anilist.co/)
     - [ ] [AniWorld.to] & [SerienStream.to]
@@ -249,57 +249,51 @@
 - [ ] Custom player
 - [ ] Colors themes
 - [ ] Installation helper
   - [ ] [MPV]
     - [ ] [Anime4k]
   - [ ] [VLC]
 - [ ] Create shortcut Windows & Linux
-- [ ] CLI args
 - [ ] CI Testing (Windows, Linux)
 - [ ] CD pip
 - [ ] [Anime4k] options
 - [ ] Modular (Custom extractors/players, API)
 - [ ] Proper error handling
 - [ ] Logging and Crash reports
 - [ ] Pre-fetching
 - [ ] improve [ani-skip](https://github.com/synacktraa/ani-skip) support
 - [ ] Use something like opencv to time match a sub from aniworld with a high quality video form another site.
 - [ ] Image preview (Kitty protocol, iterm protocol, Sixel, textual-web)
 - [ ] Support textual-web
 - [ ] Blacklist detection & bypass
-- [ ] Syncplay on Android
 - [ ] Mac support
 - [ ] IOS support
-- [ ] Option to disable update checker
 - [ ] Update checker option to perform update
 - [ ] Snap support ?
 - [ ] 404 detection inside Hoster and don't crash whole program on http error + crash reports/logs
 - [ ] s.to, aniworld.to scrape episode description
 - [ ] search in episodes
 - [ ] Focus window when ask next
 - [ ] next and cancel hotkeys
 - [ ] show hotkeys in Footer
-- [ ] ani-skip load skip plugin from src
-- [ ] ani-skip only to get chapters
 - [ ] Window in settings menu to show where files are located (data, logs, config, downloads)
 - [ ] Utilize next and previous buttons in mpv
 - [ ] Nix
 - [ ] Docker
 - [ ] Flatpack ?
 - [ ] Merge anime's from SerienStream.to to AniWorld.to to get more langs
-- [ ] Fix title
 - [ ] Do unescape and stripe only on render
 - [ ] Dont coppy code from SerienStream.to to AniWorld.to
-- [ ] FIX TYPING SOMETIMES CAUSES CRASH
-- [ ] option to disable debug logging
 - [ ] BIG CODE CLEANUP
-- [ ] Player selection
-- [ ] Hoster prio list
 - [ ] Translation
 - [ ] detect existing chapters and use them for skip
+- [ ] Better settings design
+- [ ] FIX TYPING SOMETIMES CAUSES CRASH
+- [ ] Syncplay on Android
+- [ ] More CLI args
 
 [Anime4k]: https://github.com/bloc97/Anime4K
 [MPV]: https://mpv.io/
 [VLC]: https://www.videolan.org/vlc/
 [AniWorld.to]: https://aniworld.to
 [SerienStream.to]: https://186.2.175.5
 [Python]: https://www.python.org/downloads/
```

