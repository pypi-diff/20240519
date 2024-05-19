# Comparing `tmp/mergemate-0.1.3.tar.gz` & `tmp/mergemate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergemate-0.1.3.tar", last modified: Sun May 19 12:11:53 2024, max compression
+gzip compressed data, was "mergemate-0.1.4.tar", last modified: Sun May 19 12:15:58 2024, max compression
```

## Comparing `mergemate-0.1.3.tar` & `mergemate-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.258167 mergemate-0.1.3/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.3/LICENSE
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     5366 2024-05-19 12:11:53.257958 mergemate-0.1.3/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     4973 2024-05-19 12:08:03.000000 mergemate-0.1.3/README.md
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.254401 mergemate-0.1.3/mergemate/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:34:25.000000 mergemate-0.1.3/mergemate/__init__.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.255199 mergemate-0.1.3/mergemate/llmware/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.3/mergemate/llmware/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     3017 2024-05-19 12:11:23.000000 mergemate-0.1.3/mergemate/llmware/reviewer_agent.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.255970 mergemate-0.1.3/mergemate/prompts/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:10:31.000000 mergemate-0.1.3/mergemate/prompts/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      632 2024-05-19 12:09:51.000000 mergemate-0.1.3/mergemate/prompts/answer_comment.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      644 2024-05-19 12:10:09.000000 mergemate-0.1.3/mergemate/prompts/create_review.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      360 2024-05-19 12:10:22.000000 mergemate-0.1.3/mergemate/prompts/explain_code.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.256708 mergemate-0.1.3/mergemate/providers/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.3/mergemate/providers/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.3/mergemate/providers/github.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.256822 mergemate-0.1.3/mergemate/scripts/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.3/mergemate/scripts/__init__.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.257356 mergemate-0.1.3/mergemate/scripts/github/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.3/mergemate/scripts/github/__init__.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.3/mergemate/scripts/github/comment_handler.py
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.3/mergemate/scripts/github/pr_review.py
-drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:11:53.257701 mergemate-0.1.3/mergemate.egg-info/
--rw-r--r--   0 hardeepsingh   (501) staff       (20)     5366 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/PKG-INFO
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      624 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/SOURCES.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/dependency_links.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/requires.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       10 2024-05-19 12:11:53.000000 mergemate-0.1.3/mergemate.egg-info/top_level.txt
--rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 12:11:53.258211 mergemate-0.1.3/setup.cfg
--rw-r--r--   0 hardeepsingh   (501) staff       (20)      618 2024-05-19 12:11:36.000000 mergemate-0.1.3/setup.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.481944 mergemate-0.1.4/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1070 2024-05-19 09:57:02.000000 mergemate-0.1.4/LICENSE
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     5366 2024-05-19 12:15:58.481729 mergemate-0.1.4/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     4973 2024-05-19 12:08:03.000000 mergemate-0.1.4/README.md
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.477783 mergemate-0.1.4/mergemate/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 11:34:25.000000 mergemate-0.1.4/mergemate/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.478561 mergemate-0.1.4/mergemate/llmware/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:36.000000 mergemate-0.1.4/mergemate/llmware/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     3027 2024-05-19 12:15:31.000000 mergemate-0.1.4/mergemate/llmware/reviewer_agent.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.479388 mergemate-0.1.4/mergemate/prompts/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:10:31.000000 mergemate-0.1.4/mergemate/prompts/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      632 2024-05-19 12:09:51.000000 mergemate-0.1.4/mergemate/prompts/answer_comment.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      644 2024-05-19 12:10:09.000000 mergemate-0.1.4/mergemate/prompts/create_review.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      360 2024-05-19 12:10:22.000000 mergemate-0.1.4/mergemate/prompts/explain_code.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.480130 mergemate-0.1.4/mergemate/providers/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:40.000000 mergemate-0.1.4/mergemate/providers/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     1623 2024-05-19 09:01:12.000000 mergemate-0.1.4/mergemate/providers/github.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.480429 mergemate-0.1.4/mergemate/scripts/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:45:46.000000 mergemate-0.1.4/mergemate/scripts/__init__.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.481119 mergemate-0.1.4/mergemate/scripts/github/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        0 2024-05-12 14:46:00.000000 mergemate-0.1.4/mergemate/scripts/github/__init__.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      985 2024-05-19 09:02:30.000000 mergemate-0.1.4/mergemate/scripts/github/comment_handler.py
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      834 2024-05-19 08:45:56.000000 mergemate-0.1.4/mergemate/scripts/github/pr_review.py
+drwxr-xr-x   0 hardeepsingh   (501) staff       (20)        0 2024-05-19 12:15:58.481469 mergemate-0.1.4/mergemate.egg-info/
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)     5366 2024-05-19 12:15:58.000000 mergemate-0.1.4/mergemate.egg-info/PKG-INFO
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      624 2024-05-19 12:15:58.000000 mergemate-0.1.4/mergemate.egg-info/SOURCES.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)        1 2024-05-19 12:15:58.000000 mergemate-0.1.4/mergemate.egg-info/dependency_links.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       17 2024-05-19 12:15:58.000000 mergemate-0.1.4/mergemate.egg-info/requires.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       10 2024-05-19 12:15:58.000000 mergemate-0.1.4/mergemate.egg-info/top_level.txt
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)       38 2024-05-19 12:15:58.482107 mergemate-0.1.4/setup.cfg
+-rw-r--r--   0 hardeepsingh   (501) staff       (20)      618 2024-05-19 12:15:54.000000 mergemate-0.1.4/setup.py
```

### Comparing `mergemate-0.1.3/LICENSE` & `mergemate-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/PKG-INFO` & `mergemate-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.3
+Version: 0.1.4
 Summary: An automated tool to handle GitHub pull requests and comments.
 Home-page: http://pypi.python.org/pypi/MergeMate/
 Author: Hardeep Singh
 Author-email: hardeep0khalsa122@gmail.com
 License: LICENSE.txt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `mergemate-0.1.3/README.md` & `mergemate-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/mergemate/llmware/reviewer_agent.py` & `mergemate-0.1.4/mergemate/llmware/reviewer_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from llmware.prompts import Prompt
 import os
-from prompts import answer_comment, create_review, explain_code
+from mergemate.prompts import answer_comment, create_review, explain_code
 
 class ReviewerAgent:
     def __init__(self):
         self.prompt = Prompt().load_model('gpt-3.5-turbo', api_key=os.environ['OPENAI_API_KEY'])
         self.help_commands = {
             '/help': 'List all available commands.',
             '/explain': 'Explain the current code context',
```

### Comparing `mergemate-0.1.3/mergemate/prompts/answer_comment.py` & `mergemate-0.1.4/mergemate/prompts/answer_comment.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/mergemate/prompts/create_review.py` & `mergemate-0.1.4/mergemate/prompts/create_review.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/mergemate/providers/github.py` & `mergemate-0.1.4/mergemate/providers/github.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/mergemate/scripts/github/comment_handler.py` & `mergemate-0.1.4/mergemate/scripts/github/comment_handler.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/mergemate/scripts/github/pr_review.py` & `mergemate-0.1.4/mergemate/scripts/github/pr_review.py`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/mergemate.egg-info/PKG-INFO` & `mergemate-0.1.4/mergemate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergemate
-Version: 0.1.3
+Version: 0.1.4
 Summary: An automated tool to handle GitHub pull requests and comments.
 Home-page: http://pypi.python.org/pypi/MergeMate/
 Author: Hardeep Singh
 Author-email: hardeep0khalsa122@gmail.com
 License: LICENSE.txt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `mergemate-0.1.3/mergemate.egg-info/SOURCES.txt` & `mergemate-0.1.4/mergemate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mergemate-0.1.3/setup.py` & `mergemate-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mergemate',
-    version='0.1.3',
+    version='0.1.4',
     author='Hardeep Singh',
     author_email='hardeep0khalsa122@gmail.com',
     packages=find_packages(),
     scripts=['mergemate/scripts/github/comment_handler.py'],
     url='http://pypi.python.org/pypi/MergeMate/',
     license='LICENSE.txt',
     description='An automated tool to handle GitHub pull requests and comments.',
```

