# Comparing `tmp/psgr-0.2.0.tar.gz` & `tmp/psgr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psgr-0.2.0.tar", last modified: Sat May 18 10:09:51 2024, max compression
+gzip compressed data, was "psgr-0.2.1.tar", last modified: Sat May 18 14:43:45 2024, max compression
```

## Comparing `psgr-0.2.0.tar` & `psgr-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 10:09:51.690371 psgr-0.2.0/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-18 10:09:51.690371 psgr-0.2.0/PKG-INFO
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 10:09:51.690371 psgr-0.2.0/psgr/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-05-18 09:54:37.000000 psgr-0.2.0/psgr/__init__.py
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)    11045 2024-05-18 10:09:48.000000 psgr-0.2.0/psgr/main.py
-drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 10:09:51.690371 psgr-0.2.0/psgr.egg-info/
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/PKG-INFO
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/SOURCES.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/dependency_links.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       65 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/entry_points.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       24 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/requires.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-18 10:09:51.000000 psgr-0.2.0/psgr.egg-info/top_level.txt
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-18 10:09:51.690371 psgr-0.2.0/setup.cfg
--rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      485 2024-05-18 09:51:59.000000 psgr-0.2.0/setup.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 14:43:45.871445 psgr-0.2.1/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-18 14:43:45.871445 psgr-0.2.1/PKG-INFO
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 14:43:45.871445 psgr-0.2.1/psgr/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       19 2024-05-18 09:54:37.000000 psgr-0.2.1/psgr/__init__.py
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)    17963 2024-05-18 14:43:42.000000 psgr-0.2.1/psgr/main.py
+drwxr-xr-x   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        0 2024-05-18 14:43:45.871445 psgr-0.2.1/psgr.egg-info/
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      161 2024-05-18 14:43:45.000000 psgr-0.2.1/psgr.egg-info/PKG-INFO
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      208 2024-05-18 14:43:45.000000 psgr-0.2.1/psgr.egg-info/SOURCES.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        1 2024-05-18 14:43:45.000000 psgr-0.2.1/psgr.egg-info/dependency_links.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       65 2024-05-18 14:43:45.000000 psgr-0.2.1/psgr.egg-info/entry_points.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       24 2024-05-18 14:43:45.000000 psgr-0.2.1/psgr.egg-info/requires.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)        5 2024-05-18 14:43:45.000000 psgr-0.2.1/psgr.egg-info/top_level.txt
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)       38 2024-05-18 14:43:45.871445 psgr-0.2.1/setup.cfg
+-rw-r--r--   0 nareshkarthigeyan  (1000) nareshkarthigeyan  (1000)      485 2024-05-18 11:54:48.000000 psgr-0.2.1/setup.py
```

