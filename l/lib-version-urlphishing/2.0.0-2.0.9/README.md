# Comparing `tmp/lib_version_urlphishing-2.0.0.tar.gz` & `tmp/lib_version_urlphishing-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_urlphishing-2.0.0.tar", last modified: Mon May 13 18:01:14 2024, max compression
+gzip compressed data, was "lib_version_urlphishing-2.0.9.tar", max compression
```

## Comparing `lib_version_urlphishing-2.0.0.tar` & `lib_version_urlphishing-2.0.9.tar`

### file list

```diff
@@ -1,17 +1,6 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:01:14.343223 lib_version_urlphishing-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 18:01:14.343223 lib_version_urlphishing-2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:01:14.339223 lib_version_urlphishing-2.0.0/lib_version_URLPhishing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:01:14.343223 lib_version_urlphishing-2.0.0/lib_version_URLPhishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 18:01:14.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 18:01:14.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:01:14.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 18:01:14.000000 lib_version_urlphishing-2.0.0/lib_version_URLPhishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:01:14.343223 lib_version_urlphishing-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:01:14.339223 lib_version_urlphishing-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-13 18:01:00.000000 lib_version_urlphishing-2.0.0/tests/test_version_util.py
+-rw-r--r--   0        0        0      348 2024-05-19 14:37:47.442158 lib_version_urlphishing-2.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 14:37:47.442158 lib_version_urlphishing-2.0.9/lib_version_URLPhishing/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-19 14:37:47.442158 lib_version_urlphishing-2.0.9/lib_version_URLPhishing/version.py
+-rw-r--r--   0        0        0      122 2024-05-19 14:37:47.442158 lib_version_urlphishing-2.0.9/lib_version_URLPhishing/version_util.py
+-rw-r--r--   0        0        0      822 2024-05-19 14:38:02.198195 lib_version_urlphishing-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1182 1970-01-01 00:00:00.000000 lib_version_urlphishing-2.0.9/PKG-INFO
```

