# Comparing `tmp/otonagai_dl-1.0.5.tar.gz` & `tmp/otonagai_dl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otonagai_dl-1.0.5.tar", max compression
+gzip compressed data, was "otonagai_dl-1.0.6.tar", max compression
```

## Comparing `otonagai_dl-1.0.5.tar` & `otonagai_dl-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-05-18 19:18:50.337113 otonagai_dl-1.0.5/LICENSE
--rw-r--r--   0        0        0      226 2024-05-17 06:29:48.933720 otonagai_dl-1.0.5/otonagai_dl/main.py
--rw-r--r--   0        0        0        0 2024-05-07 09:23:59.995430 otonagai_dl-1.0.5/otonagai_dl/src/__init__.py
--rw-r--r--   0        0        0     8001 2024-05-18 20:10:54.421099 otonagai_dl-1.0.5/otonagai_dl/src/controller.py
--rw-r--r--   0        0        0        0 2024-05-07 09:25:40.767261 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/__init__.py
--rw-r--r--   0        0        0     1347 2024-05-17 05:46:07.038979 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py
--rw-r--r--   0        0        0     4383 2024-05-17 06:32:03.828672 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py
--rw-r--r--   0        0        0     2554 2024-05-15 10:46:22.439118 otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py
--rw-r--r--   0        0        0      380 2024-05-18 13:24:14.953354 otonagai_dl-1.0.5/otonagai_dl/src/log_system.py
--rw-r--r--   0        0        0     4103 2024-05-18 20:17:29.741962 otonagai_dl-1.0.5/otonagai_dl/src/menu.py
--rw-r--r--   0        0        0     9271 2024-05-18 19:42:05.305401 otonagai_dl-1.0.5/otonagai_dl/src/model.py
--rw-r--r--   0        0        0     3314 2024-05-18 20:16:26.731409 otonagai_dl-1.0.5/otonagai_dl/src/utils.py
--rw-r--r--   0        0        0     7860 2024-05-18 19:19:56.618750 otonagai_dl-1.0.5/otonagai_dl/src/view.py
--rw-r--r--   0        0        0      561 2024-05-18 19:50:44.829733 otonagai_dl-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      695 2024-05-17 06:43:17.878317 otonagai_dl-1.0.5/README.md
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 otonagai_dl-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-05-18 19:18:50.337113 otonagai_dl-1.0.6/LICENSE
+-rw-r--r--   0        0        0      226 2024-05-17 06:29:48.933720 otonagai_dl-1.0.6/otonagai_dl/main.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:23:59.995430 otonagai_dl-1.0.6/otonagai_dl/src/__init__.py
+-rw-r--r--   0        0        0     8001 2024-05-18 20:10:54.421099 otonagai_dl-1.0.6/otonagai_dl/src/controller.py
+-rw-r--r--   0        0        0        0 2024-05-07 09:25:40.767261 otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/__init__.py
+-rw-r--r--   0        0        0     1347 2024-05-17 05:46:07.038979 otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py
+-rw-r--r--   0        0        0     4383 2024-05-17 06:32:03.828672 otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py
+-rw-r--r--   0        0        0     2554 2024-05-15 10:46:22.439118 otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py
+-rw-r--r--   0        0        0      380 2024-05-18 13:24:14.953354 otonagai_dl-1.0.6/otonagai_dl/src/log_system.py
+-rw-r--r--   0        0        0     4103 2024-05-18 20:17:29.741962 otonagai_dl-1.0.6/otonagai_dl/src/menu.py
+-rw-r--r--   0        0        0     9271 2024-05-18 19:42:05.305401 otonagai_dl-1.0.6/otonagai_dl/src/model.py
+-rw-r--r--   0        0        0     3314 2024-05-18 20:16:26.731409 otonagai_dl-1.0.6/otonagai_dl/src/utils.py
+-rw-r--r--   0        0        0     7860 2024-05-18 19:19:56.618750 otonagai_dl-1.0.6/otonagai_dl/src/view.py
+-rw-r--r--   0        0        0      562 2024-05-19 10:49:07.777535 otonagai_dl-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1227 2024-05-18 20:42:10.851290 otonagai_dl-1.0.6/README.md
+-rw-r--r--   0        0        0     1931 1970-01-01 00:00:00.000000 otonagai_dl-1.0.6/PKG-INFO
```

### Comparing `otonagai_dl-1.0.5/LICENSE` & `otonagai_dl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/controller.py` & `otonagai_dl-1.0.6/otonagai_dl/src/controller.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py` & `otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/hlj_batch.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py` & `otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/hlj_dl.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py` & `otonagai_dl-1.0.6/otonagai_dl/src/hobby_link_jp_scraper/hlj_ui.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/menu.py` & `otonagai_dl-1.0.6/otonagai_dl/src/menu.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/model.py` & `otonagai_dl-1.0.6/otonagai_dl/src/model.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/utils.py` & `otonagai_dl-1.0.6/otonagai_dl/src/utils.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/otonagai_dl/src/view.py` & `otonagai_dl-1.0.6/otonagai_dl/src/view.py`

 * *Files identical despite different names*

### Comparing `otonagai_dl-1.0.5/pyproject.toml` & `otonagai_dl-1.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "otonagai-dl"
-version = "1.0.5"
+version = "1.0.6"
 description = "A basic CLI tool to keep track of your favourite anime/manga/comics/pop culture merchandise"
 authors = ["Clavin Dsouza <clavind12@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 rich = "^13.7.1"
 beautifulsoup4 = "^4.12.3"
 inquirerpy = "0.3.4"
 readchar = "*"
 requests = "^2.31.0"
 
 [build-system]
```

