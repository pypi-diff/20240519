# Comparing `tmp/chordreviewsvis-0.2.3.tar.gz` & `tmp/chordreviewsvis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chordreviewsvis-0.2.3.tar", last modified: Sat May  4 15:01:35 2024, max compression
+gzip compressed data, was "chordreviewsvis-0.2.5.tar", last modified: Sun May 19 07:19:40 2024, max compression
```

## Comparing `chordreviewsvis-0.2.3.tar` & `chordreviewsvis-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 15:01:35.622136 chordreviewsvis-0.2.3/
-drwxrwxrwx   0        0        0        0 2024-05-04 15:01:35.622136 chordreviewsvis-0.2.3/ChordReviewsVis.egg-info/
--rw-rw-rw-   0        0        0      453 2024-05-04 15:01:35.000000 chordreviewsvis-0.2.3/ChordReviewsVis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-05-04 15:01:35.000000 chordreviewsvis-0.2.3/ChordReviewsVis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 15:01:35.000000 chordreviewsvis-0.2.3/ChordReviewsVis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-04 15:01:35.000000 chordreviewsvis-0.2.3/ChordReviewsVis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 15:01:35.000000 chordreviewsvis-0.2.3/ChordReviewsVis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      453 2024-05-04 15:01:35.622136 chordreviewsvis-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-04 15:01:35.622136 chordreviewsvis-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      556 2024-05-04 15:00:46.000000 chordreviewsvis-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:19:40.394365 chordreviewsvis-0.2.5/
+drwxrwxrwx   0        0        0        0 2024-05-19 07:19:40.354310 chordreviewsvis-0.2.5/ChordReviewsVis/
+-rw-rw-rw-   0        0        0    10841 2024-05-04 14:45:17.000000 chordreviewsvis-0.2.5/ChordReviewsVis/ChordReviews.py
+-rw-rw-rw-   0        0        0       38 2024-05-19 07:12:56.000000 chordreviewsvis-0.2.5/ChordReviewsVis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:19:40.384279 chordreviewsvis-0.2.5/ChordReviewsVis.egg-info/
+-rw-rw-rw-   0        0        0      453 2024-05-19 07:19:39.000000 chordreviewsvis-0.2.5/ChordReviewsVis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-19 07:19:39.000000 chordreviewsvis-0.2.5/ChordReviewsVis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 07:19:39.000000 chordreviewsvis-0.2.5/ChordReviewsVis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-19 07:19:39.000000 chordreviewsvis-0.2.5/ChordReviewsVis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-19 07:19:39.000000 chordreviewsvis-0.2.5/ChordReviewsVis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      453 2024-05-19 07:19:40.394365 chordreviewsvis-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-19 07:19:40.394365 chordreviewsvis-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      556 2024-05-19 07:18:32.000000 chordreviewsvis-0.2.5/setup.py
```

### Comparing `chordreviewsvis-0.2.3/setup.py` & `chordreviewsvis-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ChordReviewsVis',
-    version='0.2.3',
+    version='0.2.5',
     description="Process reviews data, apply text preprocessing, and generate a chord plot visualization showing word co-occurrence patterns and sentiment analysis.",
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'nltk',
         'beautifulsoup4',
```

