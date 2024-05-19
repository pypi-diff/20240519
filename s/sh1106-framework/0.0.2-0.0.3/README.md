# Comparing `tmp/sh1106_framework-0.0.2.tar.gz` & `tmp/sh1106_framework-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh1106_framework-0.0.2.tar", last modified: Sat May 18 16:59:20 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sh1106_framework-0.0.2.tar` & `sh1106_framework-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-18 16:59:20.177315 sh1106_framework-0.0.2/
--rw-r--r--   0 dan        (501) staff       (20)    11357 2024-05-02 15:27:26.000000 sh1106_framework-0.0.2/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)     1047 2024-05-18 16:59:20.177117 sh1106_framework-0.0.2/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      217 2024-05-02 15:27:26.000000 sh1106_framework-0.0.2/README.md
--rw-r--r--   0 dan        (501) staff       (20)      870 2024-05-18 16:59:08.000000 sh1106_framework-0.0.2/pyproject.toml
--rw-r--r--   0 dan        (501) staff       (20)       38 2024-05-18 16:59:20.177354 sh1106_framework-0.0.2/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      596 2024-05-18 16:59:15.000000 sh1106_framework-0.0.2/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2024-05-18 16:59:20.176900 sh1106_framework-0.0.2/sh1106_framework.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)     1047 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      201 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2024-05-18 16:59:20.000000 sh1106_framework-0.0.2/sh1106_framework.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/sh1106_font_generator.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/sh1106_framework.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/sh1106_image_generator.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/firmware/main.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/framework/constants.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/framework/states/state.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/framework/states/state_manager.py
+-rw-r--r--   0        0        0    11500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/graphics/drawing.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/graphics/fonts.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/src/sh1106_framework/graphics/images.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/tests/ping-pong/ping-pong.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/tests/ping-pong/ping.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/tests/ping-pong/pong.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/useful-assets/default-font.json
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/useful-assets/default-font.png
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/useful-assets/example-images.json
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/useful-assets/example-images.png
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/LICENSE
+-rw-r--r--   0        0        0     7561 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 sh1106_framework-0.0.3/PKG-INFO
```

### Comparing `sh1106_framework-0.0.2/LICENSE` & `sh1106_framework-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sh1106_framework-0.0.2/pyproject.toml` & `sh1106_framework-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.hatch.build.targets.wheel]
+packages = ["src/sh1106_framework"]
+
 [project]
 name = "sh1106_framework"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Dan Convey", email="author@example.com" },
 ]
 license = { text = "Apache License 2.0" }
 description = "A state manager, graphics, image, and custom font drawing package for the SH1106 OLED screen based on the luma.oled package. It works with Raspberry Pi and other Linux-based single-board computers."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.10"  
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Other OS"
 ]
```

