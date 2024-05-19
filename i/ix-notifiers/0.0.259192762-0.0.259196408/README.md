# Comparing `tmp/ix-notifiers-0.0.259192762.tar.gz` & `tmp/ix-notifiers-0.0.259196408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix-notifiers-0.0.259192762.tar", last modified: Sat Feb 20 15:20:11 2021, max compression
+gzip compressed data, was "ix-notifiers-0.0.259196408.tar", last modified: Sat Feb 20 15:38:51 2021, max compression
```

## Comparing `ix-notifiers-0.0.259192762.tar` & `ix-notifiers-0.0.259196408.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 15:20:11.028230 ix-notifiers-0.0.259192762/
--rw-r--r--   0 root         (0) root         (0)      521 2021-02-20 15:20:11.028230 ix-notifiers-0.0.259192762/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 15:20:11.028230 ix-notifiers-0.0.259192762/ix_notifiers/
--rw-rw-rw-   0 root         (0) root         (0)       47 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/ix_notifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2021-02-20 15:20:10.000000 ix-notifiers-0.0.259192762/ix_notifiers/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3312 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/ix_notifiers/core.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/ix_notifiers/gotify_notifier.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/ix_notifiers/null_notifier.py
--rw-rw-rw-   0 root         (0) root         (0)     3772 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/ix_notifiers/telegram_notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 15:20:11.028230 ix-notifiers-0.0.259192762/ix_notifiers.egg-info/
--rw-r--r--   0 root         (0) root         (0)      521 2021-02-20 15:20:10.000000 ix-notifiers-0.0.259192762/ix_notifiers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      365 2021-02-20 15:20:10.000000 ix-notifiers-0.0.259192762/ix_notifiers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-20 15:20:10.000000 ix-notifiers-0.0.259192762/ix_notifiers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2021-02-20 15:20:10.000000 ix-notifiers-0.0.259192762/ix_notifiers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-02-20 15:20:10.000000 ix-notifiers-0.0.259192762/ix_notifiers.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-20 15:20:11.028230 ix-notifiers-0.0.259192762/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      895 2021-02-20 11:45:52.000000 ix-notifiers-0.0.259192762/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 15:38:51.892476 ix-notifiers-0.0.259196408/
+-rw-r--r--   0 root         (0) root         (0)      521 2021-02-20 15:38:51.892476 ix-notifiers-0.0.259196408/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       60 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 15:38:51.892476 ix-notifiers-0.0.259196408/ix_notifiers/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/ix_notifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      167 2021-02-20 15:38:51.000000 ix-notifiers-0.0.259196408/ix_notifiers/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3312 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/ix_notifiers/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/ix_notifiers/gotify_notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/ix_notifiers/null_notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     3772 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/ix_notifiers/telegram_notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-20 15:38:51.892476 ix-notifiers-0.0.259196408/ix_notifiers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      521 2021-02-20 15:38:51.000000 ix-notifiers-0.0.259196408/ix_notifiers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      365 2021-02-20 15:38:51.000000 ix-notifiers-0.0.259196408/ix_notifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-02-20 15:38:51.000000 ix-notifiers-0.0.259196408/ix_notifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2021-02-20 15:38:51.000000 ix-notifiers-0.0.259196408/ix_notifiers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-02-20 15:38:51.000000 ix-notifiers-0.0.259196408/ix_notifiers.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-02-20 15:38:51.892476 ix-notifiers-0.0.259196408/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      895 2021-02-20 11:46:46.000000 ix-notifiers-0.0.259196408/setup.py
```

### Comparing `ix-notifiers-0.0.259192762/PKG-INFO` & `ix-notifiers-0.0.259196408/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-notifiers
-Version: 0.0.259192762
+Version: 0.0.259196408
 Summary: A python library for notifiers
 Home-page: https://gitlab.com/ix.ai/notifiers
 Author: ix.ai
 Author-email: docker@ix.ai
 License: MIT License
 Description: A python library for notifiers. Used in the ix.ai projects.
```

### Comparing `ix-notifiers-0.0.259192762/ix_notifiers/core.py` & `ix-notifiers-0.0.259196408/ix_notifiers/core.py`

 * *Files identical despite different names*

### Comparing `ix-notifiers-0.0.259192762/ix_notifiers/gotify_notifier.py` & `ix-notifiers-0.0.259196408/ix_notifiers/gotify_notifier.py`

 * *Files identical despite different names*

### Comparing `ix-notifiers-0.0.259192762/ix_notifiers/telegram_notifier.py` & `ix-notifiers-0.0.259196408/ix_notifiers/telegram_notifier.py`

 * *Files identical despite different names*

### Comparing `ix-notifiers-0.0.259192762/ix_notifiers.egg-info/PKG-INFO` & `ix-notifiers-0.0.259196408/ix_notifiers.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-notifiers
-Version: 0.0.259192762
+Version: 0.0.259196408
 Summary: A python library for notifiers
 Home-page: https://gitlab.com/ix.ai/notifiers
 Author: ix.ai
 Author-email: docker@ix.ai
 License: MIT License
 Description: A python library for notifiers. Used in the ix.ai projects.
```

### Comparing `ix-notifiers-0.0.259192762/setup.py` & `ix-notifiers-0.0.259196408/setup.py`

 * *Files identical despite different names*

