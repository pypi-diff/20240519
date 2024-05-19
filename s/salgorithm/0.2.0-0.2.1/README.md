# Comparing `tmp/salgorithm-0.2.0.tar.gz` & `tmp/salgorithm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salgorithm-0.2.0.tar", last modified: Sun May 19 00:40:03 2024, max compression
+gzip compressed data, was "salgorithm-0.2.1.tar", last modified: Sun May 19 01:00:02 2024, max compression
```

## Comparing `salgorithm-0.2.0.tar` & `salgorithm-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 00:40:03.784008 salgorithm-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 00:40:03.783008 salgorithm-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7614 2024-05-19 00:38:30.000000 salgorithm-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 00:40:03.765006 salgorithm-0.2.0/salgorithm/
--rw-r--r--   0 root         (0) root         (0)      686 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/BFS.py
--rw-r--r--   0 root         (0) root         (0)      338 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/BinarySearch.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Bubble.py
--rw-r--r--   0 root         (0) root         (0)      764 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Bucket.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/CaesarCipher.py
--rw-r--r--   0 root         (0) root         (0)      750 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Cocktail.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/DFS.py
--rw-r--r--   0 root         (0) root         (0)      761 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Greedy.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Heap.py
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Insertion.py
--rw-r--r--   0 root         (0) root         (0)      464 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Interpolation.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Jump.py
--rw-r--r--   0 root         (0) root         (0)      182 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Linear.py
--rw-r--r--   0 root         (0) root         (0)      559 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Merge.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Quick.py
--rw-r--r--   0 root         (0) root         (0)     1380 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/RSA.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Radix.py
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Selection.py
--rw-r--r--   0 root         (0) root         (0)      400 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Shell.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/Tabu.py
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/TransposeCipher.py
--rw-r--r--   0 root         (0) root         (0)      566 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/VigenereCipher.py
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      474 2024-05-19 00:38:30.000000 salgorithm-0.2.0/salgorithm/time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 00:40:03.780007 salgorithm-0.2.0/salgorithm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 00:40:03.000000 salgorithm-0.2.0/salgorithm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 00:40:03.784008 salgorithm-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 00:38:30.000000 salgorithm-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:00:02.840861 salgorithm-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 00:38:30.000000 salgorithm-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:00:02.839861 salgorithm-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7614 2024-05-19 00:38:30.000000 salgorithm-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:00:02.825860 salgorithm-0.2.1/salgorithm/
+-rw-r--r--   0 root         (0) root         (0)      686 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/BFS.py
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/BinarySearch.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Bubble.py
+-rw-r--r--   0 root         (0) root         (0)      764 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Bucket.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/CaesarCipher.py
+-rw-r--r--   0 root         (0) root         (0)      750 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Cocktail.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/DFS.py
+-rw-r--r--   0 root         (0) root         (0)      761 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Greedy.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Heap.py
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Insertion.py
+-rw-r--r--   0 root         (0) root         (0)      464 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Interpolation.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Jump.py
+-rw-r--r--   0 root         (0) root         (0)      182 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Linear.py
+-rw-r--r--   0 root         (0) root         (0)      559 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Merge.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Quick.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/RSA.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Radix.py
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Selection.py
+-rw-r--r--   0 root         (0) root         (0)      400 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Shell.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/Tabu.py
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/TransposeCipher.py
+-rw-r--r--   0 root         (0) root         (0)      566 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/VigenereCipher.py
+-rw-r--r--   0 root         (0) root         (0)      796 2024-05-19 00:38:30.000000 salgorithm-0.2.1/salgorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      465 2024-05-19 00:59:41.000000 salgorithm-0.2.1/salgorithm/time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 01:00:02.837860 salgorithm-0.2.1/salgorithm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8255 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-19 01:00:02.000000 salgorithm-0.2.1/salgorithm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-19 01:00:02.841861 salgorithm-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-05-19 00:59:58.000000 salgorithm-0.2.1/setup.py
```

### Comparing `salgorithm-0.2.0/LICENSE` & `salgorithm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/PKG-INFO` & `salgorithm-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salgorithm
-Version: 0.2.0
+Version: 0.2.1
 Summary: 让算法变得简单一点
 Home-page: https://github.com/SoulCodingYanhun/salgorithm
 Author: SoulCodingYanhun
 Author-email: souls2906@gmail.com
 Maintainer: SoulCodingYanhun
 Maintainer-email: souls2906@gmail.com
 License: Apache License
```

### Comparing `salgorithm-0.2.0/README.md` & `salgorithm-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/BFS.py` & `salgorithm-0.2.1/salgorithm/BFS.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Bucket.py` & `salgorithm-0.2.1/salgorithm/Bucket.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Cocktail.py` & `salgorithm-0.2.1/salgorithm/Cocktail.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Greedy.py` & `salgorithm-0.2.1/salgorithm/Greedy.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Heap.py` & `salgorithm-0.2.1/salgorithm/Heap.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Merge.py` & `salgorithm-0.2.1/salgorithm/Merge.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/RSA.py` & `salgorithm-0.2.1/salgorithm/RSA.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Radix.py` & `salgorithm-0.2.1/salgorithm/Radix.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/Tabu.py` & `salgorithm-0.2.1/salgorithm/Tabu.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/TransposeCipher.py` & `salgorithm-0.2.1/salgorithm/TransposeCipher.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/VigenereCipher.py` & `salgorithm-0.2.1/salgorithm/VigenereCipher.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm/__init__.py` & `salgorithm-0.2.1/salgorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/salgorithm.egg-info/PKG-INFO` & `salgorithm-0.2.1/salgorithm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salgorithm
-Version: 0.2.0
+Version: 0.2.1
 Summary: 让算法变得简单一点
 Home-page: https://github.com/SoulCodingYanhun/salgorithm
 Author: SoulCodingYanhun
 Author-email: souls2906@gmail.com
 Maintainer: SoulCodingYanhun
 Maintainer-email: souls2906@gmail.com
 License: Apache License
```

### Comparing `salgorithm-0.2.0/salgorithm.egg-info/SOURCES.txt` & `salgorithm-0.2.1/salgorithm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salgorithm-0.2.0/setup.py` & `salgorithm-0.2.1/setup.py`

 * *Files identical despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Load the README.md file for the long description
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='salgorithm',
-    version='0.2.0',
+    version='0.2.1',
     description="让算法变得简单一点",
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type as Markdown
     include_package_data=True,
     author='SoulCodingYanhun',
     author_email='souls2906@gmail.com',
     maintainer='SoulCodingYanhun',
```

