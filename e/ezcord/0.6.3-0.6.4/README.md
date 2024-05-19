# Comparing `tmp/ezcord-0.6.3.tar.gz` & `tmp/ezcord-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcord-0.6.3.tar", last modified: Thu May 16 15:17:49 2024, max compression
+gzip compressed data, was "ezcord-0.6.4.tar", last modified: Sun May 19 11:39:29 2024, max compression
```

## Comparing `ezcord-0.6.3.tar` & `ezcord-0.6.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 15:17:40.000000 ezcord-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 15:17:40.000000 ezcord-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 15:17:49.723100 ezcord-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-16 15:17:40.000000 ezcord-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.715100 ezcord-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 15:17:40.000000 ezcord-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.715100 ezcord-0.6.3/ezcord/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    35717 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/bot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/cogs/
--rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/blacklist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/cogs/dpy/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/dpy/blacklist_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/dpy/help_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/dpy/status_changer_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/cogs/pyc/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/pyc/blacklist_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/pyc/help_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/pyc/status_changer_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/cogs/status_changer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/emb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.719100 ezcord-0.6.3/ezcord/internal/dc/
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/dc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/dc/dc_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/embed_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/ezcord/internal/language/
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/language/de.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/language/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/language/languages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/ready_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/internal/translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/ezcord/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/sql/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/sql/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-16 15:17:40.000000 ezcord-0.6.3/ezcord/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/ezcord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 15:17:49.000000 ezcord-0.6.3/ezcord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 15:17:40.000000 ezcord-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 15:17:40.000000 ezcord-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:17:49.723100 ezcord-0.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:17:49.723100 ezcord-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 15:17:40.000000 ezcord-0.6.3/tests/test_libs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-16 15:17:40.000000 ezcord-0.6.3/tests/test_times.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-19 11:39:25.000000 ezcord-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 11:39:25.000000 ezcord-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-19 11:39:29.552055 ezcord-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-19 11:39:25.000000 ezcord-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.544055 ezcord-0.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 11:39:25.000000 ezcord-0.6.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.548055 ezcord-0.6.4/ezcord/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35717 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/bot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.548055 ezcord-0.6.4/ezcord/cogs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10403 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/blacklist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.548055 ezcord-0.6.4/ezcord/cogs/dpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/dpy/blacklist_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/dpy/help_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/dpy/status_changer_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.548055 ezcord-0.6.4/ezcord/cogs/pyc/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/pyc/blacklist_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/pyc/help_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/pyc/status_changer_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/cogs/status_changer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/emb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28260 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/ezcord/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/ezcord/internal/dc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/dc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/dc/dc_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/embed_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/ezcord/internal/language/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/language/languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/ready_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/internal/translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/ezcord/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/sql/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11065 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/sql/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-19 11:39:25.000000 ezcord-0.6.4/ezcord/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/ezcord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-19 11:39:29.000000 ezcord-0.6.4/ezcord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-19 11:39:29.000000 ezcord-0.6.4/ezcord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:39:29.000000 ezcord-0.6.4/ezcord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-19 11:39:29.000000 ezcord-0.6.4/ezcord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:39:29.000000 ezcord-0.6.4/ezcord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-19 11:39:25.000000 ezcord-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-19 11:39:25.000000 ezcord-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:39:29.552055 ezcord-0.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:39:29.552055 ezcord-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-19 11:39:25.000000 ezcord-0.6.4/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-19 11:39:25.000000 ezcord-0.6.4/tests/test_times.py
```

### Comparing `ezcord-0.6.3/LICENSE` & `ezcord-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/PKG-INFO` & `ezcord-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.6.3
+Version: 0.6.4
 Summary: An easy-to-use extension for Discord.py and Pycord
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord,discord.py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.6.3/README.md` & `ezcord-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/blacklist.py` & `ezcord-0.6.4/ezcord/blacklist.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/bot.py` & `ezcord-0.6.4/ezcord/bot.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/cogs/blacklist.py` & `ezcord-0.6.4/ezcord/cogs/blacklist.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/cogs/help.py` & `ezcord-0.6.4/ezcord/cogs/help.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/cogs/status_changer.py` & `ezcord-0.6.4/ezcord/cogs/status_changer.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/components.py` & `ezcord-0.6.4/ezcord/components.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/emb.py` & `ezcord-0.6.4/ezcord/emb.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/enums.py` & `ezcord-0.6.4/ezcord/enums.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/errors.py` & `ezcord-0.6.4/ezcord/errors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/i18n.py` & `ezcord-0.6.4/ezcord/i18n.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/colors.py` & `ezcord-0.6.4/ezcord/internal/colors.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/config.py` & `ezcord-0.6.4/ezcord/internal/config.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/dc/__init__.py` & `ezcord-0.6.4/ezcord/internal/dc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,24 @@
 class FakeDiscord:
     """A fake class that is used when EzCord is used without a supported Discord library."""
 
     DiscordException = Exception
     CogMeta = type
 
     def __getattr__(self, name):
-        if name in ("Embed", "View", "Modal", "ApplicationContext", "Interaction", "Bot", "Cog"):
+        if name in (
+            "ApplicationContext",
+            "AutoShardedBot",
+            "Bot",
+            "Cog",
+            "Embed",
+            "Interaction",
+            "Modal",
+            "View",
+        ):
             return NoDiscordLibFound
 
         return FakeDiscord()
 
     def __call__(self, *args, **kwargs):
         pass
```

### Comparing `ezcord-0.6.3/ezcord/internal/embed_templates.py` & `ezcord-0.6.4/ezcord/internal/embed_templates.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/language/de.json` & `ezcord-0.6.4/ezcord/internal/language/de.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/language/en.json` & `ezcord-0.6.4/ezcord/internal/language/en.json`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/language/languages.py` & `ezcord-0.6.4/ezcord/internal/language/languages.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/ready_style.py` & `ezcord-0.6.4/ezcord/internal/ready_style.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/internal/translation.py` & `ezcord-0.6.4/ezcord/internal/translation.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/logs.py` & `ezcord-0.6.4/ezcord/logs.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/sql/postgresql.py` & `ezcord-0.6.4/ezcord/sql/postgresql.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/sql/sqlite.py` & `ezcord-0.6.4/ezcord/sql/sqlite.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord/times.py` & `ezcord-0.6.4/ezcord/times.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return convert_time(abs(dt.total_seconds()), relative, use_locale=use_locale)
 
     if isinstance(dt, datetime):
         if dt.tzinfo is None:
             dt = dt.astimezone()
 
         return convert_time(
-            abs((dt - discord.utils.utcnow()).total_seconds()), relative, use_locale=use_locale
+            abs((dt - datetime.now(timezone.utc)).total_seconds()), relative, use_locale=use_locale
         )
 
 
 def dc_timestamp(
     seconds: int | float, style: Literal["t", "T", "d", "D", "f", "F", "R"] = "R"
 ) -> str:
     """Convert seconds to a Discord timestamp.
```

### Comparing `ezcord-0.6.3/ezcord/utils.py` & `ezcord-0.6.4/ezcord/utils.py`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/ezcord.egg-info/PKG-INFO` & `ezcord-0.6.4/ezcord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcord
-Version: 0.6.3
+Version: 0.6.4
 Summary: An easy-to-use extension for Discord.py and Pycord
 Author: tibue99
 License: MIT
 Project-URL: GitHub, https://github.com/tibue99/ezcord
 Project-URL: Documentation, https://ezcord.readthedocs.io
 Keywords: discord,pycord,py-cord,discord.py
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ezcord-0.6.3/ezcord.egg-info/SOURCES.txt` & `ezcord-0.6.4/ezcord.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 ezcord/internal/dc/dc_imports.py
 ezcord/internal/language/de.json
 ezcord/internal/language/en.json
 ezcord/internal/language/languages.py
 ezcord/sql/__init__.py
 ezcord/sql/postgresql.py
 ezcord/sql/sqlite.py
-tests/test_libs.py
+tests/test_general.py
 tests/test_times.py
```

### Comparing `ezcord-0.6.3/pyproject.toml` & `ezcord-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ezcord-0.6.3/tests/test_libs.py` & `ezcord-0.6.4/tests/test_general.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     async def get_users(self):
         return await self.all("SELECT user_id FROM users")
 
     async def get_coins(self, user_id):
         return await self.one("SELECT coins FROM users WHERE user_id = ?", (user_id,))
 
 
+@pytest.mark.dc
 def test_libs():
     """Test compatibility with different Discord libraries."""
 
     intents = discord.Intents.default()
     intents.message_content = True
     bot = ezcord.Bot(command_prefix="!", intents=intents)
 
@@ -48,15 +49,14 @@
 
 @pytest.mark.asyncio
 async def test_db():
     """Test the DBHandler class."""
 
     with tempfile.NamedTemporaryFile(delete=False) as db_file:
         db = UserDB(db_file.name)
-        print(db_file.name)
 
         await db.setup()
         await db.add_coins(12345, 100)
 
         assert await db.get_coins(12345) == 100
 
         await db.add_coins(54321, 0)
```

### Comparing `ezcord-0.6.3/tests/test_times.py` & `ezcord-0.6.4/tests/test_times.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 import pytest
 
 import ezcord
 from ezcord import ConvertTimeError
 
 
 def test_convert_time():
+    assert isinstance(ezcord.convert_time(5), str)
+
+
+def test_convert_dt():
     dt = datetime.now(tz=timezone.utc)
 
     assert isinstance(ezcord.convert_dt(dt), str)
     assert isinstance(ezcord.convert_dt(timedelta(seconds=5)), str)
-    assert isinstance(ezcord.convert_time(5), str)
 
 
+@pytest.mark.dc
 def test_dc_timestamp():
     result = ezcord.dc_timestamp(0)
     assert result.startswith("<t:") and result.endswith(":R>")
 
 
 def test_convert_so_seconds():
     assert ezcord.convert_to_seconds("1m 9s") == 69
```

