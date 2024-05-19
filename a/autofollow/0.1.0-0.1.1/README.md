# Comparing `tmp/autofollow-0.1.0.tar.gz` & `tmp/autofollow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofollow-0.1.0.tar", last modified: Sun May 19 13:30:03 2024, max compression
+gzip compressed data, was "autofollow-0.1.1.tar", last modified: Sun May 19 14:19:13 2024, max compression
```

## Comparing `autofollow-0.1.0.tar` & `autofollow-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 13:30:03.078430 autofollow-0.1.0/
--rw-r--r--   0 jacobsomer   (501) staff       (20)     1068 2024-05-19 13:29:28.000000 autofollow-0.1.0/LICENSE
--rw-r--r--   0 jacobsomer   (501) staff       (20)      850 2024-05-19 13:30:03.078186 autofollow-0.1.0/PKG-INFO
--rw-r--r--   0 jacobsomer   (501) staff       (20)      342 2024-05-18 21:12:48.000000 autofollow-0.1.0/README.md
-drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 13:30:03.076785 autofollow-0.1.0/autofollow/
--rw-r--r--   0 jacobsomer   (501) staff       (20)        0 2024-05-18 21:49:38.000000 autofollow-0.1.0/autofollow/__init__.py
--rw-r--r--   0 jacobsomer   (501) staff       (20)     2375 2024-05-19 00:21:36.000000 autofollow-0.1.0/autofollow/agent.py
--rw-r--r--   0 jacobsomer   (501) staff       (20)        0 2024-05-18 21:15:51.000000 autofollow-0.1.0/autofollow/common.py
--rw-r--r--   0 jacobsomer   (501) staff       (20)     3351 2024-05-19 02:17:36.000000 autofollow-0.1.0/autofollow/github.py
--rw-r--r--   0 jacobsomer   (501) staff       (20)     2943 2024-05-19 02:10:29.000000 autofollow-0.1.0/autofollow/x.py
-drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 13:30:03.077637 autofollow-0.1.0/autofollow.egg-info/
--rw-r--r--   0 jacobsomer   (501) staff       (20)      850 2024-05-19 13:30:02.000000 autofollow-0.1.0/autofollow.egg-info/PKG-INFO
--rw-r--r--   0 jacobsomer   (501) staff       (20)      353 2024-05-19 13:30:03.000000 autofollow-0.1.0/autofollow.egg-info/SOURCES.txt
--rw-r--r--   0 jacobsomer   (501) staff       (20)        1 2024-05-19 13:30:03.000000 autofollow-0.1.0/autofollow.egg-info/dependency_links.txt
--rw-r--r--   0 jacobsomer   (501) staff       (20)       94 2024-05-19 13:30:03.000000 autofollow-0.1.0/autofollow.egg-info/entry_points.txt
--rw-r--r--   0 jacobsomer   (501) staff       (20)        9 2024-05-19 13:30:03.000000 autofollow-0.1.0/autofollow.egg-info/requires.txt
--rw-r--r--   0 jacobsomer   (501) staff       (20)       11 2024-05-19 13:30:03.000000 autofollow-0.1.0/autofollow.egg-info/top_level.txt
--rw-r--r--   0 jacobsomer   (501) staff       (20)       38 2024-05-19 13:30:03.078479 autofollow-0.1.0/setup.cfg
--rw-r--r--   0 jacobsomer   (501) staff       (20)      861 2024-05-18 23:58:39.000000 autofollow-0.1.0/setup.py
-drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 13:30:03.077768 autofollow-0.1.0/tests/
--rw-r--r--   0 jacobsomer   (501) staff       (20)     1940 2024-05-18 23:58:39.000000 autofollow-0.1.0/tests/test_agent.py
+drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 14:19:13.032555 autofollow-0.1.1/
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     1068 2024-05-19 13:29:28.000000 autofollow-0.1.1/LICENSE
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     2978 2024-05-19 14:19:13.032340 autofollow-0.1.1/PKG-INFO
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     2470 2024-05-19 14:16:58.000000 autofollow-0.1.1/README.md
+drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 14:19:13.031118 autofollow-0.1.1/autofollow/
+-rw-r--r--   0 jacobsomer   (501) staff       (20)        0 2024-05-18 21:49:38.000000 autofollow-0.1.1/autofollow/__init__.py
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     2207 2024-05-19 14:16:58.000000 autofollow-0.1.1/autofollow/agent.py
+-rw-r--r--   0 jacobsomer   (501) staff       (20)        0 2024-05-18 21:15:51.000000 autofollow-0.1.1/autofollow/common.py
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     3351 2024-05-19 02:17:36.000000 autofollow-0.1.1/autofollow/github.py
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     2943 2024-05-19 02:10:29.000000 autofollow-0.1.1/autofollow/x.py
+drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 14:19:13.031891 autofollow-0.1.1/autofollow.egg-info/
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     2978 2024-05-19 14:19:12.000000 autofollow-0.1.1/autofollow.egg-info/PKG-INFO
+-rw-r--r--   0 jacobsomer   (501) staff       (20)      353 2024-05-19 14:19:12.000000 autofollow-0.1.1/autofollow.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobsomer   (501) staff       (20)        1 2024-05-19 14:19:12.000000 autofollow-0.1.1/autofollow.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobsomer   (501) staff       (20)       94 2024-05-19 14:19:12.000000 autofollow-0.1.1/autofollow.egg-info/entry_points.txt
+-rw-r--r--   0 jacobsomer   (501) staff       (20)        9 2024-05-19 14:19:12.000000 autofollow-0.1.1/autofollow.egg-info/requires.txt
+-rw-r--r--   0 jacobsomer   (501) staff       (20)       11 2024-05-19 14:19:12.000000 autofollow-0.1.1/autofollow.egg-info/top_level.txt
+-rw-r--r--   0 jacobsomer   (501) staff       (20)       38 2024-05-19 14:19:13.032608 autofollow-0.1.1/setup.cfg
+-rw-r--r--   0 jacobsomer   (501) staff       (20)      861 2024-05-19 14:18:48.000000 autofollow-0.1.1/setup.py
+drwxr-xr-x   0 jacobsomer   (501) staff       (20)        0 2024-05-19 14:19:13.032005 autofollow-0.1.1/tests/
+-rw-r--r--   0 jacobsomer   (501) staff       (20)     1940 2024-05-18 23:58:39.000000 autofollow-0.1.1/tests/test_agent.py
```

### Comparing `autofollow-0.1.0/LICENSE` & `autofollow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autofollow-0.1.0/autofollow/agent.py` & `autofollow-0.1.1/autofollow/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import random
 import time
 from selenium import webdriver
 from .x import XAgent
 from . import github
 
 class AutoFollowAgent:
-    def __init__(self, driver_path, profile_path, binary_location=None, github_username=None, github_password=None):
+    def __init__(self, driver_path, profile_path, github_username=None, github_password=None):
         self.driver_path = driver_path
         self.profile_path = profile_path
-        self.binary_location = binary_location
         self.github_username = github_username
         self.github_password = github_password
         self.driver = self.create_driver()
         self.x_agent = XAgent(self.driver)
 
     def create_driver(self):
         chrome_options = webdriver.ChromeOptions()
-        if self.binary_location:
-            chrome_options.binary_location = self.binary_location
         if self.profile_path:
             chrome_options.add_argument(f"user-data-dir={self.profile_path}")
         chrome_options.add_argument("disable-infobars")
         chrome_options.add_argument("--disable-extensions")
         chrome_options.add_argument("--disable-gpu")
         chrome_options.add_argument("--disable-dev-shm-usage")
         chrome_options.add_argument("--no-sandbox")
```

### Comparing `autofollow-0.1.0/autofollow/github.py` & `autofollow-0.1.1/autofollow/github.py`

 * *Files identical despite different names*

### Comparing `autofollow-0.1.0/autofollow/x.py` & `autofollow-0.1.1/autofollow/x.py`

 * *Files identical despite different names*

### Comparing `autofollow-0.1.0/setup.py` & `autofollow-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='autofollow',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'selenium',
     ],
     entry_points={
         'console_scripts': [
             'x_automation=autofollow.x:main',
```

### Comparing `autofollow-0.1.0/tests/test_agent.py` & `autofollow-0.1.1/tests/test_agent.py`

 * *Files identical despite different names*

