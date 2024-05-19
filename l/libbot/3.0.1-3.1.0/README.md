# Comparing `tmp/libbot-3.0.1.tar.gz` & `tmp/libbot-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbot-3.0.1.tar", last modified: Tue May 14 21:21:33 2024, max compression
+gzip compressed data, was "libbot-3.1.0.tar", last modified: Sun May 19 13:03:13 2024, max compression
```

## Comparing `libbot-3.0.1.tar` & `libbot-3.1.0.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.682850 libbot-3.0.1/
--rw-rw-rw-   0        0        0    34902 2024-04-22 21:47:22.000000 libbot-3.0.1/LICENSE
--rw-rw-rw-   0        0        0    38732 2024-05-14 21:21:33.681852 libbot-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-22 21:47:22.000000 libbot-3.0.1/README.md
--rw-rw-rw-   0        0        0     1974 2024-04-22 21:47:22.000000 libbot-3.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.619318 libbot-3.0.1/requirements/
--rw-rw-rw-   0        0        0       16 2024-04-22 21:47:22.000000 libbot-3.0.1/requirements/_.txt
--rw-rw-rw-   0        0        0      197 2024-05-14 21:19:20.000000 libbot-3.0.1/requirements/dev.txt
--rw-rw-rw-   0        0        0       35 2024-05-14 21:19:20.000000 libbot-3.0.1/requirements/pycord.txt
--rw-rw-rw-   0        0        0       43 2024-05-14 21:19:20.000000 libbot-3.0.1/requirements/pyrogram.txt
--rw-rw-rw-   0        0        0       13 2024-05-14 21:19:20.000000 libbot-3.0.1/requirements/speed.txt
--rw-rw-rw-   0        0        0       42 2024-05-14 21:21:33.683855 libbot-3.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.599319 libbot-3.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.621320 libbot-3.0.1/src/libbot/
--rw-rw-rw-   0        0        0      143 2024-05-14 21:19:20.000000 libbot-3.0.1/src/libbot/__init__.py
--rw-rw-rw-   0        0        0     2962 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.648320 libbot-3.0.1/src/libbot/i18n/
--rw-rw-rw-   0        0        0     3880 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.650315 libbot-3.0.1/src/libbot/i18n/classes/
--rw-rw-rw-   0        0        0     3980 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/i18n/classes/bot_locale.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.651316 libbot-3.0.1/src/libbot/i18n/sync/
--rw-rw-rw-   0        0        0     3771 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/i18n/sync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.602315 libbot-3.0.1/src/libbot/pycord/
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.653320 libbot-3.0.1/src/libbot/pycord/classes/
--rw-rw-rw-   0        0        0       28 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/pycord/classes/__init__.py
--rw-rw-rw-   0        0        0     1865 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/pycord/classes/bot.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.603319 libbot-3.0.1/src/libbot/pyrogram/
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.660326 libbot-3.0.1/src/libbot/pyrogram/classes/
--rw-rw-rw-   0        0        0      102 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/pyrogram/classes/__init__.py
--rw-rw-rw-   0        0        0    15428 2024-05-14 21:19:20.000000 libbot-3.0.1/src/libbot/pyrogram/classes/client.py
--rw-rw-rw-   0        0        0      176 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/pyrogram/classes/command.py
--rw-rw-rw-   0        0        0     1033 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/pyrogram/classes/commandset.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.661327 libbot-3.0.1/src/libbot/sync/
--rw-rw-rw-   0        0        0     3697 2024-04-22 21:47:22.000000 libbot-3.0.1/src/libbot/sync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.675850 libbot-3.0.1/src/libbot.egg-info/
--rw-rw-rw-   0        0        0    38732 2024-05-14 21:21:33.000000 libbot-3.0.1/src/libbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2024-05-14 21:21:33.000000 libbot-3.0.1/src/libbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 21:21:33.000000 libbot-3.0.1/src/libbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      335 2024-05-14 21:21:33.000000 libbot-3.0.1/src/libbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 21:21:33.000000 libbot-3.0.1/src/libbot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 21:21:33.673855 libbot-3.0.1/tests/
--rw-rw-rw-   0        0        0     1673 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_bot_locale.py
--rw-rw-rw-   0        0        0     1289 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_config_async.py
--rw-rw-rw-   0        0        0     1162 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_config_sync.py
--rw-rw-rw-   0        0        0     1893 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_i18n_async.py
--rw-rw-rw-   0        0        0     1758 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_i18n_sync.py
--rw-rw-rw-   0        0        0     1642 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_json_async.py
--rw-rw-rw-   0        0        0     1557 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_json_sync.py
--rw-rw-rw-   0        0        0     1511 2024-04-22 21:47:22.000000 libbot-3.0.1/tests/test_nested_set.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.899559 libbot-3.1.0/
+-rw-rw-rw-   0        0        0    34902 2024-04-22 21:47:22.000000 libbot-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4501 2024-05-19 13:03:13.898557 libbot-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2509 2024-05-19 12:46:00.000000 libbot-3.1.0/README.md
+-rw-rw-rw-   0        0        0     1998 2024-05-19 12:46:23.000000 libbot-3.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.854519 libbot-3.1.0/requirements/
+-rw-rw-rw-   0        0        0       16 2024-04-22 21:47:22.000000 libbot-3.1.0/requirements/_.txt
+-rw-rw-rw-   0        0        0      205 2024-05-19 12:48:35.000000 libbot-3.1.0/requirements/dev.txt
+-rw-rw-rw-   0        0        0       35 2024-05-14 21:19:20.000000 libbot-3.1.0/requirements/pycord.txt
+-rw-rw-rw-   0        0        0       43 2024-05-14 21:19:20.000000 libbot-3.1.0/requirements/pyrogram.txt
+-rw-rw-rw-   0        0        0       13 2024-05-14 21:19:20.000000 libbot-3.1.0/requirements/speed.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 13:03:13.900559 libbot-3.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.837184 libbot-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.857792 libbot-3.1.0/src/libbot/
+-rw-rw-rw-   0        0        0      151 2024-05-19 11:59:16.000000 libbot-3.1.0/src/libbot/__init__.py
+-rw-rw-rw-   0        0        0     2962 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.867004 libbot-3.1.0/src/libbot/errors/
+-rw-rw-rw-   0        0        0       54 2024-05-19 11:56:28.000000 libbot-3.1.0/src/libbot/errors/__init__.py
+-rw-rw-rw-   0        0        0     1508 2024-05-19 11:55:52.000000 libbot-3.1.0/src/libbot/errors/config.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.869008 libbot-3.1.0/src/libbot/i18n/
+-rw-rw-rw-   0        0        0     3880 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.871010 libbot-3.1.0/src/libbot/i18n/classes/
+-rw-rw-rw-   0        0        0     3980 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/i18n/classes/bot_locale.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.872007 libbot-3.1.0/src/libbot/i18n/sync/
+-rw-rw-rw-   0        0        0     3771 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/i18n/sync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.841514 libbot-3.1.0/src/libbot/pycord/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.874003 libbot-3.1.0/src/libbot/pycord/classes/
+-rw-rw-rw-   0        0        0       28 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pycord/classes/__init__.py
+-rw-rw-rw-   0        0        0     1985 2024-05-19 13:01:47.000000 libbot-3.1.0/src/libbot/pycord/classes/bot.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.842038 libbot-3.1.0/src/libbot/pyrogram/
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.880529 libbot-3.1.0/src/libbot/pyrogram/classes/
+-rw-rw-rw-   0        0        0      102 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pyrogram/classes/__init__.py
+-rw-rw-rw-   0        0        0    15428 2024-05-14 21:19:20.000000 libbot-3.1.0/src/libbot/pyrogram/classes/client.py
+-rw-rw-rw-   0        0        0      176 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pyrogram/classes/command.py
+-rw-rw-rw-   0        0        0     1033 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/pyrogram/classes/commandset.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.881533 libbot-3.1.0/src/libbot/sync/
+-rw-rw-rw-   0        0        0     3697 2024-04-22 21:47:22.000000 libbot-3.1.0/src/libbot/sync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.894044 libbot-3.1.0/src/libbot.egg-info/
+-rw-rw-rw-   0        0        0     4501 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      343 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 13:03:13.000000 libbot-3.1.0/src/libbot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 13:03:13.893046 libbot-3.1.0/tests/
+-rw-rw-rw-   0        0        0     1673 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_bot_locale.py
+-rw-rw-rw-   0        0        0     1289 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_config_async.py
+-rw-rw-rw-   0        0        0     1162 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_config_sync.py
+-rw-rw-rw-   0        0        0     1893 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_i18n_async.py
+-rw-rw-rw-   0        0        0     1758 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_i18n_sync.py
+-rw-rw-rw-   0        0        0     1642 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_json_async.py
+-rw-rw-rw-   0        0        0     1557 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_json_sync.py
+-rw-rw-rw-   0        0        0     1511 2024-04-22 21:47:22.000000 libbot-3.1.0/tests/test_nested_set.py
```

### Comparing `libbot-3.0.1/LICENSE` & `libbot-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/pyproject.toml` & `libbot-3.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 [project]
 name = "libbot"
 dynamic = ["version", "dependencies", "optional-dependencies"]
 authors = [{ name = "Profitroll" }]
 description = "Universal bot library with functions needed for basic Discord/Telegram bot development."
 readme = "README.md"
 requires-python = ">=3.8"
-license = { file = "LICENSE" }
+license = { text = "GPLv3" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
```

### Comparing `libbot-3.0.1/src/libbot/__main__.py` & `libbot-3.1.0/src/libbot/__main__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot/i18n/__init__.py` & `libbot-3.1.0/src/libbot/i18n/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot/i18n/classes/bot_locale.py` & `libbot-3.1.0/src/libbot/i18n/classes/bot_locale.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot/i18n/sync/__init__.py` & `libbot-3.1.0/src/libbot/i18n/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot/pycord/classes/bot.py` & `libbot-3.1.0/src/libbot/pycord/classes/bot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Any, Dict, Union
+from typing import Any, Dict, List, Union
 
 try:
     from apscheduler.schedulers.asyncio import AsyncIOScheduler
     from apscheduler.schedulers.background import BackgroundScheduler
     from discord import Bot
 except ImportError as exc:
     raise ImportError(
@@ -25,33 +25,37 @@
 class PycordBot(Bot):
     def __init__(
         self,
         config: Union[Dict[str, Any], None] = None,
         config_path: Union[str, Path] = Path("config.json"),
         locales_root: Union[str, Path, None] = None,
         scheduler: Union[AsyncIOScheduler, BackgroundScheduler, None] = None,
+        *args,
         **kwargs,
     ):
         if config is None:
             with open(config_path, "r", encoding="utf-8") as f:
                 self.config: dict = loads(f.read())
         else:
             self.config = config
 
         super().__init__(
-            debug_guilds=self.config["bot"]["debug_guilds"],
+            debug_guilds=(
+                self.config["bot"]["debug_guilds"] if self.config["debug"] else None
+            ),
             owner_ids=self.config["bot"]["owners"],
+            *args,
             **kwargs,
         )
 
         self.bot_locale: BotLocale = BotLocale(
             default_locale=self.config["locale"],
             locales_root=(Path("locale") if locales_root is None else locales_root),
         )
         self.default_locale: str = self.bot_locale.default
-        self.locales: dict = self.bot_locale.locales
+        self.locales: Dict[str, Any] = self.bot_locale.locales
 
         self._ = self.bot_locale._
         self.in_all_locales = self.bot_locale.in_all_locales
         self.in_every_locale = self.bot_locale.in_every_locale
 
         self.scheduler: Union[AsyncIOScheduler, BackgroundScheduler, None] = scheduler
```

### Comparing `libbot-3.0.1/src/libbot/pyrogram/classes/client.py` & `libbot-3.1.0/src/libbot/pyrogram/classes/client.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot/pyrogram/classes/commandset.py` & `libbot-3.1.0/src/libbot/pyrogram/classes/commandset.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot/sync/__init__.py` & `libbot-3.1.0/src/libbot/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/src/libbot.egg-info/SOURCES.txt` & `libbot-3.1.0/src/libbot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 src/libbot/__init__.py
 src/libbot/__main__.py
 src/libbot.egg-info/PKG-INFO
 src/libbot.egg-info/SOURCES.txt
 src/libbot.egg-info/dependency_links.txt
 src/libbot.egg-info/requires.txt
 src/libbot.egg-info/top_level.txt
+src/libbot/errors/__init__.py
+src/libbot/errors/config.py
 src/libbot/i18n/__init__.py
 src/libbot/i18n/classes/bot_locale.py
 src/libbot/i18n/sync/__init__.py
 src/libbot/pycord/classes/__init__.py
 src/libbot/pycord/classes/bot.py
 src/libbot/pyrogram/classes/__init__.py
 src/libbot/pyrogram/classes/client.py
```

### Comparing `libbot-3.0.1/tests/test_bot_locale.py` & `libbot-3.1.0/tests/test_bot_locale.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_config_async.py` & `libbot-3.1.0/tests/test_config_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_config_sync.py` & `libbot-3.1.0/tests/test_config_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_i18n_async.py` & `libbot-3.1.0/tests/test_i18n_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_i18n_sync.py` & `libbot-3.1.0/tests/test_i18n_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_json_async.py` & `libbot-3.1.0/tests/test_json_async.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_json_sync.py` & `libbot-3.1.0/tests/test_json_sync.py`

 * *Files identical despite different names*

### Comparing `libbot-3.0.1/tests/test_nested_set.py` & `libbot-3.1.0/tests/test_nested_set.py`

 * *Files identical despite different names*

