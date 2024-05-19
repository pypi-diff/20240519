# Comparing `tmp/SPLayout-0.5.2.tar.gz` & `tmp/splayout-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPLayout-0.5.2.tar", last modified: Mon Sep 11 11:03:05 2023, max compression
+gzip compressed data, was "splayout-0.5.3.tar", last modified: Sun May 19 11:44:50 2024, max compression
```

## Comparing `SPLayout-0.5.2.tar` & `splayout-0.5.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.094355 SPLayout-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2023-09-11 11:02:55.000000 SPLayout-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-09-11 11:03:05.094355 SPLayout-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2023-09-11 11:02:55.000000 SPLayout-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.086354 SPLayout-0.5.2/SPLayout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-09-11 11:03:05.000000 SPLayout-0.5.2/SPLayout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-09-11 11:03:05.000000 SPLayout-0.5.2/SPLayout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-11 11:03:05.000000 SPLayout-0.5.2/SPLayout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-11 11:03:05.000000 SPLayout-0.5.2/SPLayout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-11 11:03:05.000000 SPLayout-0.5.2/SPLayout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-11 11:03:05.094355 SPLayout-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-09-11 11:02:55.000000 SPLayout-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.086354 SPLayout-0.5.2/splayout/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.090355 SPLayout-0.5.2/splayout/adjointmethod/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/adjointmultitoopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/adjointshapeopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/adjointtopologyopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15631 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/scalabletoregion3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10331 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/shaperegion2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10395 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/shaperegion3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/topologyregion2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/adjointmethod/topologyregion3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.090355 SPLayout-0.5.2/splayout/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/algorithms/binarybatalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/algorithms/binarygeneticalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5669 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/algorithms/binaryparticleswarmalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/algorithms/directbinarysearchalgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/algorithms/particleswarmalgorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.090355 SPLayout-0.5.2/splayout/components/
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/AEMDgrating.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/bend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/doubleconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/filledpattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    48385 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/microring.py
--rw-r--r--   0 runner    (1001) docker     (127)    20977 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/pixelsregion.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13958 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/quarbend.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/sbend.py
--rw-r--r--   0 runner    (1001) docker     (127)    12910 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/selfdefinecomponent.py
--rw-r--r--   0 runner    (1001) docker     (127)    27611 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/simpleasymmetricdirectionalcoupler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/slowlyvaryingtaper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/taper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/components/waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.094355 SPLayout-0.5.2/splayout/lumericalcommun/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/lumericalcommun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76384 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/lumericalcommun/fdtdapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    43227 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/lumericalcommun/modeapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-11 11:03:05.094355 SPLayout-0.5.2/splayout/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14381 2023-09-11 11:02:55.000000 SPLayout-0.5.2/splayout/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-19 11:44:46.000000 splayout-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 11:44:50.962710 splayout-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-19 11:44:46.000000 splayout-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/SPLayout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 11:44:50.000000 splayout-0.5.3/SPLayout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:44:50.962710 splayout-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-19 11:44:47.000000 splayout-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.954710 splayout-0.5.3/splayout/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.958710 splayout-0.5.3/splayout/adjointmethod/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/adjointmultitoopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/adjointshapeopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/adjointtopologyopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/scalabletoregion3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/shaperegion2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/shaperegion3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11154 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/topologyregion2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/adjointmethod/topologyregion3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.958710 splayout-0.5.3/splayout/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/binarybatalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/binarygeneticalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/binaryparticleswarmalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/directbinarysearchalgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/algorithms/particleswarmalgorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/splayout/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/AEMDgrating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/bend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/doubleconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/filledpattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48385 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/microring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20977 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/pixelsregion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13958 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/quarbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/sbend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12910 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/selfdefinecomponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27611 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/simpleasymmetricdirectionalcoupler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/slowlyvaryingtaper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/taper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/components/waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/splayout/lumericalcommun/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/lumericalcommun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85189 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/lumericalcommun/fdtdapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/lumericalcommun/modeapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:44:50.962710 splayout-0.5.3/splayout/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2024-05-19 11:44:47.000000 splayout-0.5.3/splayout/utils/utils.py
```

### Comparing `SPLayout-0.5.2/LICENSE` & `splayout-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/PKG-INFO` & `splayout-0.5.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.5.2
+Version: 0.5.3
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 Requires-Dist: gdspy
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 SPLayout
 ========
 
 |GitHub repository| |GitHub license|
 
-SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
+SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a silicon photonics structures design package. It provides commonly used silicon photonics structures for fast integration and pixelated blocks for inverse design.
 
 The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
 
 
 Dependency
 ----------
```

### Comparing `SPLayout-0.5.2/README.rst` & `splayout-0.5.3/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 SPLayout
 ========
 
 |GitHub repository| |GitHub license|
 
-SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
+SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a silicon photonics structures design package. It provides commonly used silicon photonics structures for fast integration and pixelated blocks for inverse design.
 
 The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
 
 
 Dependency
 ----------
```

### Comparing `SPLayout-0.5.2/SPLayout.egg-info/PKG-INFO` & `splayout-0.5.3/SPLayout.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: SPLayout
-Version: 0.5.2
+Version: 0.5.3
 Summary: Silicon Photonics Design Tools for GDSII Files.
 Home-page: https://github.com/Hideousmon/SPLayout
 Author: Zhenyu ZHAO
 Author-email: mailtozyzhao@163.com
 License-File: LICENSE
 Requires-Dist: gdspy
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 SPLayout
 ========
 
 |GitHub repository| |GitHub license|
 
-SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a package for silicon photonics structures design. It provides commonly used silicon photonics structure classes for fast integration and pixelized blocks for inverse design and optimization. Some inverse design algorithms are also integrated in it like DBS (Direct Binary Search) and BBA (Binary Bat Algorithm).
+SPLayout (**S**\ilicon **P**\hotonics **Layout** Design Tools) is a silicon photonics structures design package. It provides commonly used silicon photonics structures for fast integration and pixelated blocks for inverse design.
 
 The GDSII streaming is based on gdspy(https://github.com/heitzmann/gdspy) and FDTD simulation is executed on Ansys Lumerical.
 
 
 Dependency
 ----------
```

### Comparing `SPLayout-0.5.2/SPLayout.egg-info/SOURCES.txt` & `splayout-0.5.3/SPLayout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/setup.py` & `splayout-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/__init__.py` & `splayout-0.5.3/splayout/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 ## Submodules
 from . import utils
 from . import components
 from . import algorithms
 from . import lumericalcommun
 from . import adjointmethod
```

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/adjointmultitoopt.py` & `splayout-0.5.3/splayout/adjointmethod/adjointmultitoopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/adjointshapeopt.py` & `splayout-0.5.3/splayout/adjointmethod/adjointshapeopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/adjointtopologyopt.py` & `splayout-0.5.3/splayout/adjointmethod/adjointtopologyopt.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/scalabletoregion3d.py` & `splayout-0.5.3/splayout/adjointmethod/scalabletoregion3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
         self.lower_epsilon = lower_index**2
         self.higher_epsilon = higher_index**2
         self.z_start = z_start
         self.z_end = z_end
         self.rename = rename
         self.index_region_name = self.rename + "_index"
         self.field_region_name = self.rename + "_field"
-        self.__initialize()
+        if not (self.fdtd_engine is None):
+            self.__initialize()
         self.epsilon_figure = None
         self.field_figure = None
 
     def __initialize(self):
         self.fdtd_engine.add_index_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max, dimension=3, index_monitor_name= self.index_region_name)
         self.fdtd_engine.fdtd.eval( 'select("{}");set("spatial interpolation","specified position");'.format(self.index_region_name))
         self.fdtd_engine.add_field_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max, dimension=3, field_monitor_name= self.field_region_name)
```

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/shaperegion2d.py` & `splayout-0.5.3/splayout/adjointmethod/shaperegion2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         self.y_positions = np.linspace(self.y_min, self.y_max, self.y_size)
         self.z_positions = np.linspace(self.z_min, self.z_max, self.z_size)
         self.z_start = z_start
         self.z_end = z_end
         self.rename = rename
         self.index_region_name = self.rename + "_index"
         self.field_region_name = self.rename + "_field"
-        self.__initialize()
+        if not (self.fdtd_engine is None):
+            self.__initialize()
         self.epsilon_figure = None
         self.field_figure = None
 
     def __initialize(self):
         self.fdtd_engine.add_index_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max,
                                           dimension=2, index_monitor_name=self.index_region_name)
         self.fdtd_engine.add_field_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max,
```

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/shaperegion3d.py` & `splayout-0.5.3/splayout/adjointmethod/shaperegion3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
         self.y_positions = np.linspace(self.y_min, self.y_max, self.y_size)
         self.z_positions = np.linspace(self.z_min, self.z_max, self.z_size)
         self.z_start = z_start
         self.z_end = z_end
         self.rename = rename
         self.index_region_name = self.rename + "_index"
         self.field_region_name = self.rename + "_field"
-        self.__initialize()
+        if not (self.fdtd_engine is None):
+            self.__initialize()
         self.epsilon_figure = None
         self.field_figure = None
 
     def __initialize(self):
 
         self.fdtd_engine.add_index_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max,
                                           dimension=3, index_monitor_name=self.index_region_name)
```

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/topologyregion2d.py` & `splayout-0.5.3/splayout/adjointmethod/topologyregion2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,16 @@
         self.z_end = z_end
         self.rename = rename
         self.filter_R = filter_R
         self.eta = eta
         self.beta = beta
         self.index_region_name = self.rename + "_index"
         self.field_region_name = self.rename + "_field"
-        self.__initialize()
+        if not (self.fdtd_engine is None):
+            self.__initialize()
         self.epsilon_figure = None
         self.field_figure = None
 
     def __initialize(self):
         self.fdtd_engine.add_index_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max, dimension=2, index_monitor_name= self.index_region_name)
         self.fdtd_engine.fdtd.eval( 'select("{}");set("spatial interpolation","specified position");'.format(self.index_region_name))
         self.fdtd_engine.add_field_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max, dimension=2, field_monitor_name= self.field_region_name)
```

### Comparing `SPLayout-0.5.2/splayout/adjointmethod/topologyregion3d.py` & `splayout-0.5.3/splayout/adjointmethod/topologyregion3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,16 @@
         self.lower_epsilon = lower_index**2
         self.higher_epsilon = higher_index**2
         self.z_start = z_start
         self.z_end = z_end
         self.rename = rename
         self.index_region_name = self.rename + "_index"
         self.field_region_name = self.rename + "_field"
-        self.__initialize()
+        if not(self.fdtd_engine is None):
+            self.__initialize()
         self.epsilon_figure = None
         self.field_figure = None
 
     def __initialize(self):
         self.fdtd_engine.add_index_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max, dimension=3, index_monitor_name= self.index_region_name)
         self.fdtd_engine.fdtd.eval( 'select("{}");set("spatial interpolation","specified position");'.format(self.index_region_name))
         self.fdtd_engine.add_field_region(self.left_down_point, self.right_up_point, z_min=self.z_min, z_max=self.z_max, dimension=3, field_monitor_name= self.field_region_name)
```

### Comparing `SPLayout-0.5.2/splayout/algorithms/binarybatalgorithm.py` & `splayout-0.5.3/splayout/algorithms/binarybatalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/algorithms/binarygeneticalgorithm.py` & `splayout-0.5.3/splayout/algorithms/binarygeneticalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/algorithms/binaryparticleswarmalgorithm.py` & `splayout-0.5.3/splayout/algorithms/binaryparticleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/algorithms/directbinarysearchalgorithm.py` & `splayout-0.5.3/splayout/algorithms/directbinarysearchalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/algorithms/particleswarmalgorithm.py` & `splayout-0.5.3/splayout/algorithms/particleswarmalgorithm.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/AEMDgrating.py` & `splayout-0.5.3/splayout/components/AEMDgrating.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/__init__.py` & `splayout-0.5.3/splayout/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 from .quarbend import QuarBend,AQuarBend
 from .selfdefinecomponent import MAKE_COMPONENT
 from .taper import Taper
 from .slowlyvaryingtaper import SlowlyVaryingTaper
 from .text import Text
 from .waveguide import Waveguide, ArbitraryAngleWaveguide
 from .sbend import SBend,ASBend
-from .filledpattern import Circle,Rectangle
+from .filledpattern import Circle, Rectangle
```

### Comparing `SPLayout-0.5.2/splayout/components/bend.py` & `splayout-0.5.3/splayout/components/bend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/doubleconnector.py` & `splayout-0.5.3/splayout/components/doubleconnector.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/filledpattern.py` & `splayout-0.5.3/splayout/components/filledpattern.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/microring.py` & `splayout-0.5.3/splayout/components/microring.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/pixelsregion.py` & `splayout-0.5.3/splayout/components/pixelsregion.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/polygon.py` & `splayout-0.5.3/splayout/components/polygon.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/quarbend.py` & `splayout-0.5.3/splayout/components/quarbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/sbend.py` & `splayout-0.5.3/splayout/components/sbend.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/selfdefinecomponent.py` & `splayout-0.5.3/splayout/components/selfdefinecomponent.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/simpleasymmetricdirectionalcoupler.py` & `splayout-0.5.3/splayout/components/simpleasymmetricdirectionalcoupler.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/slowlyvaryingtaper.py` & `splayout-0.5.3/splayout/components/slowlyvaryingtaper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/taper.py` & `splayout-0.5.3/splayout/components/taper.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/text.py` & `splayout-0.5.3/splayout/components/text.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/components/waveguide.py` & `splayout-0.5.3/splayout/components/waveguide.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/lumericalcommun/fdtdapi.py` & `splayout-0.5.3/splayout/lumericalcommun/fdtdapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,15 +126,17 @@
             self.fdtd.setglobalmonitor('use source limits', True)
             self.fdtd.setglobalmonitor('use wavelength spacing', True)
             self.fdtd.setglobalmonitor('frequency points', points)
             self.frequency_points = points
             self.global_monitor_set_flag = 1
 
 
-    def add_mode_expansion(self,position, mode_list, width=2, height=0.8, z_min = None, z_max = None, expansion_name="expansion", points = 251, update_mode = 0, normal_direction = HORIZONTAL):
+    def add_mode_expansion(self,position, mode_list, width=2, height=0.8, z_min = None, z_max = None,
+                           expansion_name="expansion", points = 251, update_mode = 0,
+                           normal_direction = HORIZONTAL, auto_update = 1):
         """
         Add mode expansion monitor in Lumerical FDTD.
 
         Parameters
         ----------
         position : Point or tuple
             Center point of the monitor.
@@ -152,14 +154,16 @@
             Name of the mode expansion monitor in Lumerical FDTD (default: "expansion").
         points : Int
             The number of the frequency points that will be monitored (default: 251).
         update_mode : Int or bool
             Whether update the mode after defining FDTD and mesh (default: 0).
         normal_direction : HORIZONAL or VERTICAL
             The direction of the monitor. HORIZONAL: x-normal, VERTICAL: y-normal.
+        update_mode : Int or bool
+            Whether enable auto update in Lumerical.
 
         Notes
         -----
         This function will automatically add a power monitor at the same position with same shape.
         If use update_mode the monitor should be put after adding fdtd region and mesh region.
         If z_min and z_max are specified, the height property will be invalid.
         """
@@ -198,18 +202,21 @@
         self.fdtd.eval("setexpansion(\"Output\",\""+power_monitor_name+"\");")
         if (type(mode_list) == str):
             self.fdtd.eval("set(\"mode selection\",\""+mode_list+"\");")
         else:
             self.fdtd.eval("set(\"mode selection\",\"user select\");")
             self.fdtd.eval("set(\"selected mode numbers\"," + self.str_list(mode_list) + ");")
 
-        if (update_mode):
+        if update_mode:
             self.fdtd.updatemodes()
         self.fdtd.eval("set(\"override global monitor settings\",0);")
-        self.fdtd.eval("set(\"auto update\",1);")
+        if auto_update:
+            self.fdtd.eval("set(\"auto update\",1);")
+        else:
+            self.fdtd.eval("set(\"auto update\",0);")
 
     def reset_mode_expansion_modes(self, expansion_name, mode_list):
         """
         Reset mode list for mode expansion monitor.
 
         Parameters
         ----------
@@ -315,15 +322,15 @@
             self.fdtd.setglobalsource('set wavelength', True)
             self.fdtd.setglobalsource('wavelength start', wavelength_start*1e-6)
             self.fdtd.setglobalsource('wavelength stop', wavelength_end*1e-6)
             self.wavelength_start = wavelength_start*1e-6
             self.wavelength_end = wavelength_end*1e-6
             self.global_source_set_flag = 1
 
-    def add_imported_source(self, position, width, height, origin_x, origin_y, origin_z, E, H = None,
+    def add_imported_source(self, position, width, height, origin_x=None, origin_y=None, origin_z=None, E=None, H = None,
                             z_min = None, z_max = None, source_name = "source", amplitude=1 , phase = 0,
                             direction = FORWARD, normal_direction = HORIZONTAL):
         """
         Add imported source in Lumerical FDTD.
 
         Parameters
         ----------
@@ -359,22 +366,14 @@
             The direction of the mode source. HORIZONAL: x-normal, VERTICAL: y-normal.
 
         Notes
         -----
         If z_min and z_max are specified, the height property will be invalid.
         """
         position = tuple_to_point(position)
-        wavelength = np.flip(self.get_wavelength())
-        frequency = np.flip(self.get_frequency())
-
-        self.fdtd.putv("lam", wavelength)
-        self.fdtd.putv("f", frequency)
-        self.fdtd.putv("Ex", E[:, :, :, :, 0])
-        self.fdtd.putv("Ey", E[:, :, :, :, 1])
-        self.fdtd.putv("Ez", E[:, :, :, :, 2])
         self.fdtd.eval("addimportedsource;")
         self.fdtd.eval("set(\"name\",\"" + source_name + "\");")
 
         if (direction == FORWARD):
             self.fdtd.eval("set(\"direction\",\"Forward\");")
         elif (direction == BACKWARD):
             self.fdtd.eval("set(\"direction\",\"Backward\");")
@@ -403,26 +402,36 @@
             else:
                 self.fdtd.eval("set(\"z span\"," + "%.6f" % (height) + "e-6);")
         else:
             raise Exception("Unsupported normal_direction specified!")
         self.fdtd.eval("set(\"amplitude\"," + "%.6f" % (amplitude) + ");")
         self.fdtd.eval("set(\"phase\"," + "%.6f" % (phase) + ");")
 
-        self.fdtd.putv("x", origin_x)
-        self.fdtd.putv("y", origin_y)
-        self.fdtd.putv("z", origin_z)
-        self.fdtd.eval("EM = rectilineardataset(\"EM fields\",x,y,z);")
-        self.fdtd.eval("EM.addparameter(\"lambda\", lam, \"f\", f);")
-        self.fdtd.eval("EM.addattribute(\"E\", Ex, Ey, Ez);")
-        if (type(H) != type(None)):
-            self.fdtd.putv("Hx", H[:, :, :, :, 0])
-            self.fdtd.putv("Hy", H[:, :, :, :, 1])
-            self.fdtd.putv("Hz", H[:, :, :, :, 2])
-            self.fdtd.eval("EM.addattribute(\"H\", Hx, Hy, Hz);")
-        self.fdtd.eval("importdataset(EM);")
+        if not((origin_x is None) and (origin_y is None) and (origin_z is None) and (E is None) and
+               (H is None)):
+            wavelength = np.flip(self.get_wavelength())
+            frequency = np.flip(self.get_frequency())
+
+            self.fdtd.putv("lam", wavelength)
+            self.fdtd.putv("f", frequency)
+            self.fdtd.putv("Ex", E[:, :, :, :, 0])
+            self.fdtd.putv("Ey", E[:, :, :, :, 1])
+            self.fdtd.putv("Ez", E[:, :, :, :, 2])
+            self.fdtd.putv("x", origin_x)
+            self.fdtd.putv("y", origin_y)
+            self.fdtd.putv("z", origin_z)
+            self.fdtd.eval("EM = rectilineardataset(\"EM fields\",x,y,z);")
+            self.fdtd.eval("EM.addparameter(\"lambda\", lam, \"f\", f);")
+            self.fdtd.eval("EM.addattribute(\"E\", Ex, Ey, Ez);")
+            if (type(H) != type(None)):
+                self.fdtd.putv("Hx", H[:, :, :, :, 0])
+                self.fdtd.putv("Hy", H[:, :, :, :, 1])
+                self.fdtd.putv("Hz", H[:, :, :, :, 2])
+                self.fdtd.eval("EM.addattribute(\"H\", Hx, Hy, Hz);")
+            self.fdtd.eval("importdataset(EM);")
 
 
     def reset_source_mode(self, source_name, mode_number):
         """
         Reset mode for source.
 
         Parameters
@@ -1724,11 +1733,207 @@
         ----------
         command : str
             Command that can be evaluated in fdtd.
         '''
         self.fdtd.eval(command)
 
 
+    def add_electric_dipole(self, center_point, source_name = "source", z_min = 0
+                            , amplitude = 1, phase = 0, wavelength_start = 1.54,
+                            wavelength_end = 1.57):
+        """
+        Add source in Lumerical FDTD.
+
+        Parameters
+        ----------
+        center_point : Point or tuple
+            Center point of the source.
+        z_min : Float
+            The position on z-axis (unit: μm, default: 0).
+        source_name : String
+            Name of the source in Lumerical FDTD (default: "source").
+        amplitude : Float or Int
+            The amplitude of the source (default: 1).
+        phase : Float or Int
+            The phase of the source (default: 0).
+        wavelength_start : Float
+            The start wavelength of the source (unit: μm, default: 1.540).
+        wavelength_end : Float
+            The end wavelength of the source (unit: μm, default: 1.570).
+        """
+        position = tuple_to_point(center_point)
+        self.fdtd.eval("adddipole;")
+        self.fdtd.eval("set(\"name\",\"" + source_name + "\");")
+
+        self.fdtd.eval("set(\"dipole type\",\"Electric dipole\");")
+
+        self.fdtd.eval("set(\"x\"," +  "%.6f"%(position.x) + "e-6);")
+        self.fdtd.eval("set(\"y\"," +  "%.6f"%(position.y) + "e-6);")
+        self.fdtd.eval("set(\"z\"," + "%.6f" % (z_min) + "e-6);")
+
+
+        self.fdtd.eval("set(\"override global source settings\",0);")
+        self.fdtd.eval("set(\"amplitude\"," +  "%.12f"%(amplitude) + ");")
+        self.fdtd.eval("set(\"phase\"," +  "%.6f"%(phase) + ");")
+        if not self.global_source_set_flag:
+            self.fdtd.setglobalsource('set wavelength', True)
+            self.fdtd.setglobalsource('wavelength start', wavelength_start*1e-6)
+            self.fdtd.setglobalsource('wavelength stop', wavelength_end*1e-6)
+            self.wavelength_start = wavelength_start*1e-6
+            self.wavelength_end = wavelength_end*1e-6
+            self.global_source_set_flag = 1
+
+
+    def add_field_point(self, center_point, z_min = 0, field_monitor_name="field", points=1):
+        """
+        Add a point field monitor in Lumerical FDTD (DFT Frequency monitor).
+
+        Parameters
+        ----------
+        center_point : Point or tuple
+            Center point of the monitor.
+        z_min : Float
+            The position on z-axis (unit: μm, default: 0).
+        field_monitor_name : String
+            Name of the monitor in Lumerical FDTD (default: "field").
+        points : Int
+            The number of the frequency points that will be monitored (default: 1).
+        """
+        self.fdtd.eval("addpower;")
+        self.fdtd.eval("set(\"name\",\"" + field_monitor_name + "\");")
+
+        position = center_point
+        self.fdtd.eval("set(\"monitor type\",1);")
+        self.fdtd.eval("set(\"x\"," + "%.6f" % (position.x) + "e-6);")
+        self.fdtd.eval("set(\"y\"," + "%.6f" % (position.y) + "e-6);")
+        self.fdtd.eval("set(\"z\"," + "%.6f" % (z_min) + "e-6);")
+
+        self.fdtd.eval("set(\"override global monitor settings\",0);")
+        if not self.global_monitor_set_flag:
+            self.fdtd.setglobalmonitor('use source limits', True)
+            self.fdtd.setglobalmonitor('use wavelength spacing', True)
+            self.fdtd.setglobalmonitor('frequency points', points)
+            self.frequency_points = points
+            self.global_monitor_set_flag = 1
+
+    def get_dipole_power(self, source_name=None, wavelengths = None,datafile = None):
+        """
+        Get source power spectrum from source.
+
+        Parameters
+        ----------
+        source_name : String
+            Name of the dipole source.
+        datafile : String
+            The name of the file for saving the data, None means no saving (default: None).
+
+        Returns
+        -------
+        out : Array
+            Spectrum, size: (1,frequency points).
+
+        Notes
+        -----
+        This function should be called after setting the frequency points in any frequency domain monitor.
+        """
+        if type(wavelengths) != type(None):
+            frequency = scipy.constants.speed_of_light / np.array([wavelengths]).flatten()
+            if (type(source_name) == type(None)):
+                source_power = self.fdtd.dipolepower(frequency)
+            else:
+                self.lumapi.putMatrix(self.fdtd.handle, "frequency", frequency)
+                self.fdtd.eval("data = dipolepower(frequency,\""+source_name+"\");")
+                source_power = self.lumapi.getVar(self.fdtd.handle, varname="data")
+        elif self.global_source_set_flag and self.global_monitor_set_flag:
+            wavelength = np.linspace(self.wavelength_start, self.wavelength_end, self.frequency_points)
+            frequency = scipy.constants.speed_of_light / wavelength
+            if (type(source_name) == type(None)):
+                source_power = self.fdtd.sourcepower(frequency)
+            else:
+                self.lumapi.putMatrix(self.fdtd.handle, "frequency", frequency)
+                self.fdtd.eval("data = dipolepower(frequency,\""+source_name+"\");")
+                source_power = self.lumapi.getVar(self.fdtd.handle, varname="data")
+        else:
+            raise Exception("The source is not well defined!")
+        if (datafile != None):
+            np.save(datafile, source_power.flatten())
+        return np.asarray(source_power).flatten()
+
+    def get_dipole_base_amplitude(self, source_name, datafile = None):
+        """
+        Get source power spectrum from source.
+
+        Parameters
+        ----------
+        source_name : String
+            Name of the dipole source.
+        datafile : String
+            The name of the file for saving the data, None means no saving (default: None).
+
+        Returns
+        -------
+        out : Array
+            Base amplitude, size: (1,frequency points).
+
+        Notes
+        -----
+        This function should be called after setting the frequency points in any frequency domain monitor.
+        """
+        self.fdtd.eval("data = getnamed(\""+source_name+"\", 'base amplitude');")
+        base_amplitued = self.lumapi.getVar(self.fdtd.handle, varname="data")
+
+        if (datafile != None):
+            np.save(datafile, base_amplitued.flatten())
+        return np.asarray(base_amplitued).flatten()
+
+    def reset_imported_source(self, origin_x, origin_y, origin_z, E, H = None, source_name = "source", amplitude=1 , phase = 0):
+        """
+        Reset imported source in Lumerical FDTD.
+
+        Parameters
+        ----------
+        origin_x : Array
+            The origin nodes distribution on x-axis.
+        origin_y : Array
+            The origin nodes distribution on y-axis.
+        origin_z : Array
+            The origin nodes distribution on z-axis.
+        E : Array
+            The imported electric field distribution.
+        H : Array
+            The imported magnetic field distribution.
+        source_name : String
+            Name of the source in Lumerical FDTD (default: "source").
+        amplitude : Float or Int
+            The amplitude of the source.
+        phase : Float or Int
+            The phase of the source.
+        """
+        wavelength = np.flip(self.get_wavelength())
+        frequency = np.flip(self.get_frequency())
+
+        self.fdtd.putv("lam", wavelength)
+        self.fdtd.putv("f", frequency)
+        self.fdtd.putv("Ex", E[:, :, :, :, 0])
+        self.fdtd.putv("Ey", E[:, :, :, :, 1])
+        self.fdtd.putv("Ez", E[:, :, :, :, 2])
+        self.fdtd.eval("select(\"" + source_name + "\");")
+
+        self.fdtd.eval("set(\"amplitude\"," + "%.6f" % (amplitude) + ");")
+        self.fdtd.eval("set(\"phase\"," + "%.6f" % (phase) + ");")
+
+        self.fdtd.putv("x", origin_x)
+        self.fdtd.putv("y", origin_y)
+        self.fdtd.putv("z", origin_z)
+        self.fdtd.eval("EM = rectilineardataset(\"EM fields\",x,y,z);")
+        self.fdtd.eval("EM.addparameter(\"lambda\", lam, \"f\", f);")
+        self.fdtd.eval("EM.addattribute(\"E\", Ex, Ey, Ez);")
+        if (type(H) != type(None)):
+            self.fdtd.putv("Hx", H[:, :, :, :, 0])
+            self.fdtd.putv("Hy", H[:, :, :, :, 1])
+            self.fdtd.putv("Hz", H[:, :, :, :, 2])
+            self.fdtd.eval("EM.addattribute(\"H\", Hx, Hy, Hz);")
+        self.fdtd.eval("importdataset(EM);")
```

### Comparing `SPLayout-0.5.2/splayout/lumericalcommun/modeapi.py` & `splayout-0.5.3/splayout/lumericalcommun/modeapi.py`

 * *Files identical despite different names*

### Comparing `SPLayout-0.5.2/splayout/utils/utils.py` & `splayout-0.5.3/splayout/utils/utils.py`

 * *Files identical despite different names*

