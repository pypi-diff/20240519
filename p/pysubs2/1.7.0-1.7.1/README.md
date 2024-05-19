# Comparing `tmp/pysubs2-1.7.0.tar.gz` & `tmp/pysubs2-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysubs2-1.7.0.tar", last modified: Sun May 19 00:30:34 2024, max compression
+gzip compressed data, was "pysubs2-1.7.1.tar", last modified: Sun May 19 13:28:05 2024, max compression
```

## Comparing `pysubs2-1.7.0.tar` & `pysubs2-1.7.1.tar`

### file list

```diff
@@ -1,41 +1,52 @@
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 00:30:34.129229 pysubs2-1.7.0/
--rw-rw-r--   0 azar      (1000) azar      (1000)     1063 2024-05-19 00:27:32.000000 pysubs2-1.7.0/LICENSE.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)       17 2024-05-04 21:05:32.000000 pysubs2-1.7.0/MANIFEST.in
--rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-19 00:30:34.129229 pysubs2-1.7.0/PKG-INFO
--rw-rw-r--   0 azar      (1000) azar      (1000)     1883 2024-05-05 13:10:42.000000 pysubs2-1.7.0/README.md
--rw-rw-r--   0 azar      (1000) azar      (1000)       85 2023-11-25 17:38:44.000000 pysubs2-1.7.0/pyproject.toml
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 00:30:34.125229 pysubs2-1.7.0/pysubs2/
--rw-rw-r--   0 azar      (1000) azar      (1000)      783 2024-05-05 12:46:10.000000 pysubs2-1.7.0/pysubs2/__init__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)      134 2023-11-25 17:38:44.000000 pysubs2-1.7.0/pysubs2/__main__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    11916 2024-05-05 16:31:09.000000 pysubs2-1.7.0/pysubs2/cli.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1503 2024-05-18 23:48:58.000000 pysubs2-1.7.0/pysubs2/common.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2318 2024-05-05 12:46:10.000000 pysubs2-1.7.0/pysubs2/exceptions.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     6291 2024-05-05 12:11:24.000000 pysubs2-1.7.0/pysubs2/ssaevent.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    23833 2024-05-18 22:28:04.000000 pysubs2-1.7.0/pysubs2/ssafile.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4031 2024-05-04 22:58:07.000000 pysubs2-1.7.0/pysubs2/ssastyle.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4739 2024-05-05 12:11:24.000000 pysubs2-1.7.0/pysubs2/time.py
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 00:30:34.129229 pysubs2-1.7.0/pysubs2.egg-info/
--rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-19 00:30:34.000000 pysubs2-1.7.0/pysubs2.egg-info/PKG-INFO
--rw-rw-r--   0 azar      (1000) azar      (1000)      928 2024-05-19 00:30:34.000000 pysubs2-1.7.0/pysubs2.egg-info/SOURCES.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)        1 2024-05-19 00:30:34.000000 pysubs2-1.7.0/pysubs2.egg-info/dependency_links.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)       49 2024-05-19 00:30:34.000000 pysubs2-1.7.0/pysubs2.egg-info/entry_points.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)        8 2024-05-19 00:30:34.000000 pysubs2-1.7.0/pysubs2.egg-info/top_level.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)     1450 2024-05-19 00:30:34.129229 pysubs2-1.7.0/setup.cfg
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 00:30:34.125229 pysubs2-1.7.0/tests/
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 00:30:34.129229 pysubs2-1.7.0/tests/data/
--rw-rw-r--   0 azar      (1000) azar      (1000)   180220 2023-11-25 17:38:44.000000 pysubs2-1.7.0/tests/data/EBGaramond08-Italic.ttf
--rw-rw-r--   0 azar      (1000) azar      (1000)   280540 2023-11-25 17:38:44.000000 pysubs2-1.7.0/tests/data/EBGaramond08-Regular.ttf
--rw-rw-r--   0 azar      (1000) azar      (1000)      343 2023-11-25 17:38:44.000000 pysubs2-1.7.0/tests/data/LICENSE.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)   622857 2023-11-25 17:38:44.000000 pysubs2-1.7.0/tests/data/subtitle_with_attached_fonts_aegisub.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)   622702 2023-11-25 17:38:44.000000 pysubs2-1.7.0/tests/data/subtitle_with_attached_fonts_no_events.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)   622836 2024-05-05 14:45:39.000000 pysubs2-1.7.0/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)     3149 2023-11-25 17:38:44.000000 pysubs2-1.7.0/tests/data/subtitle_with_attached_images_aegisub.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)     3128 2024-05-05 14:45:39.000000 pysubs2-1.7.0/tests/data/subtitle_with_attached_images_pysubs2_ref.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)     4308 2024-05-04 23:54:09.000000 pysubs2-1.7.0/tests/test_attachment.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    17652 2024-05-05 16:36:24.000000 pysubs2-1.7.0/tests/test_cli.py
--rw-rw-r--   0 azar      (1000) azar      (1000)      266 2024-05-05 00:12:16.000000 pysubs2-1.7.0/tests/test_common.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1757 2024-05-05 12:11:24.000000 pysubs2-1.7.0/tests/test_parse_tags.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2246 2024-05-05 00:09:46.000000 pysubs2-1.7.0/tests/test_ssaevent.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4009 2024-05-04 23:59:43.000000 pysubs2-1.7.0/tests/test_ssafile.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1252 2024-05-05 00:11:48.000000 pysubs2-1.7.0/tests/test_ssastyle.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     7386 2024-05-05 00:07:52.000000 pysubs2-1.7.0/tests/test_time.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1063 2024-05-19 00:27:32.000000 pysubs2-1.7.1/LICENSE.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)       82 2024-05-19 13:25:10.000000 pysubs2-1.7.1/MANIFEST.in
+-rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-19 13:28:05.047193 pysubs2-1.7.1/PKG-INFO
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1883 2024-05-05 13:10:42.000000 pysubs2-1.7.1/README.md
+-rw-rw-r--   0 azar      (1000) azar      (1000)       85 2023-11-25 17:38:44.000000 pysubs2-1.7.1/pyproject.toml
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.043193 pysubs2-1.7.1/pysubs2/
+-rw-rw-r--   0 azar      (1000) azar      (1000)      783 2024-05-05 12:46:10.000000 pysubs2-1.7.1/pysubs2/__init__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      134 2023-11-25 17:38:44.000000 pysubs2-1.7.1/pysubs2/__main__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    11916 2024-05-05 16:31:09.000000 pysubs2-1.7.1/pysubs2/cli.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1503 2024-05-19 13:25:10.000000 pysubs2-1.7.1/pysubs2/common.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2318 2024-05-05 12:46:10.000000 pysubs2-1.7.1/pysubs2/exceptions.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.043193 pysubs2-1.7.1/pysubs2/formats/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2515 2024-05-18 22:16:41.000000 pysubs2-1.7.1/pysubs2/formats/__init__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2959 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/base.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2101 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/jsonformat.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     5970 2024-05-19 00:09:39.000000 pysubs2-1.7.1/pysubs2/formats/microdvd.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1970 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/mpl2.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     7484 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/subrip.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    16795 2024-05-05 14:45:39.000000 pysubs2-1.7.1/pysubs2/formats/substation.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4100 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/tmp.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1788 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/webvtt.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1607 2024-05-05 12:42:39.000000 pysubs2-1.7.1/pysubs2/formats/whisper.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     6291 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/ssaevent.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    23833 2024-05-18 22:28:04.000000 pysubs2-1.7.1/pysubs2/ssafile.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4031 2024-05-04 22:58:07.000000 pysubs2-1.7.1/pysubs2/ssastyle.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4739 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/time.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/pysubs2.egg-info/
+-rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/PKG-INFO
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1382 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/SOURCES.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)        1 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/dependency_links.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)       49 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/entry_points.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)        8 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/top_level.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1469 2024-05-19 13:28:05.051193 pysubs2-1.7.1/setup.cfg
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/tests/
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/tests/data/
+-rw-rw-r--   0 azar      (1000) azar      (1000)   180220 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/EBGaramond08-Italic.ttf
+-rw-rw-r--   0 azar      (1000) azar      (1000)   280540 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/EBGaramond08-Regular.ttf
+-rw-rw-r--   0 azar      (1000) azar      (1000)      343 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/LICENSE.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)   622857 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_aegisub.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)   622702 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_no_events.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)   622836 2024-05-05 14:45:39.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3149 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_images_aegisub.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3128 2024-05-05 14:45:39.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_images_pysubs2_ref.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4308 2024-05-04 23:54:09.000000 pysubs2-1.7.1/tests/test_attachment.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    17652 2024-05-05 16:36:24.000000 pysubs2-1.7.1/tests/test_cli.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      266 2024-05-05 00:12:16.000000 pysubs2-1.7.1/tests/test_common.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1757 2024-05-05 12:11:24.000000 pysubs2-1.7.1/tests/test_parse_tags.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2246 2024-05-05 00:09:46.000000 pysubs2-1.7.1/tests/test_ssaevent.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4009 2024-05-04 23:59:43.000000 pysubs2-1.7.1/tests/test_ssafile.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1252 2024-05-05 00:11:48.000000 pysubs2-1.7.1/tests/test_ssastyle.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     7386 2024-05-05 00:07:52.000000 pysubs2-1.7.1/tests/test_time.py
```

### Comparing `pysubs2-1.7.0/LICENSE.txt` & `pysubs2-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/PKG-INFO` & `pysubs2-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubs2
-Version: 1.7.0
+Version: 1.7.1
 Summary: A library for editing subtitle files
 Home-page: https://github.com/tkarabela/pysubs2
 Author: Tomas Karabela
 Author-email: tkarabela@seznam.cz
 License: MIT
 Project-URL: Documentation, https://pysubs2.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/tkarabela/pysubs2/issues
```

### Comparing `pysubs2-1.7.0/README.md` & `pysubs2-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/__init__.py` & `pysubs2-1.7.1/pysubs2/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/cli.py` & `pysubs2-1.7.1/pysubs2/cli.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/common.py` & `pysubs2-1.7.1/pysubs2/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,11 +54,11 @@
         return SSA_ALIGNMENT[self.value - 1]
 
 
 SSA_ALIGNMENT: Tuple[int, ...] = (1, 2, 3, 9, 10, 11, 5, 6, 7)
 
 
 #: Version of the pysubs2 library.
-VERSION = "1.7.0"
+VERSION = "1.7.1"
 
 
 IntOrFloat = Union[int, float]
```

### Comparing `pysubs2-1.7.0/pysubs2/exceptions.py` & `pysubs2-1.7.1/pysubs2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/ssaevent.py` & `pysubs2-1.7.1/pysubs2/ssaevent.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/ssafile.py` & `pysubs2-1.7.1/pysubs2/ssafile.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/ssastyle.py` & `pysubs2-1.7.1/pysubs2/ssastyle.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2/time.py` & `pysubs2-1.7.1/pysubs2/time.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/pysubs2.egg-info/PKG-INFO` & `pysubs2-1.7.1/pysubs2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubs2
-Version: 1.7.0
+Version: 1.7.1
 Summary: A library for editing subtitle files
 Home-page: https://github.com/tkarabela/pysubs2
 Author: Tomas Karabela
 Author-email: tkarabela@seznam.cz
 License: MIT
 Project-URL: Documentation, https://pysubs2.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/tkarabela/pysubs2/issues
```

### Comparing `pysubs2-1.7.0/setup.cfg` & `pysubs2-1.7.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 	Intended Audience :: Developers
 	Intended Audience :: End Users/Desktop
 	Operating System :: OS Independent
 	License :: OSI Approved :: MIT License
 	Typing :: Typed
 
 [options]
-packages = pysubs2
+packages = 
+	pysubs2
+	pysubs2.formats
 python_requires = >=3.8
 
 [options.entry_points]
 console_scripts = 
 	pysubs2 = pysubs2.cli:__main__
 
 [mypy]
```

### Comparing `pysubs2-1.7.0/tests/data/EBGaramond08-Italic.ttf` & `pysubs2-1.7.1/tests/data/EBGaramond08-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/data/EBGaramond08-Regular.ttf` & `pysubs2-1.7.1/tests/data/EBGaramond08-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/data/subtitle_with_attached_fonts_aegisub.ass` & `pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_aegisub.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/data/subtitle_with_attached_fonts_no_events.ass` & `pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_no_events.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass` & `pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/data/subtitle_with_attached_images_aegisub.ass` & `pysubs2-1.7.1/tests/data/subtitle_with_attached_images_aegisub.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/data/subtitle_with_attached_images_pysubs2_ref.ass` & `pysubs2-1.7.1/tests/data/subtitle_with_attached_images_pysubs2_ref.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_attachment.py` & `pysubs2-1.7.1/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_cli.py` & `pysubs2-1.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_parse_tags.py` & `pysubs2-1.7.1/tests/test_parse_tags.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_ssaevent.py` & `pysubs2-1.7.1/tests/test_ssaevent.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_ssafile.py` & `pysubs2-1.7.1/tests/test_ssafile.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_ssastyle.py` & `pysubs2-1.7.1/tests/test_ssastyle.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.0/tests/test_time.py` & `pysubs2-1.7.1/tests/test_time.py`

 * *Files identical despite different names*

