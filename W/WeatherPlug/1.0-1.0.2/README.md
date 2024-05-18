# Comparing `tmp/weatherplug-1.0.tar.gz` & `tmp/weatherplug-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weatherplug-1.0.tar", last modified: Sat May 18 20:35:55 2024, max compression
+gzip compressed data, was "weatherplug-1.0.2.tar", last modified: Sat May 18 20:55:48 2024, max compression
```

## Comparing `weatherplug-1.0.tar` & `weatherplug-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 entity    (1000) entity    (1000)        0 2024-05-18 20:35:55.480799 weatherplug-1.0/
-drwxrwxr-x   0 entity    (1000) entity    (1000)        0 2024-05-18 20:35:55.480799 weatherplug-1.0/GetWeather/
--rw-rw-r--   0 entity    (1000) entity    (1000)      468 2024-05-18 20:27:53.000000 weatherplug-1.0/GetWeather/Main.py
--rw-rw-r--   0 entity    (1000) entity    (1000)       29 2024-05-18 17:17:17.000000 weatherplug-1.0/GetWeather/__init__.py
--rw-r--r--   0 entity    (1000) entity    (1000)       85 2024-05-18 20:35:55.480799 weatherplug-1.0/PKG-INFO
--rw-rw-r--   0 entity    (1000) entity    (1000)      292 2024-05-18 17:01:03.000000 weatherplug-1.0/README.md
-drwxrwxr-x   0 entity    (1000) entity    (1000)        0 2024-05-18 20:35:55.480799 weatherplug-1.0/WeatherPlug.egg-info/
--rw-r--r--   0 entity    (1000) entity    (1000)       85 2024-05-18 20:35:55.000000 weatherplug-1.0/WeatherPlug.egg-info/PKG-INFO
--rw-rw-r--   0 entity    (1000) entity    (1000)      234 2024-05-18 20:35:55.000000 weatherplug-1.0/WeatherPlug.egg-info/SOURCES.txt
--rw-rw-r--   0 entity    (1000) entity    (1000)        1 2024-05-18 20:35:55.000000 weatherplug-1.0/WeatherPlug.egg-info/dependency_links.txt
--rw-rw-r--   0 entity    (1000) entity    (1000)       17 2024-05-18 20:35:55.000000 weatherplug-1.0/WeatherPlug.egg-info/requires.txt
--rw-rw-r--   0 entity    (1000) entity    (1000)       11 2024-05-18 20:35:55.000000 weatherplug-1.0/WeatherPlug.egg-info/top_level.txt
--rw-rw-r--   0 entity    (1000) entity    (1000)       38 2024-05-18 20:35:55.480799 weatherplug-1.0/setup.cfg
--rw-rw-r--   0 entity    (1000) entity    (1000)      192 2024-05-18 20:34:17.000000 weatherplug-1.0/setup.py
+drwxrwxr-x   0 entity    (1000) entity    (1000)        0 2024-05-18 20:55:48.285292 weatherplug-1.0.2/
+-rw-r--r--   0 entity    (1000) entity    (1000)       87 2024-05-18 20:55:48.285292 weatherplug-1.0.2/PKG-INFO
+drwxrwxr-x   0 entity    (1000) entity    (1000)        0 2024-05-18 20:55:48.281293 weatherplug-1.0.2/WeatherPlug/
+-rw-rw-r--   0 entity    (1000) entity    (1000)      475 2024-05-18 20:55:42.000000 weatherplug-1.0.2/WeatherPlug/Main.py
+-rw-rw-r--   0 entity    (1000) entity    (1000)       30 2024-05-18 20:55:45.000000 weatherplug-1.0.2/WeatherPlug/__init__.py
+drwxrwxr-x   0 entity    (1000) entity    (1000)        0 2024-05-18 20:55:48.281293 weatherplug-1.0.2/WeatherPlug.egg-info/
+-rw-r--r--   0 entity    (1000) entity    (1000)       87 2024-05-18 20:55:48.000000 weatherplug-1.0.2/WeatherPlug.egg-info/PKG-INFO
+-rw-rw-r--   0 entity    (1000) entity    (1000)      226 2024-05-18 20:55:48.000000 weatherplug-1.0.2/WeatherPlug.egg-info/SOURCES.txt
+-rw-rw-r--   0 entity    (1000) entity    (1000)        1 2024-05-18 20:55:48.000000 weatherplug-1.0.2/WeatherPlug.egg-info/dependency_links.txt
+-rw-rw-r--   0 entity    (1000) entity    (1000)       17 2024-05-18 20:55:48.000000 weatherplug-1.0.2/WeatherPlug.egg-info/requires.txt
+-rw-rw-r--   0 entity    (1000) entity    (1000)       12 2024-05-18 20:55:48.000000 weatherplug-1.0.2/WeatherPlug.egg-info/top_level.txt
+-rw-rw-r--   0 entity    (1000) entity    (1000)       38 2024-05-18 20:55:48.285292 weatherplug-1.0.2/setup.cfg
+-rw-rw-r--   0 entity    (1000) entity    (1000)      209 2024-05-18 20:55:33.000000 weatherplug-1.0.2/setup.py
```

