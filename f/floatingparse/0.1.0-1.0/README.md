# Comparing `tmp/floatingparse-0.1.0.tar.gz` & `tmp/floatingparse-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floatingparse-0.1.0.tar", max compression
+gzip compressed data, was "floatingparse-1.0.tar", last modified: Sun May 19 15:07:27 2024, max compression
```

## Comparing `floatingparse-0.1.0.tar` & `floatingparse-1.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0      252 2024-05-19 14:49:27.153521 floatingparse-0.1.0/floatingparse/__init__.py
--rw-r--r--   0        0        0      113 2023-12-03 17:17:31.678327 floatingparse-0.1.0/floatingparse/config.json
--rw-r--r--   0        0        0     1520 2024-05-11 18:43:23.787881 floatingparse-0.1.0/floatingparse/floating_mail_sender.py
--rw-r--r--   0        0        0     1430 2024-05-11 18:38:32.372891 floatingparse-0.1.0/floatingparse/floating_parser.py
--rw-r--r--   0        0        0     5526 2024-05-11 18:38:03.184002 floatingparse-0.1.0/floatingparse/floating_statistics.py
--rw-r--r--   0        0        0     4412 2024-05-11 18:43:08.697563 floatingparse-0.1.0/floatingparse/floating_visualizer.py
--rw-r--r--   0        0        0     3282 2024-05-11 19:28:20.695335 floatingparse-0.1.0/floatingparse/floating_web.py
--rw-r--r--   0        0        0     2472 2024-05-11 19:28:09.305087 floatingparse-0.1.0/floatingparse/main.py
--rw-r--r--   0        0        0      369 2024-05-19 14:50:31.861810 floatingparse-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       19 2023-12-03 17:16:13.285699 floatingparse-0.1.0/README.md
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 floatingparse-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-19 15:07:27.321830 floatingparse-1.0/
+-rw-rw-rw-   0        0        0      145 2024-05-19 15:07:27.321830 floatingparse-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-12-03 17:16:13.000000 floatingparse-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 15:07:27.303830 floatingparse-1.0/floatingparse/
+-rw-rw-rw-   0        0        0      252 2024-05-19 14:49:27.000000 floatingparse-1.0/floatingparse/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-11 18:43:23.000000 floatingparse-1.0/floatingparse/floating_mail_sender.py
+-rw-rw-rw-   0        0        0     1430 2024-05-11 18:38:32.000000 floatingparse-1.0/floatingparse/floating_parser.py
+-rw-rw-rw-   0        0        0     5526 2024-05-11 18:38:03.000000 floatingparse-1.0/floatingparse/floating_statistics.py
+-rw-rw-rw-   0        0        0     4412 2024-05-11 18:43:08.000000 floatingparse-1.0/floatingparse/floating_visualizer.py
+-rw-rw-rw-   0        0        0     3282 2024-05-11 19:28:20.000000 floatingparse-1.0/floatingparse/floating_web.py
+-rw-rw-rw-   0        0        0     2472 2024-05-11 19:28:09.000000 floatingparse-1.0/floatingparse/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 15:07:27.320830 floatingparse-1.0/floatingparse.egg-info/
+-rw-rw-rw-   0        0        0      145 2024-05-19 15:07:27.000000 floatingparse-1.0/floatingparse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2024-05-19 15:07:27.000000 floatingparse-1.0/floatingparse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 15:07:27.000000 floatingparse-1.0/floatingparse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-19 15:07:27.000000 floatingparse-1.0/floatingparse.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-05-19 15:07:27.000000 floatingparse-1.0/floatingparse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2024-05-19 14:50:31.000000 floatingparse-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 15:07:27.326830 floatingparse-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      246 2024-05-19 14:45:56.000000 floatingparse-1.0/setup.py
```

### Comparing `floatingparse-0.1.0/floatingparse/floating_mail_sender.py` & `floatingparse-1.0/floatingparse/floating_mail_sender.py`

 * *Files identical despite different names*

### Comparing `floatingparse-0.1.0/floatingparse/floating_parser.py` & `floatingparse-1.0/floatingparse/floating_parser.py`

 * *Files identical despite different names*

### Comparing `floatingparse-0.1.0/floatingparse/floating_statistics.py` & `floatingparse-1.0/floatingparse/floating_statistics.py`

 * *Files identical despite different names*

### Comparing `floatingparse-0.1.0/floatingparse/floating_visualizer.py` & `floatingparse-1.0/floatingparse/floating_visualizer.py`

 * *Files identical despite different names*

### Comparing `floatingparse-0.1.0/floatingparse/floating_web.py` & `floatingparse-1.0/floatingparse/floating_web.py`

 * *Files identical despite different names*

### Comparing `floatingparse-0.1.0/floatingparse/main.py` & `floatingparse-1.0/floatingparse/main.py`

 * *Files identical despite different names*

