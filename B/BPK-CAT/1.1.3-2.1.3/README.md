# Comparing `tmp/BPK-CAT-1.1.3.tar.gz` & `tmp/BPK-CAT-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BPK-CAT-1.1.3.tar", last modified: Sun May 19 13:10:45 2024, max compression
+gzip compressed data, was "BPK-CAT-2.1.3.tar", last modified: Sun May 19 13:35:12 2024, max compression
```

## Comparing `BPK-CAT-1.1.3.tar` & `BPK-CAT-2.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:10:45.537352 BPK-CAT-1.1.3/
-drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:10:45.537352 BPK-CAT-1.1.3/BPK_CAT.egg-info/
--rw-r--r--   0 deviardn  (1000) deviardn  (1000)      199 2024-05-19 13:10:45.000000 BPK-CAT-1.1.3/BPK_CAT.egg-info/PKG-INFO
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)      275 2024-05-19 13:10:45.000000 BPK-CAT-1.1.3/BPK_CAT.egg-info/SOURCES.txt
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)        1 2024-05-19 13:10:45.000000 BPK-CAT-1.1.3/BPK_CAT.egg-info/dependency_links.txt
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)       34 2024-05-19 13:10:45.000000 BPK-CAT-1.1.3/BPK_CAT.egg-info/entry_points.txt
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)        7 2024-05-19 13:10:45.000000 BPK-CAT-1.1.3/BPK_CAT.egg-info/top_level.txt
--rw-r--r--   0 deviardn  (1000) deviardn  (1000)      199 2024-05-19 13:10:45.537352 BPK-CAT-1.1.3/PKG-INFO
-drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:10:45.537352 BPK-CAT-1.1.3/bpkcat/
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     1593 2024-05-19 13:10:29.000000 BPK-CAT-1.1.3/bpkcat/OWSequenceChecker.py
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)       43 2024-05-19 09:49:36.000000 BPK-CAT-1.1.3/bpkcat/__init__.py
-drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:10:45.537352 BPK-CAT-1.1.3/bpkcat/icons/
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     1143 2024-05-19 09:31:52.000000 BPK-CAT-1.1.3/bpkcat/icons/1.svg
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     1919 2024-05-19 09:31:58.000000 BPK-CAT-1.1.3/bpkcat/icons/2.svg
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     3737 2024-05-19 09:51:01.000000 BPK-CAT-1.1.3/bpkcat/icons/bpkcat.svg
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)       38 2024-05-19 13:10:45.537352 BPK-CAT-1.1.3/setup.cfg
--rw-rw-r--   0 deviardn  (1000) deviardn  (1000)      634 2024-05-19 13:10:00.000000 BPK-CAT-1.1.3/setup.py
+drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:35:12.650686 BPK-CAT-2.1.3/
+drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:35:12.650686 BPK-CAT-2.1.3/BPK_CAT.egg-info/
+-rw-r--r--   0 deviardn  (1000) deviardn  (1000)      199 2024-05-19 13:35:12.000000 BPK-CAT-2.1.3/BPK_CAT.egg-info/PKG-INFO
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)      304 2024-05-19 13:35:12.000000 BPK-CAT-2.1.3/BPK_CAT.egg-info/SOURCES.txt
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)        1 2024-05-19 13:35:12.000000 BPK-CAT-2.1.3/BPK_CAT.egg-info/dependency_links.txt
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)       34 2024-05-19 13:35:12.000000 BPK-CAT-2.1.3/BPK_CAT.egg-info/entry_points.txt
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)        7 2024-05-19 13:35:12.000000 BPK-CAT-2.1.3/BPK_CAT.egg-info/top_level.txt
+-rw-r--r--   0 deviardn  (1000) deviardn  (1000)      199 2024-05-19 13:35:12.650686 BPK-CAT-2.1.3/PKG-INFO
+drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:35:12.650686 BPK-CAT-2.1.3/bpkcat/
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     2353 2024-05-19 13:32:10.000000 BPK-CAT-2.1.3/bpkcat/OWDuplicateChecker.py
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     1593 2024-05-19 13:10:29.000000 BPK-CAT-2.1.3/bpkcat/OWSequenceChecker.py
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)       43 2024-05-19 09:49:36.000000 BPK-CAT-2.1.3/bpkcat/__init__.py
+drwxrwxr-x   0 deviardn  (1000) deviardn  (1000)        0 2024-05-19 13:35:12.650686 BPK-CAT-2.1.3/bpkcat/icons/
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     1143 2024-05-19 09:31:52.000000 BPK-CAT-2.1.3/bpkcat/icons/1.svg
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     1919 2024-05-19 09:31:58.000000 BPK-CAT-2.1.3/bpkcat/icons/2.svg
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)     3737 2024-05-19 09:51:01.000000 BPK-CAT-2.1.3/bpkcat/icons/bpkcat.svg
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)       38 2024-05-19 13:35:12.650686 BPK-CAT-2.1.3/setup.cfg
+-rw-rw-r--   0 deviardn  (1000) deviardn  (1000)      634 2024-05-19 13:34:37.000000 BPK-CAT-2.1.3/setup.py
```

### Comparing `BPK-CAT-1.1.3/bpkcat/OWSequenceChecker.py` & `BPK-CAT-2.1.3/bpkcat/OWSequenceChecker.py`

 * *Files identical despite different names*

### Comparing `BPK-CAT-1.1.3/bpkcat/icons/1.svg` & `BPK-CAT-2.1.3/bpkcat/icons/1.svg`

 * *Files identical despite different names*

### Comparing `BPK-CAT-1.1.3/bpkcat/icons/2.svg` & `BPK-CAT-2.1.3/bpkcat/icons/2.svg`

 * *Files identical despite different names*

### Comparing `BPK-CAT-1.1.3/bpkcat/icons/bpkcat.svg` & `BPK-CAT-2.1.3/bpkcat/icons/bpkcat.svg`

 * *Files identical despite different names*

### Comparing `BPK-CAT-1.1.3/setup.py` & `BPK-CAT-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 NAME="BPK-CAT"
-MAYOR=1 
+MAYOR=2 
 MINOR=1
 PATCH=3
 VERSION= '%d.%d.%d' % (MAYOR, MINOR, PATCH)
 
 DESCRIPTION="Orange3 BPK Computer Assisted Audit Technique Tools (CAATT)"
 AUTHOR="BPK-RI"
 AUTHOR_EMAIL="eppid@bpk.go.id"
```

