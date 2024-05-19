# Comparing `tmp/ntdgotv_langtools-0.2.0.tar.gz` & `tmp/ntdgotv_langtools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdgotv_langtools-0.2.0.tar", last modified: Sat May 18 05:21:57 2024, max compression
+gzip compressed data, was "ntdgotv_langtools-0.2.1.tar", last modified: Sun May 19 05:32:33 2024, max compression
```

## Comparing `ntdgotv_langtools-0.2.0.tar` & `ntdgotv_langtools-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 05:21:57.734403 ntdgotv_langtools-0.2.0/
--rw-rw-rw-   0        0        0      274 2024-05-18 05:21:57.731411 ntdgotv_langtools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-05-17 17:44:40.000000 ntdgotv_langtools-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 05:21:57.713156 ntdgotv_langtools-0.2.0/ntdgotv_langtools/
--rw-rw-rw-   0        0        0      303 2024-05-18 05:16:55.000000 ntdgotv_langtools-0.2.0/ntdgotv_langtools/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-18 05:11:58.000000 ntdgotv_langtools-0.2.0/ntdgotv_langtools/main.py
-drwxrwxrwx   0        0        0        0 2024-05-18 05:21:57.728419 ntdgotv_langtools-0.2.0/ntdgotv_langtools.egg-info/
--rw-rw-rw-   0        0        0      274 2024-05-18 05:21:57.000000 ntdgotv_langtools-0.2.0/ntdgotv_langtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-18 05:21:57.000000 ntdgotv_langtools-0.2.0/ntdgotv_langtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 05:21:57.000000 ntdgotv_langtools-0.2.0/ntdgotv_langtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-18 05:21:57.000000 ntdgotv_langtools-0.2.0/ntdgotv_langtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 05:21:57.735914 ntdgotv_langtools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-05-18 05:21:36.000000 ntdgotv_langtools-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 05:32:33.818526 ntdgotv_langtools-0.2.1/
+-rw-rw-rw-   0        0        0     3946 2024-05-19 05:32:33.816563 ntdgotv_langtools-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-05-19 05:00:11.000000 ntdgotv_langtools-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 05:32:33.756930 ntdgotv_langtools-0.2.1/ntdgotv_langtools/
+-rw-rw-rw-   0        0        0      303 2024-05-19 05:00:11.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-19 05:00:11.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 05:32:33.797146 ntdgotv_langtools-0.2.1/ntdgotv_langtools.egg-info/
+-rw-rw-rw-   0        0        0     3946 2024-05-19 05:32:33.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-19 05:32:33.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 05:32:33.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1322 2024-05-19 05:32:33.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-19 05:32:33.000000 ntdgotv_langtools-0.2.1/ntdgotv_langtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 05:32:33.818526 ntdgotv_langtools-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-19 05:30:43.000000 ntdgotv_langtools-0.2.1/setup.py
```

