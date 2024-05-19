# Comparing `tmp/ObjectToString-0.2.70.tar.gz` & `tmp/ObjectToString-0.2.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ObjectToString-0.2.70.tar", last modified: Sun Apr 21 15:13:57 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "ObjectToString-0.2.71.tar", last modified: Sun May 19 08:20:03 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `ObjectToString-0.2.70.tar` & `ObjectToString-0.2.71.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.69/
--rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.69/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.69/objecttostring/
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.69/ObjectToString.egg-info/
--rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.69/ObjectToString.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.69/ObjectToString.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.69/ObjectToString.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.69/ObjectToString.egg-info/top_level.txt
--rwxrwxrwx   0        0        0  3709952 2024-04-20 15:20:43.000000 ObjectToString-0.2.69/objecttostring/pdslib.cp312-win_amd64.pyd
--rwxrwxrwx   0        0        0      100 2024-04-21 15:13:35.000000 ObjectToString-0.2.69/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.69/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.69/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.71/
+-rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.71/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.71/objecttostring/
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.71/ObjectToString.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.71/ObjectToString.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.71/ObjectToString.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.71/ObjectToString.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.71/ObjectToString.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0  3708928 2024-05-19 07:59:18.000000 ObjectToString-0.2.71/objecttostring/pdslib.cp312-win_amd64.pyd
+-rwxrwxrwx   0        0        0      100 2024-05-19 08:19:49.000000 ObjectToString-0.2.71/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.71/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.71/setup.py
```
