# Comparing `tmp/mergemate-0.1.1.tar.gz` & `tmp/mergemate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergemate-0.1.1.tar", last modified: Sun May 19 10:23:23 2024, max compression
+gzip compressed data, was "mergemate-0.1.2.tar", last modified: Sun May 19 11:35:22 2024, max compression
```

## Comparing `mergemate-0.1.1.tar` & `mergemate-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.375730 mergemate-0.1.1/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.1/LICENSE
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 10:23:23.375454 mergemate-0.1.1/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4418 2024-05-19 10:19:29.000000 mergemate-0.1.1/README.md
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.371776 mergemate-0.1.1/llmware/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.1/llmware/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     3307 2024-05-19 10:20:44.000000 mergemate-0.1.1/llmware/reviewer_agent.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.374731 mergemate-0.1.1/mergemate.egg-info/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      387 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/SOURCES.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/dependency_links.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/requires.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       26 2024-05-19 10:23:23.000000 mergemate-0.1.1/mergemate.egg-info/top_level.txt
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.372907 mergemate-0.1.1/providers/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.1/providers/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.1/providers/github.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.373157 mergemate-0.1.1/scripts/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.1/scripts/__init__.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 10:23:23.374377 mergemate-0.1.1/scripts/github/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.1/scripts/github/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.1/scripts/github/comment_handler.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.1/scripts/github/pr_review.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 10:23:23.376058 mergemate-0.1.1/setup.cfg
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      608 2024-05-19 10:21:30.000000 mergemate-0.1.1/setup.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.027742 mergemate-0.1.2/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.2/LICENSE
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 11:35:22.027520 mergemate-0.1.2/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4418 2024-05-19 10:19:29.000000 mergemate-0.1.2/README.md
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.024873 mergemate-0.1.2/mergemate/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:34:25.000000 mergemate-0.1.2/mergemate/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.025692 mergemate-0.1.2/mergemate/llmware/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.2/mergemate/llmware/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     3307 2024-05-19 10:20:44.000000 mergemate-0.1.2/mergemate/llmware/reviewer_agent.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.026293 mergemate-0.1.2/mergemate/providers/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.2/mergemate/providers/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.2/mergemate/providers/github.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.026424 mergemate-0.1.2/mergemate/scripts/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.2/mergemate/scripts/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.026986 mergemate-0.1.2/mergemate/scripts/github/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.2/mergemate/scripts/github/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.2/mergemate/scripts/github/comment_handler.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.2/mergemate/scripts/github/pr_review.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:35:22.027280 mergemate-0.1.2/mergemate.egg-info/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4812 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      489 2024-05-19 11:35:22.000000 mergemate-0.1.2/mergemate.egg-info/SOURCES.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/dependency_links.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/requires.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       10 2024-05-19 11:35:21.000000 mergemate-0.1.2/mergemate.egg-info/top_level.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 11:35:22.027789 mergemate-0.1.2/setup.cfg
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      618 2024-05-19 11:35:01.000000 mergemate-0.1.2/setup.py
```

### Comparing `mergemate-0.1.1/LICENSE` & `mergemate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.1/PKG-INFO` & `mergemate-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.1
+Version: 0.1.2
 Summary: An automated tool to handle GitHub pull requests and comments.
 Home-page: http://pypi.python.org/pypi/MergeMate/
 Author: Hardeep Singh
 Author-email: hardeep0khalsa122@gmail.com
 License: LICENSE.txt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `mergemate-0.1.1/README.md` & `mergemate-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.1/llmware/reviewer_agent.py` & `mergemate-0.1.2/mergemate/llmware/reviewer_agent.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.1/mergemate.egg-info/PKG-INFO` & `mergemate-0.1.2/mergemate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.1
+Version: 0.1.2
 Summary: An automated tool to handle GitHub pull requests and comments.
 Home-page: http://pypi.python.org/pypi/MergeMate/
 Author: Hardeep Singh
 Author-email: hardeep0khalsa122@gmail.com
 License: LICENSE.txt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `mergemate-0.1.1/providers/github.py` & `mergemate-0.1.2/mergemate/providers/github.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.1/scripts/github/comment_handler.py` & `mergemate-0.1.2/mergemate/scripts/github/comment_handler.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.1/scripts/github/pr_review.py` & `mergemate-0.1.2/mergemate/scripts/github/pr_review.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.1/setup.py` & `mergemate-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mergemate',
-    version='0.1.1',
+    version='0.1.2',
     author='Hardeep Singh',
     author_email='hardeep0khalsa122@gmail.com',
     packages=find_packages(),
-    scripts=['scripts/github/comment_handler.py'],
+    scripts=['mergemate/scripts/github/comment_handler.py'],
     url='http://pypi.python.org/pypi/MergeMate/',
     license='LICENSE.txt',
     description='An automated tool to handle GitHub pull requests and comments.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "llmware",
```

