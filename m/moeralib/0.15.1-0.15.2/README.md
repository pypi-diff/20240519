# Comparing `tmp/moeralib-0.15.1.tar.gz` & `tmp/moeralib-0.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moeralib-0.15.1.tar", last modified: Sun Mar 17 03:19:28 2024, max compression
+gzip compressed data, was "moeralib-0.15.2.tar", last modified: Sun May 19 03:58:14 2024, max compression
```

## Comparing `moeralib-0.15.1.tar` & `moeralib-0.15.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.558638 moeralib-0.15.1/
--rw-rw-r--   0 balu      (1000) balu      (1000)     4302 2023-10-20 12:34:37.000000 moeralib-0.15.1/.gitignore
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.550638 moeralib-0.15.1/.idea/
--rw-rw-r--   0 balu      (1000) balu      (1000)       47 2023-10-20 12:36:28.000000 moeralib-0.15.1/.idea/.gitignore
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.550638 moeralib-0.15.1/.idea/inspectionProfiles/
--rw-rw-r--   0 balu      (1000) balu      (1000)     1009 2023-10-20 12:36:28.000000 moeralib-0.15.1/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-r--   0 balu      (1000) balu      (1000)      174 2024-01-31 02:27:06.000000 moeralib-0.15.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-r--   0 balu      (1000) balu      (1000)      314 2024-01-31 02:27:06.000000 moeralib-0.15.1/.idea/misc.xml
--rw-rw-r--   0 balu      (1000) balu      (1000)      282 2023-10-20 12:36:28.000000 moeralib-0.15.1/.idea/modules.xml
--rw-rw-r--   0 balu      (1000) balu      (1000)      352 2023-10-24 22:06:32.000000 moeralib-0.15.1/.idea/python-moeralib.iml
--rw-rw-r--   0 balu      (1000) balu      (1000)      167 2023-10-20 12:36:28.000000 moeralib-0.15.1/.idea/vcs.xml
--rw-rw-r--   0 balu      (1000) balu      (1000)    11357 2023-10-20 12:33:18.000000 moeralib-0.15.1/LICENSE
--rw-r--r--   0 balu      (1000) balu      (1000)     1090 2024-03-17 03:19:28.558638 moeralib-0.15.1/PKG-INFO
--rw-rw-r--   0 balu      (1000) balu      (1000)      236 2023-10-27 00:04:42.000000 moeralib-0.15.1/README.md
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.554638 moeralib-0.15.1/py-moera-api/
--rwxrwxr-x   0 balu      (1000) balu      (1000)       40 2023-09-18 15:58:05.000000 moeralib-0.15.1/py-moera-api/py-moera-api
--rw-rw-r--   0 balu      (1000) balu      (1000)    22558 2024-03-14 23:59:14.000000 moeralib-0.15.1/py-moera-api/pymoeraapi.py
--rw-rw-r--   0 balu      (1000) balu      (1000)      936 2024-03-17 03:18:49.000000 moeralib-0.15.1/pyproject.toml
--rw-rw-r--   0 balu      (1000) balu      (1000)      223 2024-03-17 03:19:28.558638 moeralib-0.15.1/setup.cfg
--rw-rw-r--   0 balu      (1000) balu      (1000)      197 2024-03-17 03:18:49.000000 moeralib-0.15.1/setup.py
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.550638 moeralib-0.15.1/src/
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.554638 moeralib-0.15.1/src/moeralib/
--rw-rw-r--   0 balu      (1000) balu      (1000)       33 2023-10-20 12:57:03.000000 moeralib-0.15.1/src/moeralib/__init__.py
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.554638 moeralib-0.15.1/src/moeralib/naming/
--rw-rw-r--   0 balu      (1000) balu      (1000)      152 2023-10-20 12:57:03.000000 moeralib-0.15.1/src/moeralib/naming/__init__.py
--rw-rw-r--   0 balu      (1000) balu      (1000)    10721 2024-03-15 14:00:00.000000 moeralib-0.15.1/src/moeralib/naming/naming.py
--rw-rw-r--   0 balu      (1000) balu      (1000)     1972 2023-10-20 12:57:03.000000 moeralib-0.15.1/src/moeralib/naming/schemas.py
--rw-rw-r--   0 balu      (1000) balu      (1000)     1907 2023-10-23 00:34:56.000000 moeralib-0.15.1/src/moeralib/naming/types.py
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.554638 moeralib-0.15.1/src/moeralib/node/
--rw-rw-r--   0 balu      (1000) balu      (1000)      185 2023-10-24 21:51:41.000000 moeralib-0.15.1/src/moeralib/node/__init__.py
--rw-rw-r--   0 balu      (1000) balu      (1000)    10248 2023-10-29 20:58:26.000000 moeralib-0.15.1/src/moeralib/node/caller.py
--rw-rw-r--   0 balu      (1000) balu      (1000)     1547 2023-10-25 00:20:03.000000 moeralib-0.15.1/src/moeralib/node/cartes.py
--rw-rw-r--   0 balu      (1000) balu      (1000)   101463 2024-03-17 02:39:27.000000 moeralib-0.15.1/src/moeralib/node/node.py
--rw-rw-r--   0 balu      (1000) balu      (1000)    72652 2024-03-17 02:39:27.000000 moeralib-0.15.1/src/moeralib/node/schemas.py
--rw-rw-r--   0 balu      (1000) balu      (1000)   118215 2024-03-17 02:39:27.000000 moeralib-0.15.1/src/moeralib/node/types.py
--rw-rw-r--   0 balu      (1000) balu      (1000)        0 2023-10-20 12:57:03.000000 moeralib-0.15.1/src/moeralib/py.typed
--rw-rw-r--   0 balu      (1000) balu      (1000)     3652 2023-11-02 03:30:15.000000 moeralib-0.15.1/src/moeralib/structure.py
--rw-rw-r--   0 balu      (1000) balu      (1000)     6646 2024-03-17 03:18:15.000000 moeralib-0.15.1/src/moeralib/universal_location.py
-drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-03-17 03:19:28.558638 moeralib-0.15.1/src/moeralib.egg-info/
--rw-r--r--   0 balu      (1000) balu      (1000)     1090 2024-03-17 03:19:28.000000 moeralib-0.15.1/src/moeralib.egg-info/PKG-INFO
--rw-rw-r--   0 balu      (1000) balu      (1000)      874 2024-03-17 03:19:28.000000 moeralib-0.15.1/src/moeralib.egg-info/SOURCES.txt
--rw-rw-r--   0 balu      (1000) balu      (1000)        1 2024-03-17 03:19:28.000000 moeralib-0.15.1/src/moeralib.egg-info/dependency_links.txt
--rw-rw-r--   0 balu      (1000) balu      (1000)       52 2024-03-17 03:19:28.000000 moeralib-0.15.1/src/moeralib.egg-info/requires.txt
--rw-rw-r--   0 balu      (1000) balu      (1000)        9 2024-03-17 03:19:28.000000 moeralib-0.15.1/src/moeralib.egg-info/top_level.txt
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.586640 moeralib-0.15.2/
+-rw-rw-r--   0 balu      (1000) balu      (1000)     4302 2023-10-20 12:34:37.000000 moeralib-0.15.2/.gitignore
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.582641 moeralib-0.15.2/.idea/
+-rw-rw-r--   0 balu      (1000) balu      (1000)       47 2023-10-20 12:36:28.000000 moeralib-0.15.2/.idea/.gitignore
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.582641 moeralib-0.15.2/.idea/inspectionProfiles/
+-rw-rw-r--   0 balu      (1000) balu      (1000)     1009 2023-10-20 12:36:28.000000 moeralib-0.15.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-r--   0 balu      (1000) balu      (1000)      174 2024-01-31 02:27:06.000000 moeralib-0.15.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-r--   0 balu      (1000) balu      (1000)      314 2024-01-31 02:27:06.000000 moeralib-0.15.2/.idea/misc.xml
+-rw-rw-r--   0 balu      (1000) balu      (1000)      282 2023-10-20 12:36:28.000000 moeralib-0.15.2/.idea/modules.xml
+-rw-rw-r--   0 balu      (1000) balu      (1000)      352 2023-10-24 22:06:32.000000 moeralib-0.15.2/.idea/python-moeralib.iml
+-rw-rw-r--   0 balu      (1000) balu      (1000)      167 2023-10-20 12:36:28.000000 moeralib-0.15.2/.idea/vcs.xml
+-rw-rw-r--   0 balu      (1000) balu      (1000)    11357 2023-10-20 12:33:18.000000 moeralib-0.15.2/LICENSE
+-rw-r--r--   0 balu      (1000) balu      (1000)     1090 2024-05-19 03:58:14.586640 moeralib-0.15.2/PKG-INFO
+-rw-rw-r--   0 balu      (1000) balu      (1000)      236 2023-10-27 00:04:42.000000 moeralib-0.15.2/README.md
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.582641 moeralib-0.15.2/py-moera-api/
+-rwxrwxr-x   0 balu      (1000) balu      (1000)       40 2023-09-18 15:58:05.000000 moeralib-0.15.2/py-moera-api/py-moera-api
+-rw-rw-r--   0 balu      (1000) balu      (1000)    22558 2024-03-14 23:59:14.000000 moeralib-0.15.2/py-moera-api/pymoeraapi.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)      936 2024-05-19 03:55:58.000000 moeralib-0.15.2/pyproject.toml
+-rw-rw-r--   0 balu      (1000) balu      (1000)      223 2024-05-19 03:58:14.586640 moeralib-0.15.2/setup.cfg
+-rw-rw-r--   0 balu      (1000) balu      (1000)      197 2024-05-19 03:55:58.000000 moeralib-0.15.2/setup.py
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.582641 moeralib-0.15.2/src/
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.582641 moeralib-0.15.2/src/moeralib/
+-rw-rw-r--   0 balu      (1000) balu      (1000)       33 2023-10-20 12:57:03.000000 moeralib-0.15.2/src/moeralib/__init__.py
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.586640 moeralib-0.15.2/src/moeralib/naming/
+-rw-rw-r--   0 balu      (1000) balu      (1000)      152 2023-10-20 12:57:03.000000 moeralib-0.15.2/src/moeralib/naming/__init__.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)    10721 2024-03-15 14:00:00.000000 moeralib-0.15.2/src/moeralib/naming/naming.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)     1972 2023-10-20 12:57:03.000000 moeralib-0.15.2/src/moeralib/naming/schemas.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)     1907 2023-10-23 00:34:56.000000 moeralib-0.15.2/src/moeralib/naming/types.py
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.586640 moeralib-0.15.2/src/moeralib/node/
+-rw-rw-r--   0 balu      (1000) balu      (1000)      185 2023-10-24 21:51:41.000000 moeralib-0.15.2/src/moeralib/node/__init__.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)    10248 2023-10-29 20:58:26.000000 moeralib-0.15.2/src/moeralib/node/caller.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)     1547 2023-10-25 00:20:03.000000 moeralib-0.15.2/src/moeralib/node/cartes.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)   101463 2024-05-16 22:38:25.000000 moeralib-0.15.2/src/moeralib/node/node.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)    72800 2024-05-16 22:38:25.000000 moeralib-0.15.2/src/moeralib/node/schemas.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)   118735 2024-05-16 22:38:25.000000 moeralib-0.15.2/src/moeralib/node/types.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)        0 2023-10-20 12:57:03.000000 moeralib-0.15.2/src/moeralib/py.typed
+-rw-rw-r--   0 balu      (1000) balu      (1000)     3652 2023-11-02 03:30:15.000000 moeralib-0.15.2/src/moeralib/structure.py
+-rw-rw-r--   0 balu      (1000) balu      (1000)     6646 2024-03-17 03:18:15.000000 moeralib-0.15.2/src/moeralib/universal_location.py
+drwxrwxr-x   0 balu      (1000) balu      (1000)        0 2024-05-19 03:58:14.586640 moeralib-0.15.2/src/moeralib.egg-info/
+-rw-r--r--   0 balu      (1000) balu      (1000)     1090 2024-05-19 03:58:14.000000 moeralib-0.15.2/src/moeralib.egg-info/PKG-INFO
+-rw-rw-r--   0 balu      (1000) balu      (1000)      874 2024-05-19 03:58:14.000000 moeralib-0.15.2/src/moeralib.egg-info/SOURCES.txt
+-rw-rw-r--   0 balu      (1000) balu      (1000)        1 2024-05-19 03:58:14.000000 moeralib-0.15.2/src/moeralib.egg-info/dependency_links.txt
+-rw-rw-r--   0 balu      (1000) balu      (1000)       52 2024-05-19 03:58:14.000000 moeralib-0.15.2/src/moeralib.egg-info/requires.txt
+-rw-rw-r--   0 balu      (1000) balu      (1000)        9 2024-05-19 03:58:14.000000 moeralib-0.15.2/src/moeralib.egg-info/top_level.txt
```

### Comparing `moeralib-0.15.1/.gitignore` & `moeralib-0.15.2/.gitignore`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/.idea/inspectionProfiles/Project_Default.xml` & `moeralib-0.15.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/LICENSE` & `moeralib-0.15.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/PKG-INFO` & `moeralib-0.15.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moeralib
-Version: 0.15.1
+Version: 0.15.2
 Summary: Library to interact with Moera decentralized social network
 Author-email: Shmuel Leib Melamud <balu@moera.org>
 Project-URL: Homepage, https://github.com/MoeraOrg/python-moeralib
 Project-URL: Bug Tracker, https://github.com/MoeraOrg/moera-issues/issues
 Project-URL: Overview, https://moera.org
 Keywords: Moera,library,naming,node,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moeralib-0.15.1/py-moera-api/pymoeraapi.py` & `moeralib-0.15.2/py-moera-api/pymoeraapi.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/pyproject.toml` & `moeralib-0.15.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moeralib"
-version = "0.15.1"
+version = "0.15.2"
 authors = [
     {name = "Shmuel Leib Melamud", email = "balu@moera.org"},
 ]
 description = "Library to interact with Moera decentralized social network"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["Moera", "library", "naming", "node", "API"]
```

### Comparing `moeralib-0.15.1/src/moeralib/naming/naming.py` & `moeralib-0.15.2/src/moeralib/naming/naming.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/naming/schemas.py` & `moeralib-0.15.2/src/moeralib/naming/schemas.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/naming/types.py` & `moeralib-0.15.2/src/moeralib/naming/types.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/node/caller.py` & `moeralib-0.15.2/src/moeralib/node/caller.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/node/cartes.py` & `moeralib-0.15.2/src/moeralib/node/cartes.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/node/node.py` & `moeralib-0.15.2/src/moeralib/node/node.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/node/schemas.py` & `moeralib-0.15.2/src/moeralib/node/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,14 +920,17 @@
 
 MEDIA_FILE_PREVIEW_INFO_SCHEMA: Any = {
     "type": "object",
     "properties": {
         "targetWidth": {
             "type": "integer"
         },
+        "directPath": {
+            "type": ["string", "null"]
+        },
         "width": {
             "type": "integer"
         },
         "height": {
             "type": "integer"
         },
         "original": {
@@ -1075,14 +1078,17 @@
         },
         "hash": {
             "type": "string"
         },
         "path": {
             "type": "string"
         },
+        "directPath": {
+            "type": ["string", "null"]
+        },
         "mimeType": {
             "type": "string"
         },
         "width": {
             "type": ["integer", "null"]
         },
         "height": {
```

### Comparing `moeralib-0.15.1/src/moeralib/node/types.py` & `moeralib-0.15.2/src/moeralib/node/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,14 +1071,19 @@
     image_url: str | None = None
     """URL of the image presenting the page"""
 
 
 class MediaFilePreviewInfo(Structure):
     target_width: int
     """the width the preview was prepared for viewing at"""
+    direct_path: str | None = None
+    """
+    location of the media file, relative to the ``/media``; points to a static image served directly from a filesystem;
+    static images do not accept any query parameters including authentication parameters
+    """
     width: int
     """actual width of the preview in pixels"""
     height: int
     """actual height of the preview in pixels"""
     original: bool | None = None
     """``True`` if the preview is identical to the original media, ``False`` otherwise"""
 
@@ -1211,14 +1216,19 @@
 class PrivateMediaFileInfo(Structure):
     id: str
     """ID of the media file"""
     hash: str
     """SHA-1 hash of the media file"""
     path: str
     """virtual location of the media file, relative to the ``/media`` virtual page"""
+    direct_path: str | None = None
+    """
+    location of the media file, relative to the ``/media``; points to a static image served directly from a filesystem;
+    static images do not accept any query parameters including authentication parameters
+    """
     mime_type: str
     """MIME type of the media"""
     width: int | None = None
     """width of the media in pixels (``None``, if the media file is not an image or video)"""
     height: int | None = None
     """height of the media in pixels (``None``, if the media file is not an image or video)"""
     orientation: int | None = None
```

### Comparing `moeralib-0.15.1/src/moeralib/structure.py` & `moeralib-0.15.2/src/moeralib/structure.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib/universal_location.py` & `moeralib-0.15.2/src/moeralib/universal_location.py`

 * *Files identical despite different names*

### Comparing `moeralib-0.15.1/src/moeralib.egg-info/PKG-INFO` & `moeralib-0.15.2/src/moeralib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moeralib
-Version: 0.15.1
+Version: 0.15.2
 Summary: Library to interact with Moera decentralized social network
 Author-email: Shmuel Leib Melamud <balu@moera.org>
 Project-URL: Homepage, https://github.com/MoeraOrg/python-moeralib
 Project-URL: Bug Tracker, https://github.com/MoeraOrg/moera-issues/issues
 Project-URL: Overview, https://moera.org
 Keywords: Moera,library,naming,node,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `moeralib-0.15.1/src/moeralib.egg-info/SOURCES.txt` & `moeralib-0.15.2/src/moeralib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

