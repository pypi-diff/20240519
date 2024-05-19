# Comparing `tmp/h3-4.0.0b4.tar.gz` & `tmp/h3-4.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3-4.0.0b4.tar", last modified: Sun Apr 14 17:44:12 2024, max compression
+gzip compressed data, was "h3-4.0.0b5.tar", last modified: Sun May 19 17:00:49 2024, max compression
```

## Comparing `h3-4.0.0b4.tar` & `h3-4.0.0b5.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-14 17:44:03.000000 h3-4.0.0b4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-14 17:44:03.000000 h3-4.0.0b4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 17:44:03.000000 h3-4.0.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-14 17:44:12.255481 h3-4.0.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-14 17:44:03.000000 h3-4.0.0b4/makefile
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 17:44:03.000000 h3-4.0.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-14 17:44:03.000000 h3-4.0.0b4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 17:44:03.000000 h3-4.0.0b4/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:44:12.255481 h3-4.0.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-14 17:44:03.000000 h3-4.0.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/h3/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/_cy/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/cells.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/cells.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/edges.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/edges.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/error_system.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/error_system.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/h3lib.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/latlng.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/latlng.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/memory.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/memory.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/to_multipoly.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/util.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/util.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_h3shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/api/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/api/basic_int/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_int/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/api/basic_str/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_str/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_str/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3/api/memview_int/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/memview_int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/memview_int/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3/api/numpy_int/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/numpy_int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/numpy_int/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/src/h3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3lib/
--rw-r--r--   0 runner    (1001) docker     (127)    24480 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3lib/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/cmake/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/cmake/TestWrapValgrind.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/cmake/toolchain.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/h3lib/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/h3lib/src/h3lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.251481 h3-4.0.0b4/src/h3lib/src/h3lib/include/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/algos.h
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/baseCells.h
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/bbox.h
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/coordijk.h
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/directedEdge.h
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/faceijk.h
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/h3Index.h
--rw-r--r--   0 runner    (1001) docker     (127)    24086 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/h3api.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/iterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/latLng.h
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/linkedGeo.h
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/localij.h
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/mathExtensions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/polygon.h
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/polygonAlgos.h
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vec2d.h
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vec3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vertexGraph.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/src/h3lib/src/h3lib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    44976 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/algos.c
--rw-r--r--   0 runner    (1001) docker     (127)    37631 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/baseCells.c
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/bbox.c
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/coordijk.c
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/directedEdge.c
--rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/faceijk.c
--rw-r--r--   0 runner    (1001) docker     (127)    36580 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/h3Index.c
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/iterators.c
--rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/latLng.c
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/linkedGeo.c
--rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/localij.c
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/mathExtensions.c
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/polygon.c
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec2d.c
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec3d.c
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertex.c
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertexGraph.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16108 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_cells_and_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_h3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_length_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.261967 h3-4.0.0b5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-19 17:00:37.000000 h3-4.0.0b5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 17:00:37.000000 h3-4.0.0b5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 17:00:37.000000 h3-4.0.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-19 17:00:49.261967 h3-4.0.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-19 17:00:37.000000 h3-4.0.0b5/makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 17:00:37.000000 h3-4.0.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-19 17:00:37.000000 h3-4.0.0b5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-19 17:00:37.000000 h3-4.0.0b5/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:00:49.261967 h3-4.0.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-19 17:00:37.000000 h3-4.0.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.241967 h3-4.0.0b5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.245967 h3-4.0.0b5/src/h3/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3/_cy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/cells.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/cells.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/edges.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/edges.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/error_system.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/error_system.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/h3lib.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/latlng.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/latlng.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/memory.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/memory.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/to_multipoly.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_cy/util.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_h3shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3/api/basic_int/
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/basic_int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/basic_int/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3/api/basic_str/
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/basic_str/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/basic_str/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3/api/memview_int/
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/memview_int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/memview_int/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3/api/numpy_int/
+-rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/numpy_int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-19 17:00:37.000000 h3-4.0.0b5/src/h3/api/numpy_int/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.257967 h3-4.0.0b5/src/h3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-19 17:00:49.000000 h3-4.0.0b5/src/h3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-19 17:00:49.000000 h3-4.0.0b5/src/h3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:00:49.000000 h3-4.0.0b5/src/h3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-19 17:00:49.000000 h3-4.0.0b5/src/h3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-19 17:00:49.000000 h3-4.0.0b5/src/h3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.249967 h3-4.0.0b5/src/h3lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    24480 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.253967 h3-4.0.0b5/src/h3lib/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/cmake/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/cmake/TestWrapValgrind.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/cmake/toolchain.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.245967 h3-4.0.0b5/src/h3lib/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.245967 h3-4.0.0b5/src/h3lib/src/h3lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.253967 h3-4.0.0b5/src/h3lib/src/h3lib/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/algos.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/baseCells.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/bbox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/coordijk.h
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/directedEdge.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/faceijk.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/h3Index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24086 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/h3api.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/iterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/latLng.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/linkedGeo.h
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/localij.h
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/mathExtensions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/polygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/polygonAlgos.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/vec2d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/vec3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/vertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/include/vertexGraph.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.257967 h3-4.0.0b5/src/h3lib/src/h3lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    44976 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/algos.c
+-rw-r--r--   0 runner    (1001) docker     (127)    37631 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/baseCells.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/bbox.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/coordijk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/directedEdge.c
+-rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/faceijk.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36580 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/h3Index.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/iterators.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/latLng.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/linkedGeo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/localij.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/mathExtensions.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/polygon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/vec2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/vec3d.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/vertex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-05-19 17:00:42.000000 h3-4.0.0b5/src/h3lib/src/h3lib/lib/vertexGraph.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:00:49.257967 h3-4.0.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16112 2024-05-19 17:00:37.000000 h3-4.0.0b5/tests/test_cells_and_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-19 17:00:37.000000 h3-4.0.0b5/tests/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-05-19 17:00:37.000000 h3-4.0.0b5/tests/test_h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-19 17:00:37.000000 h3-4.0.0b5/tests/test_length_area.py
```

### Comparing `h3-4.0.0b4/CHANGELOG.md` & `h3-4.0.0b5/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 avoid adding features or APIs which do not map onto the
 [H3 core API](https://uber.github.io/h3/#/documentation/api-reference/).
 
 ## Unreleased
 
 - None
 
+## [4.0.0b5] - 2024-05-19
+
+- Rename `H3Poly` and `H3MultiPoly` to `LatLngPoly` and `LatLngMultiPoly` (#364)
+- Add ability to convert from `__geo_interface__` objects with Z-coordinate (#371)
+
 ## [4.0.0b4] - 2024-04-14
 
 No changes, just testing: #360
 
 ## [4.0.0b3] - 2024-03-11
 
 - Change supported Python versions to 3.7, 3.8, 3.9, 3.10, 3.11, 3.12 (#324, #325, #347, #348)
 - New `h3.Polygon()`/GeoJSON interface (#301)
 - Use functions instead of methods for the interface functions (#334)
 - Use `list` instead of `set` for unordered Python outputs (#339)
 
-
 ## [4.0.0b2] - 2022-11-23
 
 - Build Python 3.11 wheels (#297)
 
 ## [4.0.0b1] - 2022-08-23
 
 Beta release; feedback welcome!
```

### Comparing `h3-4.0.0b4/CMakeLists.txt` & `h3-4.0.0b5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/LICENSE` & `h3-4.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/PKG-INFO` & `h3-4.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h3
-Version: 4.0.0b4
+Version: 4.0.0b5
 Summary: Hierarchical hexagonal geospatial indexing system
 Home-page: https://github.com/uber/h3-py
 Author: Uber Technologies
 Author-email: AJ Friend <ajfriend@gmail.com>
 License: Apache 2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `h3-4.0.0b4/makefile` & `h3-4.0.0b5/makefile`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 	./env/bin/pip install .[all]
 	./env/bin/pip install -r requirements.in
 
 clear:
 	-./env/bin/pip uninstall -y h3
 	-@rm -rf MANIFEST
 	-@rm -rf annotations
-	-@rm -rf .pytest_cache _skbuild dist .coverage build
+	-@rm -rf .pytest_cache _skbuild dist .coverage build docs/_build
 	-@find . -type d -name '__pycache__' | xargs rm -r
 	-@find . -type d -name '*.egg-info' | xargs rm -r
 	-@find . -type f -name '*.pyc' | xargs rm -r
 	-@find . -type f -name '*.so' | xargs rm -r
 	-@find . -type d -name '*.ipynb_checkpoints' | xargs rm -r
 	-@find ./tests -type f -name '*.c' | xargs rm -r
```

### Comparing `h3-4.0.0b4/readme.md` & `h3-4.0.0b5/readme.md`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/setup.py` & `h3-4.0.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/__init__.py` & `h3-4.0.0b5/src/h3/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/CMakeLists.txt` & `h3-4.0.0b5/src/h3/_cy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/__init__.py` & `h3-4.0.0b5/src/h3/_cy/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/cells.pxd` & `h3-4.0.0b5/src/h3/_cy/cells.pxd`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/cells.pyx` & `h3-4.0.0b5/src/h3/_cy/cells.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/edges.pxd` & `h3-4.0.0b5/src/h3/_cy/edges.pxd`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/edges.pyx` & `h3-4.0.0b5/src/h3/_cy/edges.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/error_system.pyx` & `h3-4.0.0b5/src/h3/_cy/error_system.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/h3lib.pxd` & `h3-4.0.0b5/src/h3/_cy/h3lib.pxd`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/latlng.pyx` & `h3-4.0.0b5/src/h3/_cy/latlng.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/memory.pyx` & `h3-4.0.0b5/src/h3/_cy/memory.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/to_multipoly.pyx` & `h3-4.0.0b5/src/h3/_cy/to_multipoly.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_cy/util.pyx` & `h3-4.0.0b5/src/h3/_cy/util.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3/_h3shape.py` & `h3-4.0.0b5/src/h3/_h3shape.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,87 +1,95 @@
 from abc import ABCMeta, abstractmethod
 
 
 class H3Shape(metaclass=ABCMeta):
+    """
+    Abstract parent class of ``LatLngPoly`` and ``LatLngMultiPoly``.
+    """
     @property
     @abstractmethod
     def __geo_interface__(self):
         """ https://github.com/pytest-dev/pytest-cov/issues/428 """
 
 
-class H3Poly(H3Shape):
+class LatLngPoly(H3Shape):
     """
-    Container for loops of lat/lng points describing a polygon.
+    Container for loops of lat/lng points describing a polygon, possibly with holes.
 
     Attributes
     ----------
     outer : list[tuple[float, float]]
         List of lat/lng points describing the outer loop of the polygon
 
     holes : list[list[tuple[float, float]]]
         List of loops of lat/lng points describing the holes of the polygon
 
     Examples
     --------
 
     A polygon with a single outer ring consisting of 4 points, having no holes:
 
-    >>> H3Poly(
+    >>> LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34), (37.82, -122.54)],
     ... )
-    <H3Poly: [4]>
+    <LatLngPoly: [4]>
 
     The same polygon, but with one hole consisting of 3 points:
 
-    >>> H3Poly(
+    >>> LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34), (37.82, -122.54)],
     ...     [(37.76, -122.51), (37.76, -122.44), (37.81, -122.51)],
     ... )
-    <H3Poly: [4/(3,)]>
+    <LatLngPoly: [4/(3,)]>
 
     The same as above, but with one additional hole, made up of 5 points:
 
-    >>> H3Poly(
+    >>> LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34), (37.82, -122.54)],
     ...     [(37.76, -122.51), (37.76, -122.44), (37.81, -122.51)],
     ...     [(37.71, -122.43), (37.71, -122.37), (37.73, -122.37), (37.75, -122.41),
     ...      (37.73, -122.43)],
     ... )
-    <H3Poly: [4/(3, 5)]>
+    <LatLngPoly: [4/(3, 5)]>
     """
     def __init__(self, outer, *holes):
         loops = [outer] + list(holes)
         for loop in loops:
             if len(loop) in (1, 2):
-                raise ValueError('Non-empty H3Poly loops need at least 3 points.')
+                raise ValueError('Non-empty LatLngPoly loops need at least 3 points.')
+
+            point_dimensions = set(map(len, loop))
+            # empty set is possible for empty polygons, so we check if a subset
+            if not (point_dimensions <= {2}):
+                raise ValueError('LatLngPoly only accepts 2D points: lat/lng.')
 
         self.outer = tuple(_open_ring(outer))
         self.holes = tuple(
             _open_ring(hole)
             for hole in holes
         )
 
     def __repr__(self):
-        return '<H3Poly: {}>'.format(self.loopcode)
+        return '<LatLngPoly: {}>'.format(self.loopcode)
 
     def __len__(self):
         """
         Should this be the number of points in the outer loop,
         the number of holes (or +1 for the outer loop)?
         """
-        raise NotImplementedError('No clear definition of length for H3Poly.')
+        raise NotImplementedError('No clear definition of length for LatLngPoly.')
 
     @property
     def loopcode(self):
         """ Short code for describing the length of the outer loop and each hole
 
-        Example: `[382/(18, 6, 6)]` indicates an outer loop of 382 points,
+        Example: ``[382/(18, 6, 6)]`` indicates an outer loop of 382 points,
         along with 3 holes with 18, 6, and 6 points, respectively.
 
-        Example: `[15]` indicates an outer loop of 15 points and no holes.
+        Example: ``[15]`` indicates an outer loop of 15 points and no holes.
         """
         outer = len(self.outer)
         holes = tuple(map(len, self.holes))
 
         outer = str(outer)
 
         if holes:
@@ -95,57 +103,66 @@
     def __geo_interface__(self):
         ll2 = _polygon_to_LL2(self)
         gj_dict = _LL2_to_geojson_dict(ll2)
 
         return gj_dict
 
 
-class H3MultiPoly(H3Shape):
+class LatLngMultiPoly(H3Shape):
+    """
+    Container for multiple ``LatLngPoly`` polygons.
+
+    Attributes
+    ----------
+    polys : list[LatLngPoly]
+        List of lat/lng points describing the outer loop of the polygon
+    """
     def __init__(self, *polys):
         self.polys = tuple(polys)
 
         for p in self.polys:
-            if not isinstance(p, H3Poly):
-                raise ValueError('H3MultiPoly requires each input to be an H3Poly object, instead got: ' + str(p)) # noqa
+            if not isinstance(p, LatLngPoly):
+                raise ValueError('LatLngMultiPoly requires each input to be an LatLngPoly object, instead got: ' + str(p)) # noqa
 
     def __repr__(self):
         out = [p.loopcode for p in self.polys]
         out = ', '.join(out)
-        out = '<H3MultiPoly: {}>'.format(out)
+        out = '<LatLngMultiPoly: {}>'.format(out)
         return out
 
     def __iter__(self):
         return iter(self.polys)
 
     def __len__(self):
         """ Give the number of polygons in this multi-polygon.
         """
 
         """
         TODO: Pandas series or dataframe representation changes depending
         on if __len__ is defined.
 
-        I'd prefer the one that states `H3MultiPoly`. It seems like Pandas is assuming
-        an iterable is best-described by its elements when choosing the representation.
+        I'd prefer the one that states `LatLngMultiPoly`.
+        It seems like Pandas is assuming an iterable is best-described
+        by its elements when choosing the representation.
 
         when __len__ *IS NOT* defined:
 
-        0                      <H3MultiPoly: [368], [20], [6]>
-        1    <H3MultiPoly: [632/(6, 6, 6, 6, 6)], [290/(6,)...
-        2    <H3MultiPoly: [490/(6, 6, 10, 10, 14, 10, 6)],...
-        3    <H3MultiPoly: [344/(6,)], [22], [6], [10], [6]...
-        4    <H3MultiPoly: [382/(18, 6, 6)], [32], [6], [18...
+        0                      <LatLngMultiPoly: [368], [20], [6]>
+        1    <LatLngMultiPoly: [632/(6, 6, 6, 6, 6)], [290/(6,)...
+        2    <LatLngMultiPoly: [490/(6, 6, 10, 10, 14, 10, 6)],...
+        3    <LatLngMultiPoly: [344/(6,)], [22], [6], [10], [6]...
+        4    <LatLngMultiPoly: [382/(18, 6, 6)], [32], [6], [18...
 
         when __len__ *IS* defined:
 
-        0     (<H3Poly: [368]>, <H3Poly: [20]>, <H3Poly: [6]>)
-        1    (<H3Poly: [632/(6, 6, 6, 6, 6)]>, <H3Poly: [29...
-        2    (<H3Poly: [490/(6, 6, 10, 10, 14, 10, 6)]>, <H...
-        3    (<H3Poly: [344/(6,)]>, <H3Poly: [22]>, <H3Poly...
-        4    (<H3Poly: [382/(18, 6, 6)]>, <H3Poly: [32]>, <...
+        0     (<LatLngPoly: [368]>, <LatLngPoly: [20]>, <LatLngPoly: [6]>)
+        1    (<LatLngPoly: [632/(6, 6, 6, 6, 6)]>, <LatLngPoly: [29...
+        2    (<LatLngPoly: [490/(6, 6, 10, 10, 14, 10, 6)]>, <H...
+        3    (<LatLngPoly: [344/(6,)]>, <LatLngPoly: [22]>, <LatLngPoly...
+        4    (<LatLngPoly: [382/(18, 6, 6)]>, <LatLngPoly: [32]>, <...
         """
         return len(self.polys)
 
     def __getitem__(self, index):
         return self.polys[index]
 
     @property
@@ -188,35 +205,45 @@
 
 def _LL3_to_mpoly(ll3):
     polys = [
         _LL2_to_polygon(ll2)
         for ll2 in ll3
     ]
 
-    mpoly = H3MultiPoly(*polys)
+    mpoly = LatLngMultiPoly(*polys)
 
     return mpoly
 
 
-def _polygon_to_LL2(h3poly):
-    ll2 = [h3poly.outer] + list(h3poly.holes)
+def _polygon_to_LL2(poly):
+    ll2 = [poly.outer] + list(poly.holes)
     ll2 = tuple(
         _close_ring(_swap_latlng(ll1))
         for ll1 in ll2
     )
 
     return ll2
 
 
+def _remove_z(ll1):
+    ll1 = [(a, b) for a, b, *z in ll1]
+    return ll1
+
+
 def _LL2_to_polygon(ll2):
     ll2 = [
+        _remove_z(ll1)
+        for ll1 in ll2
+    ]
+
+    ll2 = [
         _swap_latlng(ll1)
         for ll1 in ll2
     ]
-    h3poly = H3Poly(*ll2)
+    h3poly = LatLngPoly(*ll2)
 
     return h3poly
 
 
 def _LL2_to_geojson_dict(ll2):
     gj_dict = {
         'type': 'Polygon',
@@ -260,52 +287,52 @@
         ll1 = ll1[:-1]
 
     return ll1
 
 
 def geo_to_h3shape(geo):
     """
-    Translate from __geo_interface__ to H3Shape.
+    Translate from ``__geo_interface__`` to H3Shape.
 
-    `geo` either implements `__geo_interface__` or is a dict matching the format
+    ``geo`` either implements ``__geo_interface__`` or is a dict matching the format
 
     Returns
     -------
     H3Shape
     """
 
-    # geo can be dict, a __geo_interface__, a string, H3Poly or H3MultiPoly
+    # geo can be dict, a __geo_interface__, a string, LatLngPoly or LatLngMultiPoly
     if isinstance(geo, H3Shape):
         return geo
 
     if hasattr(geo, '__geo_interface__'):
         # get dict
         geo = geo.__geo_interface__
 
     assert isinstance(geo, dict)  # todo: remove
 
     t = geo['type']
     coord = geo['coordinates']
 
     if t == 'Polygon':
         ll2 = coord
-        h3shape = _LL2_to_polygon(ll2)
+        shape = _LL2_to_polygon(ll2)
     elif t == 'MultiPolygon':
         ll3 = coord
-        h3shape = _LL3_to_mpoly(ll3)
+        shape = _LL3_to_mpoly(ll3)
     else:
         raise ValueError('Unrecognized type: ' + str(t))
 
-    return h3shape
+    return shape
 
 
 def h3shape_to_geo(h3shape):
     """
-    Translate from H3Shape to a __geo_interface__ dict.
+    Translate from an ``H3Shape`` to a ``__geo_interface__`` dict.
 
-    `h3shape` should be either H3Poly or H3MultiPoly
+    ``h3shape`` should be either ``LatLngPoly`` or ``LatLngMultiPoly``
 
     Returns
     -------
     dict
     """
     return h3shape.__geo_interface__
```

### Comparing `h3-4.0.0b4/src/h3/_version.py` & `h3-4.0.0b5/src/h3/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '4.0.0b4'
+__version__ = '4.0.0b5'
 __description__ = 'Hierarchical hexagonal geospatial indexing system'
 __url__ = 'https://github.com/uber/h3-py'
 __license__ = 'Apache 2.0 License'
 __author__ = 'Uber Technologies'
 __author_email__ = 'AJ Friend <ajfriend@gmail.com>'
 __classifiers__ = [
     'Development Status :: 5 - Production/Stable',
```

### Comparing `h3-4.0.0b4/src/h3/api/basic_int/__init__.py` & `h3-4.0.0b5/src/h3/api/basic_int/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is **symlinked** across the APIs to ensure they are exactly the same.
 
 from ... import _cy
 from ..._h3shape import (
     H3Shape,
-    H3Poly,
-    H3MultiPoly,
+    LatLngPoly,
+    LatLngMultiPoly,
     geo_to_h3shape,
     h3shape_to_geo,
 )
 
 from ._convert import (
     _in_scalar,
     _out_scalar,
@@ -88,28 +88,42 @@
 def average_hexagon_area(res, unit='km^2'):
     """
     Return the average area of an H3 *hexagon*
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_area(res, unit)
 
 
 def average_hexagon_edge_length(res, unit='km'):
     """
     Return the average *hexagon* edge length
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_edge_length(res, unit)
 
 
@@ -210,17 +224,17 @@
     p = _out_scalar(p)
 
     return p
 
 
 def grid_distance(h1, h2):
     """
-    Compute the H3 distance between two cells.
+    Compute the grid distance between two cells.
 
-    The H3 distance is defined as the length of the shortest
+    The grid distance is defined as the length of the shortest
     path between the cells in the graph formed by connecting
     adjacent cells.
 
     This function will raise an exception if the
     cells are too far apart to compute the distance.
 
     Parameters
@@ -253,16 +267,16 @@
     tuple of (lat, lng) tuples
     """
     return _cy.cell_to_boundary(_in_scalar(h))
 
 
 def grid_disk(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``<= k`` from ``h``.
-    That is, the 'filled-in' disk.
+    Return unordered collection of cells with grid distance ``<= k`` from ``h``.
+    That is, the "filled-in" disk.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of disk.
 
@@ -277,15 +291,15 @@
     mv = _cy.grid_disk(_in_scalar(h), k)
 
     return _out_collection(mv)
 
 
 def grid_ring(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``== k`` from ``h``.
+    Return unordered collection of cells with grid distance ``== k`` from ``h``.
     That is, the "hollow" ring.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of ring.
@@ -342,162 +356,165 @@
     -------
     unordered collection of H3Cell
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
-    # todo: does compact_cells work on mixed-resolution collections?
     hu = _in_collection(cells)
     hc = _cy.compact_cells(hu)
 
     return _out_collection(hc)
 
 
 def uncompact_cells(cells, res):
     """
-    Reverse the `compact_cells` operation.
+    Reverse the ``compact_cells`` operation.
 
     Return a collection of H3 cells, all of resolution ``res``.
 
     Parameters
     ----------
     cells : iterable of H3Cell
     res : int
         Resolution of desired output cells.
 
     Returns
     -------
     unordered collection of H3Cell
 
-    Raises
-    ------
-    todo: add test to make sure an error is returned when input
-    contains cell smaller than output res.
-    https://github.com/uber/h3/blob/master/src/h3lib/lib/h3Index.c#L425
-
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
+    # TODO: add test to make sure an error is returned when input contains cell
+    # smaller than output res.
+
     hc = _in_collection(cells)
     hu = _cy.uncompact_cells(hc, res)
 
     return _out_collection(hu)
 
 
 def h3shape_to_cells(h3shape, res):
     """
-    Return the set of H3 cells at a given resolution whose center points
-    are contained within an `H3Poly` or `H3MultiPoly`.
+    Return the collection of H3 cells at a given resolution whose center points
+    are contained within an ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
-    h3shape : H3shape
+    h3shape : ``H3Shape``
     res : int
         Resolution of the output cells
 
     Returns
     -------
-    unordered collection of H3Cell
+    list of H3Cell
 
     Examples
     --------
 
-    >>> poly = H3Poly(
+    >>> poly = LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34),
     ...      (37.82, -122.54)],
     ... )
     >>> h3.h3shape_to_cells(poly, 6)
-    {'862830807ffffff',
+    ['862830807ffffff',
      '862830827ffffff',
      '86283082fffffff',
      '862830877ffffff',
      '862830947ffffff',
      '862830957ffffff',
-     '86283095fffffff'}
+     '86283095fffffff']
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
 
     # todo: not sure if i want this dispatch logic here. maybe in the objects?
-    if isinstance(h3shape, H3Poly):
+    if isinstance(h3shape, LatLngPoly):
         poly = h3shape
         mv = _cy.polygon_to_cells(poly.outer, res, holes=poly.holes)
-    elif isinstance(h3shape, H3MultiPoly):
+    elif isinstance(h3shape, LatLngMultiPoly):
         mpoly = h3shape
         mv = _cy.polygons_to_cells(mpoly.polys, res)
     elif isinstance(h3shape, H3Shape):
         raise ValueError('Unrecognized H3Shape: ' + str(h3shape))
     else:
         raise ValueError('Unrecognized type: ' + str(type(h3shape)))
 
     return _out_collection(mv)
 
 
-def cells_to_h3shape(cells, tight=True):
+def cells_to_h3shape(cells, *, tight=True):
     """
-    Return a H3MultiPoly describing the area covered by a set of H3 cells.
+    Return an ``H3Shape`` describing the area covered by a collection of H3 cells.
+    Will return ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
     cells : iterable of H3 cells
     tight : bool
-        If True, return H3Poly if possible. If False, always return H3MultiPoly
+        If True, return ``LatLngPoly`` if possible.
+        If False, always return ``LatLngMultiPoly``.
 
     Returns
     -------
-    H3Poly | H3MultiPoly
+    LatLngPoly | LatLngMultiPoly
 
     Examples
     --------
 
     >>> cells = ['8428309ffffffff', '842830dffffffff']
     >>> h3.cells_to_h3shape(cells, tight=True)
-    <H3Poly: [10]>
+    <LatLngPoly: [10]>
     >>> h3.cells_to_h3shape(cells, tight=False)
-    <H3MultiPoly: [10]>
+    <LatLngMultiPoly: [10]>
     """
     cells = _in_collection(cells)
     mpoly = _cy.cells_to_multi_polygon(cells)
 
-    polys = [H3Poly(*poly) for poly in mpoly]
-    out = H3MultiPoly(*polys)
+    polys = [LatLngPoly(*poly) for poly in mpoly]
+    out = LatLngMultiPoly(*polys)
 
     if tight and len(out) == 1:
         out = out[0]
 
     return out
 
 
 def geo_to_cells(geo, res):
-    """Convert from __geo_interface__ to cells.
+    """Convert from ``__geo_interface__`` to cells.
 
     Parameters
     ----------
-    geo : an object implementing `__geo_interface__` or a dictionary in that format.
-        Both H3Poly and H3MultiPoly implement the interface.
+    geo : an object implementing ``__geo_interface__`` or a dictionary in that format.
+        Both ``LatLngPoly`` and ``LatLngMultiPoly`` implement the interface.
     res : int
         Resolution of desired output cells.
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
     h3shape = geo_to_h3shape(geo)
     return h3shape_to_cells(h3shape, res)
 
 
 def cells_to_geo(cells, tight=True):
     """
+    Convert from cells to a ``__geo_interface__`` dict.
+
     Parameters
     ----------
     cells : iterable of H3 Cells
+    tight : bool
+        When ``True``, returns an ``LatLngPoly`` when possible.
+        When ``False``, always returns an ``LatLngMultiPoly``.
 
     Returns
     -------
     dict
         in `__geo_interface__` format
     """
     h3shape = cells_to_h3shape(cells, tight=tight)
@@ -670,14 +687,26 @@
     """
     mv = _cy.origin_to_directed_edges(_in_scalar(origin))
 
     return _out_collection(mv)
 
 
 def directed_edge_to_boundary(edge):
+    """
+    Returns points representing the edge (line of points
+    describing the boundary between two cells).
+
+    Parameters
+    ----------
+    edge : H3Edge
+
+    Returns
+    -------
+    tuple of (lat, lng) tuples
+    """
     return _cy.directed_edge_to_boundary(_in_scalar(edge))
 
 
 def grid_path_cells(start, end):
     """
     Returns the ordered collection of cells denoting a
     minimum-length non-unique path between cells.
@@ -890,54 +919,54 @@
     """
     Compute the spherical surface area of a specific H3 cell.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for area result (``'km^2'``, 'm^2', or 'rads^2')
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
 
 
     Returns
     -------
     The area of the H3 cell in the given units
 
 
     Notes
     -----
     This function breaks the cell into spherical triangles, and computes
     their spherical area.
     The function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     h = _in_scalar(h)
 
     return _cy.cell_area(h, unit=unit)
 
 
 def edge_length(e, unit='km'):
     """
     Compute the spherical length of a specific H3 edge.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for length result ('km', 'm', or 'rads')
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
 
 
     Returns
     -------
     The length of the edge in the given units
 
 
     Notes
     -----
     This function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     e = _in_scalar(e)
 
     return _cy.edge_length(e, unit=unit)
 
 
 def great_circle_distance(latlng1, latlng2, unit='km'):
@@ -950,16 +979,15 @@
     Parameters
     ----------
     latlng1 : tuple
         (lat, lng) tuple in degrees
     latlng2 : tuple
         (lat, lng) tuple in degrees
     unit: str
-        Unit for distance result ('km', 'm', or 'rads')
-
+        Unit for distance result (``'km'``, ``'m'``, or ``'rads'``)
 
     Returns
     -------
     The spherical distance between the points in the given units
     """
     lat1, lng1 = latlng1
     lat2, lng2 = latlng2
```

### Comparing `h3-4.0.0b4/src/h3/api/basic_str/__init__.py` & `h3-4.0.0b5/src/h3/api/basic_str/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is **symlinked** across the APIs to ensure they are exactly the same.
 
 from ... import _cy
 from ..._h3shape import (
     H3Shape,
-    H3Poly,
-    H3MultiPoly,
+    LatLngPoly,
+    LatLngMultiPoly,
     geo_to_h3shape,
     h3shape_to_geo,
 )
 
 from ._convert import (
     _in_scalar,
     _out_scalar,
@@ -88,28 +88,42 @@
 def average_hexagon_area(res, unit='km^2'):
     """
     Return the average area of an H3 *hexagon*
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_area(res, unit)
 
 
 def average_hexagon_edge_length(res, unit='km'):
     """
     Return the average *hexagon* edge length
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_edge_length(res, unit)
 
 
@@ -210,17 +224,17 @@
     p = _out_scalar(p)
 
     return p
 
 
 def grid_distance(h1, h2):
     """
-    Compute the H3 distance between two cells.
+    Compute the grid distance between two cells.
 
-    The H3 distance is defined as the length of the shortest
+    The grid distance is defined as the length of the shortest
     path between the cells in the graph formed by connecting
     adjacent cells.
 
     This function will raise an exception if the
     cells are too far apart to compute the distance.
 
     Parameters
@@ -253,16 +267,16 @@
     tuple of (lat, lng) tuples
     """
     return _cy.cell_to_boundary(_in_scalar(h))
 
 
 def grid_disk(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``<= k`` from ``h``.
-    That is, the 'filled-in' disk.
+    Return unordered collection of cells with grid distance ``<= k`` from ``h``.
+    That is, the "filled-in" disk.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of disk.
 
@@ -277,15 +291,15 @@
     mv = _cy.grid_disk(_in_scalar(h), k)
 
     return _out_collection(mv)
 
 
 def grid_ring(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``== k`` from ``h``.
+    Return unordered collection of cells with grid distance ``== k`` from ``h``.
     That is, the "hollow" ring.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of ring.
@@ -342,162 +356,165 @@
     -------
     unordered collection of H3Cell
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
-    # todo: does compact_cells work on mixed-resolution collections?
     hu = _in_collection(cells)
     hc = _cy.compact_cells(hu)
 
     return _out_collection(hc)
 
 
 def uncompact_cells(cells, res):
     """
-    Reverse the `compact_cells` operation.
+    Reverse the ``compact_cells`` operation.
 
     Return a collection of H3 cells, all of resolution ``res``.
 
     Parameters
     ----------
     cells : iterable of H3Cell
     res : int
         Resolution of desired output cells.
 
     Returns
     -------
     unordered collection of H3Cell
 
-    Raises
-    ------
-    todo: add test to make sure an error is returned when input
-    contains cell smaller than output res.
-    https://github.com/uber/h3/blob/master/src/h3lib/lib/h3Index.c#L425
-
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
+    # TODO: add test to make sure an error is returned when input contains cell
+    # smaller than output res.
+
     hc = _in_collection(cells)
     hu = _cy.uncompact_cells(hc, res)
 
     return _out_collection(hu)
 
 
 def h3shape_to_cells(h3shape, res):
     """
-    Return the set of H3 cells at a given resolution whose center points
-    are contained within an `H3Poly` or `H3MultiPoly`.
+    Return the collection of H3 cells at a given resolution whose center points
+    are contained within an ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
-    h3shape : H3shape
+    h3shape : ``H3Shape``
     res : int
         Resolution of the output cells
 
     Returns
     -------
-    unordered collection of H3Cell
+    list of H3Cell
 
     Examples
     --------
 
-    >>> poly = H3Poly(
+    >>> poly = LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34),
     ...      (37.82, -122.54)],
     ... )
     >>> h3.h3shape_to_cells(poly, 6)
-    {'862830807ffffff',
+    ['862830807ffffff',
      '862830827ffffff',
      '86283082fffffff',
      '862830877ffffff',
      '862830947ffffff',
      '862830957ffffff',
-     '86283095fffffff'}
+     '86283095fffffff']
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
 
     # todo: not sure if i want this dispatch logic here. maybe in the objects?
-    if isinstance(h3shape, H3Poly):
+    if isinstance(h3shape, LatLngPoly):
         poly = h3shape
         mv = _cy.polygon_to_cells(poly.outer, res, holes=poly.holes)
-    elif isinstance(h3shape, H3MultiPoly):
+    elif isinstance(h3shape, LatLngMultiPoly):
         mpoly = h3shape
         mv = _cy.polygons_to_cells(mpoly.polys, res)
     elif isinstance(h3shape, H3Shape):
         raise ValueError('Unrecognized H3Shape: ' + str(h3shape))
     else:
         raise ValueError('Unrecognized type: ' + str(type(h3shape)))
 
     return _out_collection(mv)
 
 
-def cells_to_h3shape(cells, tight=True):
+def cells_to_h3shape(cells, *, tight=True):
     """
-    Return a H3MultiPoly describing the area covered by a set of H3 cells.
+    Return an ``H3Shape`` describing the area covered by a collection of H3 cells.
+    Will return ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
     cells : iterable of H3 cells
     tight : bool
-        If True, return H3Poly if possible. If False, always return H3MultiPoly
+        If True, return ``LatLngPoly`` if possible.
+        If False, always return ``LatLngMultiPoly``.
 
     Returns
     -------
-    H3Poly | H3MultiPoly
+    LatLngPoly | LatLngMultiPoly
 
     Examples
     --------
 
     >>> cells = ['8428309ffffffff', '842830dffffffff']
     >>> h3.cells_to_h3shape(cells, tight=True)
-    <H3Poly: [10]>
+    <LatLngPoly: [10]>
     >>> h3.cells_to_h3shape(cells, tight=False)
-    <H3MultiPoly: [10]>
+    <LatLngMultiPoly: [10]>
     """
     cells = _in_collection(cells)
     mpoly = _cy.cells_to_multi_polygon(cells)
 
-    polys = [H3Poly(*poly) for poly in mpoly]
-    out = H3MultiPoly(*polys)
+    polys = [LatLngPoly(*poly) for poly in mpoly]
+    out = LatLngMultiPoly(*polys)
 
     if tight and len(out) == 1:
         out = out[0]
 
     return out
 
 
 def geo_to_cells(geo, res):
-    """Convert from __geo_interface__ to cells.
+    """Convert from ``__geo_interface__`` to cells.
 
     Parameters
     ----------
-    geo : an object implementing `__geo_interface__` or a dictionary in that format.
-        Both H3Poly and H3MultiPoly implement the interface.
+    geo : an object implementing ``__geo_interface__`` or a dictionary in that format.
+        Both ``LatLngPoly`` and ``LatLngMultiPoly`` implement the interface.
     res : int
         Resolution of desired output cells.
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
     h3shape = geo_to_h3shape(geo)
     return h3shape_to_cells(h3shape, res)
 
 
 def cells_to_geo(cells, tight=True):
     """
+    Convert from cells to a ``__geo_interface__`` dict.
+
     Parameters
     ----------
     cells : iterable of H3 Cells
+    tight : bool
+        When ``True``, returns an ``LatLngPoly`` when possible.
+        When ``False``, always returns an ``LatLngMultiPoly``.
 
     Returns
     -------
     dict
         in `__geo_interface__` format
     """
     h3shape = cells_to_h3shape(cells, tight=tight)
@@ -670,14 +687,26 @@
     """
     mv = _cy.origin_to_directed_edges(_in_scalar(origin))
 
     return _out_collection(mv)
 
 
 def directed_edge_to_boundary(edge):
+    """
+    Returns points representing the edge (line of points
+    describing the boundary between two cells).
+
+    Parameters
+    ----------
+    edge : H3Edge
+
+    Returns
+    -------
+    tuple of (lat, lng) tuples
+    """
     return _cy.directed_edge_to_boundary(_in_scalar(edge))
 
 
 def grid_path_cells(start, end):
     """
     Returns the ordered collection of cells denoting a
     minimum-length non-unique path between cells.
@@ -890,54 +919,54 @@
     """
     Compute the spherical surface area of a specific H3 cell.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for area result (``'km^2'``, 'm^2', or 'rads^2')
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
 
 
     Returns
     -------
     The area of the H3 cell in the given units
 
 
     Notes
     -----
     This function breaks the cell into spherical triangles, and computes
     their spherical area.
     The function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     h = _in_scalar(h)
 
     return _cy.cell_area(h, unit=unit)
 
 
 def edge_length(e, unit='km'):
     """
     Compute the spherical length of a specific H3 edge.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for length result ('km', 'm', or 'rads')
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
 
 
     Returns
     -------
     The length of the edge in the given units
 
 
     Notes
     -----
     This function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     e = _in_scalar(e)
 
     return _cy.edge_length(e, unit=unit)
 
 
 def great_circle_distance(latlng1, latlng2, unit='km'):
@@ -950,16 +979,15 @@
     Parameters
     ----------
     latlng1 : tuple
         (lat, lng) tuple in degrees
     latlng2 : tuple
         (lat, lng) tuple in degrees
     unit: str
-        Unit for distance result ('km', 'm', or 'rads')
-
+        Unit for distance result (``'km'``, ``'m'``, or ``'rads'``)
 
     Returns
     -------
     The spherical distance between the points in the given units
     """
     lat1, lng1 = latlng1
     lat2, lng2 = latlng2
```

### Comparing `h3-4.0.0b4/src/h3/api/memview_int/__init__.py` & `h3-4.0.0b5/src/h3/api/memview_int/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is **symlinked** across the APIs to ensure they are exactly the same.
 
 from ... import _cy
 from ..._h3shape import (
     H3Shape,
-    H3Poly,
-    H3MultiPoly,
+    LatLngPoly,
+    LatLngMultiPoly,
     geo_to_h3shape,
     h3shape_to_geo,
 )
 
 from ._convert import (
     _in_scalar,
     _out_scalar,
@@ -88,28 +88,42 @@
 def average_hexagon_area(res, unit='km^2'):
     """
     Return the average area of an H3 *hexagon*
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_area(res, unit)
 
 
 def average_hexagon_edge_length(res, unit='km'):
     """
     Return the average *hexagon* edge length
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_edge_length(res, unit)
 
 
@@ -210,17 +224,17 @@
     p = _out_scalar(p)
 
     return p
 
 
 def grid_distance(h1, h2):
     """
-    Compute the H3 distance between two cells.
+    Compute the grid distance between two cells.
 
-    The H3 distance is defined as the length of the shortest
+    The grid distance is defined as the length of the shortest
     path between the cells in the graph formed by connecting
     adjacent cells.
 
     This function will raise an exception if the
     cells are too far apart to compute the distance.
 
     Parameters
@@ -253,16 +267,16 @@
     tuple of (lat, lng) tuples
     """
     return _cy.cell_to_boundary(_in_scalar(h))
 
 
 def grid_disk(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``<= k`` from ``h``.
-    That is, the 'filled-in' disk.
+    Return unordered collection of cells with grid distance ``<= k`` from ``h``.
+    That is, the "filled-in" disk.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of disk.
 
@@ -277,15 +291,15 @@
     mv = _cy.grid_disk(_in_scalar(h), k)
 
     return _out_collection(mv)
 
 
 def grid_ring(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``== k`` from ``h``.
+    Return unordered collection of cells with grid distance ``== k`` from ``h``.
     That is, the "hollow" ring.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of ring.
@@ -342,162 +356,165 @@
     -------
     unordered collection of H3Cell
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
-    # todo: does compact_cells work on mixed-resolution collections?
     hu = _in_collection(cells)
     hc = _cy.compact_cells(hu)
 
     return _out_collection(hc)
 
 
 def uncompact_cells(cells, res):
     """
-    Reverse the `compact_cells` operation.
+    Reverse the ``compact_cells`` operation.
 
     Return a collection of H3 cells, all of resolution ``res``.
 
     Parameters
     ----------
     cells : iterable of H3Cell
     res : int
         Resolution of desired output cells.
 
     Returns
     -------
     unordered collection of H3Cell
 
-    Raises
-    ------
-    todo: add test to make sure an error is returned when input
-    contains cell smaller than output res.
-    https://github.com/uber/h3/blob/master/src/h3lib/lib/h3Index.c#L425
-
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
+    # TODO: add test to make sure an error is returned when input contains cell
+    # smaller than output res.
+
     hc = _in_collection(cells)
     hu = _cy.uncompact_cells(hc, res)
 
     return _out_collection(hu)
 
 
 def h3shape_to_cells(h3shape, res):
     """
-    Return the set of H3 cells at a given resolution whose center points
-    are contained within an `H3Poly` or `H3MultiPoly`.
+    Return the collection of H3 cells at a given resolution whose center points
+    are contained within an ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
-    h3shape : H3shape
+    h3shape : ``H3Shape``
     res : int
         Resolution of the output cells
 
     Returns
     -------
-    unordered collection of H3Cell
+    list of H3Cell
 
     Examples
     --------
 
-    >>> poly = H3Poly(
+    >>> poly = LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34),
     ...      (37.82, -122.54)],
     ... )
     >>> h3.h3shape_to_cells(poly, 6)
-    {'862830807ffffff',
+    ['862830807ffffff',
      '862830827ffffff',
      '86283082fffffff',
      '862830877ffffff',
      '862830947ffffff',
      '862830957ffffff',
-     '86283095fffffff'}
+     '86283095fffffff']
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
 
     # todo: not sure if i want this dispatch logic here. maybe in the objects?
-    if isinstance(h3shape, H3Poly):
+    if isinstance(h3shape, LatLngPoly):
         poly = h3shape
         mv = _cy.polygon_to_cells(poly.outer, res, holes=poly.holes)
-    elif isinstance(h3shape, H3MultiPoly):
+    elif isinstance(h3shape, LatLngMultiPoly):
         mpoly = h3shape
         mv = _cy.polygons_to_cells(mpoly.polys, res)
     elif isinstance(h3shape, H3Shape):
         raise ValueError('Unrecognized H3Shape: ' + str(h3shape))
     else:
         raise ValueError('Unrecognized type: ' + str(type(h3shape)))
 
     return _out_collection(mv)
 
 
-def cells_to_h3shape(cells, tight=True):
+def cells_to_h3shape(cells, *, tight=True):
     """
-    Return a H3MultiPoly describing the area covered by a set of H3 cells.
+    Return an ``H3Shape`` describing the area covered by a collection of H3 cells.
+    Will return ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
     cells : iterable of H3 cells
     tight : bool
-        If True, return H3Poly if possible. If False, always return H3MultiPoly
+        If True, return ``LatLngPoly`` if possible.
+        If False, always return ``LatLngMultiPoly``.
 
     Returns
     -------
-    H3Poly | H3MultiPoly
+    LatLngPoly | LatLngMultiPoly
 
     Examples
     --------
 
     >>> cells = ['8428309ffffffff', '842830dffffffff']
     >>> h3.cells_to_h3shape(cells, tight=True)
-    <H3Poly: [10]>
+    <LatLngPoly: [10]>
     >>> h3.cells_to_h3shape(cells, tight=False)
-    <H3MultiPoly: [10]>
+    <LatLngMultiPoly: [10]>
     """
     cells = _in_collection(cells)
     mpoly = _cy.cells_to_multi_polygon(cells)
 
-    polys = [H3Poly(*poly) for poly in mpoly]
-    out = H3MultiPoly(*polys)
+    polys = [LatLngPoly(*poly) for poly in mpoly]
+    out = LatLngMultiPoly(*polys)
 
     if tight and len(out) == 1:
         out = out[0]
 
     return out
 
 
 def geo_to_cells(geo, res):
-    """Convert from __geo_interface__ to cells.
+    """Convert from ``__geo_interface__`` to cells.
 
     Parameters
     ----------
-    geo : an object implementing `__geo_interface__` or a dictionary in that format.
-        Both H3Poly and H3MultiPoly implement the interface.
+    geo : an object implementing ``__geo_interface__`` or a dictionary in that format.
+        Both ``LatLngPoly`` and ``LatLngMultiPoly`` implement the interface.
     res : int
         Resolution of desired output cells.
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
     h3shape = geo_to_h3shape(geo)
     return h3shape_to_cells(h3shape, res)
 
 
 def cells_to_geo(cells, tight=True):
     """
+    Convert from cells to a ``__geo_interface__`` dict.
+
     Parameters
     ----------
     cells : iterable of H3 Cells
+    tight : bool
+        When ``True``, returns an ``LatLngPoly`` when possible.
+        When ``False``, always returns an ``LatLngMultiPoly``.
 
     Returns
     -------
     dict
         in `__geo_interface__` format
     """
     h3shape = cells_to_h3shape(cells, tight=tight)
@@ -670,14 +687,26 @@
     """
     mv = _cy.origin_to_directed_edges(_in_scalar(origin))
 
     return _out_collection(mv)
 
 
 def directed_edge_to_boundary(edge):
+    """
+    Returns points representing the edge (line of points
+    describing the boundary between two cells).
+
+    Parameters
+    ----------
+    edge : H3Edge
+
+    Returns
+    -------
+    tuple of (lat, lng) tuples
+    """
     return _cy.directed_edge_to_boundary(_in_scalar(edge))
 
 
 def grid_path_cells(start, end):
     """
     Returns the ordered collection of cells denoting a
     minimum-length non-unique path between cells.
@@ -890,54 +919,54 @@
     """
     Compute the spherical surface area of a specific H3 cell.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for area result (``'km^2'``, 'm^2', or 'rads^2')
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
 
 
     Returns
     -------
     The area of the H3 cell in the given units
 
 
     Notes
     -----
     This function breaks the cell into spherical triangles, and computes
     their spherical area.
     The function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     h = _in_scalar(h)
 
     return _cy.cell_area(h, unit=unit)
 
 
 def edge_length(e, unit='km'):
     """
     Compute the spherical length of a specific H3 edge.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for length result ('km', 'm', or 'rads')
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
 
 
     Returns
     -------
     The length of the edge in the given units
 
 
     Notes
     -----
     This function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     e = _in_scalar(e)
 
     return _cy.edge_length(e, unit=unit)
 
 
 def great_circle_distance(latlng1, latlng2, unit='km'):
@@ -950,16 +979,15 @@
     Parameters
     ----------
     latlng1 : tuple
         (lat, lng) tuple in degrees
     latlng2 : tuple
         (lat, lng) tuple in degrees
     unit: str
-        Unit for distance result ('km', 'm', or 'rads')
-
+        Unit for distance result (``'km'``, ``'m'``, or ``'rads'``)
 
     Returns
     -------
     The spherical distance between the points in the given units
     """
     lat1, lng1 = latlng1
     lat2, lng2 = latlng2
```

### Comparing `h3-4.0.0b4/src/h3/api/numpy_int/__init__.py` & `h3-4.0.0b5/src/h3/api/numpy_int/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file is **symlinked** across the APIs to ensure they are exactly the same.
 
 from ... import _cy
 from ..._h3shape import (
     H3Shape,
-    H3Poly,
-    H3MultiPoly,
+    LatLngPoly,
+    LatLngMultiPoly,
     geo_to_h3shape,
     h3shape_to_geo,
 )
 
 from ._convert import (
     _in_scalar,
     _out_scalar,
@@ -88,28 +88,42 @@
 def average_hexagon_area(res, unit='km^2'):
     """
     Return the average area of an H3 *hexagon*
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_area(res, unit)
 
 
 def average_hexagon_edge_length(res, unit='km'):
     """
     Return the average *hexagon* edge length
     for the given resolution.
 
     This average *excludes* pentagons.
 
+    Parameters
+    ----------
+    res : int
+        H3 resolution
+    unit: str
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
+
     Returns
     -------
     float
     """
     return _cy.average_hexagon_edge_length(res, unit)
 
 
@@ -210,17 +224,17 @@
     p = _out_scalar(p)
 
     return p
 
 
 def grid_distance(h1, h2):
     """
-    Compute the H3 distance between two cells.
+    Compute the grid distance between two cells.
 
-    The H3 distance is defined as the length of the shortest
+    The grid distance is defined as the length of the shortest
     path between the cells in the graph formed by connecting
     adjacent cells.
 
     This function will raise an exception if the
     cells are too far apart to compute the distance.
 
     Parameters
@@ -253,16 +267,16 @@
     tuple of (lat, lng) tuples
     """
     return _cy.cell_to_boundary(_in_scalar(h))
 
 
 def grid_disk(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``<= k`` from ``h``.
-    That is, the 'filled-in' disk.
+    Return unordered collection of cells with grid distance ``<= k`` from ``h``.
+    That is, the "filled-in" disk.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of disk.
 
@@ -277,15 +291,15 @@
     mv = _cy.grid_disk(_in_scalar(h), k)
 
     return _out_collection(mv)
 
 
 def grid_ring(h, k=1):
     """
-    Return unordered collection of cells with H3 distance ``== k`` from ``h``.
+    Return unordered collection of cells with grid distance ``== k`` from ``h``.
     That is, the "hollow" ring.
 
     Parameters
     ----------
     h : H3Cell
     k : int
         Size of ring.
@@ -342,162 +356,165 @@
     -------
     unordered collection of H3Cell
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
-    # todo: does compact_cells work on mixed-resolution collections?
     hu = _in_collection(cells)
     hc = _cy.compact_cells(hu)
 
     return _out_collection(hc)
 
 
 def uncompact_cells(cells, res):
     """
-    Reverse the `compact_cells` operation.
+    Reverse the ``compact_cells`` operation.
 
     Return a collection of H3 cells, all of resolution ``res``.
 
     Parameters
     ----------
     cells : iterable of H3Cell
     res : int
         Resolution of desired output cells.
 
     Returns
     -------
     unordered collection of H3Cell
 
-    Raises
-    ------
-    todo: add test to make sure an error is returned when input
-    contains cell smaller than output res.
-    https://github.com/uber/h3/blob/master/src/h3lib/lib/h3Index.c#L425
-
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
+    # TODO: add test to make sure an error is returned when input contains cell
+    # smaller than output res.
+
     hc = _in_collection(cells)
     hu = _cy.uncompact_cells(hc, res)
 
     return _out_collection(hu)
 
 
 def h3shape_to_cells(h3shape, res):
     """
-    Return the set of H3 cells at a given resolution whose center points
-    are contained within an `H3Poly` or `H3MultiPoly`.
+    Return the collection of H3 cells at a given resolution whose center points
+    are contained within an ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
-    h3shape : H3shape
+    h3shape : ``H3Shape``
     res : int
         Resolution of the output cells
 
     Returns
     -------
-    unordered collection of H3Cell
+    list of H3Cell
 
     Examples
     --------
 
-    >>> poly = H3Poly(
+    >>> poly = LatLngPoly(
     ...     [(37.68, -122.54), (37.68, -122.34), (37.82, -122.34),
     ...      (37.82, -122.54)],
     ... )
     >>> h3.h3shape_to_cells(poly, 6)
-    {'862830807ffffff',
+    ['862830807ffffff',
      '862830827ffffff',
      '86283082fffffff',
      '862830877ffffff',
      '862830947ffffff',
      '862830957ffffff',
-     '86283095fffffff'}
+     '86283095fffffff']
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
 
     # todo: not sure if i want this dispatch logic here. maybe in the objects?
-    if isinstance(h3shape, H3Poly):
+    if isinstance(h3shape, LatLngPoly):
         poly = h3shape
         mv = _cy.polygon_to_cells(poly.outer, res, holes=poly.holes)
-    elif isinstance(h3shape, H3MultiPoly):
+    elif isinstance(h3shape, LatLngMultiPoly):
         mpoly = h3shape
         mv = _cy.polygons_to_cells(mpoly.polys, res)
     elif isinstance(h3shape, H3Shape):
         raise ValueError('Unrecognized H3Shape: ' + str(h3shape))
     else:
         raise ValueError('Unrecognized type: ' + str(type(h3shape)))
 
     return _out_collection(mv)
 
 
-def cells_to_h3shape(cells, tight=True):
+def cells_to_h3shape(cells, *, tight=True):
     """
-    Return a H3MultiPoly describing the area covered by a set of H3 cells.
+    Return an ``H3Shape`` describing the area covered by a collection of H3 cells.
+    Will return ``LatLngPoly`` or ``LatLngMultiPoly``.
 
     Parameters
     ----------
     cells : iterable of H3 cells
     tight : bool
-        If True, return H3Poly if possible. If False, always return H3MultiPoly
+        If True, return ``LatLngPoly`` if possible.
+        If False, always return ``LatLngMultiPoly``.
 
     Returns
     -------
-    H3Poly | H3MultiPoly
+    LatLngPoly | LatLngMultiPoly
 
     Examples
     --------
 
     >>> cells = ['8428309ffffffff', '842830dffffffff']
     >>> h3.cells_to_h3shape(cells, tight=True)
-    <H3Poly: [10]>
+    <LatLngPoly: [10]>
     >>> h3.cells_to_h3shape(cells, tight=False)
-    <H3MultiPoly: [10]>
+    <LatLngMultiPoly: [10]>
     """
     cells = _in_collection(cells)
     mpoly = _cy.cells_to_multi_polygon(cells)
 
-    polys = [H3Poly(*poly) for poly in mpoly]
-    out = H3MultiPoly(*polys)
+    polys = [LatLngPoly(*poly) for poly in mpoly]
+    out = LatLngMultiPoly(*polys)
 
     if tight and len(out) == 1:
         out = out[0]
 
     return out
 
 
 def geo_to_cells(geo, res):
-    """Convert from __geo_interface__ to cells.
+    """Convert from ``__geo_interface__`` to cells.
 
     Parameters
     ----------
-    geo : an object implementing `__geo_interface__` or a dictionary in that format.
-        Both H3Poly and H3MultiPoly implement the interface.
+    geo : an object implementing ``__geo_interface__`` or a dictionary in that format.
+        Both ``LatLngPoly`` and ``LatLngMultiPoly`` implement the interface.
     res : int
         Resolution of desired output cells.
 
     Notes
     -----
     There is currently no guaranteed order of the output cells.
     """
     h3shape = geo_to_h3shape(geo)
     return h3shape_to_cells(h3shape, res)
 
 
 def cells_to_geo(cells, tight=True):
     """
+    Convert from cells to a ``__geo_interface__`` dict.
+
     Parameters
     ----------
     cells : iterable of H3 Cells
+    tight : bool
+        When ``True``, returns an ``LatLngPoly`` when possible.
+        When ``False``, always returns an ``LatLngMultiPoly``.
 
     Returns
     -------
     dict
         in `__geo_interface__` format
     """
     h3shape = cells_to_h3shape(cells, tight=tight)
@@ -670,14 +687,26 @@
     """
     mv = _cy.origin_to_directed_edges(_in_scalar(origin))
 
     return _out_collection(mv)
 
 
 def directed_edge_to_boundary(edge):
+    """
+    Returns points representing the edge (line of points
+    describing the boundary between two cells).
+
+    Parameters
+    ----------
+    edge : H3Edge
+
+    Returns
+    -------
+    tuple of (lat, lng) tuples
+    """
     return _cy.directed_edge_to_boundary(_in_scalar(edge))
 
 
 def grid_path_cells(start, end):
     """
     Returns the ordered collection of cells denoting a
     minimum-length non-unique path between cells.
@@ -890,54 +919,54 @@
     """
     Compute the spherical surface area of a specific H3 cell.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for area result (``'km^2'``, 'm^2', or 'rads^2')
+        Unit for area result (``'km^2'``, ``'m^2'``, or ``'rads^2'``)
 
 
     Returns
     -------
     The area of the H3 cell in the given units
 
 
     Notes
     -----
     This function breaks the cell into spherical triangles, and computes
     their spherical area.
     The function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     h = _in_scalar(h)
 
     return _cy.cell_area(h, unit=unit)
 
 
 def edge_length(e, unit='km'):
     """
     Compute the spherical length of a specific H3 edge.
 
     Parameters
     ----------
     h : H3Cell
     unit: str
-        Unit for length result ('km', 'm', or 'rads')
+        Unit for length result (``'km'``, ``'m'``, or ``'rads'``)
 
 
     Returns
     -------
     The length of the edge in the given units
 
 
     Notes
     -----
     This function uses the spherical distance calculation given by
-    `great_circle_distance`.
+    ``great_circle_distance()``.
     """
     e = _in_scalar(e)
 
     return _cy.edge_length(e, unit=unit)
 
 
 def great_circle_distance(latlng1, latlng2, unit='km'):
@@ -950,16 +979,15 @@
     Parameters
     ----------
     latlng1 : tuple
         (lat, lng) tuple in degrees
     latlng2 : tuple
         (lat, lng) tuple in degrees
     unit: str
-        Unit for distance result ('km', 'm', or 'rads')
-
+        Unit for distance result (``'km'``, ``'m'``, or ``'rads'``)
 
     Returns
     -------
     The spherical distance between the points in the given units
     """
     lat1, lng1 = latlng1
     lat2, lng2 = latlng2
```

### Comparing `h3-4.0.0b4/src/h3.egg-info/PKG-INFO` & `h3-4.0.0b5/src/h3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h3
-Version: 4.0.0b4
+Version: 4.0.0b5
 Summary: Hierarchical hexagonal geospatial indexing system
 Home-page: https://github.com/uber/h3-py
 Author: Uber Technologies
 Author-email: AJ Friend <ajfriend@gmail.com>
 License: Apache 2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `h3-4.0.0b4/src/h3.egg-info/SOURCES.txt` & `h3-4.0.0b5/src/h3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/CMakeLists.txt` & `h3-4.0.0b5/src/h3lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/LICENSE` & `h3-4.0.0b5/src/h3lib/LICENSE`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/README.md` & `h3-4.0.0b5/src/h3lib/README.md`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/cmake/TestWrapValgrind.cmake` & `h3-4.0.0b5/src/h3lib/cmake/TestWrapValgrind.cmake`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/cmake/toolchain.cmake` & `h3-4.0.0b5/src/h3lib/cmake/toolchain.cmake`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/algos.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/algos.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/alloc.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/alloc.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/baseCells.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/baseCells.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/bbox.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/bbox.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/constants.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/constants.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/coordijk.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/coordijk.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/directedEdge.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/directedEdge.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/faceijk.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/faceijk.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/h3Index.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/h3Index.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/h3api.h.in` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/h3api.h.in`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/iterators.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/iterators.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/latLng.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/latLng.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/linkedGeo.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/linkedGeo.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/localij.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/localij.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/mathExtensions.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/mathExtensions.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/polygon.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/polygon.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/polygonAlgos.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/polygonAlgos.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/vec2d.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/vec2d.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/vec3d.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/vec3d.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/vertex.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/vertex.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/include/vertexGraph.h` & `h3-4.0.0b5/src/h3lib/src/h3lib/include/vertexGraph.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/algos.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/algos.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/baseCells.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/baseCells.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/bbox.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/bbox.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/coordijk.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/coordijk.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/directedEdge.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/directedEdge.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/faceijk.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/faceijk.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/h3Index.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/h3Index.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/iterators.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/iterators.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/latLng.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/latLng.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/linkedGeo.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/linkedGeo.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/localij.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/localij.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/mathExtensions.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/mathExtensions.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/polygon.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/polygon.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec2d.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/vec2d.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec3d.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/vec3d.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertex.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/vertex.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertexGraph.c` & `h3-4.0.0b5/src/h3lib/src/h3lib/lib/vertexGraph.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/tests/test_cells_and_edges.py` & `h3-4.0.0b5/tests/test_cells_and_edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
     with pytest.raises(H3FailedError):
         h3.grid_distance(h1, h2)
 
 
 def get_maine_cells():
     # lat/lngs for State of Maine
-    poly = h3.H3Poly([
+    poly = h3.LatLngPoly([
         (45.137451890638886, -67.13734351262877),
         (44.8097, -66.96466),
         (44.3252, -68.03252),
         (43.98, -69.06),
         (43.68405, -70.11617),
         (43.090083319667144, -70.64573401557249),
         (43.08003225358635, -70.75102474636725),
```

### Comparing `h3-4.0.0b4/tests/test_error_codes.py` & `h3-4.0.0b5/tests/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b4/tests/test_h3.py` & `h3-4.0.0b5/tests/test_h3.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         (37.7866302000007224, -122.3805436999997056),
         (37.7198061999978478, -122.3544736999993603),
         (37.7076131999975672, -122.5123436999983966),
         (37.7835871999971715, -122.5247187000021967),
         (37.8151571999998453, -122.4798767000009008),
     ]
 
-    poly = h3.H3Poly(sf_7x7)
+    poly = h3.LatLngPoly(sf_7x7)
     cells = h3.h3shape_to_cells(poly, 9)
 
     compact_cells = h3.compact_cells(cells)
     assert len(compact_cells) == 209
 
     uncompact_cells = h3.uncompact_cells(compact_cells, 9)
     assert len(uncompact_cells) == 1253
```

### Comparing `h3-4.0.0b4/tests/test_length_area.py` & `h3-4.0.0b5/tests/test_length_area.py`

 * *Files identical despite different names*

