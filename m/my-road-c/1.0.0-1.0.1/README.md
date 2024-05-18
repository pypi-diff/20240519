# Comparing `tmp/my_road_c-1.0.0.tar.gz` & `tmp/my_road_c-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_road_c-1.0.0.tar", last modified: Sat May 18 21:58:12 2024, max compression
+gzip compressed data, was "my_road_c-1.0.1.tar", last modified: Sat May 18 22:36:02 2024, max compression
```

## Comparing `my_road_c-1.0.0.tar` & `my_road_c-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 21:58:12.524791 my_road_c-1.0.0/
--rw-rw-rw-   0        0        0     1088 2024-05-18 21:54:26.000000 my_road_c-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      193 2024-05-18 21:58:12.523791 my_road_c-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       61 2024-05-18 21:51:20.000000 my_road_c-1.0.0/my_road.py
-drwxrwxrwx   0        0        0        0 2024-05-18 21:58:12.522791 my_road_c-1.0.0/my_road_c.egg-info/
--rw-rw-rw-   0        0        0      193 2024-05-18 21:58:12.000000 my_road_c-1.0.0/my_road_c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2024-05-18 21:58:12.000000 my_road_c-1.0.0/my_road_c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 21:58:12.000000 my_road_c-1.0.0/my_road_c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 21:58:12.000000 my_road_c-1.0.0/my_road_c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 21:58:12.524791 my_road_c-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      259 2024-05-18 21:58:09.000000 my_road_c-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:36:02.054833 my_road_c-1.0.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 21:54:26.000000 my_road_c-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      193 2024-05-18 22:36:02.053833 my_road_c-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-05-18 22:35:56.000000 my_road_c-1.0.1/my_road.py
+drwxrwxrwx   0        0        0        0 2024-05-18 22:36:02.052832 my_road_c-1.0.1/my_road_c.egg-info/
+-rw-rw-rw-   0        0        0      193 2024-05-18 22:36:02.000000 my_road_c-1.0.1/my_road_c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2024-05-18 22:36:02.000000 my_road_c-1.0.1/my_road_c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 22:36:02.000000 my_road_c-1.0.1/my_road_c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 22:36:02.000000 my_road_c-1.0.1/my_road_c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 22:36:02.055832 my_road_c-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      259 2024-05-18 22:35:56.000000 my_road_c-1.0.1/setup.py
```

### Comparing `my_road_c-1.0.0/LICENSE` & `my_road_c-1.0.1/LICENSE`

 * *Files identical despite different names*

