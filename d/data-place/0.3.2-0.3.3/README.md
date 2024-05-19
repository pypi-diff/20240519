# Comparing `tmp/data-place-0.3.2.tar.gz` & `tmp/data-place-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-place-0.3.2.tar", last modified: Sat May  4 00:00:00 2024, max compression
+gzip compressed data, was "data-place-0.3.3.tar", last modified: Sun May 19 16:10:05 2024, max compression
```

## Comparing `data-place-0.3.2.tar` & `data-place-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 00:00:00.059648 data-place-0.3.2/
--rw-rw-rw-   0        0        0       44 2024-05-03 23:59:59.000000 data-place-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6073 2024-05-04 00:00:00.058646 data-place-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.3.2/README.md
--rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.3.2/build.py
-drwxrwxrwx   0        0        0        0 2024-05-04 00:00:00.057385 data-place-0.3.2/data_place.egg-info/
--rw-rw-rw-   0        0        0     6073 2024-05-03 23:59:59.000000 data-place-0.3.2/data_place.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-05-03 23:59:59.000000 data-place-0.3.2/data_place.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:59:59.000000 data-place-0.3.2/data_place.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-03 23:59:59.000000 data-place-0.3.2/data_place.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 23:59:59.000000 data-place-0.3.2/data_place.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 00:00:00.055375 data-place-0.3.2/dataplace/
--rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.3.2/dataplace/__init__.py
--rw-rw-rw-   0        0        0     2048 2024-05-03 23:59:55.000000 data-place-0.3.2/dataplace/base.py
--rw-rw-rw-   0        0        0     2304 2024-01-27 08:30:20.000000 data-place-0.3.2/dataplace/callback.py
--rw-rw-rw-   0        0        0     3178 2024-05-03 10:26:32.000000 data-place-0.3.2/dataplace/control.py
--rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.3.2/dataplace/handler.py
--rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.3.2/dataplace/io.py
--rw-rw-rw-   0        0        0     8742 2024-05-03 15:20:22.000000 data-place-0.3.2/dataplace/receive.py
--rw-rw-rw-   0        0        0    11010 2024-05-03 15:20:22.000000 data-place-0.3.2/dataplace/send.py
--rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.3.2/dataplace/store.py
--rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 00:00:00.060649 data-place-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1615 2024-05-03 23:59:55.000000 data-place-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:10:05.176020 data-place-0.3.3/
+-rw-rw-rw-   0        0        0       44 2024-05-19 16:10:05.000000 data-place-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6073 2024-05-19 16:10:05.176020 data-place-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5156 2024-01-27 16:23:24.000000 data-place-0.3.3/README.md
+-rw-rw-rw-   0        0        0     9793 2024-04-19 12:34:18.000000 data-place-0.3.3/build.py
+drwxrwxrwx   0        0        0        0 2024-05-19 16:10:05.175020 data-place-0.3.3/data_place.egg-info/
+-rw-rw-rw-   0        0        0     6073 2024-05-19 16:10:05.000000 data-place-0.3.3/data_place.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-05-19 16:10:05.000000 data-place-0.3.3/data_place.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 16:10:05.000000 data-place-0.3.3/data_place.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-19 16:10:05.000000 data-place-0.3.3/data_place.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-19 16:10:05.000000 data-place-0.3.3/data_place.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 16:10:05.172999 data-place-0.3.3/dataplace/
+-rw-rw-rw-   0        0        0      269 2024-01-20 13:15:44.000000 data-place-0.3.3/dataplace/__init__.py
+-rw-rw-rw-   0        0        0     2048 2024-05-03 23:59:55.000000 data-place-0.3.3/dataplace/base.py
+-rw-rw-rw-   0        0        0     2665 2024-05-19 16:09:32.000000 data-place-0.3.3/dataplace/callback.py
+-rw-rw-rw-   0        0        0     3178 2024-05-03 10:26:32.000000 data-place-0.3.3/dataplace/control.py
+-rw-rw-rw-   0        0        0     3556 2024-02-11 17:10:37.000000 data-place-0.3.3/dataplace/handler.py
+-rw-rw-rw-   0        0        0     2771 2024-01-25 20:35:44.000000 data-place-0.3.3/dataplace/io.py
+-rw-rw-rw-   0        0        0     8742 2024-05-03 15:20:22.000000 data-place-0.3.3/dataplace/receive.py
+-rw-rw-rw-   0        0        0    11010 2024-05-03 15:20:22.000000 data-place-0.3.3/dataplace/send.py
+-rw-rw-rw-   0        0        0     7260 2024-04-27 12:38:35.000000 data-place-0.3.3/dataplace/store.py
+-rw-rw-rw-   0        0        0       10 2024-01-20 13:15:44.000000 data-place-0.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 16:10:05.177020 data-place-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2024-05-19 16:10:01.000000 data-place-0.3.3/setup.py
```

### Comparing `data-place-0.3.2/PKG-INFO` & `data-place-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.3.2
+Version: 0.3.3
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.3.2/README.md` & `data-place-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/build.py` & `data-place-0.3.3/build.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/data_place.egg-info/PKG-INFO` & `data-place-0.3.3/data_place.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-place
-Version: 0.3.2
+Version: 0.3.3
 Summary: A powerfull and flexible framework for designing async socket based data streaming and distribution systems, with automated parsing, dynamic data store and high-level control hooks.
 Home-page: https://github.com/Shahaf-F-S/data-place
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `data-place-0.3.2/dataplace/base.py` & `data-place-0.3.3/dataplace/base.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/dataplace/control.py` & `data-place-0.3.3/dataplace/control.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/dataplace/handler.py` & `data-place-0.3.3/dataplace/handler.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/dataplace/io.py` & `data-place-0.3.3/dataplace/io.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/dataplace/receive.py` & `data-place-0.3.3/dataplace/receive.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/dataplace/send.py` & `data-place-0.3.3/dataplace/send.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/dataplace/store.py` & `data-place-0.3.3/dataplace/store.py`

 * *Files identical despite different names*

### Comparing `data-place-0.3.2/setup.py` & `data-place-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='data-place',
-        version='0.3.2',
+        version='0.3.3',
         description=(
             "A powerfull and flexible framework for designing async "
             "socket based data streaming and distribution systems, "
             "with automated parsing, dynamic data store and "
             "high-level control hooks."
         ),
         license='MIT',
```

