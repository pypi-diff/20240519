# Comparing `tmp/qrawl-0.2.2.tar.gz` & `tmp/qrawl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrawl-0.2.2.tar", max compression
+gzip compressed data, was "qrawl-0.2.3.tar", max compression
```

## Comparing `qrawl-0.2.2.tar` & `qrawl-0.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.2.2/LICENSE
--rw-r--r--   0        0        0      794 2024-05-16 00:48:12.094647 qrawl-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.2.2/qrawl/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.2.2/qrawl/common.py
--rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.2.2/qrawl/exceptions.py
--rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.2.2/qrawl/google_sheets/__init__.py
--rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.2.2/qrawl/google_sheets/column.py
--rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.2.2/qrawl/playwright/async_api/__init__.py
--rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.2.2/qrawl/playwright/async_api/async_playwright.py
--rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.2.2/qrawl/playwright/async_api/common.py
--rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.2.2/qrawl/playwright/sync_api/__init__.py
--rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.2.2/qrawl/playwright/sync_api/common.py
--rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.2.2/qrawl/playwright/sync_api/sync_playwright.py
--rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.2.2/qrawl/scrapy/__init__.py
--rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.2.2/qrawl/selenium/__init__.py
--rw-r--r--   0        0        0     7026 2024-05-05 01:32:19.143557 qrawl-0.2.2/qrawl/selenium/browsermob_proxy_wrapper.py
--rw-r--r--   0        0        0     2034 2024-05-16 00:47:46.260772 qrawl-0.2.2/qrawl/selenium/exceptions.py
--rw-r--r--   0        0        0    14837 2024-05-16 00:47:12.978008 qrawl-0.2.2/qrawl/selenium/selenium.py
--rw-r--r--   0        0        0     2870 2024-05-15 22:58:40.129052 qrawl-0.2.2/qrawl/selenium/wait.py
--rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.2.2/qrawl/xpath.py
--rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.2.2/README.md
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 20:13:30.588327 qrawl-0.2.3/LICENSE
+-rw-r--r--   0        0        0      794 2024-05-19 04:48:15.161551 qrawl-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-09 08:01:21.111154 qrawl-0.2.3/qrawl/__init__.py
+-rw-r--r--   0        0        0     1267 2024-04-09 07:59:51.136473 qrawl-0.2.3/qrawl/common.py
+-rw-r--r--   0        0        0      322 2024-05-01 06:43:35.164934 qrawl-0.2.3/qrawl/exceptions.py
+-rw-r--r--   0        0        0       28 2024-04-05 07:23:15.121016 qrawl-0.2.3/qrawl/google_sheets/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-10 20:17:48.321751 qrawl-0.2.3/qrawl/google_sheets/column.py
+-rw-r--r--   0        0        0       56 2024-04-09 23:05:42.684682 qrawl-0.2.3/qrawl/playwright/async_api/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-10 20:18:37.778395 qrawl-0.2.3/qrawl/playwright/async_api/async_playwright.py
+-rw-r--r--   0        0        0      663 2024-04-05 06:47:08.312708 qrawl-0.2.3/qrawl/playwright/async_api/common.py
+-rw-r--r--   0        0        0       55 2024-04-09 23:05:16.406743 qrawl-0.2.3/qrawl/playwright/sync_api/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-09 23:01:33.394056 qrawl-0.2.3/qrawl/playwright/sync_api/common.py
+-rw-r--r--   0        0        0     3933 2024-04-11 06:02:26.308965 qrawl-0.2.3/qrawl/playwright/sync_api/sync_playwright.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:46:13.447864 qrawl-0.2.3/qrawl/scrapy/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-10 20:18:05.787009 qrawl-0.2.3/qrawl/selenium/__init__.py
+-rw-r--r--   0        0        0     7026 2024-05-05 01:32:19.143557 qrawl-0.2.3/qrawl/selenium/browsermob_proxy_wrapper.py
+-rw-r--r--   0        0        0     2034 2024-05-16 00:47:46.260772 qrawl-0.2.3/qrawl/selenium/exceptions.py
+-rw-r--r--   0        0        0    14837 2024-05-16 00:47:12.978008 qrawl-0.2.3/qrawl/selenium/selenium.py
+-rw-r--r--   0        0        0     4508 2024-05-19 04:45:34.908327 qrawl-0.2.3/qrawl/selenium/wait.py
+-rw-r--r--   0        0        0     1321 2024-04-05 07:18:07.077122 qrawl-0.2.3/qrawl/xpath.py
+-rw-r--r--   0        0        0       37 2024-04-10 20:13:30.588327 qrawl-0.2.3/README.md
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 qrawl-0.2.3/PKG-INFO
```

### Comparing `qrawl-0.2.2/LICENSE` & `qrawl-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/pyproject.toml` & `qrawl-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qrawl"
-version = "0.2.2"
+version = "0.2.3"
 description = "Python Crawling Utilities."
 authors = ["GGLionCross"]
 license = "Apache 2.0"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `qrawl-0.2.2/qrawl/common.py` & `qrawl-0.2.3/qrawl/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/google_sheets/column.py` & `qrawl-0.2.3/qrawl/google_sheets/column.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/playwright/async_api/async_playwright.py` & `qrawl-0.2.3/qrawl/playwright/async_api/async_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/playwright/async_api/common.py` & `qrawl-0.2.3/qrawl/playwright/async_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/playwright/sync_api/common.py` & `qrawl-0.2.3/qrawl/playwright/sync_api/common.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/playwright/sync_api/sync_playwright.py` & `qrawl-0.2.3/qrawl/playwright/sync_api/sync_playwright.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/selenium/browsermob_proxy_wrapper.py` & `qrawl-0.2.3/qrawl/selenium/browsermob_proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/selenium/exceptions.py` & `qrawl-0.2.3/qrawl/selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/selenium/selenium.py` & `qrawl-0.2.3/qrawl/selenium/selenium.py`

 * *Files identical despite different names*

### Comparing `qrawl-0.2.2/qrawl/xpath.py` & `qrawl-0.2.3/qrawl/xpath.py`

 * *Files identical despite different names*

