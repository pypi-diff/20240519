# Comparing `tmp/budgeteer-0.1.2.tar.gz` & `tmp/budgeteer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgeteer-0.1.2.tar", last modified: Sat Aug  5 10:00:39 2023, max compression
+gzip compressed data, was "budgeteer-0.1.3.tar", last modified: Sun May 19 11:00:53 2024, max compression
```

## Comparing `budgeteer-0.1.2.tar` & `budgeteer-0.1.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.301003 budgeteer-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-05 10:00:19.000000 budgeteer-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 10:00:19.000000 budgeteer-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-05 10:00:39.301003 budgeteer-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-08-05 10:00:19.000000 budgeteer-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.285003 budgeteer-0.1.2/budgeteer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/budget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.289003 budgeteer-0.1.2/budgeteer/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.293003 budgeteer-0.1.2/budgeteer/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.293003 budgeteer-0.1.2/budgeteer/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.285003 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.293003 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.301003 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    85787 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20752 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
--rw-r--r--   0 runner    (1001) docker     (123)    64371 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
--rw-r--r--   0 runner    (1001) docker     (123)    28960 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
--rw-r--r--   0 runner    (1001) docker     (123)   231964 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
--rw-r--r--   0 runner    (1001) docker     (123)    60654 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76081 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22835 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
--rw-r--r--   0 runner    (1001) docker     (123)    51150 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-05 10:00:38.000000 budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-08-05 10:00:19.000000 budgeteer-0.1.2/budgeteer/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:00:39.289003 budgeteer-0.1.2/budgeteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 10:00:39.000000 budgeteer-0.1.2/budgeteer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:00:39.301003 budgeteer-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-05 10:00:19.000000 budgeteer-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.356775 budgeteer-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-19 11:00:35.000000 budgeteer-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-19 11:00:35.000000 budgeteer-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-19 11:00:53.356775 budgeteer-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-19 11:00:35.000000 budgeteer-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.348775 budgeteer-0.1.3/budgeteer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.352775 budgeteer-0.1.3/budgeteer/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.352775 budgeteer-0.1.3/budgeteer/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/providers/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.352775 budgeteer-0.1.3/budgeteer/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.348775 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.352775 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.356775 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    85787 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20752 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    64371 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js
+-rw-r--r--   0 runner    (1001) docker     (127)   231964 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css
+-rw-r--r--   0 runner    (1001) docker     (127)    60654 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js
+-rw-r--r--   0 runner    (1001) docker     (127)   164360 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76081 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css
+-rw-r--r--   0 runner    (1001) docker     (127)   121340 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    24455 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22835 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51150 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11521 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-19 11:00:52.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-05-19 11:00:35.000000 budgeteer-0.1.3/budgeteer/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:00:53.348775 budgeteer-0.1.3/budgeteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:00:53.000000 budgeteer-0.1.3/budgeteer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:00:53.356775 budgeteer-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-19 11:00:35.000000 budgeteer-0.1.3/setup.py
```

### Comparing `budgeteer-0.1.2/LICENSE.md` & `budgeteer-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/PKG-INFO` & `budgeteer-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: budgeteer
-Version: 0.1.2
-Summary: Einfacher Überblick über das eigene Budget
-Home-page: https://github.com/rix1337/BudgeTeer
-Author: rix1337
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # BudgeTeer
 
 <img src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 Einfacher Überblick über das eigene Budget 
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/BudgeTeer/CreateRelease.yml?branch=main)](https://github.com/rix1337/BudgeTeer/actions/workflows/CreateRelease.yml)
@@ -64,22 +49,36 @@
 
 ### Start
 
 ```budgeteer``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
 ### [Docker Image](https://hub.docker.com/r/rix1337/docker-budgeteer/)
 
+```
+docker run -d \
+  --name="BudgeTeer" \
+  -p port:2808 \
+  -v /path/to/config/:/config:rw \
+  --log-opt max-size=50m \
+  rix1337/docker-budgeteer
+  ```
+
 * Der Betrieb als Docker-Container empfiehlt sich als Standardinstallation - vor allem für NAS-Systeme, Homeserver und
   sonstige Geräte die dauerhaft und möglichst wartungsfrei (headless) betrieben werden sollen.
 * Bei jedem Release wird ein getaggtes Image erstellt. Damit kann man auf der Wunschversion verbleiben oder im Falle
   eines Bugs zu einer stabilen Version zurück kehren.
 * Um immer auf dem aktuellen Stand zu sein, einfach das mit `latest` getaggte Image nutzen.
 * Für UNRAID-Server kann das Image direkt über die Community Applications bezogen und der Container so eingerichtet
   werden.
 
+Das Image `rix1377/docker-budgeteer` wird standardmäßig auf das `:latest`-Tag aufgelöst. Dieses wird mit jedem Release auf die neue Version aktualisiert. Mit jedem Release wird ebenfalls eine getaggte Version des Images erzeugt. Auf letztere kann man wechseln, um beispielsweise bei Fehlern in der neuen Version auf einen funktionierenden Stand zurück zu kehren.
+
+Beispiel:
+
+`docker pull rix1337/docker-budgeteer:0.0.2`
+
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/BudgeTeer/releases) wird eine selbstständig unter Windows lauffähige
   Version des BudgeTeers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
-* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
-
+* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
```

### Comparing `budgeteer-0.1.2/README.md` & `budgeteer-0.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: budgeteer
+Version: 0.1.3
+Summary: Einfacher Überblick über das eigene Budget
+Home-page: https://github.com/rix1337/BudgeTeer
+Author: rix1337
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # BudgeTeer
 
 <img src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" data-canonical-src="https://raw.githubusercontent.com/rix1337/BudgeTeer/main/budgeteer/web_interface/vuejs_frontend/public/favicon.ico" width="64" height="64" />
 
 Einfacher Überblick über das eigene Budget 
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rix1337/BudgeTeer/CreateRelease.yml?branch=main)](https://github.com/rix1337/BudgeTeer/actions/workflows/CreateRelease.yml)
@@ -49,21 +64,37 @@
 
 ### Start
 
 ```budgeteer``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
 ### [Docker Image](https://hub.docker.com/r/rix1337/docker-budgeteer/)
 
+```
+docker run -d \
+  --name="BudgeTeer" \
+  -p port:2808 \
+  -v /path/to/config/:/config:rw \
+  --log-opt max-size=50m \
+  rix1337/docker-budgeteer
+  ```
+
 * Der Betrieb als Docker-Container empfiehlt sich als Standardinstallation - vor allem für NAS-Systeme, Homeserver und
   sonstige Geräte die dauerhaft und möglichst wartungsfrei (headless) betrieben werden sollen.
 * Bei jedem Release wird ein getaggtes Image erstellt. Damit kann man auf der Wunschversion verbleiben oder im Falle
   eines Bugs zu einer stabilen Version zurück kehren.
 * Um immer auf dem aktuellen Stand zu sein, einfach das mit `latest` getaggte Image nutzen.
 * Für UNRAID-Server kann das Image direkt über die Community Applications bezogen und der Container so eingerichtet
   werden.
 
+Das Image `rix1377/docker-budgeteer` wird standardmäßig auf das `:latest`-Tag aufgelöst. Dieses wird mit jedem Release auf die neue Version aktualisiert. Mit jedem Release wird ebenfalls eine getaggte Version des Images erzeugt. Auf letztere kann man wechseln, um beispielsweise bei Fehlern in der neuen Version auf einen funktionierenden Stand zurück zu kehren.
+
+Beispiel:
+
+`docker pull rix1337/docker-budgeteer:0.0.2`
+
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/BudgeTeer/releases) wird eine selbstständig unter Windows lauffähige
   Version des BudgeTeers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
-* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
+* Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
+
```

### Comparing `budgeteer-0.1.2/budgeteer/budget.py` & `budgeteer-0.1.3/budgeteer/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from budgeteer.providers.config import BudgetConfig
 from budgeteer.providers.sqlite_database import remove_redundant_db_tables
 from budgeteer.web_interface.web_server import web_server
 
 version = "v." + version.get_version()
 
 
-def start_budgeteer():
+def main():
     with multiprocessing.Manager() as manager:
         shared_state_dict = manager.dict()
         shared_state_lock = manager.Lock()
         shared_state.set_state(shared_state_dict, shared_state_lock)
 
         parser = argparse.ArgumentParser()
         parser.add_argument("--log-level", help="Legt fest, wie genau geloggt wird (INFO, DEBUG)")
@@ -100,8 +100,8 @@
                 signal.pause()
         except AttributeError:
             while True:
                 time.sleep(1)
 
 
 if __name__ == "__main__":
-    start_budgeteer()
+    main()
```

### Comparing `budgeteer-0.1.2/budgeteer/providers/common_functions.py` & `budgeteer-0.1.3/budgeteer/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/config.py` & `budgeteer-0.1.3/budgeteer/providers/config.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/http_requests/cache_handler.py` & `budgeteer-0.1.3/budgeteer/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/http_requests/cloudflare_handlers.py` & `budgeteer-0.1.3/budgeteer/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/http_requests/request_handler.py` & `budgeteer-0.1.3/budgeteer/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/shared_state.py` & `budgeteer-0.1.3/budgeteer/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/sqlite_database.py` & `budgeteer-0.1.3/budgeteer/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/providers/version.py` & `budgeteer-0.1.3/budgeteer/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "0.1.2"
+    return "0.1.3"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@formkit-606708a1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@popperjs-8746c87e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@vue-de7d3d24.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/@vueuse-0fe84a4c.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/axios-4a70c6fc.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-39a9ac22.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-85852bd1.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-abbba2f8.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/index-9c267a1e.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/index-e2d31524.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-router-4cd13335.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-tippy-7086acf8.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vue-toastification-6aa87443.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/assets/vuex-636235de.js`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/vuejs_frontend/dist/index.html` & `budgeteer-0.1.3/budgeteer/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer/web_interface/web_server.py` & `budgeteer-0.1.3/budgeteer/web_interface/web_server.py`

 * *Files identical despite different names*

### Comparing `budgeteer-0.1.2/budgeteer.egg-info/PKG-INFO` & `budgeteer-0.1.3/budgeteer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgeteer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Einfacher Überblick über das eigene Budget
 Home-page: https://github.com/rix1337/BudgeTeer
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -64,22 +64,37 @@
 
 ### Start
 
 ```budgeteer``` in der Konsole (Python muss im System-PATH hinterlegt sein)
 
 ### [Docker Image](https://hub.docker.com/r/rix1337/docker-budgeteer/)
 
+```
+docker run -d \
+  --name="BudgeTeer" \
+  -p port:2808 \
+  -v /path/to/config/:/config:rw \
+  --log-opt max-size=50m \
+  rix1337/docker-budgeteer
+  ```
+
 * Der Betrieb als Docker-Container empfiehlt sich als Standardinstallation - vor allem für NAS-Systeme, Homeserver und
   sonstige Geräte die dauerhaft und möglichst wartungsfrei (headless) betrieben werden sollen.
 * Bei jedem Release wird ein getaggtes Image erstellt. Damit kann man auf der Wunschversion verbleiben oder im Falle
   eines Bugs zu einer stabilen Version zurück kehren.
 * Um immer auf dem aktuellen Stand zu sein, einfach das mit `latest` getaggte Image nutzen.
 * Für UNRAID-Server kann das Image direkt über die Community Applications bezogen und der Container so eingerichtet
   werden.
 
+Das Image `rix1377/docker-budgeteer` wird standardmäßig auf das `:latest`-Tag aufgelöst. Dieses wird mit jedem Release auf die neue Version aktualisiert. Mit jedem Release wird ebenfalls eine getaggte Version des Images erzeugt. Auf letztere kann man wechseln, um beispielsweise bei Fehlern in der neuen Version auf einen funktionierenden Stand zurück zu kehren.
+
+Beispiel:
+
+`docker pull rix1337/docker-budgeteer:0.0.2`
+
 ### Windows Build
 
 * Jedem [Release](https://github.com/rix1337/BudgeTeer/releases) wird eine selbstständig unter Windows lauffähige
   Version des BudgeTeers beigefügt.
 * Hierfür müssen weder Python, noch die Zusatzpakete installiert werden.
 * Einfach die jeweilige Exe herunterladen und ausführen bzw. bei Updates die Exe ersetzen.
```

### Comparing `budgeteer-0.1.2/budgeteer.egg-info/SOURCES.txt` & `budgeteer-0.1.3/budgeteer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 budgeteer/__init__.py
-budgeteer/budget.py
+budgeteer/run.py
 budgeteer.egg-info/PKG-INFO
 budgeteer.egg-info/SOURCES.txt
 budgeteer.egg-info/dependency_links.txt
 budgeteer.egg-info/entry_points.txt
 budgeteer.egg-info/not-zip-safe
 budgeteer.egg-info/requires.txt
 budgeteer.egg-info/top_level.txt
```

### Comparing `budgeteer-0.1.2/setup.py` & `budgeteer-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,11 +34,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'budgeteer = budgeteer.budget:start_budgeteer',
+            'budgeteer = budgeteer.run:main',
         ],
     },
 )
```

