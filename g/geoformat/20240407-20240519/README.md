# Comparing `tmp/geoformat-20240407.tar.gz` & `tmp/geoformat-20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoformat-20240407.tar", last modified: Sun Apr  7 21:37:18 2024, max compression
+gzip compressed data, was "geoformat-20240519.tar", last modified: Sun May 19 14:04:54 2024, max compression
```

## Comparing `geoformat-20240407.tar` & `geoformat-20240519.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.672978 geoformat-20240407/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1148 2024-03-14 13:56:28.000000 geoformat-20240407/LICENSE
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   117768 2024-04-07 21:37:18.672978 geoformat-20240407/PKG-INFO
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   116864 2024-04-07 21:36:33.000000 geoformat-20240407/README.md
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.636977 geoformat-20240407/geoformat/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15151 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      280 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/_version.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/conf/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conf/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2044 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conf/decorator.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      836 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conf/driver_variable.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3840 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/conf/error_messages.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3588 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conf/fields_variable.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1744 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conf/format_data.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)       35 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conf/geoformat_var.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3990 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conf/geometry_variable.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4897 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conf/path.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      700 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conf/proj_var.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10042 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conf/timer.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/constraints/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/constraints/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1810 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/constraints/primary_key.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/conversion/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conversion/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1381 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conversion/bbox_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4858 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conversion/bytes_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    11935 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/conversion/coordinates_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12354 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conversion/datetime_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    46111 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conversion/feature_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    19623 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conversion/fields_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7507 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conversion/geolayer_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    50297 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/conversion/geometry_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7331 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/conversion/metadata_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      701 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conversion/precision_tolerance_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1732 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/conversion/segment_conversion.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/db/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/db/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2070 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/db/db_request.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/draw/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/draw/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    13743 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/draw/draw.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/driver/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/driver/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2695 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/driver/common_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    13306 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/driver/csv_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    40428 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/driver/esri_shapefile_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12243 2024-04-07 21:36:33.000000 geoformat-20240407/geoformat/driver/geojson_driver.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/driver/ogr/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/driver/ogr/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    41141 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/driver/ogr/ogr_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9989 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/driver/postgresql_driver.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.640977 geoformat-20240407/geoformat/explore_data/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/explore_data/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5345 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/explore_data/duplicate.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    16452 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/explore_data/print_data.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1403 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/explore_data/random_geometry.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/geoprocessing/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1256 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/area.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/geoprocessing/connectors/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/connectors/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2143 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/connectors/operations.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12104 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/connectors/predicates.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/geoprocessing/generalization/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/generalization/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2209 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4979 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/geoprocessing/generalization/visvalingam_whyatt.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/geoprocessing/geoparameters/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/geoparameters/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3396 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/geoprocessing/geoparameters/bbox.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      877 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/geoparameters/boundaries.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5335 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/geoparameters/lines.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1362 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/length.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    11568 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/geoprocessing/line_merge.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/geoprocessing/matrix/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/matrix/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5681 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/geoprocessing/matrix/adjacency.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/geoprocessing/measure/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/measure/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1328 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/measure/area.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3561 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/geoprocessing/measure/distance.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      560 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/measure/length.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7220 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/geoprocessing/merge_geometries.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7441 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/point_on_linestring.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3824 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/simplify.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5237 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/split.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2084 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/geoprocessing/union.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/index/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/index/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/index/attributes/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/index/attributes/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      684 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/index/attributes/hash.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/index/geometry/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/index/geometry/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    14749 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/index/geometry/grid.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/manipulation/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/manipulation/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2859 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/manipulation/feature_manipulation.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    20872 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/manipulation/geolayer_manipulation.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10063 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/manipulation/metadata_manipulation.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/obj/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/obj/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      774 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/obj/geometry.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/processing/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/processing/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/processing/data/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/geoformat/processing/data/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9722 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/processing/data/clauses.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10584 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/processing/data/field_statistics.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.644977 geoformat-20240407/geoformat/processing/data/join/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/processing/data/join/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    27534 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/processing/data/join/join.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    11975 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/processing/data/join/merge_objects.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5199 2024-03-14 13:56:28.000000 geoformat-20240407/geoformat/processing/data/union.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.636977 geoformat-20240407/geoformat.egg-info/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   117768 2024-04-07 21:37:18.000000 geoformat-20240407/geoformat.egg-info/PKG-INFO
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7800 2024-04-07 21:37:18.000000 geoformat-20240407/geoformat.egg-info/SOURCES.txt
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        1 2024-04-07 21:37:18.000000 geoformat-20240407/geoformat.egg-info/dependency_links.txt
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)       16 2024-04-07 21:37:18.000000 geoformat-20240407/geoformat.egg-info/top_level.txt
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)       38 2024-04-07 21:37:18.672978 geoformat-20240407/setup.cfg
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1217 2024-03-14 13:56:28.000000 geoformat-20240407/setup.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.636977 geoformat-20240407/tests/
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.660977 geoformat-20240407/tests/data/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/data/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    16040 2024-04-07 21:36:33.000000 geoformat-20240407/tests/data/coordinates.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    48663 2024-03-14 13:56:28.000000 geoformat-20240407/tests/data/features.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2545 2024-03-14 13:56:28.000000 geoformat-20240407/tests/data/fields_metadata.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513) 24175079 2024-03-14 13:56:28.000000 geoformat-20240407/tests/data/geolayers.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    26847 2024-04-07 21:36:33.000000 geoformat-20240407/tests/data/geometries.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    58422 2023-08-01 15:43:07.000000 geoformat-20240407/tests/data/geometry_index.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2725 2024-03-14 13:56:28.000000 geoformat-20240407/tests/data/index.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      232 2023-08-01 15:43:07.000000 geoformat-20240407/tests/data/matrix.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     6652 2024-03-14 13:56:28.000000 geoformat-20240407/tests/data/metadata.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      435 2023-08-01 15:43:07.000000 geoformat-20240407/tests/data/segments.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.660977 geoformat-20240407/tests/geoformat/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.660977 geoformat-20240407/tests/geoformat/conf/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/conf/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3617 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conf/test_format_data.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     8737 2024-04-07 21:36:33.000000 geoformat-20240407/tests/geoformat/conf/test_path.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.660977 geoformat-20240407/tests/geoformat/constraints/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/constraints/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2987 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/constraints/test_primary_key.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.664977 geoformat-20240407/tests/geoformat/conversion/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/conversion/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2380 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_bbox_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    17731 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_bytes_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    19439 2024-04-07 21:36:33.000000 geoformat-20240407/tests/geoformat/conversion/test_coordinates_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7580 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_datetime_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   205565 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_feature_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   241595 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_fields_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    13309 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_geolayer_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    92781 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_geometry_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    65479 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_metadata_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1238 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_precision_tolerance_conversion.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3245 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/conversion/test_segment_conversion.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.664977 geoformat-20240407/tests/geoformat/db/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/db/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.664977 geoformat-20240407/tests/geoformat/driver/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/driver/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.664977 geoformat-20240407/tests/geoformat/driver/ogr/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/driver/ogr/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      369 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/ogr/compare_ogr_files.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1251 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/ogr/geolayer_to_geojson.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1263 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/ogr/geolayer_to_postgresql.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2155 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/ogr/geolayer_to_shapefile.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    16408 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/test_common_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    29687 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/test_csv_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   321121 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/test_esri_shapefile_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)  1461478 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/test_geojson_driver.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   114134 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/driver/test_postgresql_driver.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.664977 geoformat-20240407/tests/geoformat/explore_data/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/explore_data/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    17339 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/explore_data/test_duplicate.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    66158 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/explore_data/test_print_data.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/geoprocessing/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/geoprocessing/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/geoprocessing/connectors/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/geoprocessing/connectors/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4728 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/connectors/test_operations.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15761 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/connectors/test_predicates.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/geoprocessing/generalization/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/geoprocessing/generalization/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2176 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1845 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3562 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/test_bbox.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      901 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9425 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/test_lines.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/geoprocessing/matrix/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/geoprocessing/matrix/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1645 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/matrix/test_adjacency.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/geoprocessing/measure/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/geoprocessing/measure/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2234 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/measure/test_area.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3736 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/measure/test_distance.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1525 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/measure/test_length.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1758 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_area.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2337 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_length.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15898 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_line_merge.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4976 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_merge_geometries.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4575 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_point_on_linestring.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    14514 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_simplify.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    53164 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_split.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1387 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/geoprocessing/test_union.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/index/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/index/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/index/attributes/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/index/attributes/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      880 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/index/attributes/test_hash.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/index/geometry/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/index/geometry/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15928 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/index/geometry/test_grid.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/manipulation/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/manipulation/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12109 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/manipulation/test_feature_manipulation.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   233933 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/manipulation/test_geolayer_manipulation.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    38653 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/manipulation/test_metadata_manipulation.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/obj/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/obj/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1928 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/obj/test_geometry.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/processing/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/processing/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.668977 geoformat-20240407/tests/geoformat/processing/data/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/geoformat/processing/data/__init__.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.672978 geoformat-20240407/tests/geoformat/processing/data/join/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/processing/data/join/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   614826 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/processing/data/join/test_join.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    20394 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/processing/data/join/test_merge_objects.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     6947 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/processing/data/test_clauses.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7807 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/processing/data/test_field_statistics.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9170 2024-03-14 13:56:28.000000 geoformat-20240407/tests/geoformat/processing/data/test_union.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.672978 geoformat-20240407/tests/inspector/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/inspector/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    17958 2024-04-07 21:36:33.000000 geoformat-20240407/tests/inspector/geoformat_inspector.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.672978 geoformat-20240407/tests/perf/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240407/tests/perf/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10403 2024-03-14 13:56:28.000000 geoformat-20240407/tests/perf/compare_func.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.672978 geoformat-20240407/tests/unit/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-29 14:32:46.000000 geoformat-20240407/tests/unit/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2139 2024-03-31 14:29:48.000000 geoformat-20240407/tests/unit/test_separate_coordinates_dimensions.py
-drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-07 21:37:18.672978 geoformat-20240407/tests/utils/
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240407/tests/utils/__init__.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1379 2024-03-14 13:56:28.000000 geoformat-20240407/tests/utils/compare.py
--rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     6701 2024-03-14 13:56:28.000000 geoformat-20240407/tests/utils/tests_utils.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.574097 geoformat-20240519/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1148 2024-03-14 13:56:28.000000 geoformat-20240519/LICENSE
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   117768 2024-05-19 14:04:54.574097 geoformat-20240519/PKG-INFO
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   116864 2024-05-19 13:26:15.000000 geoformat-20240519/README.md
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.534098 geoformat-20240519/geoformat/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15151 2024-05-19 13:26:15.000000 geoformat-20240519/geoformat/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      280 2024-05-19 13:42:20.000000 geoformat-20240519/geoformat/_version.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.538098 geoformat-20240519/geoformat/conf/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conf/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2044 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conf/decorator.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      836 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conf/driver_variable.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3966 2024-05-19 13:58:44.000000 geoformat-20240519/geoformat/conf/error_messages.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3588 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conf/fields_variable.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1744 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conf/format_data.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)       35 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conf/geoformat_var.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3990 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conf/geometry_variable.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4897 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conf/path.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      700 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conf/proj_var.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10042 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conf/timer.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.538098 geoformat-20240519/geoformat/constraints/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/constraints/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1810 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/constraints/primary_key.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/conversion/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conversion/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1381 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conversion/bbox_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4858 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conversion/bytes_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    11935 2024-04-08 17:31:01.000000 geoformat-20240519/geoformat/conversion/coordinates_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12354 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conversion/datetime_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    46111 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conversion/feature_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    19623 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conversion/fields_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7507 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conversion/geolayer_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    50297 2024-04-08 19:21:39.000000 geoformat-20240519/geoformat/conversion/geometry_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7331 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/conversion/metadata_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      701 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conversion/precision_tolerance_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1732 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/conversion/segment_conversion.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/db/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/db/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2070 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/db/db_request.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/draw/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-04-08 17:31:01.000000 geoformat-20240519/geoformat/draw/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10690 2024-05-19 13:58:44.000000 geoformat-20240519/geoformat/draw/draw.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/driver/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/driver/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2695 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/driver/common_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    13306 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/driver/csv_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    40428 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/driver/esri_shapefile_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12243 2024-04-08 17:31:01.000000 geoformat-20240519/geoformat/driver/geojson_driver.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/driver/ogr/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/driver/ogr/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    41141 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/driver/ogr/ogr_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9989 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/driver/postgresql_driver.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/explore_data/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/explore_data/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5345 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/explore_data/duplicate.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    16452 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/explore_data/print_data.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1403 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/explore_data/random_geometry.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/geoprocessing/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1256 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/area.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.542098 geoformat-20240519/geoformat/geoprocessing/connectors/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/connectors/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2143 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/connectors/operations.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12104 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/connectors/predicates.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/geoprocessing/generalization/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/generalization/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2209 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4979 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/geoprocessing/generalization/visvalingam_whyatt.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/geoprocessing/geoparameters/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/geoparameters/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3396 2024-05-19 13:26:15.000000 geoformat-20240519/geoformat/geoprocessing/geoparameters/bbox.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      877 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/geoparameters/boundaries.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5335 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/geoparameters/lines.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1362 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/length.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    11568 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/geoprocessing/line_merge.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/geoprocessing/matrix/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/matrix/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5681 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/geoprocessing/matrix/adjacency.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/geoprocessing/measure/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/measure/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1328 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/measure/area.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3561 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/geoprocessing/measure/distance.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      560 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/measure/length.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7220 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/geoprocessing/merge_geometries.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7441 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/point_on_linestring.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3824 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/simplify.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5237 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/split.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2084 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/geoprocessing/union.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/index/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/index/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/index/attributes/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/index/attributes/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      684 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/index/attributes/hash.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/index/geometry/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/index/geometry/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    14749 2024-05-19 13:26:15.000000 geoformat-20240519/geoformat/index/geometry/grid.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/manipulation/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/manipulation/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2859 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/manipulation/feature_manipulation.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    20872 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/manipulation/geolayer_manipulation.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10063 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/manipulation/metadata_manipulation.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/obj/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/obj/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      774 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/obj/geometry.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/processing/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/processing/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/processing/data/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/geoformat/processing/data/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9722 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/processing/data/clauses.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10584 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/processing/data/field_statistics.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.546098 geoformat-20240519/geoformat/processing/data/join/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/processing/data/join/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    27534 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/processing/data/join/join.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    11975 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/processing/data/join/merge_objects.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     5199 2024-03-14 13:56:28.000000 geoformat-20240519/geoformat/processing/data/union.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.538098 geoformat-20240519/geoformat.egg-info/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   117768 2024-05-19 14:04:54.000000 geoformat-20240519/geoformat.egg-info/PKG-INFO
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7800 2024-05-19 14:04:54.000000 geoformat-20240519/geoformat.egg-info/SOURCES.txt
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        1 2024-05-19 14:04:54.000000 geoformat-20240519/geoformat.egg-info/dependency_links.txt
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)       16 2024-05-19 14:04:54.000000 geoformat-20240519/geoformat.egg-info/top_level.txt
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)       38 2024-05-19 14:04:54.574097 geoformat-20240519/setup.cfg
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1217 2024-03-14 13:56:28.000000 geoformat-20240519/setup.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.534098 geoformat-20240519/tests/
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.562098 geoformat-20240519/tests/data/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/data/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    16040 2024-04-08 17:31:01.000000 geoformat-20240519/tests/data/coordinates.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    48663 2024-03-14 13:56:28.000000 geoformat-20240519/tests/data/features.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2545 2024-03-14 13:56:28.000000 geoformat-20240519/tests/data/fields_metadata.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513) 24175079 2024-03-14 13:56:28.000000 geoformat-20240519/tests/data/geolayers.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    26847 2024-04-08 17:31:01.000000 geoformat-20240519/tests/data/geometries.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    58422 2023-08-01 15:43:07.000000 geoformat-20240519/tests/data/geometry_index.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2725 2024-03-14 13:56:28.000000 geoformat-20240519/tests/data/index.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      232 2023-08-01 15:43:07.000000 geoformat-20240519/tests/data/matrix.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     6652 2024-03-14 13:56:28.000000 geoformat-20240519/tests/data/metadata.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      435 2023-08-01 15:43:07.000000 geoformat-20240519/tests/data/segments.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.562098 geoformat-20240519/tests/geoformat/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.562098 geoformat-20240519/tests/geoformat/conf/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/conf/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3617 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conf/test_format_data.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     8737 2024-04-08 17:31:01.000000 geoformat-20240519/tests/geoformat/conf/test_path.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.562098 geoformat-20240519/tests/geoformat/constraints/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/constraints/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2987 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/constraints/test_primary_key.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.562098 geoformat-20240519/tests/geoformat/conversion/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/conversion/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2380 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_bbox_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    17731 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_bytes_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    19439 2024-04-08 17:31:01.000000 geoformat-20240519/tests/geoformat/conversion/test_coordinates_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7580 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_datetime_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   205565 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_feature_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   241595 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_fields_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    13309 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_geolayer_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    92781 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_geometry_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    65479 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_metadata_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1238 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_precision_tolerance_conversion.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3245 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/conversion/test_segment_conversion.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.562098 geoformat-20240519/tests/geoformat/db/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/db/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.566098 geoformat-20240519/tests/geoformat/driver/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/driver/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.566098 geoformat-20240519/tests/geoformat/driver/ogr/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/driver/ogr/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      369 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/ogr/compare_ogr_files.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1251 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/ogr/geolayer_to_geojson.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1263 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/ogr/geolayer_to_postgresql.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2155 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/ogr/geolayer_to_shapefile.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    16408 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/test_common_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    29687 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/test_csv_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   321121 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/test_esri_shapefile_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)  1461478 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/test_geojson_driver.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   114134 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/driver/test_postgresql_driver.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.566098 geoformat-20240519/tests/geoformat/explore_data/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/explore_data/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    17339 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/explore_data/test_duplicate.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    66158 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/explore_data/test_print_data.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.566098 geoformat-20240519/tests/geoformat/geoprocessing/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/geoprocessing/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.566098 geoformat-20240519/tests/geoformat/geoprocessing/connectors/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/geoprocessing/connectors/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4728 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/connectors/test_operations.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15761 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/connectors/test_predicates.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/geoprocessing/generalization/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/geoprocessing/generalization/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2176 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1845 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3562 2024-05-19 13:26:15.000000 geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/test_bbox.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      901 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9425 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/test_lines.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/geoprocessing/matrix/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/geoprocessing/matrix/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1645 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/matrix/test_adjacency.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/geoprocessing/measure/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/geoprocessing/measure/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2234 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/measure/test_area.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     3736 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/measure/test_distance.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1525 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/measure/test_length.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1758 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_area.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2337 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_length.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15898 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_line_merge.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4976 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_merge_geometries.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     4575 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_point_on_linestring.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    14514 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_simplify.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    53164 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_split.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1387 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/geoprocessing/test_union.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/index/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/index/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/index/attributes/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/index/attributes/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)      880 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/index/attributes/test_hash.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/index/geometry/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/index/geometry/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    15928 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/index/geometry/test_grid.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/manipulation/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/manipulation/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    12109 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/manipulation/test_feature_manipulation.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   233933 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/manipulation/test_geolayer_manipulation.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    38653 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/manipulation/test_metadata_manipulation.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/obj/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/obj/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1928 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/obj/test_geometry.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/processing/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/processing/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/processing/data/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/geoformat/processing/data/__init__.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/geoformat/processing/data/join/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/processing/data/join/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)   614826 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/processing/data/join/test_join.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    20394 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/processing/data/join/test_merge_objects.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     6947 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/processing/data/test_clauses.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     7807 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/processing/data/test_field_statistics.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     9170 2024-03-14 13:56:28.000000 geoformat-20240519/tests/geoformat/processing/data/test_union.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.570098 geoformat-20240519/tests/inspector/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/inspector/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    17958 2024-04-08 17:31:01.000000 geoformat-20240519/tests/inspector/geoformat_inspector.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.574097 geoformat-20240519/tests/perf/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2023-08-01 15:43:07.000000 geoformat-20240519/tests/perf/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)    10403 2024-03-14 13:56:28.000000 geoformat-20240519/tests/perf/compare_func.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.574097 geoformat-20240519/tests/unit/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-29 14:32:46.000000 geoformat-20240519/tests/unit/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     2139 2024-03-31 14:29:48.000000 geoformat-20240519/tests/unit/test_separate_coordinates_dimensions.py
+drwxr-xr-x   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-05-19 14:04:54.574097 geoformat-20240519/tests/utils/
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)        0 2024-03-14 13:56:28.000000 geoformat-20240519/tests/utils/__init__.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     1379 2024-03-14 13:56:28.000000 geoformat-20240519/tests/utils/compare.py
+-rw-r--r--   0 x2025202 (1176801568) utilisateurs du domaine (1176800513)     6701 2024-03-14 13:56:28.000000 geoformat-20240519/tests/utils/tests_utils.py
```

### Comparing `geoformat-20240407/LICENSE` & `geoformat-20240519/LICENSE`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/PKG-INFO` & `geoformat-20240519/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6f66  : 2.1.Name: geof
 00000020: 6f72 6d61 740a 5665 7273 696f 6e3a 2032  ormat.Version: 2
-00000030: 3032 3430 3430 370a 5375 6d6d 6172 793a  0240407.Summary:
+00000030: 3032 3430 3531 390a 5375 6d6d 6172 793a  0240519.Summary:
 00000040: 2047 656f 666f 726d 6174 2069 7320 6120   Geoformat is a 
 00000050: 3939 2025 2070 7974 686f 6e20 6765 6f73  99 % python geos
 00000060: 7061 7469 616c 2062 6c61 636b 736d 6974  patial blacksmit
 00000070: 680a 486f 6d65 2d70 6167 653a 2068 7474  h.Home-page: htt
 00000080: 7073 3a2f 2f66 7261 6d61 6769 742e 6f72  ps://framagit.or
 00000090: 672f 4775 696c 6861 696e 2f47 656f 666f  g/Guilhain/Geofo
 000000a0: 726d 6174 0a41 7574 686f 723a 2047 7569  rmat.Author: Gui
```

### Comparing `geoformat-20240407/README.md` & `geoformat-20240519/README.md`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/__init__.py` & `geoformat-20240519/geoformat/__init__.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/decorator.py` & `geoformat-20240519/geoformat/conf/decorator.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/driver_variable.py` & `geoformat-20240519/geoformat/conf/driver_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/error_messages.py` & `geoformat-20240519/geoformat/conf/error_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 # driver
 import_lib_error = "cannot run this function ! {lib} library not installed"
 import_ogr_error = import_lib_error.format(lib="Python-gdal")
 import_psycopg2_error = import_lib_error.format(lib="psycopg2")
 import_pyproj_error = import_lib_error.format(lib="pyproj")
 import_shapefile_error = import_lib_error.format(lib="shapefile")
+import_matplotlib_error = import_lib_error.format(lib="matplotlib")
+import_numpy_error = import_lib_error.format(lib="numpy")
 
 key_parameter_invalid = "key : {key} not supported"
 
 
 # path
 path_not_valid = "path : {path} is not valid"
 path_not_a_dir = f"{path_not_valid}, it must be a directory"
```

### Comparing `geoformat-20240407/geoformat/conf/fields_variable.py` & `geoformat-20240519/geoformat/conf/fields_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/format_data.py` & `geoformat-20240519/geoformat/conf/format_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/geometry_variable.py` & `geoformat-20240519/geoformat/conf/geometry_variable.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/path.py` & `geoformat-20240519/geoformat/conf/path.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/proj_var.py` & `geoformat-20240519/geoformat/conf/proj_var.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conf/timer.py` & `geoformat-20240519/geoformat/conf/timer.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/constraints/primary_key.py` & `geoformat-20240519/geoformat/constraints/primary_key.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/bbox_conversion.py` & `geoformat-20240519/geoformat/conversion/bbox_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/bytes_conversion.py` & `geoformat-20240519/geoformat/conversion/bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/coordinates_conversion.py` & `geoformat-20240519/geoformat/conversion/coordinates_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/datetime_conversion.py` & `geoformat-20240519/geoformat/conversion/datetime_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/feature_conversion.py` & `geoformat-20240519/geoformat/conversion/feature_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/fields_conversion.py` & `geoformat-20240519/geoformat/conversion/fields_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/geolayer_conversion.py` & `geoformat-20240519/geoformat/conversion/geolayer_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/geometry_conversion.py` & `geoformat-20240519/geoformat/conversion/geometry_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/metadata_conversion.py` & `geoformat-20240519/geoformat/conversion/metadata_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/precision_tolerance_conversion.py` & `geoformat-20240519/geoformat/conversion/precision_tolerance_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/conversion/segment_conversion.py` & `geoformat-20240519/geoformat/conversion/segment_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/db/db_request.py` & `geoformat-20240519/geoformat/db/db_request.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/driver/common_driver.py` & `geoformat-20240519/geoformat/driver/common_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/driver/csv_driver.py` & `geoformat-20240519/geoformat/driver/csv_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/driver/esri_shapefile_driver.py` & `geoformat-20240519/geoformat/driver/esri_shapefile_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/driver/geojson_driver.py` & `geoformat-20240519/geoformat/driver/geojson_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/driver/ogr/ogr_driver.py` & `geoformat-20240519/geoformat/driver/ogr/ogr_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/driver/postgresql_driver.py` & `geoformat-20240519/geoformat/driver/postgresql_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/explore_data/duplicate.py` & `geoformat-20240519/geoformat/explore_data/duplicate.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/explore_data/print_data.py` & `geoformat-20240519/geoformat/explore_data/print_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/explore_data/random_geometry.py` & `geoformat-20240519/geoformat/explore_data/random_geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/area.py` & `geoformat-20240519/geoformat/geoprocessing/area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/connectors/operations.py` & `geoformat-20240519/geoformat/geoprocessing/connectors/operations.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/connectors/predicates.py` & `geoformat-20240519/geoformat/geoprocessing/connectors/predicates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py` & `geoformat-20240519/geoformat/geoprocessing/generalization/ramer_douglas_peucker.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/generalization/visvalingam_whyatt.py` & `geoformat-20240519/geoformat/geoprocessing/generalization/visvalingam_whyatt.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/geoparameters/bbox.py` & `geoformat-20240519/geoformat/geoprocessing/geoparameters/bbox.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/geoparameters/boundaries.py` & `geoformat-20240519/geoformat/geoprocessing/geoparameters/boundaries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/geoparameters/lines.py` & `geoformat-20240519/geoformat/geoprocessing/geoparameters/lines.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/length.py` & `geoformat-20240519/geoformat/geoprocessing/length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/line_merge.py` & `geoformat-20240519/geoformat/geoprocessing/line_merge.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/matrix/adjacency.py` & `geoformat-20240519/geoformat/geoprocessing/matrix/adjacency.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/measure/area.py` & `geoformat-20240519/geoformat/geoprocessing/measure/area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/measure/distance.py` & `geoformat-20240519/geoformat/geoprocessing/measure/distance.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/measure/length.py` & `geoformat-20240519/geoformat/geoprocessing/measure/length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/merge_geometries.py` & `geoformat-20240519/geoformat/geoprocessing/merge_geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/point_on_linestring.py` & `geoformat-20240519/geoformat/geoprocessing/point_on_linestring.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/simplify.py` & `geoformat-20240519/geoformat/geoprocessing/simplify.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/split.py` & `geoformat-20240519/geoformat/geoprocessing/split.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/geoprocessing/union.py` & `geoformat-20240519/geoformat/geoprocessing/union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/index/attributes/hash.py` & `geoformat-20240519/geoformat/index/attributes/hash.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/index/geometry/grid.py` & `geoformat-20240519/geoformat/index/geometry/grid.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/manipulation/feature_manipulation.py` & `geoformat-20240519/geoformat/manipulation/feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/manipulation/geolayer_manipulation.py` & `geoformat-20240519/geoformat/manipulation/geolayer_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/manipulation/metadata_manipulation.py` & `geoformat-20240519/geoformat/manipulation/metadata_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/obj/geometry.py` & `geoformat-20240519/geoformat/obj/geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/processing/data/clauses.py` & `geoformat-20240519/geoformat/processing/data/clauses.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/processing/data/field_statistics.py` & `geoformat-20240519/geoformat/processing/data/field_statistics.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/processing/data/join/join.py` & `geoformat-20240519/geoformat/processing/data/join/join.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/processing/data/join/merge_objects.py` & `geoformat-20240519/geoformat/processing/data/join/merge_objects.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat/processing/data/union.py` & `geoformat-20240519/geoformat/processing/data/union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/geoformat.egg-info/PKG-INFO` & `geoformat-20240519/geoformat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6f66  : 2.1.Name: geof
 00000020: 6f72 6d61 740a 5665 7273 696f 6e3a 2032  ormat.Version: 2
-00000030: 3032 3430 3430 370a 5375 6d6d 6172 793a  0240407.Summary:
+00000030: 3032 3430 3531 390a 5375 6d6d 6172 793a  0240519.Summary:
 00000040: 2047 656f 666f 726d 6174 2069 7320 6120   Geoformat is a 
 00000050: 3939 2025 2070 7974 686f 6e20 6765 6f73  99 % python geos
 00000060: 7061 7469 616c 2062 6c61 636b 736d 6974  patial blacksmit
 00000070: 680a 486f 6d65 2d70 6167 653a 2068 7474  h.Home-page: htt
 00000080: 7073 3a2f 2f66 7261 6d61 6769 742e 6f72  ps://framagit.or
 00000090: 672f 4775 696c 6861 696e 2f47 656f 666f  g/Guilhain/Geofo
 000000a0: 726d 6174 0a41 7574 686f 723a 2047 7569  rmat.Author: Gui
```

### Comparing `geoformat-20240407/geoformat.egg-info/SOURCES.txt` & `geoformat-20240519/geoformat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/setup.py` & `geoformat-20240519/setup.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/coordinates.py` & `geoformat-20240519/tests/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/features.py` & `geoformat-20240519/tests/data/features.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/fields_metadata.py` & `geoformat-20240519/tests/data/fields_metadata.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/geolayers.py` & `geoformat-20240519/tests/data/geolayers.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/geometries.py` & `geoformat-20240519/tests/data/geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/geometry_index.py` & `geoformat-20240519/tests/data/geometry_index.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/index.py` & `geoformat-20240519/tests/data/index.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/data/metadata.py` & `geoformat-20240519/tests/data/metadata.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conf/test_format_data.py` & `geoformat-20240519/tests/geoformat/conf/test_format_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conf/test_path.py` & `geoformat-20240519/tests/geoformat/conf/test_path.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/constraints/test_primary_key.py` & `geoformat-20240519/tests/geoformat/constraints/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_bbox_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_bbox_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_bytes_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_bytes_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_coordinates_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_coordinates_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_datetime_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_datetime_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_feature_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_feature_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_fields_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_fields_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_geolayer_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_geolayer_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_geometry_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_geometry_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_metadata_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_metadata_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_precision_tolerance_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_precision_tolerance_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/conversion/test_segment_conversion.py` & `geoformat-20240519/tests/geoformat/conversion/test_segment_conversion.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/ogr/geolayer_to_geojson.py` & `geoformat-20240519/tests/geoformat/driver/ogr/geolayer_to_geojson.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/ogr/geolayer_to_postgresql.py` & `geoformat-20240519/tests/geoformat/driver/ogr/geolayer_to_postgresql.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/ogr/geolayer_to_shapefile.py` & `geoformat-20240519/tests/geoformat/driver/ogr/geolayer_to_shapefile.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/test_common_driver.py` & `geoformat-20240519/tests/geoformat/driver/test_common_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/test_csv_driver.py` & `geoformat-20240519/tests/geoformat/driver/test_csv_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/test_esri_shapefile_driver.py` & `geoformat-20240519/tests/geoformat/driver/test_esri_shapefile_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/test_geojson_driver.py` & `geoformat-20240519/tests/geoformat/driver/test_geojson_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/driver/test_postgresql_driver.py` & `geoformat-20240519/tests/geoformat/driver/test_postgresql_driver.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/explore_data/test_duplicate.py` & `geoformat-20240519/tests/geoformat/explore_data/test_duplicate.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/explore_data/test_print_data.py` & `geoformat-20240519/tests/geoformat/explore_data/test_print_data.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/connectors/test_operations.py` & `geoformat-20240519/tests/geoformat/geoprocessing/connectors/test_operations.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/connectors/test_predicates.py` & `geoformat-20240519/tests/geoformat/geoprocessing/connectors/test_predicates.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py` & `geoformat-20240519/tests/geoformat/geoprocessing/generalization/test_ramer_douglas_peucker.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py` & `geoformat-20240519/tests/geoformat/geoprocessing/generalization/test_visvalingam_whyatt.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/test_bbox.py` & `geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/test_bbox.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py` & `geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/geoparameters/test_lines.py` & `geoformat-20240519/tests/geoformat/geoprocessing/geoparameters/test_lines.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/matrix/test_adjacency.py` & `geoformat-20240519/tests/geoformat/geoprocessing/matrix/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/measure/test_area.py` & `geoformat-20240519/tests/geoformat/geoprocessing/measure/test_area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/measure/test_distance.py` & `geoformat-20240519/tests/geoformat/geoprocessing/measure/test_distance.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/measure/test_length.py` & `geoformat-20240519/tests/geoformat/geoprocessing/measure/test_length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_area.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_area.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_length.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_length.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_line_merge.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_line_merge.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_merge_geometries.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_merge_geometries.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_point_on_linestring.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_point_on_linestring.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_simplify.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_simplify.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_split.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_split.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/geoprocessing/test_union.py` & `geoformat-20240519/tests/geoformat/geoprocessing/test_union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/index/attributes/test_hash.py` & `geoformat-20240519/tests/geoformat/index/attributes/test_hash.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/index/geometry/test_grid.py` & `geoformat-20240519/tests/geoformat/index/geometry/test_grid.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/manipulation/test_feature_manipulation.py` & `geoformat-20240519/tests/geoformat/manipulation/test_feature_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/manipulation/test_geolayer_manipulation.py` & `geoformat-20240519/tests/geoformat/manipulation/test_geolayer_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/manipulation/test_metadata_manipulation.py` & `geoformat-20240519/tests/geoformat/manipulation/test_metadata_manipulation.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/obj/test_geometry.py` & `geoformat-20240519/tests/geoformat/obj/test_geometry.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/processing/data/join/test_join.py` & `geoformat-20240519/tests/geoformat/processing/data/join/test_join.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/processing/data/join/test_merge_objects.py` & `geoformat-20240519/tests/geoformat/processing/data/join/test_merge_objects.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/processing/data/test_clauses.py` & `geoformat-20240519/tests/geoformat/processing/data/test_clauses.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/processing/data/test_field_statistics.py` & `geoformat-20240519/tests/geoformat/processing/data/test_field_statistics.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/geoformat/processing/data/test_union.py` & `geoformat-20240519/tests/geoformat/processing/data/test_union.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/inspector/geoformat_inspector.py` & `geoformat-20240519/tests/inspector/geoformat_inspector.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/perf/compare_func.py` & `geoformat-20240519/tests/perf/compare_func.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/unit/test_separate_coordinates_dimensions.py` & `geoformat-20240519/tests/unit/test_separate_coordinates_dimensions.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/utils/compare.py` & `geoformat-20240519/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `geoformat-20240407/tests/utils/tests_utils.py` & `geoformat-20240519/tests/utils/tests_utils.py`

 * *Files identical despite different names*

