# Comparing `tmp/dvr-scan-1.6.tar.gz` & `tmp/dvr_scan-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvr-scan-1.6.tar", last modified: Mon Oct 16 04:33:41 2023, max compression
+gzip compressed data, was "dvr_scan-1.6.1.tar", last modified: Sun May 19 03:58:57 2024, max compression
```

## Comparing `dvr-scan-1.6.tar` & `dvr_scan-1.6.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 04:33:41.414267 dvr-scan-1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-10-16 04:32:29.000000 dvr-scan-1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-10-16 04:33:41.414267 dvr-scan-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-10-16 04:32:29.000000 dvr-scan-1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 04:33:41.414267 dvr-scan-1.6/dist/
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-10-16 04:32:29.000000 dvr-scan-1.6/dist/package-info.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr-scan.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 04:33:41.414267 dvr-scan-1.6/dvr_scan/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 04:33:41.414267 dvr-scan-1.6/dvr_scan/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    24638 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22011 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/cli/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/opencv_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/overlays.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    31239 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/region.py
--rw-r--r--   0 runner    (1001) docker     (127)    47005 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/scanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/subtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-10-16 04:32:29.000000 dvr-scan-1.6/dvr_scan/video_joiner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 04:33:41.414267 dvr-scan-1.6/dvr_scan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-10-16 04:33:41.000000 dvr-scan-1.6/dvr_scan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-16 04:33:41.000000 dvr-scan-1.6/dvr_scan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 04:33:41.000000 dvr-scan-1.6/dvr_scan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-10-16 04:33:41.000000 dvr-scan-1.6/dvr_scan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-16 04:33:41.000000 dvr-scan-1.6/dvr_scan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-16 04:33:41.000000 dvr-scan-1.6/dvr_scan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-10-16 04:32:29.000000 dvr-scan-1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-10-16 04:33:41.414267 dvr-scan-1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:58:57.675465 dvr_scan-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-19 03:58:57.675465 dvr_scan-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:58:57.671465 dvr_scan-1.6.1/dist/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dist/package-info.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr-scan.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:58:57.671465 dvr_scan-1.6.1/dvr_scan/
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:58:57.671465 dvr_scan-1.6.1/dvr_scan/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    24740 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22043 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14130 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/cli/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/opencv_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/overlays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34629 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48649 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/subtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/dvr_scan/video_joiner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:58:57.675465 dvr_scan-1.6.1/dvr_scan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-19 03:58:57.000000 dvr_scan-1.6.1/dvr_scan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-19 03:58:57.000000 dvr_scan-1.6.1/dvr_scan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:58:57.000000 dvr_scan-1.6.1/dvr_scan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 03:58:57.000000 dvr_scan-1.6.1/dvr_scan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-19 03:58:57.000000 dvr_scan-1.6.1/dvr_scan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 03:58:57.000000 dvr_scan-1.6.1/dvr_scan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 03:58:16.000000 dvr_scan-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-19 03:58:57.675465 dvr_scan-1.6.1/setup.cfg
```

### Comparing `dvr-scan-1.6/LICENSE` & `dvr_scan-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvr-scan-1.6/PKG-INFO` & `dvr_scan-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvr-scan
-Version: 1.6
+Version: 1.6.1
 Summary: Tool for finding and extracting motion events in video files (e.g. security camera footage).
 Home-page: https://www.dvr-scan.com/
 Author: Brandon Castellano
 Author-email: brandon248@gmail.com
 License: BSD 2-Clause License
 Project-URL: Homepage, https://www.dvr-scan.com/
 Project-URL: Repository, https://github.com/Breakthrough/DVR-Scan
@@ -16,24 +16,24 @@
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Multimedia :: Video :: Non-Linear Editor
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: platformdirs
 Requires-Dist: numpy
 Requires-Dist: scenedetect
 Requires-Dist: screeninfo
 Requires-Dist: tqdm
```

### Comparing `dvr-scan-1.6/README.md` & `dvr_scan-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,13 +44,13 @@
 
 <img alt="example of bounding boxes" src="https://raw.githubusercontent.com/Breakthrough/DVR-Scan/releases/1.6/docs/assets/bounding-box.gif" width="480"/>
 
 Use `ffmpeg` to extract events:
 
     dvr-scan -i video.mp4 -m ffmpeg
 
-See [the documentation](docs.md) for a complete list of all command-line and configuration file options which can be set. You can also type `dvr-scan --help` for an overview of command line options. Some program options can also be set [using a config file](docs.md#config-file).
+See [the documentation](https://www.dvr-scan.com/docs) for a complete list of all command-line and configuration file options which can be set. You can also type `dvr-scan --help` for an overview of command line options. Some program options can also be set [using a config file](https://www.dvr-scan.com/docs/#config-file).
 
 ------------------------------------------------
 
 Copyright © 2016-2023 Brandon Castellano. All rights reserved.
 Licensed under BSD 2-Clause (see the LICENSE file for details).
```

### Comparing `dvr-scan-1.6/dist/package-info.rst` & `dvr_scan-1.6.1/dist/package-info.rst`

 * *Files identical despite different names*

### Comparing `dvr-scan-1.6/dvr-scan.cfg` & `dvr_scan-1.6.1/dvr-scan.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -83,21 +83,26 @@
 # while too low of a threshold can result in false detection events.
 #threshold = 0.15
 
 # Scores of this amount or higher are ignored. 255.0 is the maximum score, so
 # values greater than 255.0 will disable the filter.
 #max-threshold = 255.0
 
+# Value between 0.0 and 1.0 indicating how fast the background model is updated,
+# or set to -1 to set rate automatically based on history length. A value of 0.0
+# will not update the model at all, and 1.0 would re-initialize it on every frame.
+#learning-rate = -1
+
 # Size (in pixels) of the noise reduction kernel. Can be odd integer starting
 # from 3, 0 to disable, or -1 to auto-set using video resolution.
 #kernel-size = -1
 
-# Region file to limit detection area. Region files can be created using the
-# -r/--region-editor or -s/--save-region flags.
-#region-file = roi.txt
+# Region file to limit detection areas. Can be created with the -r / --region-editor
+# See < http://www.dvr-scan.com/guide/#region-editor > for an overview of the editor.
+#load-region = roi.txt
 
 # Integer factor to shrink video before processing. Values <= 1 have no effect.
 #downscale-factor = 0
 
 # Number of frames to skip between processing when looking for motion events.
 #frame-skip = 0
```

### Comparing `dvr-scan-1.6/dvr_scan/LICENSE` & `dvr_scan-1.6.1/dvr_scan/LICENSE`

 * *Files identical despite different names*

### Comparing `dvr-scan-1.6/dvr_scan/__init__.py` & `dvr_scan-1.6.1/dvr_scan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """``dvr_scan`` Module
 
 This is the main DVR-Scan module containing all application logic,
 motion detection implementation, and command line processing. The
@@ -39,15 +39,15 @@
 # Handle loading OpenCV. This **MUST** be first before any other DVR-Scan or third-party
 # packages are imported which might attempt to import the `cv2` module.
 import dvr_scan.opencv_loader as _
 
 from dvr_scan.platform import init_logger
 
 # Used for module/distribution identification.
-__version__ = '1.6'
+__version__ = '1.6.1'
 
 
 def get_license_info() -> str:
     """Get license/copyright information for the package or standalone executable."""
     try:
         # If we're running a frozen/standalone executable distribution, make sure we include
         # the license information for the third-party components we redistribute.
```

### Comparing `dvr-scan-1.6/dvr_scan/__main__.py` & `dvr_scan-1.6.1/dvr_scan/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """ ``dvr_scan.__main__`` Module
 
 Provides entry point for DVR-Scan's command-line interface (CLI).
 """
```

### Comparing `dvr-scan-1.6/dvr_scan/cli/__init__.py` & `dvr_scan-1.6.1/dvr_scan/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """ ``dvr_scan.cli`` Module
 
 This module provides the command-line business logic for the `dvr-scan` command. The entry point
 starts the program by calling :py:func:`dvr_scan.cli.controller.run_dvr_scan`.
@@ -431,30 +431,33 @@
         nargs='*',
         action=RegionAction,
         help=(
             "Limit motion detection to a region of the frame. The region is defined as a sequence "
             "of 3 or more points forming a closed shape inside the video. Coordinate 0 0 is top "
             "left of the frame, and WIDTH-1 HEIGHT-1 is bottom right. Can be specified multiple "
             "times to add more regions."))
+
+    # TODO: Consider merging the load/save region options into a single --region-file option.
+
     parser.add_argument(
         "-R",
         "--load-region",
-        metavar="FILE.txt",
+        metavar="REGIONS.txt",
         type=str,
         help=("Load region data from file. Each line must be a list of points in the format "
               "specified by -a/--add-region. Each line is treated as a separate polygon."),
     )
 
     parser.add_argument(
         "-s",
         "--save-region",
-        metavar="FILE.txt",
+        metavar="REGIONS.txt",
         type=str,
-        help=("Save detection regions to FILE.txt before processing. If FILE.txt exists it will be "
-              "overwritten. Allows loading same regions using -R/--load-region."))
+        help=("Save regions before processing. If REGIONS.txt exists it will be overwritten. "
+              "The region editor will save regions here instead of asking for a path."))
 
     parser.add_argument(
         '-b',
         '--bg-subtractor',
         metavar='type',
         type=string_type_check(['MOG2', 'CNT', 'MOG2_CUDA'], False, 'type'),
         help=('The type of background subtractor to use, must be one of: '
```

### Comparing `dvr-scan-1.6/dvr_scan/cli/config.py` & `dvr_scan-1.6.1/dvr_scan/cli/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #         PySceneDetect: Python-Based Video Scene Detector
 #   ---------------------------------------------------------------
 #     [  Site:   http://www.scenedetect.scenedetect.com/         ]
 #     [  Docs:   http://manual.scenedetect.scenedetect.com/      ]
 #     [  Github: https://github.com/Breakthrough/PySceneDetect/  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # PySceneDetect is licensed under the BSD 3-Clause License; see the
 # included LICENSE file, or visit one of the above pages for details.
 #
 """``dvr_scan.cli.config`` Module
 
 Handles loading configuration files from disk and validating each setting. Only validation
 of the config file schema and data types are performed. The constants and default values
@@ -318,14 +318,15 @@
 
                                                          # Detection Parameters
     'bg-subtractor': 'MOG2',
     'threshold': 0.15,
     'max-threshold': 255.0,
     'kernel-size': KernelSizeValue(),
     'downscale-factor': 0,
+    'learning-rate': float(-1),
                                                          # TODO(v1.7): Remove, replaced with region files.
     'region-of-interest': RegionValueDeprecated(),
     'load-region': '',
     'frame-skip': 0,
 
                                                          # Overlays
```

### Comparing `dvr-scan-1.6/dvr_scan/cli/controller.py` & `dvr_scan-1.6.1/dvr_scan/cli/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """ ``dvr_scan.cli.controller`` Module
 
 This module manages the DVR-Scan program control flow, starting with `run_dvr_scan()`.
 """
@@ -270,53 +270,46 @@
 
     scanner.set_detection_params(
         detector_type=DetectorType[settings.get('bg-subtractor').upper()],
         threshold=settings.get('threshold'),
         max_threshold=settings.get('max-threshold'),
         kernel_size=settings.get('kernel-size'),
         downscale_factor=settings.get('downscale-factor'),
+        learning_rate=settings.get('learning-rate'),
     )
 
     scanner.set_event_params(
         min_event_len=settings.get('min-event-length'),
         time_pre_event=settings.get('time-before-event'),
         time_post_event=settings.get('time-post-event'),
     )
 
     scanner.set_video_time(
         start_time=settings.get_arg('start-time'),
         end_time=settings.get_arg('end-time'),
         duration=settings.get_arg('duration'),
     )
 
-    # If the user specified some regions on the command line, ignore the load-regions setting in the
-    # config file.
-    load_region = settings.get_arg('load-region')
-    if load_region is None:
-        load_region = settings.config.get_value('load-region', ignore_default=True)
-        if not settings.get_arg('regions') is None:
-            load_region = None
-
     scanner.set_regions(
-        region_editor=settings.get_arg('region-editor'),
+        region_editor=settings.get('region-editor'),
         regions=settings.get_arg('regions'),
-        load_region=load_region,
+        load_region=settings.get('load-region'),
         save_region=settings.get_arg('save-region'),
         roi_deprecated=settings.get('region-of-interest'),
     )
 
     # Scan video for motion with specified parameters.
     processing_start = time.time()
     result = scanner.scan()
     if result is None:
         logging.debug("Exiting early, scan() returned None.")
         return
     processing_time = time.time() - processing_start
-    # Display results and performance.
 
+    # Display results and performance.
     processing_rate = float(result.num_frames) / processing_time
     logger.info("Processed %d frames read in %3.1f secs (avg %3.1f FPS).", result.num_frames,
                 processing_time, processing_rate)
     if not result.event_list:
         logger.info("No motion events detected in input.")
         return
     logger.info("Detected %d motion events in input.", len(result.event_list))
```

### Comparing `dvr-scan-1.6/dvr_scan/detector.py` & `dvr_scan-1.6.1/dvr_scan/detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """ ``dvr_scan.detector`` Module
 
 Contains the motion detection algorithm (`MotionDetector`) for DVR-Scan.  It calculates a score that
 represents the relative amount of movement of consecutive frames in a video.
```

### Comparing `dvr-scan-1.6/dvr_scan/opencv_loader.py` & `dvr_scan-1.6.1/dvr_scan/opencv_loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """``dvr_scan.opencv_loader`` Module
 
 Ensures required DLL files can be loaded by Python when importing OpenCV, and provides
 better error messaging in cases where the module isn't installed.
 """
 
 import os
 import sys
 
 # On Windows, make sure we include any required DLL paths.
 if os.name == 'nt':
-    # If we're running a frozen version of the app, the EXE path should include all required DLLs.
-    # TODO(v1.6): This path might need to be updated with the latest version of Pyinstaller.
-    if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
-        os.add_dll_directory(os.path.abspath(os.path.dirname(sys.executable)))
     # If CUDA is installed, include those DLLs in the search paths.
-    if 'CUDA_PATH' in os.environ and os.path.exists(os.environ['CUDA_PATH']):
-        os.add_dll_directory(os.path.abspath(os.path.join(os.environ['CUDA_PATH'], 'bin')))
+    CUDA_PATH = os.environ['CUDA_PATH'] if 'CUDA_PATH' in os.environ else None
+    if CUDA_PATH and os.path.exists(CUDA_PATH):
+        CUDA_BIN_PATH = os.path.abspath(os.path.join(CUDA_PATH, 'bin'))
+        os.add_dll_directory(CUDA_BIN_PATH)
 
 # OpenCV is a required package, but we don't have it as an explicit dependency since we
 # need to support both opencv-python and opencv-python-headless. Include some additional
 # context with the exception if this is the case.
 try:
     import cv2 as _
 except ModuleNotFoundError as ex:
```

### Comparing `dvr-scan-1.6/dvr_scan/overlays.py` & `dvr_scan-1.6.1/dvr_scan/overlays.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """ ``dvr_scan.overlays`` Module
 
 This module contains various classes used to draw overlays onto video frames.
 """
```

### Comparing `dvr-scan-1.6/dvr_scan/platform.py` & `dvr_scan-1.6.1/dvr_scan/platform.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """``dvr_scan.platform`` Module
 
 Provides logging and platform/operating system compatibility.
 """
```

### Comparing `dvr-scan-1.6/dvr_scan/region.py` & `dvr_scan-1.6.1/dvr_scan/region.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """DVR-Scan Region Editor handles detection region input and processing.
 
 Regions are represented as a set of closed polygons defined by lists of points.
 """
@@ -26,22 +26,27 @@
 import numpy as np
 
 from dvr_scan.platform import HAS_TKINTER, IS_WINDOWS, temp_tk_window, set_icon
 
 if HAS_TKINTER:
     import tkinter
     import tkinter.filedialog
+    import tkinter.messagebox
 
-# TODO(v1.6): Update screenshots to reflect release title.
-_WINDOW_NAME = "DVR-Scan Region Editor"
-"""Title given to the ROI selection window."""
+# TODO: Update screenshots to reflect release title.
+WINDOW_TITLE = "DVR-Scan Region Editor"
+PROMPT_TITLE = "DVR-Scan"
+PROMPT_MESSAGE = "You have unsaved changes.\nDo you want to save?"
+SAVE_TITLE = "Save Region File"
+LOAD_TITLE = "Load Region File"
 
 KEYCODE_ESCAPE = ord('\x1b')
 KEYCODE_RETURN = ord('\r')
 KEYCODE_SPACE = ord(' ')
+# Control + Z/Y for undo/redo only seem to work on Windows.
 KEYCODE_WINDOWS_UNDO = 26
 KEYCODE_WINDOWS_REDO = 25
 
 DEFAULT_WINDOW_MODE = (cv2.WINDOW_AUTOSIZE if IS_WINDOWS else cv2.WINDOW_KEEPRATIO)
 """Minimum height/width for a ROI created using the mouse."""
 
 MIN_SIZE = 16
@@ -55,19 +60,19 @@
 
 @dataclass
 class Snapshot:
     regions: ty.List[ty.List[Point]]
     active_shape: ty.Optional[int]
 
 
-def check_tkinter_support(warn_if_notkinter: bool):
-    if warn_if_notkinter and not HAS_TKINTER:
+def warn_if_tkinter_missing():
+    if not HAS_TKINTER:
         logger.warning(
-            "Warning: Tkinter is not installed. To save the region to disk, use "
-            "-s/--save-region [FILE], or install python3-tk (e.g. `sudo apt install python3-tk`).")
+            "Warning: Tkinter is not installed. Install the python3-tk package to ensure region "
+            "data is saved, or specify -s/--save-region.")
 
 
 class RegionValidator:
     """Validator for a set of points representing a closed polygon."""
 
     _IGNORE_CHARS = [',', '/', '(', ')', '[', ']']
     """Characters to ignore."""
@@ -94,27 +99,31 @@
 
     def __str__(self) -> str:
         return ", ".join(f'P({x},{y})' for x, y in self._value)
 
 
 # TODO(v1.7): Allow controlling some of these settings in the config file.
 @dataclass
-class SelectionWindowSettings:
+class EditorSettings:
+    video_path: str
+    """The first input video path specified by -i/--input."""
+    save_path: ty.Optional[str] = False
+    """The path specified by the -s/--save-regions option if set."""
     use_aa: bool = True
     mask_source: bool = False
     window_mode: int = DEFAULT_WINDOW_MODE
     line_color: ty.Tuple[int, int, int] = (255, 0, 0)
     line_color_alt: ty.Tuple[int, int, int] = (255, 153, 51)
     hover_color: ty.Tuple[int, int, int] = (0, 127, 255)
     hover_color_alt: ty.Tuple[int, int, int] = (0, 0, 255)
     interact_color: ty.Tuple[int, int, int] = (0, 255, 255)
     highlight_insert: bool = False
 
 
-# TODO(v1.7): Move more of these to SelectionWindowSettings.
+# TODO(v1.7): Move more of these constants to EditorSettings.
 MIN_NUM_POINTS = 3
 MAX_HISTORY_SIZE = 1024
 MIN_DOWNSCALE_FACTOR = 1
 MAX_DOWNSCALE_FACTOR = 50
 MAX_UPDATE_RATE_NORMAL = 20
 MAX_UPDATE_RATE_DRAGGING = 5
 HOVER_DISPLAY_DISTANCE = 260**2
@@ -175,36 +184,36 @@
     # Right click is disabled on Linux/OSX due to a context manager provided by the UI framework
     # showing up when right clicking.
     _WINDOWS_ONLY = 'Right, ' if IS_WINDOWS else ''
 
     logger.info(f"""ROI Window Controls:
 
 Editor:
-  Mask On/Off         Key: {str(KEYBIND_MASK).upper()}
+  Mask On/Off         Key: {KEYBIND_MASK.upper()}
   Start Scan          Key: Space, Enter
   Quit                Key: Escape
-  Save                Key: {str(KEYBIND_SAVE).upper()}
-  Load                Key: {str(KEYBIND_LOAD).upper()}
-  Undo                Key: {str(KEYBIND_UNDO).upper()}
-  Redo                Key: {str(KEYBIND_REDO).upper()}
-  Print Points        Key: {str(KEYBIND_OUTPUT_LIST).upper()}
+  Save                Key: {KEYBIND_SAVE.upper()}
+  Load                Key: {KEYBIND_LOAD.upper()}
+  Undo                Key: {"CTRL + " if IS_WINDOWS else ""}{KEYBIND_UNDO.upper()}
+  Redo                Key: {"CTRL + " if IS_WINDOWS else ""}{KEYBIND_REDO.upper()}
+  Print Points        Key: {KEYBIND_OUTPUT_LIST.upper()}
 
 Regions:
-  Add Point           Key: {str(KEYBIND_POINT_ADD).upper()},  Mouse: Left
-  Delete Point        Key: {str(KEYBIND_POINT_DELETE).upper()},  Mouse: {_WINDOWS_ONLY}Middle
-  Add Region          Key: Shift + {str(KEYBIND_REGION_ADD).upper()}
-  Delete Region       Key: Shift + {str(KEYBIND_REGION_DELETE).upper()}
+  Add Point           Key: {KEYBIND_POINT_ADD.upper()},  Mouse: Left
+  Delete Point        Key: {KEYBIND_POINT_DELETE.upper()},  Mouse: {_WINDOWS_ONLY}Middle
+  Add Region          Key: {KEYBIND_REGION_ADD.upper()}
+  Delete Region       Key: {KEYBIND_REGION_DELETE.upper()}
   Select Region       Key: 1 - 9
-  Next Region         Key: {str(KEYBIND_REGION_NEXT).upper()}
-  Previous Region     Key: {str(KEYBIND_REGION_PREVIOUS).upper()}
+  Next Region         Key: {KEYBIND_REGION_NEXT.upper()}
+  Previous Region     Key: {KEYBIND_REGION_PREVIOUS.upper()}
 
 Display:
-  Downscale +/-       Key: {str(KEYBIND_DOWNSCALE_INC).upper()}(+), {str(KEYBIND_DOWNSCALE_DEC).upper()} (-)
-  Antialiasing        Key: {str(KEYBIND_TOGGLE_AA).upper()}
-  Window Mode         Key: {str(KEYBIND_WINDOW_MODE).upper()}
+  Downscale +/-       Key: {KEYBIND_DOWNSCALE_INC.upper()}(+), {KEYBIND_DOWNSCALE_DEC.upper()} (-)
+  Antialiasing        Key: {KEYBIND_TOGGLE_AA.upper()}
+  Window Mode         Key: {KEYBIND_WINDOW_MODE.upper()}
 """)
 
 
 def initial_point_list(frame_size: Size) -> ty.List[Point]:
     # For now start with a rectangle covering 1/4 of the frame in the middle.
     top_left = Point(x=frame_size.w // 4, y=frame_size.h // 4)
     box_size = Size(w=frame_size.w // 2, h=frame_size.h // 2)
@@ -233,18 +242,28 @@
             RegionValidator(region).value
             for region in filter(None, (region.strip() for region in region_data)))
     return []
 
 
 # TODO(v1.7): Allow multiple polygons by adding new ones using keyboard.
 # TODO(v1.7): Allow shifting polygons by using middle mouse button.
-class SelectionWindow:
+class RegionEditor:
+
+    def __init__(
+        self,
+        frame: np.ndarray,
+        initial_shapes: ty.Optional[ty.List[ty.List[Point]]],
+        initial_scale: ty.Optional[int],
+        debug_mode: bool,
+        video_path: str,
+        save_path: ty.Optional[str],
+    ):
+        # TODO: Move more fields from this class into `EditorSettings`.
+        self._settings = EditorSettings(video_path=video_path, save_path=save_path)
 
-    def __init__(self, frame: np.ndarray, initial_shapes: ty.Optional[ty.List[ty.List[Point]]],
-                 initial_scale: ty.Optional[int], debug_mode: bool):
         self._source_frame = frame.copy()   # Frame before downscaling
         self._source_size = Size(w=frame.shape[1], h=frame.shape[0])
         self._scale: int = 1 if initial_scale is None else initial_scale
         self._frame = frame.copy()          # Workspace
         self._frame_size = Size(w=frame.shape[1], h=frame.shape[0])
         self._original_frame = frame.copy() # Copy to redraw on
         if initial_shapes:
@@ -262,16 +281,16 @@
         self._dragging = False
         self._drag_start = None
         self._debug_mode = debug_mode
         self._segment_dist = []             # Square distance of segment from point i to i+1
         self._mouse_dist = []               # Square distance of mouse to point i
         if self._scale > 1:
             self._rescale()
-        self._settings = SelectionWindowSettings()
-        self._commit()
+        self._persisted = True              # Indicates if we've saved outstanding changes to disk.
+        self._commit(persisted=True)        # Add initial history for undo.
 
     @property
     def shapes(self) -> ty.Iterable[ty.Iterable[Point]]:
         return self._regions
 
     @property
     def active_region(self) -> ty.Optional[ty.List[Point]]:
@@ -303,28 +322,35 @@
             snapshot = deepcopy(self._history[self._history_pos])
             self._regions = snapshot.regions
             self._active_shape = snapshot.active_shape
             self._recalculate = True
             self._redraw = True
             logger.debug("Redo: [%d/%d]", self._history_pos, len(self._history) - 1)
 
-    def _commit(self):
+    def _commit(self, persisted=False):
+        # TODO: Make it so if we edit a snapshot, that adds a new entry in the buffer, instead of
+        # rewriting history from that point.
+        # Take a copy of the current state and put it in the history buffer.
         snapshot = deepcopy(Snapshot(regions=self._regions, active_shape=self._active_shape))
         self._history = self._history[self._history_pos:]
         self._history.insert(0, snapshot)
         self._history = self._history[:MAX_HISTORY_SIZE]
         self._history_pos = 0
+        # Update state.
         self._recalculate = True
         self._redraw = True
+        self._persisted = persisted
 
     def _emit_points(self):
         region_info = []
         for shape in self._regions:
-            region_info.append("--region %s" % " ".join(f"{x} {y}" for x, y in shape))
-        logger.info("Region data for CLI:\n%s", " ".join(region_info))
+            region_info.append("-a %s" % " ".join(f"{x} {y}" for x, y in shape))
+        data = " ".join(region_info)
+        logger.info("Command to scan region:\n"
+                    f"dvr-scan -i {self._settings.video_path} {data}")
 
     def _draw(self):
         if self._recalculate:
             self._recalculate_data()
         if not self._redraw:
             return
 
@@ -406,15 +432,15 @@
                     frame,
                     start,
                     end,
                     color,
                     thickness=cv2.FILLED,
                 )
         self._frame = frame
-        cv2.imshow(_WINDOW_NAME, self._frame)
+        cv2.imshow(WINDOW_TITLE, self._frame)
         self._redraw = False
 
     def _find_nearest(self) -> ty.Tuple[int, int]:
         nearest_seg, nearest_dist, largest_cosine = 0, 2**31, math.pi
         for i in range(len(self.active_region)):
             # Create a triangle where side a's length is the mouse to closest point on the line,
             # side c is the length to the furthest point, and side b is the line segment length.
@@ -446,115 +472,167 @@
                 min_i = i
         # If we've shrunk the image, we need to compensate for the size difference in the image.
         # The control handles remain the same size but the image is smaller
         return min_i if self._mouse_dist[min_i] <= (4 * control_handle_radius(self._scale) *
                                                     self._scale)**2 else None
 
     def _init_window(self):
-        cv2.namedWindow(_WINDOW_NAME, self._settings.window_mode)
+        cv2.namedWindow(WINDOW_TITLE, self._settings.window_mode)
         if self._settings.window_mode == cv2.WINDOW_AUTOSIZE:
-            cv2.resizeWindow(_WINDOW_NAME, width=self._frame_size.w, height=self._frame_size.h)
-        cv2.imshow(_WINDOW_NAME, mat=self._frame)
-        cv2.setMouseCallback(_WINDOW_NAME, on_mouse=self._handle_mouse_input)
+            cv2.resizeWindow(WINDOW_TITLE, width=self._frame_size.w, height=self._frame_size.h)
+        cv2.imshow(WINDOW_TITLE, mat=self._frame)
+        cv2.setMouseCallback(WINDOW_TITLE, on_mouse=self._handle_mouse_input)
+        set_icon(WINDOW_TITLE)
 
     def _breakpoint(self):
         if self._debug_mode:
             breakpoint()
 
     def _create_keymap(self) -> ty.Dict[int, ty.Callable]:
         return {
             KEYBIND_BREAKPOINT: lambda: self._breakpoint,
             KEYBIND_DOWNSCALE_INC: lambda: self._adjust_downscale(1),
             KEYBIND_DOWNSCALE_DEC: lambda: self._adjust_downscale(-1),
             KEYBIND_HELP: lambda: show_controls(),
-            KEYBIND_LOAD: lambda: self._load(),
+            KEYBIND_LOAD: lambda: self._prompt_load(),
             KEYBIND_MASK: lambda: self._toggle_mask(),
             KEYBIND_OUTPUT_LIST: lambda: self._emit_points(),
             KEYBIND_POINT_ADD: lambda: self._add_point(),
             KEYBIND_POINT_DELETE: lambda: self._delete_point(),
             KEYBIND_REGION_ADD: lambda: self._add_region(),
             KEYBIND_REGION_DELETE: lambda: self._delete_region(),
             KEYBIND_REGION_NEXT: lambda: self._next_region(),
             KEYBIND_REGION_PREVIOUS: lambda: self._prev_region(),
-            KEYBIND_REDO: lambda: self._redo(),
             KEYBIND_TOGGLE_AA: lambda: self._toggle_antialiasing(),
-            KEYBIND_SAVE: lambda: self._save(),
-            KEYBIND_UNDO: lambda: self._undo(),
+            KEYBIND_SAVE: lambda: self._prompt_save(),
             KEYBIND_WINDOW_MODE: lambda: self._toggle_window_mode(),
-            chr(KEYCODE_WINDOWS_REDO): lambda: self._redo(),
-            chr(KEYCODE_WINDOWS_UNDO): lambda: self._undo(),
+            chr(KEYCODE_WINDOWS_REDO) if IS_WINDOWS else KEYBIND_REDO: lambda: self._redo(),
+            chr(KEYCODE_WINDOWS_UNDO) if IS_WINDOWS else KEYBIND_UNDO: lambda: self._undo(),
         }
 
-    def run(self, warn_if_notkinter: bool) -> bool:
+    def run(self) -> bool:
+        """Run the region editor. Returns True if the video should be scanned, False otherwise."""
         try:
+            if not self._settings.save_path:
+                # Warn the user if changes to region data won't be saved if a path wasn't specified,
+                # and a file dialog box cannot be shown to choose a path.
+                warn_if_tkinter_missing()
             logger.debug("Creating window for frame (scale = %d)", self._scale)
             self._init_window()
-            check_tkinter_support(warn_if_notkinter)
-            set_icon(_WINDOW_NAME)
-            regions_valid = False
-            logger.info(f"Region editor active. Press {KEYBIND_HELP} to show controls.")
+            should_scan = False
+            logger.info(f"Region editor active. Press {KEYBIND_HELP.upper()} to show controls.")
             keyboard_callbacks = self._create_keymap()
             while True:
-                if not cv2.getWindowProperty(_WINDOW_NAME, cv2.WND_PROP_VISIBLE):
+                if not cv2.getWindowProperty(WINDOW_TITLE, cv2.WND_PROP_VISIBLE):
                     logger.debug("Main window closed.")
-                    break
+                    if self._prompt_save_on_quit():
+                        break
+                    logger.debug("Re-initializing window.")
+                    self._init_window()
+                    continue
                 self._draw()
                 key = cv2.waitKey(MAX_UPDATE_RATE_NORMAL
                                   if not self._dragging else MAX_UPDATE_RATE_DRAGGING) & 0xFF
                 if key == KEYCODE_ESCAPE:
-                    break
+                    if self._prompt_save_on_quit():
+                        break
                 elif key in (KEYCODE_SPACE, KEYCODE_RETURN):
-                    regions_valid = True
-                    break
+                    if self._prompt_save_on_quit():
+                        should_scan = True
+                        break
                 elif key >= ord('0') and key <= ord('9'):
                     self._select_region((key - ord('1')) % 10)
                 elif chr(key) in keyboard_callbacks:
                     keyboard_callbacks[chr(key)]()
                 elif key != 0xFF and self._debug_mode:
                     logger.debug("Unhandled key: %s", str(key))
-            return regions_valid
+            return should_scan
 
         finally:
             cv2.destroyAllWindows()
 
     def _adjust_downscale(self, amount: int):
         # scale is clamped to MIN_DOWNSCALE_FACTOR/MAX_DOWNSCALE_FACTOR.
         scale = self._scale + amount
         self._scale = (
             MIN_DOWNSCALE_FACTOR if scale < MIN_DOWNSCALE_FACTOR else
             scale if scale < MAX_DOWNSCALE_FACTOR else MAX_DOWNSCALE_FACTOR)
+        logger.info(f"Downscale factor: {self._scale}")
         self._rescale()
 
-    def _save(self):
+    def _prompt_save(self):
+        """Save region data, prompting the user if a save path wasn't specified by command line."""
+        if self._save():
+            return
         if not HAS_TKINTER:
             logger.debug("Cannot show file dialog.")
             return
         save_path = None
         with temp_tk_window() as _:
             save_path = tkinter.filedialog.asksaveasfilename(
-                title="DVR-Scan: Save Region",
+                title=SAVE_TITLE,
                 filetypes=[("Region File", "*.txt")],
                 defaultextension=".txt",
                 confirmoverwrite=True,
             )
         if save_path:
-            with open(save_path, "wt") as region_file:
-                for shape in self._regions:
-                    region_file.write(" ".join(f"{x} {y}" for x, y in shape))
-                    region_file.write("\n")
-            logger.info('Saved region to: %s', save_path)
+            self._save(save_path)
+
+    def _prompt_save_on_quit(self):
+        """Saves any changes that weren't persisted, prompting the user if a path wasn't specified.
+        Returns True if we should quit the program, False if we should not quit."""
+        if not HAS_TKINTER:
+            logger.debug("Cannot show dialog.")
+            self._save()
+            return True
+        # Don't prompt user if changes are already saved.
+        if self._persisted:
+            return True
+        with temp_tk_window() as _:
+            should_save = tkinter.messagebox.askyesnocancel(
+                title=PROMPT_TITLE, message=PROMPT_MESSAGE, icon=tkinter.messagebox.WARNING)
+            if should_save is None:
+                return False
+            if should_save and not self._save():
+                save_path = None
+                with temp_tk_window() as _:
+                    save_path = tkinter.filedialog.asksaveasfilename(
+                        title=SAVE_TITLE,
+                        filetypes=[("Region File", "*.txt")],
+                        defaultextension=".txt",
+                        confirmoverwrite=True,
+                    )
+                if not save_path:
+                    return False
+                self._save(save_path)
+            else:
+                logger.debug("Quitting with unsaved changes.")
+        return True
+
+    def _save(self, path=None):
+        if path is None:
+            if not self._settings.save_path:
+                return False
+            path = self._settings.save_path
+        with open(path, "wt") as region_file:
+            for shape in self._regions:
+                region_file.write(" ".join(f"{x} {y}" for x, y in shape))
+                region_file.write("\n")
+        logger.info('Saved region data to: %s', path)
+        self._persisted = True
+        return True
 
-    def _load(self):
+    def _prompt_load(self):
         if not HAS_TKINTER:
             logger.debug("Cannot show file dialog.")
             return
         load_path = None
         with temp_tk_window() as _:
             load_path = tkinter.filedialog.askopenfilename(
-                title="DVR-Scan: Load Region",
+                title=LOAD_TITLE,
                 filetypes=[("Region File", "*.txt")],
                 defaultextension=".txt",
             )
         if not load_path:
             return
         if not os.path.exists(load_path):
             logger.error(f"File does not exist: {load_path}")
@@ -573,14 +651,15 @@
                          's' if len(regions) > 1 else '',
                          "\n".join(f"[{i}] = {points}" for i, points in enumerate(regions)))
 
             self._regions = [
                 [bound_point(point, self._source_size) for point in shape] for shape in regions
             ]
             self._commit()
+            self._persisted = True
             self._active_shape = 0 if len(self._regions) > 0 else None
 
     def _delete_point(self):
         if not self._hover_point is None and not self._dragging:
             if len(self.active_region) > MIN_NUM_POINTS:
                 hover = self._hover_point
                 x, y = self.active_region[hover]
@@ -601,15 +680,15 @@
 
     def _toggle_mask(self):
         self._settings.mask_source = not self._settings.mask_source
         logger.debug("Masking: %s", "ON" if self._settings.mask_source else "OFF")
         self._redraw = True
 
     def _toggle_window_mode(self):
-        cv2.destroyWindow(_WINDOW_NAME)
+        cv2.destroyWindow(WINDOW_TITLE)
         if self._settings.window_mode == cv2.WINDOW_KEEPRATIO:
             self._settings.window_mode = cv2.WINDOW_AUTOSIZE
         else:
             self._settings.window_mode = cv2.WINDOW_KEEPRATIO
         logger.debug(
             "Window Mode: %s",
             "KEEPRATIO" if self._settings.window_mode == cv2.WINDOW_KEEPRATIO else "AUTOSIZE")
@@ -662,15 +741,16 @@
         # TODO: Map mouse events to callbacks rather than handling each event conditionally.
         drag_started = False
         bounded = bound_point(point=Point(x, y), size=self._frame_size)
         self._curr_mouse_pos = Point(bounded.x * self._scale, bounded.y * self._scale)
 
         if event == cv2.EVENT_LBUTTONDOWN:
             if not self._regions:
-                logger.info(f"No regions to edit, add a new one by pressing {KEYBIND_REGION_ADD}.")
+                logger.info(
+                    f"No regions to edit, add a new one by pressing {KEYBIND_REGION_ADD.upper()}.")
             if not self._hover_point is None:
                 self._dragging = True
                 self._drag_start = self._curr_mouse_pos
                 self._redraw = True
                 drag_started = True
             else:
                 drag_started = self._add_point()
```

### Comparing `dvr-scan-1.6/dvr_scan/scanner.py` & `dvr_scan-1.6.1/dvr_scan/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """``dvr_scan.scanner`` Module
 
 Contains the motion scanning engine (`MotionScanner`) for DVR-Scan.
 """
@@ -30,15 +30,15 @@
 from scenedetect import FrameTimecode
 from scenedetect.platform import FakeTqdmObject
 from tqdm import tqdm
 
 from dvr_scan.detector import MotionDetector
 from dvr_scan.overlays import BoundingBoxOverlay, TextOverlay
 from dvr_scan.platform import get_filename, get_min_screen_bounds, is_ffmpeg_available
-from dvr_scan.region import SelectionWindow, Point, Size, bound_point, load_regions
+from dvr_scan.region import RegionEditor, Point, Size, bound_point, load_regions
 from dvr_scan.subtractor import SubtractorMOG2, SubtractorCNT, SubtractorCudaMOG2
 from dvr_scan.video_joiner import VideoJoiner
 
 logger = logging.getLogger('dvr_scan')
 
 DEFAULT_VIDEOWRITER_CODEC = 'XVID'
 """Default codec to use with OpenCV VideoWriter."""
@@ -84,22 +84,22 @@
     FFMPEG = 4
     """Output using ffmpeg."""
 
 
 @dataclass
 class DecodeEvent:
     """Event generated by decode thread on each video frame."""
-    frame_rgb: np.ndarray
+    frame_bgr: np.ndarray
     timecode: FrameTimecode
 
 
 @dataclass
 class EncodeFrameEvent:
     """Event generated by main thread for each frame in a motion event."""
-    frame_rgb: np.ndarray
+    frame_bgr: np.ndarray
     timecode: FrameTimecode
     score: float
     bounding_box: Tuple[int, int, int, int]
     end_of_event: bool = False
 
 
 @dataclass
@@ -219,27 +219,29 @@
         # Output Parameters (set_output)
         self._comp_file: Optional[AnyStr] = None       # -o/--output
         self._mask_file: Optional[AnyStr] = None       # -mo/--mask-output
         self._fourcc: Any = None                       # opencv-codec
         self._output_mode: OutputMode = None           # -m/--output-mode / -so/--scan-only
         self._ffmpeg_input_args: Optional[str] = None  # input args for OutputMode.FFMPEG/COPY
         self._ffmpeg_output_args: Optional[str] = None # output args for OutputMode.FFMPEG
-                                                       # TODO: Replace uses of self._output_dir with a helper function called "get_output_path".
         self._output_dir: AnyStr = ''                  # -d/--directory
+                                                       # TODO: Replace uses of self._output_dir with
+                                                       # a helper function called "get_output_path".
 
         # Overlay Parameters (set_overlays)
         self._timecode_overlay = None # -tc/--time-code, None or TextOverlay
         self._metrics_overlay = None  # -fm/--frame-metrics, None or TextOverlay
         self._bounding_box = None     # -bb/--bounding-box, None or BoundingBoxOverlay
 
         # Motion Detection Parameters (set_detection_params)
         self._subtractor_type = DetectorType.MOG2 # -b/--bg-subtractor
         self._threshold = 0.15                    # -t/--threshold
         self._kernel_size = None                  # -k/--kernel-size
         self._downscale_factor = 1                # -df/--downscale-factor
+        self._learningRate = -1                   # learning-rate
         self._max_threshold = 255.0               # max-threshold
 
         # Motion Event Parameters (set_event_params)
         self._min_event_len = None  # -l/--min-event-length
         self._pre_event_len = None  # -tb/--time-before-event
         self._post_event_len = None # -tp/--time-post-event
 
@@ -259,14 +261,15 @@
         self._end_time: FrameTimecode = None                 # -et/--end-time
 
         # Internal Variables
         self._stop: threading.Event = threading.Event()
         self._decode_thread_exception = None
         self._encode_thread_exception = None
         self._video_writer: Optional[cv2.VideoWriter] = None
+        self._mask_size: Tuple[int, int] = None
         self._mask_writer: Optional[cv2.VideoWriter] = None
         self._num_events: int = 0
 
         # Make sure we initialize defaults now that we loaded the input videos.
         self.set_detection_params()
         self.set_event_params()
         self.set_video_time()
@@ -361,24 +364,33 @@
     def set_detection_params(
         self,
         detector_type: DetectorType = DetectorType.MOG2,
         threshold: float = 0.15,
         max_threshold: float = 255.0,
         kernel_size: int = -1,
         downscale_factor: int = 1,
+        learning_rate: float = -1,
     ):
         """Set detection parameters."""
         self._threshold = threshold
         self._max_threshold = max_threshold
         self._subtractor_type = detector_type
         if downscale_factor < 0:
             raise ValueError("Downscale factor must be positive.")
         self._downscale_factor = max(downscale_factor, 1)
         assert kernel_size == -1 or kernel_size == 0 or kernel_size >= 3
         self._kernel_size = kernel_size
+        # TODO: Also allow ability to customize history size, as this is another factor that
+        # influences how quickly the background model is updated. When calculated automatically,
+        # OpenCV sets learning rate as:
+        #
+        #     learning_rate = 1.0 / min(num_frames, history_length)
+        #
+        # We should also investigate how this works for CNT and other subtractors.
+        self._learning_rate = learning_rate
 
     def set_regions(self,
                     region_editor: bool = False,
                     regions: Optional[List[List[Point]]] = None,
                     load_region: Optional[str] = None,
                     save_region: Optional[str] = None,
                     roi_deprecated: Optional[List[int]] = None):
@@ -478,44 +490,44 @@
                 frame_w, frame_h = frame_for_crop.shape[1], frame_for_crop.shape[0]
                 if (max_h > 0 and frame_h > max_h) or (max_w > 0 and frame_w > max_w):
                     logger.debug('Max window size: %d x %d', max_w, max_h)
                     # Downscale the image if it's too large for the screen.
                     factor_h = frame_h / float(max_h) if max_h > 0 and frame_h > max_h else 1
                     factor_w = frame_w / float(max_w) if max_w > 0 and frame_w > max_w else 1
                     scale_factor = round(max(factor_h, factor_w))
-            regions = SelectionWindow(
+            regions = RegionEditor(
                 frame=frame_for_crop,
                 initial_shapes=self._regions,
                 initial_scale=scale_factor,
-                debug_mode=self._debug_mode)
-            save_was_specified = bool(self._save_region)
-            if not regions.run(warn_if_notkinter=not save_was_specified):
+                debug_mode=self._debug_mode,
+                video_path=self._input.paths[0],
+                save_path=self._save_region)
+            if not regions.run():
                 return False
-
             self._regions = list(regions.shapes)
-        if self._regions:
-            logger.info(f"Limiting detection to {len(self._regions)} "
-                        f"region{'s' if len(self._regions) > 1 else ''}.")
-        else:
-            logger.debug("No regions selected.")
-        if self._save_region:
+        elif self._save_region:
             regions = self._regions if self._regions else [[
                 Point(0, 0),
                 Point(self._input.resolution[0] - 1, 0),
                 Point(self._input.resolution[0] - 1, self._input.resolution[1] - 1),
                 Point(0, self._input.resolution[1] - 1)
             ]]
             path = self._save_region
             if self._output_dir:
                 path = os.path.join(self._output_dir, path)
             with open(path, 'wt') as region_file:
                 for shape in self._regions:
                     region_file.write(" ".join(f"{x} {y}" for x, y in shape))
                     region_file.write("\n")
             logger.info(f"Saved region data to: {path}")
+        if self._regions:
+            logger.info(f"Limiting detection to {len(self._regions)} "
+                        f"region{'s' if len(self._regions) > 1 else ''}.")
+        else:
+            logger.debug("No regions selected.")
         return True
 
     def _create_progress_bar(self) -> tqdm:
         num_frames = self._input.total_frames
         # Correct for end time.
         if self._end_time and self._end_time.frame_num < num_frames:
             num_frames = self._end_time.frame_num
@@ -557,24 +569,26 @@
             kernel_size = _recommended_kernel_size(self._input.resolution[0],
                                                    self._downscale_factor)
         else:
             kernel_size = _scale_kernel_size(self._kernel_size, self._downscale_factor)
 
         # Create background subtractor and motion detector.
         detector = MotionDetector(
-            subtractor=self._subtractor_type.value(kernel_size=kernel_size),
+            subtractor=self._subtractor_type.value(
+                kernel_size=kernel_size, learning_rate=self._learning_rate),
             frame_size=self._input.resolution,
             downscale=self._downscale_factor,
             regions=self._regions)
 
         logger.info(
-            'Using subtractor %s with kernel_size = %s%s',
+            'Using subtractor %s with kernel_size = %s%s and learning_rate = %s',
             self._subtractor_type.name,
             str(kernel_size) if kernel_size else 'off',
             ' (auto)' if self._kernel_size == -1 else '',
+            str(self._learning_rate) if self._learning_rate != -1 else 'auto',
         )
 
         # Correct event length parameters to account frame skip.
         post_event_len: int = self._post_event_len.frame_num // (self._frame_skip + 1)
         pre_event_len: int = self._pre_event_len.frame_num // (self._frame_skip + 1)
         min_event_len: int = max(self._min_event_len.frame_num // (self._frame_skip + 1), 1)
 
@@ -624,22 +638,25 @@
 
         # TODO: The main scanning loop should be refactored into a state machine.
         while not self._stop.is_set():
             # Keep polling decode queue until it's empty (signaled via None).
             frame: Optional[DecodeEvent] = decode_queue.get()
             if frame is None:
                 break
-            assert frame.frame_rgb is not None
-            # TODO(v1.7): Is this copy necessary?
-            frame_copy = (
-                frame.frame_rgb
-                if not self._output_mode == OutputMode.OPENCV else frame.frame_rgb.copy())
-            result = detector.update(frame_copy)
+            assert frame.frame_bgr is not None
+            frame_size = (frame.frame_bgr.shape[1], frame.frame_bgr.shape[0])
+            if frame_size != self._input.resolution:
+                time = frame.timecode
+                video_res = self._input.resolution
+                logger.warn(
+                    f"WARNING: Frame {time.frame_num} [{time.get_timecode()}] has unexpected size: "
+                    f"{frame_size[0]}x{frame_size[1]}, expected {video_res[0]}x{video_res[1]}")
+            result = detector.update(frame.frame_bgr)
             frame_score = result.score
-            # TODO(v1.6): Allow disabling the rejection filter or customizing amount of
+            # TODO(1.7): Allow disabling the rejection filter or customizing amount of
             # consecutive frames it will ignore.
             if frame_score >= self._max_threshold:
                 frame_score = 0
             above_threshold = frame_score >= self._threshold
             event_window.append(frame_score)
             # The first frame fed to the detector can sometimes produce unreliable results due
             # to it not having any previous information to compare against.
@@ -693,26 +710,26 @@
                         if self._output_mode != OutputMode.SCAN_ONLY:
                             encode_queue.put(MotionEvent(start=event_start, end=event_end))
 
                 # Send frame to encode thread.
                 if in_motion_event and self._output_mode == OutputMode.OPENCV:
                     encode_queue.put(
                         EncodeFrameEvent(
-                            frame_rgb=frame.frame_rgb,
+                            frame_bgr=frame.frame_bgr,
                             timecode=frame.timecode,
                             bounding_box=bounding_box,
                             score=frame_score,
                         ))
             # Not already in a motion event, look for a new one.
             else:
                 # Buffer the required amount of frames and overlay data until we find an event.
                 if self._output_mode == OutputMode.OPENCV:
                     buffered_frames.append(
                         EncodeFrameEvent(
-                            frame_rgb=frame.frame_rgb,
+                            frame_bgr=frame.frame_bgr,
                             timecode=frame.timecode,
                             bounding_box=bounding_box,
                             score=frame_score,
                         ))
                     buffered_frames = buffered_frames[-buff_len:]
                 # Start a new event once all frames in the event window have motion.
                 if len(event_window) >= min_event_len and all(
@@ -785,24 +802,24 @@
         try:
             while not self._stop.is_set():
                 if self._end_time is not None and self._input.position >= self._end_time:
                     break
                 for _ in range(self._frame_skip):
                     if self._input.read(decode=False) is None:
                         break
-                frame_rgb = self._input.read()
-                if frame_rgb is None:
+                frame_bgr = self._input.read()
+                if frame_bgr is None:
                     break
                 # self._input.position points to the time at the end of the current frame (i.e. the
                 # first frame has a frame_num of 1), so we correct that for presentation time.
                 assert self._input.position.frame_num > 0
                 presentation_time = FrameTimecode(
                     timecode=self._input.position.frame_num - 1, fps=self._input.framerate)
                 if not self._stop.is_set():
-                    decode_queue.put(DecodeEvent(frame_rgb, presentation_time))
+                    decode_queue.put(DecodeEvent(frame_bgr, presentation_time))
 
         # We'll re-raise any exceptions from the main thread.
         # pylint: disable=bare-except
         except:
             self._stop.set()
             logger.critical('Fatal error: Exception raised in decode thread.')
             logger.debug(sys.exc_info())
@@ -818,32 +835,37 @@
             path = os.path.join(self._output_dir, path)
         effective_framerate = (
             self._input.framerate if self._frame_skip < 1 else self._input.framerate /
             (1 + self._frame_skip))
         return cv2.VideoWriter(path, self._fourcc, effective_framerate, frame_size)
 
     def _on_encode_frame_event(self, event: EncodeFrameEvent):
-        # Got a frame we need to export, create a new VideoWriter if we don't have one (i.e. this
-        # is the first event, or the previous event finished).
+        size = (event.frame_bgr.shape[1], event.frame_bgr.shape[0])
+        if size != self._input.resolution:
+            time = event.timecode
+            video = self._input.resolution
+            logger.warn(
+                f"WARNING: Failed to write event at frame {time.frame_num} [{time.get_timecode()}] "
+                f"due to size mismatch: {size[0]}x{size[1]}, expected {video[0]}x{video[1]}")
+            return
         if self._video_writer is None:
             # Use the first input video name as a filename template.
             video_name = get_filename(path=self._input.paths[0], include_extension=False)
             output_path = (
                 self._comp_file if self._comp_file else OUTPUT_FILE_TEMPLATE.format(
                     VIDEO_NAME=video_name,
                     EVENT_NUMBER='%04d' % (1 + self._num_events),
                     EXTENSION='avi',
                 ))
-            resolution = (event.frame_rgb.shape[1], event.frame_rgb.shape[0])
-            assert resolution == self._input.resolution
-            self._video_writer = self._init_video_writer(output_path, resolution)
-        # Render all overlays onto frame in-place.
-        self._draw_overlays(event.frame_rgb, event.timecode, event.score, event.bounding_box)
+            self._video_writer = self._init_video_writer(output_path, size)
+        # *NOTE*: Overlays are currently rendered in-place by modifying the event itself.
+        self._draw_overlays(event.frame_bgr, event.timecode, event.score, event.bounding_box)
         # Encode and write frame to disk.
-        self._video_writer.write(event.frame_rgb)
+
+        self._video_writer.write(event.frame_bgr)
 
     def _draw_overlays(
         self,
         frame: np.ndarray,
         timecode: FrameTimecode,
         frame_score: float,
         bounding_box: Optional[Tuple[int, int, int, int]],
@@ -856,17 +878,25 @@
             self._metrics_overlay.draw(frame, text=to_display)
         if not self._bounding_box is None and not bounding_box is None:
             self._bounding_box.draw(frame, bounding_box, use_shift)
 
     def _on_mask_event(self, event: MotionMaskEvent):
         # Initialize the VideoWriter used for mask output.
         if self._mask_writer is None:
-            resolution = event.motion_mask.shape[1], event.motion_mask.shape[0]
-            self._mask_writer = self._init_video_writer(self._mask_file, resolution)
+            self._mask_size = event.motion_mask.shape[1], event.motion_mask.shape[0]
+            self._mask_writer = self._init_video_writer(self._mask_file, self._mask_size)
         # Write the motion mask to the output file.
+        size = (event.motion_mask.shape[1], event.motion_mask.shape[0])
+        if size != self._mask_size:
+            time = event.timecode
+            logger.warn(
+                f"WARNING: Failed to write mask at frame {time.frame_num} [{time.get_timecode()}] "
+                f"due to size mismatch: {size[0]}x{size[1]}, "
+                f" expected {self._mask_size[0]}x{self._mask_size[1]}")
+            return
         out_frame = cv2.cvtColor(event.motion_mask, cv2.COLOR_GRAY2BGR)
         self._draw_overlays(
             out_frame, event.timecode, event.score, event.bounding_box, use_shift=False)
         self._mask_writer.write(out_frame)
 
     def _on_motion_event(self, event: MotionEvent):
         self._num_events += 1
```

### Comparing `dvr-scan-1.6/dvr_scan/subtractor.py` & `dvr_scan-1.6.1/dvr_scan/subtractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """``dvr_scan.subtractor`` Module
 
 Defines an interface to background subtraction (`Subtractor`), and provides several implementations.
 All current subtractors use algorithms backed by OpenCV, but this is not a requirement.
@@ -49,30 +49,32 @@
 
     def __init__(
         self,
         kernel_size: int,
         history: int = 500,
         variance_threshold: int = 16,
         detect_shadows: bool = False,
+        learning_rate: float = -1,
     ):
         if kernel_size < 0 or (kernel_size > 1 and kernel_size % 2 == 0):
             raise ValueError("kernel_size must be >= 0")
         self._kernel = numpy.ones(
             (kernel_size, kernel_size), numpy.uint8) if kernel_size > 1 else None
         self._subtractor = cv2.createBackgroundSubtractorMOG2(
             history=history,
             varThreshold=variance_threshold,
             detectShadows=detect_shadows,
         )
         # Default shadow value is 127, set to 0 so they are discarded before filtering.
         self._subtractor.setShadowValue(0)
+        self._learning_rate = learning_rate
 
     def apply(self, frame: numpy.ndarray) -> numpy.ndarray:
         frame_gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
-        frame_mask = self._subtractor.apply(frame_gray)
+        frame_mask = self._subtractor.apply(frame_gray, learningRate=self._learning_rate)
         if not self._kernel is None:
             frame_filt = cv2.morphologyEx(frame_mask, cv2.MORPH_OPEN, self._kernel)
         else:
             frame_filt = frame_mask
         return frame_filt
 
     @staticmethod
@@ -86,25 +88,27 @@
     def __init__(
         self,
         kernel_size: int,
         min_pixel_stability: int = 15,
         use_history: bool = True,
         max_pixel_stability: int = 15 * 60,
         is_parallel: bool = True,
+        learning_rate: float = -1,
     ):
         if kernel_size < 0 or (kernel_size > 1 and kernel_size % 2 == 0):
             raise ValueError("kernel_size must be odd integer >= 1 or zero (0)")
         self._kernel = numpy.ones(
             (kernel_size, kernel_size), numpy.uint8) if kernel_size > 1 else None
         self._subtractor = cv2.bgsegm.createBackgroundSubtractorCNT(
             minPixelStability=min_pixel_stability,
             useHistory=use_history,
             maxPixelStability=max_pixel_stability,
             isParallel=is_parallel,
         )
+        self._learning_rate = learning_rate
 
     @staticmethod
     def is_available():
         return hasattr(cv2, 'bgsegm') and hasattr(cv2.bgsegm, 'createBackgroundSubtractorCNT')
 
 
 class SubtractorCudaMOG2(SubtractorMOG2):
@@ -112,34 +116,36 @@
 
     def __init__(
         self,
         kernel_size: int,
         history: int = 500,
         variance_threshold: int = 16,
         detect_shadows: bool = False,
+        learning_rate: float = -1,
     ):
         if kernel_size < 0 or (kernel_size > 1 and kernel_size % 2 == 0):
             raise ValueError("kernel_size must be odd integer >= 1 or zero (0)")
         self._filter = cv2.cuda.createMorphologyFilter(
             cv2.MORPH_OPEN, cv2.CV_8UC1, numpy.ones(
                 (kernel_size, kernel_size), numpy.uint8)) if kernel_size > 1 else None
         self._subtractor = cv2.cuda.createBackgroundSubtractorMOG2(
             history=history,
             varThreshold=variance_threshold,
             detectShadows=detect_shadows,
         )
         # Default shadow value is 127, set to 0 so they are discarded before filtering.
         self._subtractor.setShadowValue(0)
+        self._learning_rate = learning_rate
 
     def apply(self, frame: numpy.ndarray) -> numpy.ndarray:
         stream = cv2.cuda_Stream()
-        frame_rgb_dev = cv2.cuda_GpuMat()
-        frame_rgb_dev.upload(frame, stream=stream)
-        frame_gray_dev = cv2.cuda.cvtColor(frame_rgb_dev, cv2.COLOR_BGR2GRAY, stream=stream)
-        frame_mask_dev = self._subtractor.apply(frame_gray_dev, -1, stream=stream)
+        frame_bgr_dev = cv2.cuda_GpuMat()
+        frame_bgr_dev.upload(frame, stream=stream)
+        frame_gray_dev = cv2.cuda.cvtColor(frame_bgr_dev, cv2.COLOR_BGR2GRAY, stream=stream)
+        frame_mask_dev = self._subtractor.apply(frame_gray_dev, self._learning_rate, stream=stream)
         if not self._filter is None:
             frame_filt_dev = self._filter.apply(frame_mask_dev, stream=stream)
         else:
             frame_filt_dev = frame_mask_dev
         frame_filt = frame_filt_dev.download(stream=stream)
         stream.waitForCompletion()
         return frame_filt
```

### Comparing `dvr-scan-1.6/dvr_scan/video_joiner.py` & `dvr_scan-1.6.1/dvr_scan/video_joiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 #      DVR-Scan: Video Motion Event Detection & Extraction Tool
 #   --------------------------------------------------------------
 #       [  Site: https://www.dvr-scan.com/                 ]
 #       [  Repo: https://github.com/Breakthrough/DVR-Scan  ]
 #
-# Copyright (C) 2014-2023 Brandon Castellano <http://www.bcastell.com>.
+# Copyright (C) 2014-2024 Brandon Castellano <http://www.bcastell.com>.
 # DVR-Scan is licensed under the BSD 2-Clause License; see the included
 # LICENSE file, or visit one of the above pages for details.
 #
 """ ``dvr_scan.video_joiner`` Module
 
 Contains a helper class to concatenate multiple videos and treat it as a single,
 contiguous video file.
```

### Comparing `dvr-scan-1.6/dvr_scan.egg-info/PKG-INFO` & `dvr_scan-1.6.1/dvr_scan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvr-scan
-Version: 1.6
+Version: 1.6.1
 Summary: Tool for finding and extracting motion events in video files (e.g. security camera footage).
 Home-page: https://www.dvr-scan.com/
 Author: Brandon Castellano
 Author-email: brandon248@gmail.com
 License: BSD 2-Clause License
 Project-URL: Homepage, https://www.dvr-scan.com/
 Project-URL: Repository, https://github.com/Breakthrough/DVR-Scan
@@ -16,24 +16,24 @@
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Multimedia :: Video :: Conversion
 Classifier: Topic :: Multimedia :: Video :: Non-Linear Editor
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: platformdirs
 Requires-Dist: numpy
 Requires-Dist: scenedetect
 Requires-Dist: screeninfo
 Requires-Dist: tqdm
```

### Comparing `dvr-scan-1.6/dvr_scan.egg-info/SOURCES.txt` & `dvr_scan-1.6.1/dvr_scan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvr-scan-1.6/setup.cfg` & `dvr_scan-1.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 	Environment :: Console :: Curses
 	Intended Audience :: Developers
 	Intended Audience :: End Users/Desktop
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Multimedia :: Video
 	Topic :: Multimedia :: Video :: Conversion
 	Topic :: Multimedia :: Video :: Non-Linear Editor
 	Topic :: Utilities
 keywords = video computer-vision analysis
 
 [options]
@@ -40,15 +40,15 @@
 	numpy
 	scenedetect
 	screeninfo
 	tqdm
 packages = 
 	dvr_scan
 	dvr_scan.cli
-python_requires = >=3.7
+python_requires = >=3.8
 include_package_data = True
 
 [options.extras_require]
 opencv = opencv-python
 opencv-headless = opencv-python-headless
 
 [options.entry_points]
```

