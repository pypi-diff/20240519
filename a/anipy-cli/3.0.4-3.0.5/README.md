# Comparing `tmp/anipy_cli-3.0.4.tar.gz` & `tmp/anipy_cli-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_cli-3.0.4.tar", max compression
+gzip compressed data, was "anipy_cli-3.0.5.tar", max compression
```

## Comparing `anipy_cli-3.0.4.tar` & `anipy_cli-3.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1974 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/README.md
--rw-r--r--   0        0        0      855 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/__init__.py
--rw-r--r--   0        0        0     5299 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/arg_parser.py
--rw-r--r--   0        0        0     1922 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/cli.py
--rw-r--r--   0        0        0      411 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/__init__.py
--rw-r--r--   0        0        0      609 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/base_cli.py
--rw-r--r--   0        0        0     2281 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/binge_cli.py
--rw-r--r--   0        0        0     2815 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/default_cli.py
--rw-r--r--   0        0        0     3197 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/download_cli.py
--rw-r--r--   0        0        0     2675 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/history_cli.py
--rw-r--r--   0        0        0     2258 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/mal_cli.py
--rw-r--r--   0        0        0      616 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/clis/seasonal_cli.py
--rw-r--r--   0        0        0      916 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/colors.py
--rw-r--r--   0        0        0    15404 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/config.py
--rw-r--r--   0        0        0     1160 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/discord.py
--rw-r--r--   0        0        0     6981 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/mal_proxy.py
--rw-r--r--   0        0        0      185 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/__init__.py
--rw-r--r--   0        0        0     1140 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/base_menu.py
--rw-r--r--   0        0        0    24077 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/mal_menu.py
--rw-r--r--   0        0        0     6179 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/menu.py
--rw-r--r--   0        0        0     9097 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/menus/seasonal_menu.py
--rw-r--r--   0        0        0     7119 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/prompts.py
--rw-r--r--   0        0        0     7684 2024-05-16 14:00:40.764930 anipy_cli-3.0.4/src/anipy_cli/util.py
--rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 anipy_cli-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1974 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/README.md
+-rw-r--r--   0        0        0      855 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/src/anipy_cli/__init__.py
+-rw-r--r--   0        0        0     5299 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/src/anipy_cli/arg_parser.py
+-rw-r--r--   0        0        0     1922 2024-05-19 09:41:00.160333 anipy_cli-3.0.5/src/anipy_cli/cli.py
+-rw-r--r--   0        0        0      411 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/__init__.py
+-rw-r--r--   0        0        0      609 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/base_cli.py
+-rw-r--r--   0        0        0     2281 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/binge_cli.py
+-rw-r--r--   0        0        0     2815 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/default_cli.py
+-rw-r--r--   0        0        0     3197 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/download_cli.py
+-rw-r--r--   0        0        0     2675 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/history_cli.py
+-rw-r--r--   0        0        0     2258 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/mal_cli.py
+-rw-r--r--   0        0        0      616 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/clis/seasonal_cli.py
+-rw-r--r--   0        0        0      916 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/colors.py
+-rw-r--r--   0        0        0    15404 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/config.py
+-rw-r--r--   0        0        0     1160 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/discord.py
+-rw-r--r--   0        0        0     6981 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/mal_proxy.py
+-rw-r--r--   0        0        0      185 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/__init__.py
+-rw-r--r--   0        0        0     1140 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/base_menu.py
+-rw-r--r--   0        0        0    24077 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/mal_menu.py
+-rw-r--r--   0        0        0     6179 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/menu.py
+-rw-r--r--   0        0        0     9097 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/menus/seasonal_menu.py
+-rw-r--r--   0        0        0     7119 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/prompts.py
+-rw-r--r--   0        0        0     7684 2024-05-19 09:41:00.164333 anipy_cli-3.0.5/src/anipy_cli/util.py
+-rw-r--r--   0        0        0     3084 1970-01-01 00:00:00.000000 anipy_cli-3.0.5/PKG-INFO
```

### Comparing `anipy_cli-3.0.4/README.md` & `anipy_cli-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/pyproject.toml` & `anipy_cli-3.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-cli"
-version = "3.0.4"
+version = "3.0.5"
 description = "Watch and Download anime from the comfort of your Terminal"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-cli"
 keywords = ["anime", "cli"]
```

### Comparing `anipy_cli-3.0.4/src/anipy_cli/arg_parser.py` & `anipy_cli-3.0.5/src/anipy_cli/arg_parser.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/cli.py` & `anipy_cli-3.0.5/src/anipy_cli/cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/base_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/base_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/binge_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/binge_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/default_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/default_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/download_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/download_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/history_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/history_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/mal_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/mal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/clis/seasonal_cli.py` & `anipy_cli-3.0.5/src/anipy_cli/clis/seasonal_cli.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/colors.py` & `anipy_cli-3.0.5/src/anipy_cli/colors.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/config.py` & `anipy_cli-3.0.5/src/anipy_cli/config.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/discord.py` & `anipy_cli-3.0.5/src/anipy_cli/discord.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/mal_proxy.py` & `anipy_cli-3.0.5/src/anipy_cli/mal_proxy.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/menus/base_menu.py` & `anipy_cli-3.0.5/src/anipy_cli/menus/base_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/menus/mal_menu.py` & `anipy_cli-3.0.5/src/anipy_cli/menus/mal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/menus/menu.py` & `anipy_cli-3.0.5/src/anipy_cli/menus/menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/menus/seasonal_menu.py` & `anipy_cli-3.0.5/src/anipy_cli/menus/seasonal_menu.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/prompts.py` & `anipy_cli-3.0.5/src/anipy_cli/prompts.py`

 * *Files identical despite different names*

### Comparing `anipy_cli-3.0.4/src/anipy_cli/util.py` & `anipy_cli-3.0.5/src/anipy_cli/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                 error(
                     f"> failed to migrate {name}, as it was configured as dub but"
                     f"{gogo.BASE_URL}/category/{identifier}-dub or {gogo.BASE_URL}/category/{identifier}-japanese-dub was not found!"
                 )
                 continue
 
             new_entry = LocalListEntry(
-                provider="gogoanmie",
+                provider="gogoanime",
                 name=name,
                 identifier=identifier,
                 episode=episode,
                 language=LanguageTypeEnum.DUB if is_dub else LanguageTypeEnum.SUB,
                 languages=langs,
                 timestamp=int(time.time()),
             )
```

### Comparing `anipy_cli-3.0.4/PKG-INFO` & `anipy_cli-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-cli
-Version: 3.0.4
+Version: 3.0.5
 Summary: Watch and Download anime from the comfort of your Terminal
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,cli
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: anipy-cli Version: 3.0.4 Summary: Watch and
+Metadata-Version: 2.1 Name: anipy-cli Version: 3.0.5 Summary: Watch and
 Download anime from the comfort of your Terminal Home-page: https://
 sdaqo.github.io/anipy-cli License: GPL-3.0 Keywords: anime,cli Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
```

