# Comparing `tmp/srt_trans-1.0.8.tar.gz` & `tmp/srt_trans-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srt_trans-1.0.8.tar", last modified: Thu Apr  4 19:33:00 2024, max compression
+gzip compressed data, was "srt_trans-1.0.9.tar", last modified: Thu Apr  4 19:42:07 2024, max compression
```

## Comparing `srt_trans-1.0.8.tar` & `srt_trans-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 19:33:00.355875 srt_trans-1.0.8/
--rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1873 2024-04-04 19:33:00.353549 srt_trans-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2024-04-04 19:01:00.000000 srt_trans-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 19:33:00.356691 srt_trans-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1045 2024-04-04 19:32:50.000000 srt_trans-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:33:00.312174 srt_trans-1.0.8/srt_trans/
--rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.8/srt_trans/__init__.py
--rw-rw-rw-   0        0        0     7954 2024-04-04 19:32:18.000000 srt_trans-1.0.8/srt_trans/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-04 19:33:00.349548 srt_trans-1.0.8/srt_trans.egg-info/
--rw-rw-rw-   0        0        0     1873 2024-04-04 19:33:00.000000 srt_trans-1.0.8/srt_trans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-04-04 19:33:00.000000 srt_trans-1.0.8/srt_trans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 19:33:00.000000 srt_trans-1.0.8/srt_trans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-04 19:33:00.000000 srt_trans-1.0.8/srt_trans.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2024-04-04 19:33:00.000000 srt_trans-1.0.8/srt_trans.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 19:33:00.000000 srt_trans-1.0.8/srt_trans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-04 19:42:07.671046 srt_trans-1.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-04-04 00:36:54.000000 srt_trans-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1873 2024-04-04 19:42:07.669896 srt_trans-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2024-04-04 19:01:00.000000 srt_trans-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 19:42:07.672827 srt_trans-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2024-04-04 19:41:59.000000 srt_trans-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:42:07.630990 srt_trans-1.0.9/srt_trans/
+-rw-rw-rw-   0        0        0        0 2024-04-04 00:36:54.000000 srt_trans-1.0.9/srt_trans/__init__.py
+-rw-rw-rw-   0        0        0     7966 2024-04-04 19:39:49.000000 srt_trans-1.0.9/srt_trans/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-04 19:42:07.665917 srt_trans-1.0.9/srt_trans.egg-info/
+-rw-rw-rw-   0        0        0     1873 2024-04-04 19:42:07.000000 srt_trans-1.0.9/srt_trans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-04-04 19:42:07.000000 srt_trans-1.0.9/srt_trans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 19:42:07.000000 srt_trans-1.0.9/srt_trans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-04 19:42:07.000000 srt_trans-1.0.9/srt_trans.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-04-04 19:42:07.000000 srt_trans-1.0.9/srt_trans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-04 19:42:07.000000 srt_trans-1.0.9/srt_trans.egg-info/top_level.txt
```

### Comparing `srt_trans-1.0.8/LICENSE` & `srt_trans-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.8/PKG-INFO` & `srt_trans-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt_trans
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `srt_trans-1.0.8/README.md` & `srt_trans-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `srt_trans-1.0.8/setup.py` & `srt_trans-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='srt_trans',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             "srt_trans = srt_trans.cli:main"
         ],
     },
     install_requires=[
```

### Comparing `srt_trans-1.0.8/srt_trans/cli.py` & `srt_trans-1.0.9/srt_trans/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,15 @@
     source_language = "en"      # Source language code (e.g., "en" for English)
     target_language = "zh-CN"   # Target language code (e.g., "zh-CN" for Simple Chinese)
     
     if str(input_file).lower().endswith(".mkv"):
         track_number = 1
         video_file = ""
         if len(sys.argv) == 2:
-            video_file = input_file
-            input_file = video_file.replace(".mkv", ".srt")
+            pass
         elif len(sys.argv) == 4 and sys.argv[2] == "-track_number":
             track_number = sys.argv[3]
         elif len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
             source_language = sys.argv[3]
             target_language = sys.argv[5]
         elif len(sys.argv) == 8 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang" and sys.argv[6] == "-track_number":
             source_language = sys.argv[3]
@@ -155,14 +154,17 @@
             os.environ['https_proxy'] = proxy
         else:
             print("Invalid arguments!")
             return
         if not str(track_number).isdigit():
             print("Invalid track_number, it should be an int!")
             return
+
+        video_file = input_file
+        input_file = video_file.replace(".mkv", ".srt")
         extract_subtitles(video_file, input_file, int(track_number))
     else:
         if len(sys.argv) == 2:
             pass
         elif len(sys.argv) == 6 and sys.argv[2] == "-src_lang" and sys.argv[4] == "-dest_lang":
             source_language = sys.argv[3]
             target_language = sys.argv[5]
```

### Comparing `srt_trans-1.0.8/srt_trans.egg-info/PKG-INFO` & `srt_trans-1.0.9/srt_trans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srt-trans
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple translator for any SubRip(.srt) files.
 Home-page: https://github.com/bumblezhou/srt_trans
 Author: Jack
 Author-email: bumble.zhou@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

