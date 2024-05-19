# Comparing `tmp/e2D-1.4.8.tar.gz` & `tmp/e2D-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-1.4.8.tar", last modified: Sat Jan 27 02:50:14 2024, max compression
+gzip compressed data, was "e2D-1.4.9.tar", last modified: Sun Feb 11 03:44:07 2024, max compression
```

## Comparing `e2D-1.4.8.tar` & `e2D-1.4.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 02:50:14.578009 e2D-1.4.8/
--rw-rw-rw-   0        0        0     1066 2023-09-05 13:34:59.000000 e2D-1.4.8/LICENSE
--rw-rw-rw-   0        0        0     9608 2024-01-27 02:50:14.575008 e2D-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     8715 2023-09-16 00:14:51.000000 e2D-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-27 02:50:14.510000 e2D-1.4.8/e2D/
--rw-rw-rw-   0        0        0    34198 2024-01-27 02:46:41.000000 e2D-1.4.8/e2D/__init__.py
--rw-rw-rw-   0        0        0     4396 2024-01-27 02:49:18.000000 e2D-1.4.8/e2D/envs.py
--rw-rw-rw-   0        0        0    31542 2024-01-27 02:46:41.000000 e2D-1.4.8/e2D/plots.py
--rw-rw-rw-   0        0        0     5513 2024-01-27 02:46:41.000000 e2D-1.4.8/e2D/utils.py
--rw-rw-rw-   0        0        0     1218 2024-01-27 02:46:41.000000 e2D-1.4.8/e2D/winrec.py
-drwxrwxrwx   0        0        0        0 2024-01-27 02:50:14.572004 e2D-1.4.8/e2D.egg-info/
--rw-rw-rw-   0        0        0     9608 2024-01-27 02:50:14.000000 e2D-1.4.8/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-01-27 02:50:14.000000 e2D-1.4.8/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-27 02:50:14.000000 e2D-1.4.8/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-01-27 02:50:14.000000 e2D-1.4.8/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-01-27 02:50:14.000000 e2D-1.4.8/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      100 2023-09-05 13:34:59.000000 e2D-1.4.8/pyproject.toml
--rw-rw-rw-   0        0        0      730 2024-01-27 02:50:14.583005 e2D-1.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-11 03:44:07.799737 e2D-1.4.9/
+-rw-rw-rw-   0        0        0     1066 2023-09-05 13:34:59.000000 e2D-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0     9608 2024-02-11 03:44:07.798737 e2D-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8715 2023-09-16 00:14:51.000000 e2D-1.4.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-11 03:44:07.758736 e2D-1.4.9/e2D/
+-rw-rw-rw-   0        0        0    56506 2024-02-11 03:36:00.000000 e2D-1.4.9/e2D/__init__.py
+-rw-rw-rw-   0        0        0    37445 2024-02-11 01:49:19.000000 e2D-1.4.9/e2D/cvb.py
+-rw-rw-rw-   0        0        0     4396 2024-02-11 00:35:24.000000 e2D-1.4.9/e2D/envs.py
+-rw-rw-rw-   0        0        0    31542 2024-01-27 02:52:19.000000 e2D-1.4.9/e2D/plots.py
+-rw-rw-rw-   0        0        0     5513 2024-01-27 02:52:19.000000 e2D-1.4.9/e2D/utils.py
+-rw-rw-rw-   0        0        0     1218 2024-01-27 02:52:19.000000 e2D-1.4.9/e2D/winrec.py
+drwxrwxrwx   0        0        0        0 2024-02-11 03:44:07.795737 e2D-1.4.9/e2D.egg-info/
+-rw-rw-rw-   0        0        0     9608 2024-02-11 03:44:07.000000 e2D-1.4.9/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-02-11 03:44:07.000000 e2D-1.4.9/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-11 03:44:07.000000 e2D-1.4.9/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-02-11 03:44:07.000000 e2D-1.4.9/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-02-11 03:44:07.000000 e2D-1.4.9/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      100 2023-09-05 13:34:59.000000 e2D-1.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2024-02-11 03:44:07.802744 e2D-1.4.9/setup.cfg
```

### Comparing `e2D-1.4.8/LICENSE` & `e2D-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-1.4.8/PKG-INFO` & `e2D-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-1.4.8/README.md` & `e2D-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `e2D-1.4.8/e2D/envs.py` & `e2D-1.4.9/e2D/envs.py`

 * *Files identical despite different names*

### Comparing `e2D-1.4.8/e2D/plots.py` & `e2D-1.4.9/e2D/plots.py`

 * *Files identical despite different names*

### Comparing `e2D-1.4.8/e2D/utils.py` & `e2D-1.4.9/e2D/utils.py`

 * *Files identical despite different names*

### Comparing `e2D-1.4.8/e2D/winrec.py` & `e2D-1.4.9/e2D/winrec.py`

 * *Files identical despite different names*

### Comparing `e2D-1.4.8/e2D.egg-info/PKG-INFO` & `e2D-1.4.9/e2D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-1.4.8/setup.cfg` & `e2D-1.4.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 312e 342e 380d 0a61 7574 686f 7220  = 1.4.8..author 
+00000020: 3d20 312e 342e 390d 0a61 7574 686f 7220  = 1.4.9..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

