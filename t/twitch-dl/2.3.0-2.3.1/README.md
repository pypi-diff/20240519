# Comparing `tmp/twitch_dl-2.3.0.tar.gz` & `tmp/twitch_dl-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dl-2.3.0.tar", last modified: Sat Apr 27 18:24:51 2024, max compression
+gzip compressed data, was "twitch_dl-2.3.1.tar", last modified: Sun May 19 07:13:21 2024, max compression
```

## Comparing `twitch_dl-2.3.0.tar` & `twitch_dl-2.3.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.601963 twitch_dl-2.3.0/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/.flake8
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.587963 twitch_dl-2.3.0/.github/
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.590963 twitch_dl-2.3.0/.github/workflows/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 12:52:36.000000 twitch_dl-2.3.0/.github/workflows/test.yml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/.gitignore
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/.vermin
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10556 2024-04-27 18:23:25.000000 twitch_dl-2.3.0/CHANGELOG.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/LICENSE
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      959 2024-04-27 18:22:52.000000 twitch_dl-2.3.0/Makefile
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-27 18:24:51.601963 twitch_dl-2.3.0/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/README.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2022-11-13 13:02:23.000000 twitch_dl-2.3.0/TODO.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/book.css
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/book.toml
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8805 2024-04-27 18:23:09.000000 twitch_dl-2.3.0/changelog.yaml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.591963 twitch_dl-2.3.0/docs/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/SUMMARY.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/advanced.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10556 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/changelog.md
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.592963 twitch_dl-2.3.0/docs/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/commands/auth_token.png
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/clips.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/download.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/env.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/info.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-04-27 18:23:26.000000 twitch_dl-2.3.0/docs/commands/videos.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/environment_variables.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/installation.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/introduction.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/license.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/docs/shell_completion.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2022-08-27 09:42:13.000000 twitch_dl-2.3.0/docs/usage.md
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1308 2024-04-24 06:19:51.000000 twitch_dl-2.3.0/pyproject.toml
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.593963 twitch_dl-2.3.0/scripts/
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2022-11-13 13:02:23.000000 twitch_dl-2.3.0/scripts/generate_changelog
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/scripts/generate_docs
--rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-10 06:26:52.000000 twitch_dl-2.3.0/scripts/tag_version
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-04-27 18:24:51.601963 twitch_dl-2.3.0/setup.cfg
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.596963 twitch_dl-2.3.0/tests/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2076 2024-04-24 12:38:54.000000 twitch_dl-2.3.0/tests/test_api.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4659 2024-04-24 12:44:22.000000 twitch_dl-2.3.0/tests/test_cli.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2518 2024-04-27 18:22:52.000000 twitch_dl-2.3.0/tests/test_patterns.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2605 2022-11-13 13:02:23.000000 twitch_dl-2.3.0/tests/test_progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/tests/test_utils.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2022-08-04 08:32:39.000000 twitch_dl-2.3.0/twitch-dl.1.scd
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.600963 twitch_dl-2.3.0/twitch_dl.egg-info/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/PKG-INFO
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1240 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/entry_points.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      133 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/requires.txt
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-04-27 18:24:51.000000 twitch_dl-2.3.0/twitch_dl.egg-info/top_level.txt
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.599963 twitch_dl-2.3.0/twitchdl/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/twitchdl/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/twitchdl/__main__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9715 2024-04-24 06:58:58.000000 twitch_dl-2.3.0/twitchdl/cli.py
-drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-04-27 18:24:51.600963 twitch_dl-2.3.0/twitchdl/commands/
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-03-29 07:50:11.000000 twitch_dl-2.3.0/twitchdl/commands/__init__.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-24 05:25:48.000000 twitch_dl-2.3.0/twitchdl/commands/clips.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11691 2024-04-27 17:02:55.000000 twitch_dl-2.3.0/twitchdl/commands/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3015 2024-04-27 16:59:23.000000 twitch_dl-2.3.0/twitchdl/commands/info.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2039 2024-04-24 12:30:02.000000 twitch_dl-2.3.0/twitchdl/commands/videos.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-24 05:25:48.000000 twitch_dl-2.3.0/twitchdl/download.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-24 05:25:48.000000 twitch_dl-2.3.0/twitchdl/entities.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-04 06:27:17.000000 twitch_dl-2.3.0/twitchdl/exceptions.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-24 12:09:16.000000 twitch_dl-2.3.0/twitchdl/http.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4775 2024-04-27 18:22:53.000000 twitch_dl-2.3.0/twitchdl/output.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4553 2024-04-27 18:22:53.000000 twitch_dl-2.3.0/twitchdl/playlists.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4722 2024-04-12 07:42:26.000000 twitch_dl-2.3.0/twitchdl/progress.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12422 2024-04-24 12:29:56.000000 twitch_dl-2.3.0/twitchdl/twitch.py
--rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3113 2024-04-27 18:22:52.000000 twitch_dl-2.3.0/twitchdl/utils.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.906749 twitch_dl-2.3.1/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       41 2022-08-04 08:32:39.000000 twitch_dl-2.3.1/.flake8
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.895748 twitch_dl-2.3.1/.github/
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.898748 twitch_dl-2.3.1/.github/workflows/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-04-24 12:52:36.000000 twitch_dl-2.3.1/.github/workflows/test.yml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      166 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/.gitignore
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       65 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/.vermin
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10701 2024-05-19 07:12:58.000000 twitch_dl-2.3.1/CHANGELOG.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    35147 2022-08-04 08:32:39.000000 twitch_dl-2.3.1/LICENSE
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      959 2024-04-27 18:22:52.000000 twitch_dl-2.3.1/Makefile
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-05-19 07:13:21.905749 twitch_dl-2.3.1/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1627 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/README.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      343 2022-11-13 13:02:23.000000 twitch_dl-2.3.1/TODO.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      481 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/book.css
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      223 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/book.toml
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     8909 2024-05-19 07:12:58.000000 twitch_dl-2.3.1/changelog.yaml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.899749 twitch_dl-2.3.1/docs/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      484 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/docs/SUMMARY.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      282 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/docs/advanced.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    10701 2024-05-19 07:12:58.000000 twitch_dl-2.3.1/docs/changelog.md
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.900749 twitch_dl-2.3.1/docs/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    69599 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/docs/commands/auth_token.png
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2499 2024-05-19 07:11:36.000000 twitch_dl-2.3.1/docs/commands/clips.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     6159 2024-05-19 07:11:36.000000 twitch_dl-2.3.1/docs/commands/download.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      722 2024-05-19 07:11:36.000000 twitch_dl-2.3.1/docs/commands/env.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      670 2024-05-19 07:11:36.000000 twitch_dl-2.3.1/docs/commands/info.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2030 2024-05-19 07:11:36.000000 twitch_dl-2.3.1/docs/commands/videos.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      420 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/docs/environment_variables.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1653 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/docs/installation.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1169 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/docs/introduction.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    34916 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/docs/license.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      664 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/docs/shell_completion.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      690 2022-08-27 09:42:13.000000 twitch_dl-2.3.1/docs/usage.md
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1308 2024-04-28 07:30:24.000000 twitch_dl-2.3.1/pyproject.toml
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.901749 twitch_dl-2.3.1/scripts/
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1026 2022-11-13 13:02:23.000000 twitch_dl-2.3.1/scripts/generate_changelog
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     3686 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/scripts/generate_docs
+-rwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)     1587 2024-04-10 06:26:52.000000 twitch_dl-2.3.1/scripts/tag_version
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       38 2024-05-19 07:13:21.906749 twitch_dl-2.3.1/setup.cfg
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.901749 twitch_dl-2.3.1/tests/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2076 2024-04-24 12:38:54.000000 twitch_dl-2.3.1/tests/test_api.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4659 2024-04-24 12:44:22.000000 twitch_dl-2.3.1/tests/test_cli.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2518 2024-04-27 18:22:52.000000 twitch_dl-2.3.1/tests/test_patterns.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2857 2024-04-30 07:57:48.000000 twitch_dl-2.3.1/tests/test_progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      456 2022-08-04 08:32:39.000000 twitch_dl-2.3.1/tests/test_utils.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1350 2022-08-04 08:32:39.000000 twitch_dl-2.3.1/twitch-dl.1.scd
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.904749 twitch_dl-2.3.1/twitch_dl.egg-info/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    43270 2024-05-19 07:13:21.000000 twitch_dl-2.3.1/twitch_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     1240 2024-05-19 07:13:21.000000 twitch_dl-2.3.1/twitch_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        1 2024-05-19 07:13:21.000000 twitch_dl-2.3.1/twitch_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       47 2024-05-19 07:13:21.000000 twitch_dl-2.3.1/twitch_dl.egg-info/entry_points.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      133 2024-05-19 07:13:21.000000 twitch_dl-2.3.1/twitch_dl.egg-info/requires.txt
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        9 2024-05-19 07:13:21.000000 twitch_dl-2.3.1/twitch_dl.egg-info/top_level.txt
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.904749 twitch_dl-2.3.1/twitchdl/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      196 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/twitchdl/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)       36 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/twitchdl/__main__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     9715 2024-04-24 06:58:58.000000 twitch_dl-2.3.1/twitchdl/cli.py
+drwxr-xr-x   0 ihabunek  (1000) ihabunek  (1000)        0 2024-05-19 07:13:21.904749 twitch_dl-2.3.1/twitchdl/commands/
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)        0 2024-03-29 07:50:11.000000 twitch_dl-2.3.1/twitchdl/commands/__init__.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2561 2024-04-24 05:25:48.000000 twitch_dl-2.3.1/twitchdl/commands/clips.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    11798 2024-05-19 07:07:51.000000 twitch_dl-2.3.1/twitchdl/commands/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3015 2024-04-27 16:59:23.000000 twitch_dl-2.3.1/twitchdl/commands/info.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     2039 2024-04-24 12:30:02.000000 twitch_dl-2.3.1/twitchdl/commands/videos.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      932 2024-04-24 05:25:48.000000 twitch_dl-2.3.1/twitchdl/download.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      522 2024-04-24 05:25:48.000000 twitch_dl-2.3.1/twitchdl/entities.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)      139 2024-04-04 06:27:17.000000 twitch_dl-2.3.1/twitchdl/exceptions.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4138 2024-04-28 07:54:04.000000 twitch_dl-2.3.1/twitchdl/http.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4775 2024-04-27 18:22:53.000000 twitch_dl-2.3.1/twitchdl/output.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4553 2024-04-27 18:22:53.000000 twitch_dl-2.3.1/twitchdl/playlists.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     4494 2024-04-30 07:57:48.000000 twitch_dl-2.3.1/twitchdl/progress.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)    12424 2024-05-19 07:12:58.000000 twitch_dl-2.3.1/twitchdl/twitch.py
+-rw-r--r--   0 ihabunek  (1000) ihabunek  (1000)     3113 2024-04-27 18:22:52.000000 twitch_dl-2.3.1/twitchdl/utils.py
```

### Comparing `twitch_dl-2.3.0/.github/workflows/test.yml` & `twitch_dl-2.3.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/CHANGELOG.md` & `twitch_dl-2.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.3.1 (2024-05-19)](https://github.com/ihabunek/twitch-dl/releases/tag/2.3.1)
+
+* Fix fetching access token (#155, thanks @KryptonicDragon)
+
 ### [2.3.0 (2024-04-27)](https://github.com/ihabunek/twitch-dl/releases/tag/2.3.0)
 
 * Show more playlist data when choosing quality
 * Improve detection of 'source' quality for Twitch Enhanced Broadcast Streams
   (#154)
 
 ### [2.2.4 (2024-04-25)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.4)
```

### Comparing `twitch_dl-2.3.0/LICENSE` & `twitch_dl-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/Makefile` & `twitch_dl-2.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/PKG-INFO` & `twitch_dl-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.3.0
+Version: 2.3.1
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click<9.0.0,>=8.0.0
 Requires-Dist: httpx<1.0.0,>=0.17.0
-Requires-Dist: m3u8<4.0.0,>=1.0.0
+Requires-Dist: m3u8<5.0.0,>=3.0.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: vermin; extra == "dev"
```

### Comparing `twitch_dl-2.3.0/README.md` & `twitch_dl-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/changelog.yaml` & `twitch_dl-2.3.1/changelog.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2.3.1:
+  date: 2024-05-19
+  changes:
+    - "Fix fetching access token (#155, thanks @KryptonicDragon)"
+
 2.3.0:
   date: 2024-04-27
   changes:
     - "Show more playlist data when choosing quality"
     - "Improve detection of 'source' quality for Twitch Enhanced Broadcast Streams (#154)"
 
 2.2.4:
```

### Comparing `twitch_dl-2.3.0/docs/changelog.md` & `twitch_dl-2.3.1/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 twitch-dl changelog
 ===================
 
 <!-- Do not edit. This file is automatically generated from changelog.yaml.-->
 
+### [2.3.1 (2024-05-19)](https://github.com/ihabunek/twitch-dl/releases/tag/2.3.1)
+
+* Fix fetching access token (#155, thanks @KryptonicDragon)
+
 ### [2.3.0 (2024-04-27)](https://github.com/ihabunek/twitch-dl/releases/tag/2.3.0)
 
 * Show more playlist data when choosing quality
 * Improve detection of 'source' quality for Twitch Enhanced Broadcast Streams
   (#154)
 
 ### [2.2.4 (2024-04-25)](https://github.com/ihabunek/twitch-dl/releases/tag/2.2.4)
```

### Comparing `twitch_dl-2.3.0/docs/commands/auth_token.png` & `twitch_dl-2.3.1/docs/commands/auth_token.png`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/commands/clips.md` & `twitch_dl-2.3.1/docs/commands/clips.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/commands/download.md` & `twitch_dl-2.3.1/docs/commands/download.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/commands/env.md` & `twitch_dl-2.3.1/docs/commands/env.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/commands/info.md` & `twitch_dl-2.3.1/docs/commands/info.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/commands/videos.md` & `twitch_dl-2.3.1/docs/commands/videos.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/installation.md` & `twitch_dl-2.3.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/introduction.md` & `twitch_dl-2.3.1/docs/introduction.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/license.md` & `twitch_dl-2.3.1/docs/license.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/shell_completion.md` & `twitch_dl-2.3.1/docs/shell_completion.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/docs/usage.md` & `twitch_dl-2.3.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/pyproject.toml` & `twitch_dl-2.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
     "click>=8.0.0,<9.0.0",
     "httpx>=0.17.0,<1.0.0",
-    "m3u8>=1.0.0,<4.0.0",
+    "m3u8>=3.0.0,<5.0.0",
 ]
 
 [tool.setuptools]
 packages = [
     "twitchdl",
     "twitchdl.commands",
 ]
```

### Comparing `twitch_dl-2.3.0/scripts/generate_changelog` & `twitch_dl-2.3.1/scripts/generate_changelog`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/scripts/generate_docs` & `twitch_dl-2.3.1/scripts/generate_docs`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/scripts/tag_version` & `twitch_dl-2.3.1/scripts/tag_version`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/tests/test_api.py` & `twitch_dl-2.3.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/tests/test_cli.py` & `twitch_dl-2.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/tests/test_patterns.py` & `twitch_dl-2.3.1/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/tests/test_progress.py` & `twitch_dl-2.3.1/tests/test_progress.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,43 +19,49 @@
     progress.start(3, 300)
 
     assert progress.downloaded == 0
     assert progress.progress_bytes == 0
     assert progress.progress_perc == 0
 
     progress.advance(1, 100)
+    progress._recalculate()
     assert progress.downloaded == 100
     assert progress.progress_bytes == 100
     assert progress.progress_perc == 11
 
     progress.advance(2, 200)
+    progress._recalculate()
     assert progress.downloaded == 300
     assert progress.progress_bytes == 300
     assert progress.progress_perc == 33
 
     progress.advance(3, 150)
+    progress._recalculate()
     assert progress.downloaded == 450
     assert progress.progress_bytes == 450
     assert progress.progress_perc == 50
 
     progress.advance(1, 50)
+    progress._recalculate()
     assert progress.downloaded == 500
     assert progress.progress_bytes == 500
     assert progress.progress_perc == 55
 
     progress.abort(2)
+    progress._recalculate()
     assert progress.downloaded == 500
     assert progress.progress_bytes == 300
     assert progress.progress_perc == 33
 
     progress.start(2, 300)
 
     progress.advance(1, 150)
     progress.advance(2, 300)
     progress.advance(3, 150)
+    progress._recalculate()
 
     assert progress.downloaded == 1100
     assert progress.progress_bytes == 900
     assert progress.progress_perc == 100
 
     progress.end(1)
     progress.end(2)
@@ -67,20 +73,23 @@
 
 
 def test_estimated_total():
     progress = Progress(3)
     assert progress.estimated_total is None
 
     progress.start(1, 12000)
+    progress._recalculate()
     assert progress.estimated_total == 12000 * 3
 
     progress.start(2, 11000)
+    progress._recalculate()
     assert progress.estimated_total == 11500 * 3
 
     progress.start(3, 10000)
+    progress._recalculate()
     assert progress.estimated_total == 11000 * 3
 
 
 def test_vod_downloaded_count():
     progress = Progress(3)
 
     progress.start(1, 100)
```

### Comparing `twitch_dl-2.3.0/twitch-dl.1.scd` & `twitch_dl-2.3.1/twitch-dl.1.scd`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitch_dl.egg-info/PKG-INFO` & `twitch_dl-2.3.1/twitch_dl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dl
-Version: 2.3.0
+Version: 2.3.1
 Summary: Quickly download videos from twitch.tv from the comort of your terminal emulator
 Author-email: Ivan Habunek <ivan@habunek.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -686,15 +686,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click<9.0.0,>=8.0.0
 Requires-Dist: httpx<1.0.0,>=0.17.0
-Requires-Dist: m3u8<4.0.0,>=1.0.0
+Requires-Dist: m3u8<5.0.0,>=3.0.0
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pyyaml; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: vermin; extra == "dev"
```

### Comparing `twitch_dl-2.3.0/twitch_dl.egg-info/SOURCES.txt` & `twitch_dl-2.3.1/twitch_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/cli.py` & `twitch_dl-2.3.1/twitchdl/cli.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/commands/clips.py` & `twitch_dl-2.3.1/twitchdl/commands/clips.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/commands/download.py` & `twitch_dl-2.3.1/twitchdl/commands/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import platform
 import re
 import shutil
 import subprocess
 import tempfile
 from os import path
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Optional
 from urllib.parse import urlencode, urlparse
 
 import click
 import httpx
 
 from twitchdl import twitch, utils
 from twitchdl.download import download_file
@@ -26,14 +26,18 @@
     parse_playlists,
     select_playlist,
 )
 from twitchdl.twitch import Chapter, Clip, ClipAccessToken, Video
 
 
 def download(ids: List[str], args: DownloadOptions):
+    if not ids:
+        print_log("No IDs to downlad given")
+        return
+
     for video_id in ids:
         download_one(video_id, args)
 
 
 def download_one(video: str, args: DownloadOptions):
     video_id = utils.parse_video_identifier(video)
     if video_id:
@@ -152,15 +156,15 @@
     """Create a temp dir to store downloads if it doesn't exist."""
     path = urlparse(base_uri).path.lstrip("/")
     temp_dir = Path(tempfile.gettempdir(), "twitch-dl", path)
     temp_dir.mkdir(parents=True, exist_ok=True)
     return str(temp_dir)
 
 
-def _get_clip_url(access_token: ClipAccessToken, quality: str) -> str:
+def _get_clip_url(access_token: ClipAccessToken, quality: Optional[str]) -> str:
     qualities = access_token["videoQualities"]
 
     # Quality given as an argument
     if quality:
         if quality == "source":
             return qualities[0]["sourceURL"]
 
@@ -180,15 +184,15 @@
     click.echo()
 
     no = utils.read_int("Choose quality", min=1, max=len(qualities), default=1)
     selected_quality = qualities[no - 1]
     return selected_quality["sourceURL"]
 
 
-def get_clip_authenticated_url(slug: str, quality: str):
+def get_clip_authenticated_url(slug: str, quality: Optional[str]):
     print_log("Fetching access token...")
     access_token = twitch.get_clip_access_token(slug)
 
     if not access_token:
         raise ConsoleError(f"Access token not found for slug '{slug}'")
 
     url = _get_clip_url(access_token, quality)
```

### Comparing `twitch_dl-2.3.0/twitchdl/commands/info.py` & `twitch_dl-2.3.1/twitchdl/commands/info.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/commands/videos.py` & `twitch_dl-2.3.1/twitchdl/commands/videos.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/download.py` & `twitch_dl-2.3.1/twitchdl/download.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/entities.py` & `twitch_dl-2.3.1/twitchdl/entities.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/http.py` & `twitch_dl-2.3.1/twitchdl/http.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/output.py` & `twitch_dl-2.3.1/twitchdl/output.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/playlists.py` & `twitch_dl-2.3.1/twitchdl/playlists.py`

 * *Files identical despite different names*

### Comparing `twitch_dl-2.3.0/twitchdl/progress.py` & `twitch_dl-2.3.1/twitchdl/progress.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import time
 from collections import deque
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from statistics import mean
 from typing import Deque, Dict, NamedTuple, Optional
 
 import click
 
 from twitchdl.output import blue
 from twitchdl.utils import format_size, format_time
@@ -27,69 +27,60 @@
 
 
 class Sample(NamedTuple):
     downloaded: int
     timestamp: float
 
 
-@dataclass
 class Progress:
-    vod_count: int
-    downloaded: int = 0
-    estimated_total: Optional[int] = None
-    last_printed: float = field(default_factory=time.time)
-    progress_bytes: int = 0
-    progress_perc: int = 0
-    remaining_time: Optional[int] = None
-    speed: Optional[float] = None
-    start_time: float = field(default_factory=time.time)
-    tasks: Dict[TaskId, Task] = field(default_factory=dict)
-    vod_downloaded_count: int = 0
-    samples: Deque[Sample] = field(default_factory=lambda: deque(maxlen=100))
+    def __init__(self, vod_count: int):
+        self.downloaded: int = 0
+        self.estimated_total: Optional[int] = None
+        self.last_printed: Optional[float] = None
+        self.progress_bytes: int = 0
+        self.progress_perc: int = 0
+        self.remaining_time: Optional[int] = None
+        self.samples: Deque[Sample] = deque(maxlen=1000)
+        self.speed: Optional[float] = None
+        self.tasks: Dict[TaskId, Task] = {}
+        self.vod_count = vod_count
+        self.vod_downloaded_count: int = 0
 
     def start(self, task_id: int, size: int):
         if task_id in self.tasks:
             raise ValueError(f"Task {task_id}: cannot start, already started")
 
         self.tasks[task_id] = Task(task_id, size)
-        self._calculate_total()
-        self._calculate_progress()
         self.print()
 
     def advance(self, task_id: int, size: int):
         if task_id not in self.tasks:
             raise ValueError(f"Task {task_id}: cannot advance, not started")
 
         self.downloaded += size
         self.progress_bytes += size
         self.tasks[task_id].advance(size)
         self.samples.append(Sample(self.downloaded, time.time()))
-        self._calculate_progress()
         self.print()
 
     def already_downloaded(self, task_id: int, size: int):
         if task_id in self.tasks:
             raise ValueError(f"Task {task_id}: cannot mark as downloaded, already started")
 
         self.tasks[task_id] = Task(task_id, size)
         self.progress_bytes += size
         self.vod_downloaded_count += 1
-        self._calculate_total()
-        self._calculate_progress()
         self.print()
 
     def abort(self, task_id: int):
         if task_id not in self.tasks:
             raise ValueError(f"Task {task_id}: cannot abort, not started")
 
         del self.tasks[task_id]
         self.progress_bytes = sum(t.downloaded for t in self.tasks.values())
-
-        self._calculate_total()
-        self._calculate_progress()
         self.print()
 
     def end(self, task_id: int):
         if task_id not in self.tasks:
             raise ValueError(f"Task {task_id}: cannot end, not started")
 
         task = self.tasks[task_id]
@@ -97,20 +88,18 @@
             logger.warn(
                 f"Taks {task_id} ended with {task.downloaded}b downloaded, expected {task.size}b."
             )
 
         self.vod_downloaded_count += 1
         self.print()
 
-    def _calculate_total(self):
+    def _recalculate(self):
         self.estimated_total = (
             int(mean(t.size for t in self.tasks.values()) * self.vod_count) if self.tasks else None
         )
-
-    def _calculate_progress(self):
         self.speed = self._calculate_speed()
         self.progress_perc = (
             int(100 * self.progress_bytes / self.estimated_total) if self.estimated_total else 0
         )
         self.remaining_time = (
             int((self.estimated_total - self.progress_bytes) / self.speed)
             if self.estimated_total and self.speed
@@ -129,17 +118,19 @@
 
         return size / duration if duration > 0 else None
 
     def print(self):
         now = time.time()
 
         # Don't print more often than 10 times per second
-        if now - self.last_printed < 0.1:
+        if self.last_printed and now - self.last_printed < 0.1:
             return
 
+        self._recalculate()
+
         click.echo(f"\rDownloaded {self.vod_downloaded_count}/{self.vod_count} VODs", nl=False)
         click.secho(f" {self.progress_perc}%", fg="blue", nl=False)
 
         if self.estimated_total is not None:
             total = f"~{format_size(self.estimated_total)}"
             click.echo(f" of {blue(total)}", nl=False)
```

### Comparing `twitch_dl-2.3.0/twitchdl/twitch.py` & `twitch_dl-2.3.1/twitchdl/twitch.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
     return videos["totalCount"], _generator(videos, max_videos)
 
 
 def get_access_token(video_id: str, auth_token: Optional[str] = None) -> AccessToken:
     query = f"""
     {{
         videoPlaybackAccessToken(
-            id: {video_id},
+            id: "{video_id}",
             params: {{
                 platform: "web",
                 playerBackend: "mediaplayer",
                 playerType: "site"
             }}
         ) {{
             signature
```

### Comparing `twitch_dl-2.3.0/twitchdl/utils.py` & `twitch_dl-2.3.1/twitchdl/utils.py`

 * *Files identical despite different names*

