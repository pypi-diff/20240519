# Comparing `tmp/colorist-1.7.2.tar.gz` & `tmp/colorist-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorist-1.7.2.tar", last modified: Mon Apr  8 23:37:28 2024, max compression
+gzip compressed data, was "colorist-1.7.3.tar", last modified: Sun May 19 10:18:49 2024, max compression
```

## Comparing `colorist-1.7.2.tar` & `colorist-1.7.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.447076 colorist-1.7.2/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.7.2/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      193 2023-08-21 13:25:11.000000 colorist-1.7.2/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    15403 2024-04-08 23:37:28.446899 colorist-1.7.2/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    12374 2024-04-08 23:34:40.000000 colorist-1.7.2/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      108 2023-12-06 00:13:36.000000 colorist-1.7.2/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1779 2024-04-08 23:37:28.447396 colorist-1.7.2/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.429982 colorist-1.7.2/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.432297 colorist-1.7.2/src/colorist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2724 2023-04-23 11:04:46.000000 colorist-1.7.2/src/colorist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.434348 colorist-1.7.2/src/colorist/constants/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.7.2/src/colorist/constants/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2181 2023-04-11 11:49:16.000000 colorist-1.7.2/src/colorist/constants/ansi.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.7.2/src/colorist/constants/ascii.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.437121 colorist-1.7.2/src/colorist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.7.2/src/colorist/helper/.coverage
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.437806 colorist-1.7.2/src/colorist/helper/.pytest_cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.7.2/src/colorist/helper/.pytest_cache/.gitignore
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.7.2/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.7.2/src/colorist/helper/.pytest_cache/README.md
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.430356 colorist-1.7.2/src/colorist/helper/.pytest_cache/v/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.438458 colorist-1.7.2/src/colorist/helper/.pytest_cache/v/cache/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.7.2/src/colorist/helper/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.7.2/src/colorist/helper/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-23 10:26:22.000000 colorist-1.7.2/src/colorist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1997 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/helper/convert.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      733 2023-04-22 10:25:27.000000 colorist-1.7.2/src/colorist/helper/error.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.7.2/src/colorist/helper/generate.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1195 2024-02-19 00:11:29.000000 colorist-1.7.2/src/colorist/helper/print.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      493 2023-04-23 11:04:46.000000 colorist-1.7.2/src/colorist/helper/validate.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.439118 colorist-1.7.2/src/colorist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1789 2023-04-22 08:37:25.000000 colorist-1.7.2/src/colorist/model/README.MD
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/model/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.440769 colorist-1.7.2/src/colorist/model/abc/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/abc/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/abc/effect.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1329 2023-04-22 10:25:27.000000 colorist-1.7.2/src/colorist/model/abc/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/abc/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      424 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/model/abc/mkdocstrings.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/abc/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.441919 colorist-1.7.2/src/colorist/model/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/model/background/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1137 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/model/background/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1280 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/model/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1215 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/model/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.443042 colorist-1.7.2/src/colorist/model/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/model/foreground/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-11 07:01:26.000000 colorist-1.7.2/src/colorist/model/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1114 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/model/foreground/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1252 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/model/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1174 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/model/foreground/rgb.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.443654 colorist-1.7.2/src/colorist/print/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/print/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.444725 colorist-1.7.2/src/colorist/print/background/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/print/background/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     6033 2024-02-19 01:16:59.000000 colorist-1.7.2/src/colorist/print/background/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     5469 2024-02-19 01:16:59.000000 colorist-1.7.2/src/colorist/print/background/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1310 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/print/background/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1512 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/print/background/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1353 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/print/background/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     8014 2024-02-19 01:16:59.000000 colorist-1.7.2/src/colorist/print/effect.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.446076 colorist-1.7.2/src/colorist/print/foreground/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.2/src/colorist/print/foreground/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     5408 2024-02-19 01:16:59.000000 colorist-1.7.2/src/colorist/print/foreground/bright_color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     4842 2024-02-19 01:16:59.000000 colorist-1.7.2/src/colorist/print/foreground/color.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1191 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/print/foreground/hex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1436 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/print/foreground/hsl.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1266 2023-10-23 16:26:56.000000 colorist-1.7.2/src/colorist/print/foreground/rgb.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1318 2023-04-23 11:04:46.000000 colorist-1.7.2/src/colorist/print/general.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.7.2/src/colorist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2024-04-08 23:34:49.000000 colorist-1.7.2/src/colorist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-04-08 23:37:28.446279 colorist-1.7.2/src/colorist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    15403 2024-04-08 23:37:28.000000 colorist-1.7.2/src/colorist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2217 2024-04-08 23:37:28.000000 colorist-1.7.2/src/colorist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2024-04-08 23:37:28.000000 colorist-1.7.2/src/colorist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.7.2/src/colorist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2024-04-08 23:37:28.000000 colorist-1.7.2/src/colorist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2024-04-08 23:37:28.000000 colorist-1.7.2/src/colorist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.056576 colorist-1.7.3/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1503 2023-04-02 09:11:33.000000 colorist-1.7.3/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      193 2023-08-21 13:25:11.000000 colorist-1.7.3/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    15404 2024-05-19 10:18:49.056425 colorist-1.7.3/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    12374 2024-05-19 10:16:15.000000 colorist-1.7.3/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      108 2023-12-06 00:13:36.000000 colorist-1.7.3/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1780 2024-05-19 10:18:49.056922 colorist-1.7.3/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.041182 colorist-1.7.3/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.043138 colorist-1.7.3/src/colorist/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2724 2023-04-23 11:04:46.000000 colorist-1.7.3/src/colorist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.045026 colorist-1.7.3/src/colorist/constants/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      149 2023-04-09 23:12:39.000000 colorist-1.7.3/src/colorist/constants/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2181 2023-04-11 11:49:16.000000 colorist-1.7.3/src/colorist/constants/ansi.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      502 2023-04-09 23:12:39.000000 colorist-1.7.3/src/colorist/constants/ascii.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.047690 colorist-1.7.3/src/colorist/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)   110592 2023-04-09 21:09:53.000000 colorist-1.7.3/src/colorist/helper/.coverage
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.048409 colorist-1.7.3/src/colorist/helper/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       37 2023-04-02 09:52:54.000000 colorist-1.7.3/src/colorist/helper/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      191 2023-04-02 09:52:54.000000 colorist-1.7.3/src/colorist/helper/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      302 2023-04-02 09:52:54.000000 colorist-1.7.3/src/colorist/helper/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.041525 colorist-1.7.3/src/colorist/helper/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.048856 colorist-1.7.3/src/colorist/helper/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.7.3/src/colorist/helper/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        2 2023-04-09 21:09:53.000000 colorist-1.7.3/src/colorist/helper/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      215 2023-04-23 10:26:22.000000 colorist-1.7.3/src/colorist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1997 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/helper/convert.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      733 2023-04-22 10:25:27.000000 colorist-1.7.3/src/colorist/helper/error.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1222 2023-04-09 23:12:39.000000 colorist-1.7.3/src/colorist/helper/generate.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1195 2024-02-19 00:11:29.000000 colorist-1.7.3/src/colorist/helper/print.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      493 2023-04-23 11:04:46.000000 colorist-1.7.3/src/colorist/helper/validate.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.049494 colorist-1.7.3/src/colorist/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1789 2023-04-22 08:37:25.000000 colorist-1.7.3/src/colorist/model/README.MD
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/model/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.050753 colorist-1.7.3/src/colorist/model/abc/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      572 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/abc/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      426 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/abc/effect.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1329 2023-04-22 10:25:27.000000 colorist-1.7.3/src/colorist/model/abc/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1915 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/abc/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      424 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/model/abc/mkdocstrings.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1326 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/abc/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.051808 colorist-1.7.3/src/colorist/model/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/model/background/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1410 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1306 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1137 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/model/background/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1280 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/model/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1215 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/model/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1516 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.052660 colorist-1.7.3/src/colorist/model/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/model/foreground/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1402 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-04-11 07:01:26.000000 colorist-1.7.3/src/colorist/model/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1114 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/model/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1252 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/model/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1174 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/model/foreground/rgb.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.053130 colorist-1.7.3/src/colorist/print/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/print/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.054346 colorist-1.7.3/src/colorist/print/background/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/print/background/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     6033 2024-02-19 01:16:59.000000 colorist-1.7.3/src/colorist/print/background/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     5469 2024-02-19 01:16:59.000000 colorist-1.7.3/src/colorist/print/background/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1310 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/print/background/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1512 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/print/background/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1353 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/print/background/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    10597 2024-05-19 10:17:10.000000 colorist-1.7.3/src/colorist/print/effect.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.055520 colorist-1.7.3/src/colorist/print/foreground/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-08-21 13:25:11.000000 colorist-1.7.3/src/colorist/print/foreground/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     5408 2024-02-19 01:16:59.000000 colorist-1.7.3/src/colorist/print/foreground/bright_color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4842 2024-02-19 01:16:59.000000 colorist-1.7.3/src/colorist/print/foreground/color.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1191 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/print/foreground/hex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1436 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/print/foreground/hsl.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1266 2023-10-23 16:26:56.000000 colorist-1.7.3/src/colorist/print/foreground/rgb.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1318 2023-04-23 11:04:46.000000 colorist-1.7.3/src/colorist/print/general.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:58:40.000000 colorist-1.7.3/src/colorist/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      174 2024-05-19 10:16:30.000000 colorist-1.7.3/src/colorist/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2024-05-19 10:18:49.055758 colorist-1.7.3/src/colorist.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    15404 2024-05-19 10:18:49.000000 colorist-1.7.3/src/colorist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2217 2024-05-19 10:18:49.000000 colorist-1.7.3/src/colorist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2024-05-19 10:18:49.000000 colorist-1.7.3/src/colorist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:13:43.000000 colorist-1.7.3/src/colorist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       98 2024-05-19 10:18:49.000000 colorist-1.7.3/src/colorist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        9 2024-05-19 10:18:49.000000 colorist-1.7.3/src/colorist.egg-info/top_level.txt
```

### Comparing `colorist-1.7.2/LICENSE.md` & `colorist-1.7.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/PKG-INFO` & `colorist-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.7.2
+Version: 1.7.3
 Summary: Colorist for Python
 Home-page: https://jakob-bagterp.github.io/colorist-for-python/
 Download-URL: https://pypi.org/project/colorist/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
@@ -21,22 +21,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: testing
-Requires-Dist: coverage==7.4.4; extra == "testing"
+Requires-Dist: coverage==7.5.1; extra == "testing"
 Requires-Dist: flake8==7.0.0; extra == "testing"
-Requires-Dist: mypy==1.9.0; extra == "testing"
-Requires-Dist: pytest==8.1.1; extra == "testing"
+Requires-Dist: mypy==1.10.0; extra == "testing"
+Requires-Dist: pytest==8.2.0; extra == "testing"
 Requires-Dist: pytest-cov==5.0.0; extra == "testing"
-Requires-Dist: tox==4.14.2; extra == "testing"
+Requires-Dist: tox==4.15.0; extra == "testing"
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.7.2&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.7.3&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
 [![Python 3.10 | 3.11 | 3.12 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![CodeQL](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
```

### Comparing `colorist-1.7.2/README.md` & `colorist-1.7.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.7.2&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.7.3&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
 [![Python 3.10 | 3.11 | 3.12 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![CodeQL](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
```

### Comparing `colorist-1.7.2/setup.cfg` & `colorist-1.7.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = colorist
-version = 1.7.2
+version = 1.7.3
 author = Jakob Bagterp
 author_email = jakob_bagterp@hotmail.com
 maintainer = Jakob Bagterp
 maintainer_email = jakob_bagterp@hotmail.com
 description = Colorist for Python
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
@@ -36,20 +36,20 @@
 packages = find:
 python_requires = >=3.10
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage==7.4.4
+	coverage==7.5.1
 	flake8==7.0.0
-	mypy==1.9.0
-	pytest==8.1.1
+	mypy==1.10.0
+	pytest==8.2.0
 	pytest-cov==5.0.0
-	tox==4.14.2
+	tox==4.15.0
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `colorist-1.7.2/src/colorist/__init__.py` & `colorist-1.7.3/src/colorist/__init__.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/constants/ansi.py` & `colorist-1.7.3/src/colorist/constants/ansi.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/helper/.coverage` & `colorist-1.7.3/src/colorist/helper/.coverage`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/helper/convert.py` & `colorist-1.7.3/src/colorist/helper/convert.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/helper/error.py` & `colorist-1.7.3/src/colorist/helper/error.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/helper/generate.py` & `colorist-1.7.3/src/colorist/helper/generate.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/helper/print.py` & `colorist-1.7.3/src/colorist/helper/print.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/README.MD` & `colorist-1.7.3/src/colorist/model/README.MD`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/abc/color.py` & `colorist-1.7.3/src/colorist/model/abc/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/abc/hex.py` & `colorist-1.7.3/src/colorist/model/abc/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/abc/hsl.py` & `colorist-1.7.3/src/colorist/model/abc/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/abc/rgb.py` & `colorist-1.7.3/src/colorist/model/abc/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/background/bright_color.py` & `colorist-1.7.3/src/colorist/model/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/background/color.py` & `colorist-1.7.3/src/colorist/model/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/background/hex.py` & `colorist-1.7.3/src/colorist/model/background/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/background/hsl.py` & `colorist-1.7.3/src/colorist/model/background/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/background/rgb.py` & `colorist-1.7.3/src/colorist/model/background/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/effect.py` & `colorist-1.7.3/src/colorist/model/effect.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/foreground/bright_color.py` & `colorist-1.7.3/src/colorist/model/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/foreground/color.py` & `colorist-1.7.3/src/colorist/model/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/foreground/hex.py` & `colorist-1.7.3/src/colorist/model/foreground/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/foreground/hsl.py` & `colorist-1.7.3/src/colorist/model/foreground/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/model/foreground/rgb.py` & `colorist-1.7.3/src/colorist/model/foreground/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/background/bright_color.py` & `colorist-1.7.3/src/colorist/print/background/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/background/color.py` & `colorist-1.7.3/src/colorist/print/background/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/background/hex.py` & `colorist-1.7.3/src/colorist/print/background/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/background/hsl.py` & `colorist-1.7.3/src/colorist/print/background/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/background/rgb.py` & `colorist-1.7.3/src/colorist/print/background/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/foreground/bright_color.py` & `colorist-1.7.3/src/colorist/print/foreground/bright_color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/foreground/color.py` & `colorist-1.7.3/src/colorist/print/foreground/color.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/foreground/hex.py` & `colorist-1.7.3/src/colorist/print/foreground/hex.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/foreground/hsl.py` & `colorist-1.7.3/src/colorist/print/foreground/hsl.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/foreground/rgb.py` & `colorist-1.7.3/src/colorist/print/foreground/rgb.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist/print/general.py` & `colorist-1.7.3/src/colorist/print/general.py`

 * *Files identical despite different names*

### Comparing `colorist-1.7.2/src/colorist.egg-info/PKG-INFO` & `colorist-1.7.3/src/colorist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorist
-Version: 1.7.2
+Version: 1.7.3
 Summary: Colorist for Python
 Home-page: https://jakob-bagterp.github.io/colorist-for-python/
 Download-URL: https://pypi.org/project/colorist/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
@@ -21,22 +21,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Provides-Extra: testing
-Requires-Dist: coverage==7.4.4; extra == "testing"
+Requires-Dist: coverage==7.5.1; extra == "testing"
 Requires-Dist: flake8==7.0.0; extra == "testing"
-Requires-Dist: mypy==1.9.0; extra == "testing"
-Requires-Dist: pytest==8.1.1; extra == "testing"
+Requires-Dist: mypy==1.10.0; extra == "testing"
+Requires-Dist: pytest==8.2.0; extra == "testing"
 Requires-Dist: pytest-cov==5.0.0; extra == "testing"
-Requires-Dist: tox==4.14.2; extra == "testing"
+Requires-Dist: tox==4.15.0; extra == "testing"
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.7.2&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.7.3&color=yellowgreen)](https://github.com/jakob-bagterp/colorist-for-python/releases/latest)
 [![Python 3.10 | 3.11 | 3.12 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%20|%203.12%2B&color=blueviolet)](https://www.python.org)
 [![BSD-3-Clause license](https://img.shields.io/static/v1?label=license&message=BSD-3-Clause&color=blue)](https://github.com/jakob-bagterp/colorist-for-python/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/colorist-for-python/branch/master/graph/badge.svg?token=1E69VOP4ED)](https://codecov.io/gh/jakob-bagterp/colorist-for-python)
 [![CodeQL](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/colorist-for-python/actions/workflows/test.yml)
 [![Downloads](https://static.pepy.tech/badge/colorist)](https://pepy.tech/project/colorist)
```

### Comparing `colorist-1.7.2/src/colorist.egg-info/SOURCES.txt` & `colorist-1.7.3/src/colorist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

