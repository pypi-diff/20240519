# Comparing `tmp/qablet_contracts-0.2.1.tar.gz` & `tmp/qablet_contracts-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qablet_contracts-0.2.1.tar", last modified: Thu Apr 11 16:00:29 2024, max compression
+gzip compressed data, was "qablet_contracts-0.2.2.tar", last modified: Sun May 19 20:50:09 2024, max compression
```

## Comparing `qablet_contracts-0.2.1.tar` & `qablet_contracts-0.2.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.937814 qablet_contracts-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 16:00:29.937814 qablet_contracts-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/docs/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/docs/specifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/docs/specifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/bnd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bnd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bnd/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bnd/zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/bond/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bond/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/bond/zero.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.929814 qablet_contracts-0.2.1/qablet_contracts/eq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/autocall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/cliquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/eq/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts/equity/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/autocall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/cliquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/forward_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/rainbow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/equity/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/dcf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/swap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/ir/swaption.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts/rate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/rate/swaption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/qablet_contracts/timetable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/qablet_contracts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 16:00:29.000000 qablet_contracts-0.2.1/qablet_contracts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 16:00:29.937814 qablet_contracts-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:29.933814 qablet_contracts-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/test_equity.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-11 16:00:22.000000 qablet_contracts-0.2.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.045034 qablet_contracts-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-19 20:50:09.045034 qablet_contracts-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.033033 qablet_contracts-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.033033 qablet_contracts-0.2.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/docs/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.033033 qablet_contracts-0.2.2/docs/specifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/docs/specifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.037033 qablet_contracts-0.2.2/qablet_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.037033 qablet_contracts-0.2.2/qablet_contracts/bnd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/bnd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/bnd/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/bnd/zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.037033 qablet_contracts-0.2.2/qablet_contracts/bond/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/bond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/bond/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/bond/zero.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.037033 qablet_contracts-0.2.2/qablet_contracts/eq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8078 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/autocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/cliquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/eq/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.041033 qablet_contracts-0.2.2/qablet_contracts/equity/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/autocall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/cliquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/forward_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/equity/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.041033 qablet_contracts-0.2.2/qablet_contracts/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/ir/dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/ir/swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/ir/swaption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.041033 qablet_contracts-0.2.2/qablet_contracts/rate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/rate/swaption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/qablet_contracts/timetable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.041033 qablet_contracts-0.2.2/qablet_contracts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-19 20:50:08.000000 qablet_contracts-0.2.2/qablet_contracts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-19 20:50:09.000000 qablet_contracts-0.2.2/qablet_contracts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:50:08.000000 qablet_contracts-0.2.2/qablet_contracts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-19 20:50:08.000000 qablet_contracts-0.2.2/qablet_contracts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 20:50:08.000000 qablet_contracts-0.2.2/qablet_contracts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-19 20:50:09.045034 qablet_contracts-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:09.041033 qablet_contracts-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/tests/test_equity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-19 20:50:00.000000 qablet_contracts-0.2.2/tests/test_schema.py
```

### Comparing `qablet_contracts-0.2.1/LICENSE` & `qablet_contracts-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/PKG-INFO` & `qablet_contracts-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qablet_contracts
-Version: 0.2.1
+Version: 0.2.2
 Summary: qablet_contracts created by qablet
 Home-page: https://github.com/qablet/qablet-contracts/
 Author: qablet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
 Requires-Dist: pandas
```

### Comparing `qablet_contracts-0.2.1/README.md` & `qablet_contracts-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/bnd/fixed.py` & `qablet_contracts-0.2.2/qablet_contracts/bnd/fixed.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/bnd/zero.py` & `qablet_contracts-0.2.2/qablet_contracts/bnd/zero.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/bond/fixed.py` & `qablet_contracts-0.2.2/qablet_contracts/bond/fixed.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/bond/zero.py` & `qablet_contracts-0.2.2/qablet_contracts/bond/zero.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/eq/barrier.py` & `qablet_contracts-0.2.2/qablet_contracts/eq/barrier.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/eq/cliquet.py` & `qablet_contracts-0.2.2/qablet_contracts/eq/cliquet.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 import pandas as pd
 
 from qablet_contracts.timetable import EventsMixin
 
 
 @dataclass
 class Accumulator(EventsMixin):
-    """In an **Accumulator** the returns over consecutive periods are
-
-    - subject to a local floor and cap
-    - accumulated by adding
-    - the accumulated payoff is subject to a global floor
+    """In an **Accumulator** the asset returns are calculated over a series of consecutive periods.
+    Each return is subject to a local floor and cap, then accumulated by adding, and finally the
+    accumulated payoff is subject to a global floor.
 
     Args:
         ccy: the currency of the bond.
         asset_name: the name of the underlying asset.
         fix_dates: the fixing times of the cliquet.
         global_floor: the global floor of the cliquet.
         local_floor: the local floor of the cliquet.
         local_cap: the local cap of the cliquet.
+        notional: the notional of the cliquet.
         track: an optional identifier for the contract.
 
     Examples:
         >>> fix_dates = pd.bdate_range(datetime(2021, 12, 31), datetime(2024, 12, 31), freq="2BQE")
         >>> tt = Accumulator("USD", "SPX", fix_dates, 0.0, -0.03, 0.05).timetable()
         >>> print(tt["events"].to_pandas())
           track                      time   op  quantity     unit
@@ -38,23 +37,24 @@
         1   NaN 2022-06-30 00:00:00+00:00  NaN       0.0  CALCFIX
         2   NaN 2022-12-30 00:00:00+00:00  NaN       0.0  CALCFIX
         3   NaN 2023-06-30 00:00:00+00:00  NaN       0.0  CALCFIX
         4   NaN 2023-12-29 00:00:00+00:00  NaN       0.0  CALCFIX
         5   NaN 2024-06-28 00:00:00+00:00  NaN       0.0  CALCFIX
         6   NaN 2024-12-31 00:00:00+00:00  NaN       0.0  CALCFIX
         7       2024-12-31 00:00:00+00:00    >       0.0      USD
-        8       2024-12-31 00:00:00+00:00    +       1.0      ACC
+        8       2024-12-31 00:00:00+00:00    +     100.0      ACC
     """
 
     ccy: str
     asset_name: str
     fix_dates: List[datetime]
     global_floor: float
     local_floor: float
     local_cap: float
+    notional: float = 100.0
     track: str = ""
     state: dict = field(default_factory=dict)
 
     def events(self):
         maturity = self.fix_dates[-1]
 
         events = [
@@ -86,15 +86,15 @@
             }
         )
         events.append(
             {
                 "track": self.track,
                 "time": maturity,
                 "op": "+",  # pay the accumulated amount
-                "quantity": 1,
+                "quantity": self.notional,
                 "unit": "ACC",
             }
         )
         return events
 
     def expressions(self):
         last_acc = self.state.get("ACC", 0.0)
```

### Comparing `qablet_contracts-0.2.1/qablet_contracts/eq/forward.py` & `qablet_contracts-0.2.2/qablet_contracts/eq/forward.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/eq/rainbow.py` & `qablet_contracts-0.2.2/qablet_contracts/eq/rainbow.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/eq/vanilla.py` & `qablet_contracts-0.2.2/qablet_contracts/eq/vanilla.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/equity/autocall.py` & `qablet_contracts-0.2.2/qablet_contracts/equity/autocall.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/equity/barrier.py` & `qablet_contracts-0.2.2/qablet_contracts/equity/barrier.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/equity/cliquet.py` & `qablet_contracts-0.2.2/qablet_contracts/equity/cliquet.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/equity/forward_start.py` & `qablet_contracts-0.2.2/qablet_contracts/equity/forward_start.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/equity/rainbow.py` & `qablet_contracts-0.2.2/qablet_contracts/equity/rainbow.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/equity/vanilla.py` & `qablet_contracts-0.2.2/qablet_contracts/equity/vanilla.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/ir/dcf.py` & `qablet_contracts-0.2.2/qablet_contracts/ir/dcf.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/ir/swap.py` & `qablet_contracts-0.2.2/qablet_contracts/ir/swap.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/ir/swaption.py` & `qablet_contracts-0.2.2/qablet_contracts/ir/swaption.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/rate/swaption.py` & `qablet_contracts-0.2.2/qablet_contracts/rate/swaption.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts/timetable.py` & `qablet_contracts-0.2.2/qablet_contracts/timetable.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/qablet_contracts.egg-info/PKG-INFO` & `qablet_contracts-0.2.2/qablet_contracts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qablet_contracts
-Version: 0.2.1
+Version: 0.2.2
 Summary: qablet_contracts created by qablet
 Home-page: https://github.com/qablet/qablet-contracts/
 Author: qablet
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyarrow
 Requires-Dist: pandas
```

### Comparing `qablet_contracts-0.2.1/qablet_contracts.egg-info/SOURCES.txt` & `qablet_contracts-0.2.2/qablet_contracts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/setup.py` & `qablet_contracts-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `qablet_contracts-0.2.1/tests/test_eq.py` & `qablet_contracts-0.2.2/tests/test_eq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from datetime import datetime
 
 import pandas as pd
 
-from qablet_contracts.eq.autocall import AutoCallable
+from qablet_contracts.eq.autocall import DiscountCert, ReverseCB
 from qablet_contracts.eq.barrier import OptionKO
 from qablet_contracts.eq.cliquet import Accumulator
 from qablet_contracts.eq.forward import ForwardOption
 
 
 def test_classes():
-    # Autocallable
+    # Autocallable Discount Certificate and Reverse Convertible
     start = datetime(2024, 3, 31)
     maturity = datetime(2024, 9, 30)
     barrier_dates = pd.date_range(
         start, maturity, freq="ME", inclusive="right"
     )
-    tt = AutoCallable(
+    tt = DiscountCert(
         "USD", "AAPL", 100, 80, start, maturity, 102, barrier_dates, 0.092
     ).timetable()
     assert len(tt["events"]) == 7
 
+    tt = ReverseCB(
+        "USD", "AAPL", 100, 80, start, maturity, 102, barrier_dates, 0.10
+    ).timetable()
+    assert len(tt["events"]) == 13
+
     # Barrier
     start = datetime(2024, 3, 31)
     maturity = datetime(2024, 9, 30)
     barrier_dates = pd.date_range(
         start, maturity, freq="ME", inclusive="right"
     )
     tt = OptionKO(
```

### Comparing `qablet_contracts-0.2.1/tests/test_equity.py` & `qablet_contracts-0.2.2/tests/test_equity.py`

 * *Files identical despite different names*

