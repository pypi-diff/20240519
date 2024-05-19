# Comparing `tmp/photobooth-0.0.1b2.tar.gz` & `tmp/photobooth-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photobooth-0.0.1b2.tar", last modified: Thu Sep  7 18:39:49 2023, max compression
+gzip compressed data, was "photobooth-0.0.1b3.tar", last modified: Sun May 19 11:46:32 2024, max compression
```

## Comparing `photobooth-0.0.1b2.tar` & `photobooth-0.0.1b3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.009058 photobooth-0.0.1b2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-09-07 18:39:49.009058 photobooth-0.0.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-07 18:39:49.009058 photobooth-0.0.1b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.001058 photobooth-0.0.1b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.001058 photobooth-0.0.1b2/src/photobooth/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.001058 photobooth-0.0.1b2/src/photobooth/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/adapters/buttons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/adapters/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/adapters/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.005058 photobooth-0.0.1b2/src/photobooth/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/entrypoints/main_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/entrypoints/page_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/entrypoints/picture_item.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.005058 photobooth-0.0.1b2/src/photobooth/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  2872296 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/resources/oak.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.005058 photobooth-0.0.1b2/src/photobooth/service_layer/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/service_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2023-09-07 18:39:29.000000 photobooth-0.0.1b2/src/photobooth/service_layer/messagebus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-07 18:39:49.001058 photobooth-0.0.1b2/src/photobooth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-09-07 18:39:48.000000 photobooth-0.0.1b2/src/photobooth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-09-07 18:39:49.000000 photobooth-0.0.1b2/src/photobooth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-07 18:39:48.000000 photobooth-0.0.1b2/src/photobooth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-09-07 18:39:48.000000 photobooth-0.0.1b2/src/photobooth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-07 18:39:48.000000 photobooth-0.0.1b2/src/photobooth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-07 18:39:48.000000 photobooth-0.0.1b2/src/photobooth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.142351 photobooth-0.0.1b3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-19 11:46:32.138351 photobooth-0.0.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:46:32.142351 photobooth-0.0.1b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.130351 photobooth-0.0.1b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.130351 photobooth-0.0.1b3/src/photobooth/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.134351 photobooth-0.0.1b3/src/photobooth/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/adapters/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/adapters/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/adapters/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.134351 photobooth-0.0.1b3/src/photobooth/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/entrypoints/main_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/entrypoints/page_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/entrypoints/picture_item.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.134351 photobooth-0.0.1b3/src/photobooth/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  2872296 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/resources/oak.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.138351 photobooth-0.0.1b3/src/photobooth/service_layer/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/service_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-19 11:46:26.000000 photobooth-0.0.1b3/src/photobooth/service_layer/messagebus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:46:32.138351 photobooth-0.0.1b3/src/photobooth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-19 11:46:32.000000 photobooth-0.0.1b3/src/photobooth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-19 11:46:32.000000 photobooth-0.0.1b3/src/photobooth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:46:32.000000 photobooth-0.0.1b3/src/photobooth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 11:46:32.000000 photobooth-0.0.1b3/src/photobooth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-19 11:46:32.000000 photobooth-0.0.1b3/src/photobooth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 11:46:32.000000 photobooth-0.0.1b3/src/photobooth.egg-info/top_level.txt
```

### Comparing `photobooth-0.0.1b2/LICENSE` & `photobooth-0.0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/PKG-INFO` & `photobooth-0.0.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Photobooth python package. Based on QTs Web Interface and gphoto2 package.
 Author-email: Patrick Schleiter <git.pschleiter@gmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/pschleiter/photobooth
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics :: Capture
 Classifier: Intended Audience :: End Users/Desktop
@@ -20,15 +20,15 @@
 Requires-Dist: click>=8.1.3
 Requires-Dist: pyqt5>=5.15.2
 Provides-Extra: rpi
 Requires-Dist: gpiozero==1.6.2; extra == "rpi"
 Provides-Extra: dslr
 Requires-Dist: gphoto2==2.3.4; extra == "dslr"
 Provides-Extra: upload
-Requires-Dist: requests==2.29.0; extra == "upload"
+Requires-Dist: httpx==0.27.0; extra == "upload"
 Requires-Dist: pillow>=10.0.0; extra == "upload"
 
 # Photobooth
 
 > Photobooth application purely written in Python. Controlling a dslr camera and capturing photo.
 
 ![PyPI - Licence](https://img.shields.io/pypi/l/photobooth)
```

### Comparing `photobooth-0.0.1b2/README.md` & `photobooth-0.0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/pyproject.toml` & `photobooth-0.0.1b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 35.0.2", "wheel >= 0.29.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "photobooth"
-authors = [{ name = "Patrick Schleiter", email = "git.pschleiter@gmail.com"}]
+authors = [{ name = "Patrick Schleiter", email = "git.pschleiter@gmail.com" }]
 description = "Photobooth python package. Based on QTs Web Interface and gphoto2 package."
 requires-python = ">=3.9.2"
 license = { text = "MIT License" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Multimedia :: Graphics :: Capture",
     "Intended Audience :: End Users/Desktop",
@@ -21,15 +21,15 @@
 ]
 dependencies = ["click>=8.1.3", "pyqt5>=5.15.2"]
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 rpi = ["gpiozero==1.6.2"]
 dslr = ["gphoto2==2.3.4"]
-upload = ["requests==2.29.0", "pillow>=10.0.0"]
+upload = ["httpx==0.27.0", "pillow>=10.0.0"]
 
 [project.scripts]
 photobooth = "photobooth.cli:cli"
 
 [project.urls]
 "Source Code" = "https://github.com/pschleiter/photobooth"
```

### Comparing `photobooth-0.0.1b2/src/photobooth/adapters/buttons.py` & `photobooth-0.0.1b3/src/photobooth/adapters/buttons.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/adapters/camera.py` & `photobooth-0.0.1b3/src/photobooth/adapters/camera.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/adapters/upload.py` & `photobooth-0.0.1b3/src/photobooth/adapters/upload.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,36 +9,32 @@
         domain: str,
         resolution: typing.Tuple[int, int],
         auth: typing.Optional[typing.Tuple[str, str]],
         *args,
         **kwargs,
     ) -> None:
         super().__init__(*args, **kwargs)
+        import httpx
 
-        self._domain = domain
+        self._client = httpx.Client(
+            auth=auth,
+        )
+        self._url = domain
         self._resolution = resolution
-        self._auth = auth
 
     def upload(self, image_data: bytes, filename: str):
         try:
-            import requests
-            from requests.auth import HTTPDigestAuth
             from PIL import Image
 
             image = Image.open(io.BytesIO(image_data))
             image.thumbnail(self._resolution)
             buffer = io.BytesIO()
             image.save(buffer, "JPEG", exif=image.getexif())
             buffer.seek(0)
 
-            auth = None
-            if self._auth is not None:
-                auth = HTTPDigestAuth(*self._auth)
-
-            requests.put(
-                self._domain,
+            self._client.put(
+                self._url,
                 params=dict(filename=filename),
                 data=buffer.getvalue(),
-                auth=auth,
             )
         except Exception:
             pass
```

### Comparing `photobooth-0.0.1b2/src/photobooth/cli.py` & `photobooth-0.0.1b3/src/photobooth/cli.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/config.py` & `photobooth-0.0.1b3/src/photobooth/config.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/entrypoints/main_widget.py` & `photobooth-0.0.1b3/src/photobooth/entrypoints/main_widget.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/entrypoints/page_widget.py` & `photobooth-0.0.1b3/src/photobooth/entrypoints/page_widget.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/entrypoints/picture_item.py` & `photobooth-0.0.1b3/src/photobooth/entrypoints/picture_item.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/resources/oak.jpg` & `photobooth-0.0.1b3/src/photobooth/resources/oak.jpg`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth/service_layer/messagebus.py` & `photobooth-0.0.1b3/src/photobooth/service_layer/messagebus.py`

 * *Files identical despite different names*

### Comparing `photobooth-0.0.1b2/src/photobooth.egg-info/PKG-INFO` & `photobooth-0.0.1b3/src/photobooth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Photobooth python package. Based on QTs Web Interface and gphoto2 package.
 Author-email: Patrick Schleiter <git.pschleiter@gmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/pschleiter/photobooth
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Multimedia :: Graphics :: Capture
 Classifier: Intended Audience :: End Users/Desktop
@@ -20,15 +20,15 @@
 Requires-Dist: click>=8.1.3
 Requires-Dist: pyqt5>=5.15.2
 Provides-Extra: rpi
 Requires-Dist: gpiozero==1.6.2; extra == "rpi"
 Provides-Extra: dslr
 Requires-Dist: gphoto2==2.3.4; extra == "dslr"
 Provides-Extra: upload
-Requires-Dist: requests==2.29.0; extra == "upload"
+Requires-Dist: httpx==0.27.0; extra == "upload"
 Requires-Dist: pillow>=10.0.0; extra == "upload"
 
 # Photobooth
 
 > Photobooth application purely written in Python. Controlling a dslr camera and capturing photo.
 
 ![PyPI - Licence](https://img.shields.io/pypi/l/photobooth)
```

### Comparing `photobooth-0.0.1b2/src/photobooth.egg-info/SOURCES.txt` & `photobooth-0.0.1b3/src/photobooth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

