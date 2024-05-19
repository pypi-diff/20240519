# Comparing `tmp/PyThea-0.9.0.tar.gz` & `tmp/PyThea-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyThea-0.9.0.tar", last modified: Wed Feb 28 15:53:37 2024, max compression
+gzip compressed data, was "PyThea-0.9.1.tar", last modified: Wed Mar  6 19:15:58 2024, max compression
```

## Comparing `PyThea-0.9.0.tar` & `PyThea-0.9.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.798571 PyThea-0.9.0/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     3277 2024-02-22 22:02:58.000000 PyThea-0.9.0/CHANGELOG.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    33872 2023-01-03 18:26:41.000000 PyThea-0.9.0/LICENSE.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      381 2023-01-03 18:26:41.000000 PyThea-0.9.0/MANIFEST.in
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     7728 2024-02-28 15:53:37.798331 PyThea-0.9.0/PKG-INFO
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.772814 PyThea-0.9.0/PyThea/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    22431 2024-02-22 22:02:58.000000 PyThea-0.9.0/PyThea/PyThea_app.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)       44 2023-01-25 19:20:20.000000 PyThea-0.9.0/PyThea/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      411 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea/_version.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2856 2023-01-25 22:38:03.000000 PyThea-0.9.0/PyThea/callbacks.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.777511 PyThea-0.9.0/PyThea/config/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      132 2023-01-25 22:38:03.000000 PyThea-0.9.0/PyThea/config/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2834 2024-01-30 13:44:44.000000 PyThea-0.9.0/PyThea/config/app_styles.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     4975 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/config/config_sliders.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      521 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/config/selected_bodies.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2918 2023-12-08 13:50:26.000000 PyThea-0.9.0/PyThea/config/selected_imagers.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.778292 PyThea-0.9.0/PyThea/data/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2024-02-21 01:33:31.000000 PyThea-0.9.0/PyThea/data/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      535 2024-02-21 01:33:31.000000 PyThea-0.9.0/PyThea/data/sample_data.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.779454 PyThea-0.9.0/PyThea/extensions/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1075 2023-01-25 22:38:03.000000 PyThea-0.9.0/PyThea/extensions/LICENSE_gcs_python.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/extensions/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2996 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/extensions/buttons.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    30760 2024-02-21 15:41:03.000000 PyThea-0.9.0/PyThea/geometrical_models.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    11293 2024-02-28 15:52:37.000000 PyThea-0.9.0/PyThea/modules.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     2499 2024-02-09 01:02:01.000000 PyThea-0.9.0/PyThea/pythea_cli.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.779811 PyThea-0.9.0/PyThea/sunpy_dev/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-19 20:37:41.000000 PyThea-0.9.0/PyThea/sunpy_dev/__init__.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.780033 PyThea-0.9.0/PyThea/sunpy_dev/extern/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/sunpy_dev/extern/__init__.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.780241 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/__init__.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.780660 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2024-02-22 22:02:58.000000 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      642 2024-02-22 22:02:58.000000 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/utils.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.781156 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     5402 2024-02-22 22:02:58.000000 PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.781764 PyThea-0.9.0/PyThea/sunpy_dev/map/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-03-28 18:07:04.000000 PyThea-0.9.0/PyThea/sunpy_dev/map/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     8543 2024-02-28 15:52:37.000000 PyThea-0.9.0/PyThea/sunpy_dev/map/maputils.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.784290 PyThea-0.9.0/PyThea/test/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      239 2024-02-28 15:52:35.000000 PyThea-0.9.0/PyThea/test/Pythea_test.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/test/__init__.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      439 2023-01-03 18:26:41.000000 PyThea-0.9.0/PyThea/test/conftest.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     4524 2024-01-30 13:44:44.000000 PyThea-0.9.0/PyThea/test/test_geometrical_models.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      554 2024-02-09 01:02:01.000000 PyThea-0.9.0/PyThea/test/test_imports.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     3003 2024-02-09 01:01:27.000000 PyThea-0.9.0/PyThea/test/test_remote_clients.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     3414 2024-02-28 15:52:35.000000 PyThea-0.9.0/PyThea/test/test_utils.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)    17955 2024-02-28 15:52:37.000000 PyThea-0.9.0/PyThea/utils.py
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1000 2023-01-25 22:38:03.000000 PyThea-0.9.0/PyThea/version.py
-drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-02-28 15:53:37.797449 PyThea-0.9.0/PyThea.egg-info/
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     6148 2023-05-15 13:18:05.000000 PyThea-0.9.0/PyThea.egg-info/.DS_Store
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     7728 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea.egg-info/PKG-INFO
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1477 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea.egg-info/SOURCES.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea.egg-info/dependency_links.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)       50 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea.egg-info/entry_points.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2023-01-19 20:30:28.000000 PyThea-0.9.0/PyThea.egg-info/not-zip-safe
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      184 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea.egg-info/requires.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)        7 2024-02-28 15:53:37.000000 PyThea-0.9.0/PyThea.egg-info/top_level.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     7109 2024-01-30 13:44:44.000000 PyThea-0.9.0/README.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     6303 2024-01-30 13:44:44.000000 PyThea-0.9.0/README_pypi.md
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      591 2024-02-22 22:02:58.000000 PyThea-0.9.0/environment.yml
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      107 2023-01-03 18:26:41.000000 PyThea-0.9.0/pyproject.toml
--rw-r--r--   0 kouloa1  (44305931) staff       (20)      184 2024-02-22 22:02:58.000000 PyThea-0.9.0/requirements.txt
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1058 2024-02-28 15:53:37.799403 PyThea-0.9.0/setup.cfg
--rw-r--r--   0 kouloa1  (44305931) staff       (20)     1893 2024-01-30 13:44:44.000000 PyThea-0.9.0/setup.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:58.000627 PyThea-0.9.1/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     3588 2024-03-06 19:15:51.000000 PyThea-0.9.1/CHANGELOG.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    33872 2023-01-03 18:26:41.000000 PyThea-0.9.1/LICENSE.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      381 2023-01-03 18:26:41.000000 PyThea-0.9.1/MANIFEST.in
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     7728 2024-03-06 19:15:58.000318 PyThea-0.9.1/PKG-INFO
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.983105 PyThea-0.9.1/PyThea/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    22431 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/PyThea_app.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)       44 2023-01-25 19:20:20.000000 PyThea-0.9.1/PyThea/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      411 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea/_version.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2856 2023-01-25 22:38:03.000000 PyThea-0.9.1/PyThea/callbacks.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.986455 PyThea-0.9.1/PyThea/config/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      132 2023-01-25 22:38:03.000000 PyThea-0.9.1/PyThea/config/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2834 2024-01-30 13:44:44.000000 PyThea-0.9.1/PyThea/config/app_styles.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     4975 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/config/config_sliders.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      521 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/config/selected_bodies.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2918 2023-12-08 13:50:26.000000 PyThea-0.9.1/PyThea/config/selected_imagers.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.986928 PyThea-0.9.1/PyThea/data/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2024-02-21 01:33:31.000000 PyThea-0.9.1/PyThea/data/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      535 2024-02-21 01:33:31.000000 PyThea-0.9.1/PyThea/data/sample_data.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.987645 PyThea-0.9.1/PyThea/extensions/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1075 2023-01-25 22:38:03.000000 PyThea-0.9.1/PyThea/extensions/LICENSE_gcs_python.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/extensions/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2996 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/extensions/buttons.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    30760 2024-02-21 15:41:03.000000 PyThea-0.9.1/PyThea/geometrical_models.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     9991 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/modules.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     2499 2024-02-09 01:02:01.000000 PyThea-0.9.1/PyThea/pythea_cli.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.987868 PyThea-0.9.1/PyThea/sunpy_dev/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-19 20:37:41.000000 PyThea-0.9.1/PyThea/sunpy_dev/__init__.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.988072 PyThea-0.9.1/PyThea/sunpy_dev/extern/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/sunpy_dev/extern/__init__.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.988314 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/__init__.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.988742 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      642 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/utils.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.989201 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     5402 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.989637 PyThea-0.9.1/PyThea/sunpy_dev/map/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-03-28 18:07:04.000000 PyThea-0.9.1/PyThea/sunpy_dev/map/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     8644 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/sunpy_dev/map/maputils.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.991607 PyThea-0.9.1/PyThea/test/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      239 2024-03-05 21:24:19.000000 PyThea-0.9.1/PyThea/test/Pythea_test.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        0 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/test/__init__.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      439 2023-01-03 18:26:41.000000 PyThea-0.9.1/PyThea/test/conftest.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     4524 2024-01-30 13:44:44.000000 PyThea-0.9.1/PyThea/test/test_geometrical_models.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      554 2024-02-09 01:02:01.000000 PyThea-0.9.1/PyThea/test/test_imports.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     3003 2024-02-09 01:01:27.000000 PyThea-0.9.1/PyThea/test/test_remote_clients.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     3414 2024-03-05 21:24:19.000000 PyThea-0.9.1/PyThea/test/test_utils.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)    19772 2024-03-06 19:15:51.000000 PyThea-0.9.1/PyThea/utils.py
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1000 2023-01-25 22:38:03.000000 PyThea-0.9.1/PyThea/version.py
+drwxr-xr-x   0 kouloa1  (44305931) staff       (20)        0 2024-03-06 19:15:57.999288 PyThea-0.9.1/PyThea.egg-info/
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     6148 2023-05-15 13:18:05.000000 PyThea-0.9.1/PyThea.egg-info/.DS_Store
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     7728 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea.egg-info/PKG-INFO
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1477 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea.egg-info/SOURCES.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea.egg-info/dependency_links.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)       50 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea.egg-info/entry_points.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        1 2023-01-19 20:30:28.000000 PyThea-0.9.1/PyThea.egg-info/not-zip-safe
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      184 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea.egg-info/requires.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)        7 2024-03-06 19:15:57.000000 PyThea-0.9.1/PyThea.egg-info/top_level.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     7109 2024-01-30 13:44:44.000000 PyThea-0.9.1/README.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     6303 2024-01-30 13:44:44.000000 PyThea-0.9.1/README_pypi.md
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      591 2024-03-06 19:15:51.000000 PyThea-0.9.1/environment.yml
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      107 2023-01-03 18:26:41.000000 PyThea-0.9.1/pyproject.toml
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)      184 2024-03-06 19:15:51.000000 PyThea-0.9.1/requirements.txt
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1058 2024-03-06 19:15:58.001438 PyThea-0.9.1/setup.cfg
+-rw-r--r--   0 kouloa1  (44305931) staff       (20)     1893 2024-01-30 13:44:44.000000 PyThea-0.9.1/setup.py
```

### Comparing `PyThea-0.9.0/CHANGELOG.md` & `PyThea-0.9.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# v0.9.1 (5-March-2024)
+
+## Features
+ - A utility added to load the json fitting files
+
+## Minor Changes
+- Simplifies the code structure for loading the fitting files in the app
+
+## Bug Fixes
+- Fixes a bug when passing no maps in maputils
+- Fixes a bug when corrupted fits files loaded and imager load skipped
+
 # v0.9.0 (8-Feb-2024)
 
 ## Features
 - Adds sample data methods for testing and document builds
 - Adds tests: test_get_horizons_coord, test_vso_search, test_hek_client, and test_parameter_fit_polynomial
 - Adds calibration for AIA, LASCO, and STEREO EUVI
```

### Comparing `PyThea-0.9.0/LICENSE.md` & `PyThea-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PKG-INFO` & `PyThea-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThea
-Version: 0.9.0
+Version: 0.9.1
 Summary: PyThea: A software package to reconstruct the 3D structure of CMEs and shock waves
 Home-page: https://github.com/AthKouloumvakos/PyThea
 Author: Athanasios Kouloumvakos
 Author-email: athkouloumvakos@gmail.com
 License: GPL-3.0
 Keywords: science,solar physics,solar,sun,shock waves
 Platform: any
```

### Comparing `PyThea-0.9.0/PyThea/PyThea_app.py` & `PyThea-0.9.1/PyThea/PyThea_app.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/callbacks.py` & `PyThea-0.9.1/PyThea/callbacks.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/config/app_styles.py` & `PyThea-0.9.1/PyThea/config/app_styles.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/config/config_sliders.py` & `PyThea-0.9.1/PyThea/config/config_sliders.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/config/selected_bodies.py` & `PyThea-0.9.1/PyThea/config/selected_bodies.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/config/selected_imagers.py` & `PyThea-0.9.1/PyThea/config/selected_imagers.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/data/sample_data.py` & `PyThea-0.9.1/PyThea/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/extensions/LICENSE_gcs_python.md` & `PyThea-0.9.1/PyThea/extensions/LICENSE_gcs_python.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/extensions/buttons.py` & `PyThea-0.9.1/PyThea/extensions/buttons.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/geometrical_models.py` & `PyThea-0.9.1/PyThea/geometrical_models.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/modules.py` & `PyThea-0.9.1/PyThea/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 import datetime
-import json
 
 import astropy.units as u
 import numpy as np
-import pandas as pd
 
 from PyThea.callbacks import change_fitting_sliders, change_long_lat_sliders
 from PyThea.config.config_sliders import sliders_dict as sd
 from PyThea.geometrical_models import ellipsoid, gcs, spheroid
 from PyThea.utils import get_hek_flare, model_fittings
 
 
@@ -64,37 +62,22 @@
             st.form_submit_button()
     elif initialisation == 'File':
         uploaded_file = st.sidebar.file_uploader('Provide a fitting file', accept_multiple_files=False)
         if uploaded_file:
             if uploaded_file.type != 'application/json':
                 st.sidebar.error('Unsupported file type')
                 st.stop()
-            fitting = json.loads(uploaded_file.read())
-            st.session_state.event_selected = fitting['event_selected']
-            st.session_state.date_process  = datetime.datetime.strptime(fitting['date_process'], '%Y-%m-%dT%H:%M:%S.%f')
-            st.session_state.geometrical_model = fitting['geometrical_model']['type']
-            table_indx = [datetime.datetime.strptime(t, '%Y-%m-%dT%H:%M:%S.%f') for t in fitting['geometrical_model']['parameters']['time']]
-            parameters = pd.DataFrame(fitting['geometrical_model']['parameters'], index=table_indx)
-            parameters = parameters.drop(['time'], axis=1)
-
-            if 'kinematics' in fitting:
-                kinematics = fitting['kinematics']
-            else:
-                # TODO: Remove this in version 1.0.0
-                st.warning('**Warning:** The .json fitting file does not contain the "kinematics" information. \
-                            This means that the file was prodused using Pythea with <V0.6.0. \
-                            **To resolve this:** Just do a save of the loaded fitting now and replace \
-                            the old file with the new one. This will not alter your fittings.')
-                kinematics = {'fit_method': {'type': 'polynomial', 'order': 1}}
-
-            st.session_state.model_fittings = model_fittings(fitting['event_selected'],
-                                                             fitting['date_process'],
-                                                             fitting['geometrical_model']['type'],
-                                                             parameters,
-                                                             kinematics=kinematics)
+
+            st.session_state.model_fittings = model_fittings.load_from_json(uploaded_file)
+
+            st.session_state.event_selected = st.session_state.model_fittings.event_selected
+            st.session_state.date_process  = \
+                datetime.datetime.strptime(st.session_state.model_fittings.date_process, '%Y-%m-%dT%H:%M:%S.%f')
+            st.session_state.geometrical_model = st.session_state.model_fittings.geometrical_model
+
             st.rerun()
 
 
 def fitting_and_slider_options_container(st):
     container = st.sidebar.container()
 
     with container.expander('Options'):
```

### Comparing `PyThea-0.9.0/PyThea/pythea_cli.py` & `PyThea-0.9.1/PyThea/pythea_cli.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/utils.py` & `PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/lasco/utils.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py` & `PyThea-0.9.1/PyThea/sunpy_dev/extern/sunkit_instruments/stereo/utils.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/sunpy_dev/map/maputils.py` & `PyThea-0.9.1/PyThea/sunpy_dev/map/maputils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
     Returns
     -------
     `~sunpy.map.GenericMap`
         A SunPy map.
     """
 
+    if len(map_sequence) == 0:
+        return []
+
     normalized = True if True in [tmap.exposure_time == 1.0*u.second for tmap in map_sequence] else False
     if not normalized:
         warnings.warn('Warning [maps_sequence_processing]: The exposure time of the maps is not normalized.')
 
     smap = []
     if seq_type == 'Running Diff.':
         for i in range(1, len(map_sequence)):
@@ -128,14 +131,17 @@
     Returns
     -------
     `~sunpy.map.GenericMap`
         A SunPy map.
 
     '''
 
+    if len(map_sequence) == 0:
+        return []
+
     if 'exposure' in kwargs.keys():
         map_sequence = [tmap for tmap in map_sequence if tmap.exposure_time > kwargs['exposure']*u.second]
 
     if 'dimensions' in kwargs.keys():
         map_sequence = [tmap for tmap in map_sequence if (tmap.dimensions[0], tmap.dimensions[1]) == kwargs['dimensions']]
 
     if 'polar' in kwargs.keys():
@@ -165,20 +171,21 @@
 
     Returns
     -------
     `~sunpy.map.GenericMap`
         A SunPy map.
 
     '''
-    detector = map_sequence[0].detector
-    print(f'Preparing image sequence for {detector}.')
 
     if len(map_sequence) == 0:
         return []
 
+    detector = map_sequence[0].detector
+    print(f'Preparing image sequence for {detector}.')
+
     # Prepare the maps before anything else
     if detector == 'AIA':
         map_sequence = [update_pointing(tmap) for tmap in map_sequence]
         map_sequence = [fix_observer_location(tmap) for tmap in map_sequence]
     elif detector == 'COR1':
         if 'polar' not in kwargs.keys():
             map_sequence = PyThea.sunpy_dev.extern.sunkit_instruments.stereo.utils.cor_polariz(map_sequence)
```

### Comparing `PyThea-0.9.0/PyThea/test/test_geometrical_models.py` & `PyThea-0.9.1/PyThea/test/test_geometrical_models.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/test/test_imports.py` & `PyThea-0.9.1/PyThea/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/test/test_remote_clients.py` & `PyThea-0.9.1/PyThea/test/test_remote_clients.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/test/test_utils.py` & `PyThea-0.9.1/PyThea/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea/utils.py` & `PyThea-0.9.1/PyThea/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 import datetime
 import io
 import json
 import os
 import re
+import warnings
 from copy import copy
 from pathlib import Path
 
 import astropy.units as u
 import matplotlib.colors as colors
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
@@ -130,32 +131,34 @@
 def download_fits(date_process, imager, time_range=[-1, 1]):
     '''
     Downloads the imaging data (fits files) from VSO
     '''
     timerange = a.Time(date_process + datetime.timedelta(hours=time_range[0]),
                        date_process + datetime.timedelta(hours=time_range[1]))
 
-    map_ = {}
+    maps_ = []
     args = imager_dict[imager][0]
     result = Fido.search(timerange, *args)
     print(result)
     if result:
         downloaded_files = Fido.fetch(result, path=f'{database_dir}'+'/data/{source}/{instrument}/'+'/{file}')
-        try:
-            map_ = sunpy.map.Map(downloaded_files)
-        except RuntimeError as err:
-            print('Handling RuntimeError error:', err)
-            map_ = []
-        except OSError as err:
-            print('Handling OSError error:', err)
-            map_ = []
-    else:
-        map_ = []
+        for file_path in downloaded_files:
+            try:
+                map_ = sunpy.map.Map(file_path)
+                maps_.append(map_)
+            except RuntimeError as err:
+                print('Handling RuntimeError error:', err)
+            except OSError as err:
+                print('Handling OSError error:', err)
+                os.remove(file_path)
+                print(f"File '{file_path}' has been removed.")
+        if maps_:
+            maps_ = sunpy.map.Map(maps_, sequence=True)
 
-    return map_
+    return maps_
 
 
 def maps_process(maps_dict_in, imagers_list_in, image_mode, **kwargs):
     '''
     Process the images for the selected imagers and return the final maps and the list of imagers loaded.
 
     Note
@@ -203,14 +206,44 @@
     def __init__(self, event_selected, date_process, geometrical_model, model_parameters, kinematics={'fit_method': None}):
         self.event_selected = event_selected
         self.date_process = date_process
         self.geometrical_model = geometrical_model
         self.parameters = model_parameters
         self.kinematics = kinematics
 
+    @staticmethod
+    def load_from_json(json_file):
+        if isinstance(json_file, str):
+            with open(json_file, 'r') as file:
+                json_content = file.read()
+                fitting = json.loads(json_content)
+        else:
+            fitting = json.loads(json_file.read())
+
+        table_indx = [datetime.datetime.strptime(t, '%Y-%m-%dT%H:%M:%S.%f') for t in fitting['geometrical_model']['parameters']['time']]
+        parameters = pd.DataFrame(fitting['geometrical_model']['parameters'], index=table_indx)
+        parameters = parameters.drop(['time'], axis=1)
+        if 'kinematics' in fitting:
+            kinematics = fitting['kinematics']
+        else:
+            # TODO: Remove this in version 1.0.0
+            warnings.warn('The .json fitting file does not contain the "kinematics" information. \n \
+                            This means that the file was prodused using Pythea with <V0.6.0. \n \
+                            To resolve this: Just do a save of the loaded fitting now and replace \n \
+                            the old file with the new one. This will not alter your fittings.')
+            kinematics = {'fit_method': {'type': 'polynomial', 'order': 1}}
+
+        model_fittings_class = model_fittings(fitting['event_selected'],
+                                              fitting['date_process'],
+                                              fitting['geometrical_model']['type'],
+                                              parameters,
+                                              kinematics=kinematics)
+
+        return model_fittings_class
+
     def model_id(self):
         str_id = self.event_selected.replace('-', '').replace(':', '').replace('|', 'D').replace('.', 'p') + 'M' + self.geometrical_model
         return str_id
 
     def to_dict(self):
         parameters = copy(self.parameters)
         parameters['time'] = parameters.index.strftime('%Y-%m-%dT%H:%M:%S.%f')
```

### Comparing `PyThea-0.9.0/PyThea/version.py` & `PyThea-0.9.1/PyThea/version.py`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea.egg-info/.DS_Store` & `PyThea-0.9.1/PyThea.egg-info/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/PyThea.egg-info/PKG-INFO` & `PyThea-0.9.1/PyThea.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyThea
-Version: 0.9.0
+Version: 0.9.1
 Summary: PyThea: A software package to reconstruct the 3D structure of CMEs and shock waves
 Home-page: https://github.com/AthKouloumvakos/PyThea
 Author: Athanasios Kouloumvakos
 Author-email: athkouloumvakos@gmail.com
 License: GPL-3.0
 Keywords: science,solar physics,solar,sun,shock waves
 Platform: any
```

### Comparing `PyThea-0.9.0/PyThea.egg-info/SOURCES.txt` & `PyThea-0.9.1/PyThea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/README.md` & `PyThea-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/README_pypi.md` & `PyThea-0.9.1/README_pypi.md`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/environment.yml` & `PyThea-0.9.1/environment.yml`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/setup.cfg` & `PyThea-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `PyThea-0.9.0/setup.py` & `PyThea-0.9.1/setup.py`

 * *Files identical despite different names*

