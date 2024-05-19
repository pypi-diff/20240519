# Comparing `tmp/anipy_api-3.0.4.tar.gz` & `tmp/anipy_api-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.0.4.tar", max compression
+gzip compressed data, was "anipy_api-3.0.5.tar", max compression
```

## Comparing `anipy_api-3.0.4.tar` & `anipy_api-3.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      227 2024-05-16 14:00:40.760930 anipy_api-3.0.4/README.md
--rw-r--r--   0        0        0      847 2024-05-16 14:00:40.760930 anipy_api-3.0.4/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5417 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11550 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/error.py
--rw-r--r--   0        0        0     7953 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-16 14:00:40.760930 anipy_api-3.0.4/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2651 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0       96 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12230 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     1482 2024-05-16 14:00:40.764930 anipy_api-3.0.4/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-19 09:41:00.160333 anipy_api-3.0.5/README.md
+-rw-r--r--   0        0        0      847 2024-05-19 09:41:00.160333 anipy_api-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5417 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11550 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/error.py
+-rw-r--r--   0        0        0     7953 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2651 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0       96 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12230 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     1482 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.0.5/PKG-INFO
```

### Comparing `anipy_api-3.0.4/pyproject.toml` & `anipy_api-3.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.0.4"
+version = "3.0.5"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
```

### Comparing `anipy_api-3.0.4/src/anipy_api/anime.py` & `anipy_api-3.0.5/src/anipy_api/anime.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/download.py` & `anipy_api-3.0.5/src/anipy_api/download.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/error.py` & `anipy_api-3.0.5/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/locallist.py` & `anipy_api-3.0.5/src/anipy_api/locallist.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/mal.py` & `anipy_api-3.0.5/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/player/base.py` & `anipy_api-3.0.5/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/player/player.py` & `anipy_api-3.0.5/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/player/players/mpv.py` & `anipy_api-3.0.5/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.0.5/src/anipy_api/player/players/mpv_control.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.0.5/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/player/players/vlc.py` & `anipy_api-3.0.5/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/provider/__init__.py` & `anipy_api-3.0.5/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/provider/base.py` & `anipy_api-3.0.5/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/provider/filter.py` & `anipy_api-3.0.5/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/provider/provider.py` & `anipy_api-3.0.5/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.0.5/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/src/anipy_api/provider/utils.py` & `anipy_api-3.0.5/src/anipy_api/provider/utils.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.4/PKG-INFO` & `anipy_api-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.0.4
+Version: 3.0.5
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

