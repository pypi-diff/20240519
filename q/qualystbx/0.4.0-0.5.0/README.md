# Comparing `tmp/qualystbx-0.4.0.tar.gz` & `tmp/qualystbx-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualystbx-0.4.0.tar", last modified: Sat May 18 13:31:42 2024, max compression
+gzip compressed data, was "qualystbx-0.5.0.tar", last modified: Sun May 19 12:15:12 2024, max compression
```

## Comparing `qualystbx-0.4.0.tar` & `qualystbx-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 13:31:42.011084 qualystbx-0.4.0/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.4.0/LICENSE.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       20 2024-04-24 16:23:40.000000 qualystbx-0.4.0/MANIFEST.in
--rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-18 13:31:42.011084 qualystbx-0.4.0/PKG-INFO
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.4.0/README.md
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.4.0/license.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      103 2024-01-30 19:38:49.000000 qualystbx-0.4.0/pyproject.toml
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 13:31:42.007084 qualystbx-0.4.0/qualys_tbx/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.4.0/qualys_tbx/README.md
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       21 2024-05-18 13:30:53.000000 qualystbx-0.4.0/qualys_tbx/__init__.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 13:31:42.011084 qualystbx-0.4.0/qualys_tbx/qtbx_lib/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-03-28 10:53:29.000000 qualystbx-0.4.0/qualys_tbx/qtbx_lib/__init__.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3599 2024-05-14 05:39:58.000000 qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    17131 2024-05-14 04:00:20.000000 qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     4462 2024-05-18 12:24:25.000000 qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3131 2024-05-14 03:56:41.000000 qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     6824 2024-05-10 03:04:01.000000 qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 13:31:42.011084 qualystbx-0.4.0/qualys_tbx/qtbx_policy_merge/
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-04-02 10:51:14.000000 qualystbx-0.4.0/qualys_tbx/qtbx_policy_merge/__init__.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    24191 2024-05-14 05:59:14.000000 qualystbx-0.4.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     8402 2024-05-18 12:55:18.000000 qualystbx-0.4.0/qualys_tbx/qualystbx.py
-drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-18 13:31:42.011084 qualystbx-0.4.0/qualystbx.egg-info/
--rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-18 13:31:42.000000 qualystbx-0.4.0/qualystbx.egg-info/PKG-INFO
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      635 2024-05-18 13:31:42.000000 qualystbx-0.4.0/qualystbx.egg-info/SOURCES.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        1 2024-05-18 13:31:42.000000 qualystbx-0.4.0/qualystbx.egg-info/dependency_links.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       56 2024-05-18 13:31:42.000000 qualystbx-0.4.0/qualystbx.egg-info/entry_points.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       11 2024-05-18 13:31:42.000000 qualystbx-0.4.0/qualystbx.egg-info/top_level.txt
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       38 2024-05-18 13:31:42.011084 qualystbx-0.4.0/setup.cfg
--rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     1835 2024-05-18 13:30:53.000000 qualystbx-0.4.0/setup.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:15:12.695397 qualystbx-0.5.0/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.5.0/LICENSE.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       20 2024-04-24 16:23:40.000000 qualystbx-0.5.0/MANIFEST.in
+-rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-19 12:15:12.695397 qualystbx-0.5.0/PKG-INFO
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.5.0/README.md
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    11359 2024-01-30 19:38:49.000000 qualystbx-0.5.0/license.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      103 2024-01-30 19:38:49.000000 qualystbx-0.5.0/pyproject.toml
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:15:12.691397 qualystbx-0.5.0/qualys_tbx/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     7718 2024-05-17 20:45:34.000000 qualystbx-0.5.0/qualys_tbx/README.md
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       21 2024-05-19 12:07:15.000000 qualystbx-0.5.0/qualys_tbx/__init__.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:15:12.695397 qualystbx-0.5.0/qualys_tbx/qtbx_lib/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-03-28 10:53:29.000000 qualystbx-0.5.0/qualys_tbx/qtbx_lib/__init__.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3599 2024-05-14 05:39:58.000000 qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    17131 2024-05-14 04:00:20.000000 qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     4462 2024-05-18 12:24:25.000000 qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     3131 2024-05-14 03:56:41.000000 qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     6824 2024-05-10 03:04:01.000000 qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:15:12.695397 qualystbx-0.5.0/qualys_tbx/qtbx_policy_merge/
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        0 2024-04-02 10:51:14.000000 qualystbx-0.5.0/qualys_tbx/qtbx_policy_merge/__init__.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)    24191 2024-05-14 05:59:14.000000 qualystbx-0.5.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     9639 2024-05-19 12:07:14.000000 qualystbx-0.5.0/qualys_tbx/qualystbx.py
+drwxrwxr-x   0 dgregory  (1000) dgregory  (1000)        0 2024-05-19 12:15:12.695397 qualystbx-0.5.0/qualystbx.egg-info/
+-rw-r--r--   0 dgregory  (1000) dgregory  (1000)     8578 2024-05-19 12:15:12.000000 qualystbx-0.5.0/qualystbx.egg-info/PKG-INFO
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)      635 2024-05-19 12:15:12.000000 qualystbx-0.5.0/qualystbx.egg-info/SOURCES.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)        1 2024-05-19 12:15:12.000000 qualystbx-0.5.0/qualystbx.egg-info/dependency_links.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       56 2024-05-19 12:15:12.000000 qualystbx-0.5.0/qualystbx.egg-info/entry_points.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       11 2024-05-19 12:15:12.000000 qualystbx-0.5.0/qualystbx.egg-info/top_level.txt
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)       38 2024-05-19 12:15:12.695397 qualystbx-0.5.0/setup.cfg
+-rw-rw-r--   0 dgregory  (1000) dgregory  (1000)     1835 2024-05-19 12:07:15.000000 qualystbx-0.5.0/setup.py
```

### Comparing `qualystbx-0.4.0/LICENSE.txt` & `qualystbx-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/PKG-INFO` & `qualystbx-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualystbx
-Version: 0.4.0
+Version: 0.5.0
 Summary: Qualys Tool Box - Tools for running various functions in Qualys.
 Home-page: https://pypi.org/project/qualystbx/
 Author: David Gregory
 Author-email: dgregory@qualys.com, dave@davidgregory.com
 License: Apache
 Project-URL: Documentation, https://dg-cafe.github.io/qualystbx/
 Keywords: qualys,qualystoolbox,qualys.com,david gregory,qualystbx,qualysapi
```

### Comparing `qualystbx-0.4.0/README.md` & `qualystbx-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/license.txt` & `qualystbx-0.5.0/license.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/README.md` & `qualystbx-0.5.0/qualys_tbx/README.md`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py` & `qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_argparser.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py` & `qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_authentication.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py` & `qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_config.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py` & `qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_functions.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py` & `qualystbx-0.5.0/qualys_tbx/qtbx_lib/qtbx_lib_logger.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py` & `qualystbx-0.5.0/qualys_tbx/qtbx_policy_merge/policy_merge_01.py`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/qualys_tbx/qualystbx.py` & `qualystbx-0.5.0/qualys_tbx/qualystbx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import fcntl
 import sys
 import time
 import re
 import shutil
 from contextlib import redirect_stdout, redirect_stderr
 from qualys_tbx.qtbx_policy_merge import policy_merge_01
 from qualys_tbx.qtbx_lib import qtbx_lib_config
@@ -108,35 +107,63 @@
         log_file_size = log_file_path.stat().st_size  # In Bytes
         if log_file_size > log_file_max_size:
             shutil.copy2(log_file_path, log_file_rotate_path, follow_symlinks=True)
             fo = open(log_file_path, 'w+')
             fo.close()
 
 
+# def execute_qualystbx(lock_file=None, log_dir=None, log_file_path=None, log_to_console=True, log_file_rotate_path=None):
+#     if log_to_console:
+#         qtbx_main()
+#     else:
+#         try:
+#             with open(lock_file, 'wb+') as lock_program_fcntl:  # If locked, exit.
+#                 fcntl.flock(lock_program_fcntl, fcntl.LOCK_EX | fcntl.LOCK_NB)
+#                 exception_message = "ERROR: rotate_log_check. Please retry later: "
+#                 rotate_log_check(log_file_path=log_file_path,
+#                                  log_file_max_size=10000000,
+#                                  log_file_rotate_path=log_file_rotate_path
+#                                  )
+#                 if log_dir.is_dir():
+#                     exception_message = "ERROR: spawn_etl_in_background. Please retry later: "
+#                     with open(log_file_path, 'a', newline='', encoding='utf-8') as log_fo:
+#                         with redirect_stdout(log_fo), redirect_stderr(sys.stdout):
+#                             qtbx_main()
+#                             log_fo.flush()
+#                 else:
+#                     exception_message = f"ERROR: logdir_missing: {log_dir} - Potential permissions issue."
+#                     raise Exception(exception_message)
+#
+#
+#         except Exception as e:
+#             print(f"{exception_message} {__file__} ")
+#             print(f"Exception: {e}")
+#             exit(1)
+
+
 def execute_qualystbx(lock_file=None, log_dir=None, log_file_path=None, log_to_console=True, log_file_rotate_path=None):
     if log_to_console:
         qtbx_main()
     else:
+        exception_message = ""
         try:
-            with open(lock_file, 'wb+') as lock_program_fcntl:  # If locked, exit.
-                fcntl.flock(lock_program_fcntl, fcntl.LOCK_EX | fcntl.LOCK_NB)
-                exception_message = "ERROR: rotate_log_check. Please retry later: "
-                rotate_log_check(log_file_path=log_file_path,
-                                 log_file_max_size=10000000,
-                                 log_file_rotate_path=log_file_rotate_path
-                                 )
-                if log_dir.is_dir():
-                    exception_message = "ERROR: spawn_etl_in_background. Please retry later: "
-                    with open(log_file_path, 'a', newline='', encoding='utf-8') as log_fo:
-                        with redirect_stdout(log_fo), redirect_stderr(sys.stdout):
-                            qtbx_main()
-                            log_fo.flush()
-                else:
-                    exception_message = f"ERROR: logdir_missing: {log_dir} - Potential permissions issue."
-                    raise Exception(exception_message)
+            exception_message = "ERROR: rotate_log_check. Please retry later: "
+            rotate_log_check(log_file_path=log_file_path,
+                             log_file_max_size=10000000,
+                             log_file_rotate_path=log_file_rotate_path
+                             )
+            if log_dir.is_dir():
+                exception_message = "ERROR: spawn_etl_in_background. Please retry later: "
+                with open(log_file_path, 'a', newline='', encoding='utf-8') as log_fo:
+                    with redirect_stdout(log_fo), redirect_stderr(sys.stdout):
+                        qtbx_main()
+                        log_fo.flush()
+            else:
+                exception_message = f"ERROR: logdir_missing: {log_dir} - Potential permissions issue."
+                raise Exception(exception_message)
 
 
         except Exception as e:
             print(f"{exception_message} {__file__} ")
             print(f"Exception: {e}")
             exit(1)
```

### Comparing `qualystbx-0.4.0/qualystbx.egg-info/PKG-INFO` & `qualystbx-0.5.0/qualystbx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualystbx
-Version: 0.4.0
+Version: 0.5.0
 Summary: Qualys Tool Box - Tools for running various functions in Qualys.
 Home-page: https://pypi.org/project/qualystbx/
 Author: David Gregory
 Author-email: dgregory@qualys.com, dave@davidgregory.com
 License: Apache
 Project-URL: Documentation, https://dg-cafe.github.io/qualystbx/
 Keywords: qualys,qualystoolbox,qualys.com,david gregory,qualystbx,qualysapi
```

### Comparing `qualystbx-0.4.0/qualystbx.egg-info/SOURCES.txt` & `qualystbx-0.5.0/qualystbx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qualystbx-0.4.0/setup.py` & `qualystbx-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 long_description = (here_qualys_tbx / 'README.md').read_text(encoding='utf-8')
 
 
 setup(
     name='qualystbx',
-    version='0.4.0',
+    version='0.5.0',
     packages=find_packages(include=[
         'qualys_tbx',
         'qualys_tbx.qtbx_lib',
         'qualys_tbx.qtbx_policy_merge',
         'qualys_tbx.*',
         'qualys_tbx.qtbx_lib.*',
         'qualys_tbx.qtbx_policy_merge.*',
```

