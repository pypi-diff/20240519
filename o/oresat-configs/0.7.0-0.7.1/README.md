# Comparing `tmp/oresat_configs-0.7.0.tar.gz` & `tmp/oresat_configs-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_configs-0.7.0.tar", last modified: Sun Apr 28 22:01:08 2024, max compression
+gzip compressed data, was "oresat_configs-0.7.1.tar", last modified: Sun May 19 20:46:54 2024, max compression
```

## Comparing `oresat_configs-0.7.0.tar` & `oresat_configs-0.7.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.260057 oresat_configs-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.244057 oresat_configs-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 22:01:08.260057 oresat_configs-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/build_and_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/oresat0/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/oresat0_5/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/oresat1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/scripts/gen_beacon_rst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.248057 oresat_configs-0.7.0/docs/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/yamls/beacon_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/yamls/card_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/docs/yamls/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.252057 oresat_configs-0.7.0/oresat_configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/_yaml_to_od.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.256057 oresat_configs-0.7.0/oresat_configs/base/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/adcs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/battery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17032 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/cfc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/diode_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/dxwifi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/fw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/gps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/reaction_wheel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/solar.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/star_tracker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/base/sw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/beacon_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/card_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/card_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/cards.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.256057 oresat_configs-0.7.0/oresat_configs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat0/battery_overlay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat0/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.256057 oresat_configs-0.7.0/oresat_configs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat0_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat0_5/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.256057 oresat_configs-0.7.0/oresat_configs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/oresat1/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.260057 oresat_configs-0.7.0/oresat_configs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/gen_dbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/gen_dcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/gen_fw_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/gen_xtce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/list_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/pdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/print_od.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/scripts/sdo_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/oresat_configs/standard_objects.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.260057 oresat_configs-0.7.0/oresat_configs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 22:01:08.000000 oresat_configs-0.7.0/oresat_configs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 22:01:08.260057 oresat_configs-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:01:08.260057 oresat_configs-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/tests/test_config_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/tests/test_oresat0.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/tests/test_oresat0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-28 22:01:03.000000 oresat_configs-0.7.0/tests/test_oresat1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.479317 oresat_configs-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/build_and_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/oresat0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/oresat0_5/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/oresat1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/scripts/gen_beacon_rst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.483317 oresat_configs-0.7.1/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.487317 oresat_configs-0.7.1/docs/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/yamls/beacon_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/yamls/card_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/docs/yamls/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.487317 oresat_configs-0.7.1/oresat_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28421 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/_yaml_to_od.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/adcs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/battery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17233 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/cfc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/diode_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/dxwifi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/fw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/gps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/reaction_wheel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/solar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/star_tracker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/base/sw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/beacon_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/card_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/card_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/cards.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0/battery_overlay.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat0_5/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.491317 oresat_configs-0.7.1/oresat_configs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/oresat1/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/oresat_configs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_dbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26434 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_fw_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/gen_xtce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/list_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/pdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/print_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/scripts/sdo_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/oresat_configs/standard_objects.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/oresat_configs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 20:46:54.000000 oresat_configs-0.7.1/oresat_configs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:46:54.495317 oresat_configs-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_config_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_oresat0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_oresat0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 20:46:49.000000 oresat_configs-0.7.1/tests/test_oresat1.py
```

### Comparing `oresat_configs-0.7.0/.github/workflows/pypi.yaml` & `oresat_configs-0.7.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/.github/workflows/tests.yaml` & `oresat_configs-0.7.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/.gitignore` & `oresat_configs-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/LICENSE` & `oresat_configs-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/PKG-INFO` & `oresat_configs-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.7.0
+Version: 0.7.1
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_configs-0.7.0/README.md` & `oresat_configs-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/docs/Makefile` & `oresat_configs-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/docs/conf.py` & `oresat_configs-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/docs/make.bat` & `oresat_configs-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/docs/scripts/gen_beacon_rst.py` & `oresat_configs-0.7.1/docs/scripts/gen_beacon_rst.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/docs/yamls/card_config.rst` & `oresat_configs-0.7.1/docs/yamls/card_config.rst`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/__init__.py` & `oresat_configs-0.7.1/oresat_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/__main__.py` & `oresat_configs-0.7.1/oresat_configs/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/_yaml_to_od.py` & `oresat_configs-0.7.1/oresat_configs/_yaml_to_od.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Convert OreSat configs to ODs."""
 
 import os
+from collections import namedtuple
 from copy import deepcopy
 from typing import Union
 
 import canopen
 from canopen import ObjectDictionary
 from canopen.objectdictionary import Array, Record, Variable
 from dacite import from_dict
@@ -19,15 +20,15 @@
 STD_OBJS_FILE_NAME = f"{os.path.dirname(os.path.abspath(__file__))}/standard_objects.yaml"
 
 RPDO_COMM_START = 0x1400
 RPDO_PARA_START = 0x1600
 TPDO_COMM_START = 0x1800
 TPDO_PARA_START = 0x1A00
 
-OD_DATA_TYPES = {
+STR_2_OD_DATA_TYPE = {
     "bool": canopen.objectdictionary.BOOLEAN,
     "int8": canopen.objectdictionary.INTEGER8,
     "int16": canopen.objectdictionary.INTEGER16,
     "int32": canopen.objectdictionary.INTEGER32,
     "int64": canopen.objectdictionary.INTEGER64,
     "uint8": canopen.objectdictionary.UNSIGNED8,
     "uint16": canopen.objectdictionary.UNSIGNED16,
@@ -36,46 +37,31 @@
     "float32": canopen.objectdictionary.REAL32,
     "float64": canopen.objectdictionary.REAL64,
     "str": canopen.objectdictionary.VISIBLE_STRING,
     "octet_str": canopen.objectdictionary.OCTET_STRING,
     "domain": canopen.objectdictionary.DOMAIN,
 }
 
-OD_DATA_TYPE_SIZE = {
-    canopen.objectdictionary.BOOLEAN: 8,
-    canopen.objectdictionary.INTEGER8: 8,
-    canopen.objectdictionary.INTEGER16: 16,
-    canopen.objectdictionary.INTEGER32: 32,
-    canopen.objectdictionary.INTEGER64: 64,
-    canopen.objectdictionary.UNSIGNED8: 8,
-    canopen.objectdictionary.UNSIGNED16: 16,
-    canopen.objectdictionary.UNSIGNED32: 32,
-    canopen.objectdictionary.UNSIGNED64: 64,
-    canopen.objectdictionary.REAL32: 32,
-    canopen.objectdictionary.REAL64: 64,
-    canopen.objectdictionary.VISIBLE_STRING: 0,
-    canopen.objectdictionary.OCTET_STRING: 0,
-    canopen.objectdictionary.DOMAIN: 0,
-}
+OdDataTypeInfo = namedtuple("OdDataTypeInfo", ("default", "size", "low_limit", "high_limit"))
 
-OD_DEFAULTS = {
-    canopen.objectdictionary.BOOLEAN: False,
-    canopen.objectdictionary.INTEGER8: 0,
-    canopen.objectdictionary.INTEGER16: 0,
-    canopen.objectdictionary.INTEGER32: 0,
-    canopen.objectdictionary.INTEGER64: 0,
-    canopen.objectdictionary.UNSIGNED8: 0,
-    canopen.objectdictionary.UNSIGNED16: 0,
-    canopen.objectdictionary.UNSIGNED32: 0,
-    canopen.objectdictionary.UNSIGNED64: 0,
-    canopen.objectdictionary.REAL32: 0.0,
-    canopen.objectdictionary.REAL64: 0.0,
-    canopen.objectdictionary.VISIBLE_STRING: "",
-    canopen.objectdictionary.OCTET_STRING: b"",
-    canopen.objectdictionary.DOMAIN: None,
+OD_DATA_TYPES = {
+    canopen.objectdictionary.BOOLEAN: OdDataTypeInfo(False, 8, None, None),
+    canopen.objectdictionary.INTEGER8: OdDataTypeInfo(0, 8, -(2**8) // 2, 2**8 // 2 - 1),
+    canopen.objectdictionary.INTEGER16: OdDataTypeInfo(0, 16, -(2**16) // 2, 2**16 // 2 - 1),
+    canopen.objectdictionary.INTEGER32: OdDataTypeInfo(0, 16, -(2**32) // 2, 2**32 // 2 - 1),
+    canopen.objectdictionary.INTEGER64: OdDataTypeInfo(0, 16, -(2**64) // 2, 2**64 // 2 - 1),
+    canopen.objectdictionary.UNSIGNED8: OdDataTypeInfo(0, 8, 0, 2**8 - 1),
+    canopen.objectdictionary.UNSIGNED16: OdDataTypeInfo(0, 16, 0, 2**16 - 1),
+    canopen.objectdictionary.UNSIGNED32: OdDataTypeInfo(0, 32, 0, 2**32 - 1),
+    canopen.objectdictionary.UNSIGNED64: OdDataTypeInfo(0, 64, 0, 2**64 - 1),
+    canopen.objectdictionary.REAL32: OdDataTypeInfo(0.0, 32, None, None),
+    canopen.objectdictionary.REAL64: OdDataTypeInfo(0.0, 64, None, None),
+    canopen.objectdictionary.VISIBLE_STRING: OdDataTypeInfo("", 0, None, None),
+    canopen.objectdictionary.OCTET_STRING: OdDataTypeInfo(b"", 0, None, None),
+    canopen.objectdictionary.DOMAIN: OdDataTypeInfo(None, 0, None, None),
 }
 
 DYNAMIC_LEN_DATA_TYPES = [
     canopen.objectdictionary.VISIBLE_STRING,
     canopen.objectdictionary.OCTET_STRING,
     canopen.objectdictionary.DOMAIN,
 ]
@@ -84,15 +70,15 @@
 def _set_var_default(obj: ConfigObject, var: Variable) -> None:
     """Set the variables default value based off of configs."""
 
     default = obj.default
     if obj.data_type == "octet_str":
         default = b"\x00" * obj.length
     elif default is None:
-        default = OD_DEFAULTS[var.data_type]
+        default = OD_DATA_TYPES[var.data_type].default
     elif var.data_type in canopen.objectdictionary.INTEGER_TYPES and isinstance(default, str):
         # remove node id
         if "+$NODE_ID" in default:
             default = default.split("+")[0]
         elif "$NODE_ID+" in default:
             default = var.default.split("+")[1]
 
@@ -111,20 +97,24 @@
     for name, bits in obj.bit_definitions.items():
         var.add_bit_definition(name, bits)
     for name, value in obj.value_descriptions.items():
         var.add_value_description(value, name)
     var.unit = obj.unit
     if obj.scale_factor != 1:
         var.factor = obj.scale_factor
-    var.data_type = OD_DATA_TYPES[obj.data_type]
+    var.data_type = STR_2_OD_DATA_TYPE[obj.data_type]
     _set_var_default(obj, var)
     if var.data_type not in DYNAMIC_LEN_DATA_TYPES:
         var.pdo_mappable = True
-    var.high_limit = obj.high_limit
-    var.low_limit = obj.low_limit
+    if obj.value_descriptions:
+        var.max = obj.high_limit or max(obj.value_descriptions.values())
+        var.min = obj.low_limit or min(obj.value_descriptions.values())
+    else:
+        var.max = obj.high_limit or OD_DATA_TYPES[var.data_type].high_limit
+        var.min = obj.low_limit or OD_DATA_TYPES[var.data_type].low_limit
     return var
 
 
 def _make_rec(obj: IndexObject) -> Record:
     index = obj.index
     rec = canopen.objectdictionary.Record(obj.name, index)
 
@@ -152,41 +142,47 @@
     var0 = canopen.objectdictionary.Variable("highest_index_supported", index, 0x0)
     var0.access_type = "const"
     var0.data_type = canopen.objectdictionary.UNSIGNED8
     arr.add_member(var0)
 
     subindexes = []
     names = []
-    generate_subindexes = obj.generate_subindexes
-    if generate_subindexes is None:
+    gen_sub = obj.generate_subindexes
+    if gen_sub is None:
         raise ValueError("IndexObject for array missing generate_subindexes: {obj}")
 
-    if generate_subindexes.subindexes == "fixed_length":
-        subindexes = list(range(1, generate_subindexes.length + 1))
+    if gen_sub.subindexes == "fixed_length":
+        subindexes = list(range(1, gen_sub.length + 1))
         names = [obj.name + f"_{subindex}" for subindex in subindexes]
-    elif generate_subindexes.subindexes == "node_ids":
+    elif gen_sub.subindexes == "node_ids":
         for name, sub in node_ids.items():
             if sub == 0:
                 continue  # a node_id of 0 is flag for not on can bus
             names.append(name)
             subindexes.append(sub)
 
     for subindex, name in zip(subindexes, names):
         if subindex in arr.subindices:
             raise ValueError(f"subindex 0x{subindex:X} aleady in record at array 0x{index:X}")
         var = canopen.objectdictionary.Variable(name, index, subindex)
-        var.access_type = generate_subindexes.access_type
-        var.data_type = OD_DATA_TYPES[generate_subindexes.data_type]
-        for name, bits in generate_subindexes.bit_definitions.items():
+        var.access_type = gen_sub.access_type
+        var.data_type = STR_2_OD_DATA_TYPE[gen_sub.data_type]
+        for name, bits in gen_sub.bit_definitions.items():
             var.add_bit_definition(name, bits)
-        for name, value in generate_subindexes.value_descriptions.items():
+        for name, value in gen_sub.value_descriptions.items():
             var.add_value_description(value, name)
-        var.unit = generate_subindexes.unit
-        var.factor = generate_subindexes.scale_factor
-        _set_var_default(generate_subindexes, var)
+        var.unit = gen_sub.unit
+        var.factor = gen_sub.scale_factor
+        if obj.value_descriptions:
+            var.max = gen_sub.high_limit or max(gen_sub.value_descriptions.values())
+            var.min = gen_sub.low_limit or min(gen_sub.value_descriptions.values())
+        else:
+            var.max = gen_sub.high_limit or OD_DATA_TYPES[var.data_type].high_limit
+            var.min = gen_sub.low_limit or OD_DATA_TYPES[var.data_type].low_limit
+        _set_var_default(gen_sub, var)
         if var.data_type not in DYNAMIC_LEN_DATA_TYPES:
             var.pdo_mappable = True
         arr.add_member(var)
         var0.default = subindex
 
     return arr
 
@@ -246,15 +242,15 @@
             elif len(t_field) == 2:
                 mapped_obj = od[t_field[0]][t_field[1]]
             else:
                 raise ValueError("tpdo field must be a 1 or 2 values")
             mapped_subindex = mapped_obj.subindex
             value = mapped_obj.index << 16
             value += mapped_subindex << 8
-            value += OD_DATA_TYPE_SIZE[mapped_obj.data_type]
+            value += OD_DATA_TYPES[mapped_obj.data_type].size
             var.default = value
             map_rec.add_member(var)
 
         var0.default = len(map_rec) - 1
 
         # index 0 for comms index
         var0 = canopen.objectdictionary.Variable("highest_index_supported", comm_index, 0x0)
@@ -405,14 +401,16 @@
             var.access_type = "rw"
             var.data_type = tpdo_mapped_obj.data_type
             var.default = tpdo_mapped_obj.default
             var.unit = tpdo_mapped_obj.unit
             var.factor = tpdo_mapped_obj.factor
             var.bit_definitions = deepcopy(tpdo_mapped_obj.bit_definitions)
             var.value_descriptions = deepcopy(tpdo_mapped_obj.value_descriptions)
+            var.max = tpdo_mapped_obj.max
+            var.min = tpdo_mapped_obj.min
             var.pdo_mappable = True
             rpdo_mapped_rec.add_member(var)
 
         # master node mapping obj
         rpdo_mapping_subindex = rpdo_mapping_rec[0].default + 1
         var = canopen.objectdictionary.Variable(
             f"mapping_object_{rpdo_mapping_subindex}",
@@ -423,15 +421,15 @@
         var.data_type = canopen.objectdictionary.UNSIGNED32
         value = rpdo_mapped_index << 16
         value += rpdo_mapped_subindex << 8
         if rpdo_mapped_subindex == 0:
             rpdo_mapped_obj = rpdo_node_od[rpdo_mapped_index]
         else:
             rpdo_mapped_obj = rpdo_node_od[rpdo_mapped_index][rpdo_mapped_subindex]
-        value += OD_DATA_TYPE_SIZE[rpdo_mapped_obj.data_type]
+        value += OD_DATA_TYPES[rpdo_mapped_obj.data_type].size
         var.default = value
         rpdo_mapping_rec.add_member(var)
 
         # update these
         if not time_sync_tpdo:
             rpdo_mapped_rec[0].default += 1
         rpdo_mapping_rec[0].default += 1
@@ -493,22 +491,26 @@
             if obj.index != obj2.index:
                 continue
 
             obj2.name = obj.name
             if obj.object_type == "variable":
                 obj2.data_type = obj.data_type
                 obj2.access_type = obj.access_type
+                obj2.high_limit = obj.high_limit
+                obj2.low_limit = obj.low_limit
             else:
                 for sub_obj in obj.subindexes:
                     sub_overlayed = False
                     for sub_obj2 in obj2.subindexes:
                         if sub_obj.subindex == sub_obj2.subindex:
                             sub_obj2.name = sub_obj.name
                             sub_obj2.data_type = sub_obj.data_type
                             sub_obj2.access_type = sub_obj.access_type
+                            sub_obj2.high_limit = sub_obj.high_limit
+                            sub_obj2.low_limit = sub_obj.low_limit
                             overlayed = True
                             sub_overlayed = True
                             break  # obj was found, search for next one
                     if not sub_overlayed:  # add it
                         obj2.subindexes.append(deepcopy(sub_obj))
             overlayed = True
             break  # obj was found, search for next one
@@ -658,34 +660,38 @@
 
 def _gen_c3_fram_defs(c3_od: ObjectDictionary, config: CardConfig) -> list[Variable]:
     """Get the list of objects in saved to fram."""
 
     fram_objs = []
 
     for fields in config.fram:
+        obj = None
         if len(fields) == 1:
             obj = c3_od[fields[0]]
         elif len(fields) == 2:
             obj = c3_od[fields[0]][fields[1]]
-        fram_objs.append(obj)
+        if obj is not None:
+            fram_objs.append(obj)
 
     return fram_objs
 
 
 def _gen_c3_beacon_defs(c3_od: ObjectDictionary, beacon_def: BeaconConfig) -> list[Variable]:
     """Get the list of objects in the beacon from OD."""
 
     beacon_objs = []
 
     for fields in beacon_def.fields:
+        obj = None
         if len(fields) == 1:
             obj = c3_od[fields[0]]
         elif len(fields) == 2:
             obj = c3_od[fields[0]][fields[1]]
-        beacon_objs.append(obj)
+        if obj is not None:
+            beacon_objs.append(obj)
 
     return beacon_objs
 
 
 def _gen_fw_base_od(mission: Consts, config_path: str) -> canopen.ObjectDictionary:
     """Generate all ODs for a OreSat mission."""
```

### Comparing `oresat_configs-0.7.0/oresat_configs/base/__init__.py` & `oresat_configs-0.7.1/oresat_configs/base/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/adcs.yaml` & `oresat_configs-0.7.1/oresat_configs/base/adcs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/battery.yaml` & `oresat_configs-0.7.1/oresat_configs/base/battery.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/c3.yaml` & `oresat_configs-0.7.1/oresat_configs/base/c3.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     value_descriptions:
       pre_deply: 66
       deploy: 67
       standby: 68
       beacon: 69
       edl: 70
     access_type: ro
+    default: 66
 
   - index: 0x4001
     name: reset_timeout
     data_type: uint32
     description: the reset system timeout
     access_type: const
     default: 86400 # 24 hours
@@ -250,15 +251,15 @@
         length: 32
 
       - subindex: 0x5
         name: active_crypto_key
         data_type: uint8
         description: selected edl crypto key
         access_type: ro
-        high_level: 3
+        high_limit: 3
 
       - subindex: 0x6
         name: sequence_count
         data_type: uint32
         description: edl sequence count
         access_type: ro
 
@@ -389,14 +390,21 @@
       - subindex: 0xc
         name: node_reset_attempts
         data_type: uint8
         description: number of reset attempts for a opd node before it is considered dead
         access_type: rw
         default: 3
 
+      - subindex: 0xd
+        name: uart_node_select
+        data_type: uint8
+        description: select a node to connect to UART or 0 for no node
+        access_type: rw
+        default: 0
+
   - index: 0x400a
     name: beacon
     object_type: record
     subindexes:
       - subindex: 0x1
         name: revision
         data_type: uint8
@@ -596,21 +604,21 @@
           none: 0
           standby: 1
           hold: 2
           calibrate: 3
           spindown: 4
           detumble: 5
           bbq: 6
-          point: 7 
+          point: 7
           manual: 8
-      
+
       - subindex: 0x2
         name: status
         data_type: uint8
-        description: adcs service status 
+        description: adcs service status
         access_type: ro
         value_descriptions:
           none: 0
           idle: 1
           starting: 2
           mission: 3
           degraded: 4
```

### Comparing `oresat_configs-0.7.0/oresat_configs/base/cfc.yaml` & `oresat_configs-0.7.1/oresat_configs/base/cfc.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/dxwifi.yaml` & `oresat_configs-0.7.1/oresat_configs/base/dxwifi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/fw_common.yaml` & `oresat_configs-0.7.1/oresat_configs/base/fw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/gps.yaml` & `oresat_configs-0.7.1/oresat_configs/base/gps.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -37,52 +37,60 @@
         high_limit: 12
 
       - subindex: 0x3
         name: gps_week
         data_type: uint16
         description: gps week number
         access_type: ro
+        high_limit: 1023
 
       - subindex: 0x4
         name: tow
         data_type: uint32
         description: time of the week
         access_type: ro
         scale_factor: 0.01
         unit: s
+        high_limit: 60480000
 
       - subindex: 0x5
         name: latitude
         data_type: int32
         description: latitude
         access_type: ro
         scale_factor: 0.0000001 # 1e-7
         unit: deg
+        low_limit: -900000000
+        high_limit: 900000000
 
       - subindex: 0x6
         name: longitude
         data_type: int32
         description: longitude
         access_type: ro
         scale_factor: 0.0000001 # 1e-7
         unit: deg
+        low_limit: -1800000000
+        high_limit: 1800000000
 
       - subindex: 0x7
         name: ellipsoid_alt
         data_type: uint32
         description: height above ellipsoid
         access_type: ro
-        unit: cm
+        unit: km
+        scale_factor: 0.00001 # cm to km
 
       - subindex: 0x8
         name: mean_sea_lvl_alt
         data_type: uint32
         description: mean sea level
         access_type: ro
-        unit: cm
+        unit: km
+        scale_factor: 0.00001 # cm to km
 
       - subindex: 0x9
         name: gdop
         data_type: uint16
         description: geometric diluttion of precision
         access_type: ro
         scale_factor: 0.01
@@ -116,50 +124,56 @@
         scale_factor: 0.01
 
       - subindex: 0xe
         name: ecef_x
         data_type: int32
         description: ecef x coordinate
         access_type: ro
-        unit: cm
+        unit: km
+        scale_factor: 0.00001 # cm to km
 
       - subindex: 0xf
         name: ecef_y
         data_type: int32
         description: ecef y coordinate
         access_type: ro
-        unit: cm
+        unit: km
+        scale_factor: 0.00001 # cm to km
 
       - subindex: 0x10
         name: ecef_z
         data_type: int32
         description: ecef z coordinate
         access_type: ro
-        unit: cm
+        unit: km
+        scale_factor: 0.00001 # cm to km
 
       - subindex: 0x11
         name: ecef_vx
         data_type: int32
         description: ecef x velocity
         access_type: ro
-        unit: cm/s
+        unit: km/s
+        scale_factor: 0.00001 # cm/s to km/s
 
       - subindex: 0x12
         name: ecef_vy
         data_type: int32
         description: ecef y velocity
         access_type: ro
-        unit: cm/s
+        unit: km/s
+        scale_factor: 0.00001 # cm/s to km/s
 
       - subindex: 0x13
         name: ecef_vz
         data_type: int32
         description: ecef z velocity
         access_type: ro
-        unit: cm/s
+        unit: km/s
+        scale_factor: 0.00001 # cm/s to km/s
 
       - subindex: 0x14
         name: time_since_midnight
         data_type: uint32
         description: time since midnight when the gps data was received
         access_type: ro
         unit: ms
```

### Comparing `oresat_configs-0.7.0/oresat_configs/base/reaction_wheel.yaml` & `oresat_configs-0.7.1/oresat_configs/base/reaction_wheel.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/solar.yaml` & `oresat_configs-0.7.1/oresat_configs/base/solar.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/star_tracker.yaml` & `oresat_configs-0.7.1/oresat_configs/base/star_tracker.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/base/sw_common.yaml` & `oresat_configs-0.7.1/oresat_configs/base/sw_common.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -65,34 +65,35 @@
     object_type: record
     subindexes:
       - subindex: 0x1
         name: reset
         data_type: uint8
         description: reset the app
         value_descriptions:
+          no_stop: 0
           soft_reset: 1
           hard_reset: 2
           factory_reset: 3
           poweroff: 4
         access_type: wo
 
       - subindex: 0x2
         name: storage_percent
         data_type: uint8
         description: the current storage percent used
         access_type: ro
-        high_level: 100
+        high_limit: 100
         unit: "%"
 
       - subindex: 0x3
         name: ram_percent
         data_type: uint8
         description: the current ram percent used
         access_type: ro
-        high_level: 100
+        high_limit: 100
         unit: "%"
 
       - subindex: 0x4
         name: unix_time
         data_type: uint32
         description: unix time
         access_type: ro
@@ -109,15 +110,15 @@
         name: power_cycles
         data_type: uint16
         description: the number of power cycles
         access_type: ro
 
       # subindex 0x7 reserved for temperature
       # subindex 0x8 reserved for vrefint
-      
+
       - subindex: 0x9
         name: boot_select
         data_type: uint8
         bit_definitions:
           CURRENT_BOOT: 0
           NEXT_BOOT: 1
         access_type: ro
```

### Comparing `oresat_configs-0.7.0/oresat_configs/beacon_config.py` & `oresat_configs-0.7.1/oresat_configs/beacon_config.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/card_config.py` & `oresat_configs-0.7.1/oresat_configs/card_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,25 @@
     description: str = ""
     """Description of object."""
     value_descriptions: dict[str, int] = field(default_factory=dict)
     """Optional: Can be used to define enum values for an unsigned integer data types."""
     bit_definitions: dict[str, Union[int, str]] = field(default_factory=dict)
     """Optional: Can be used to define bitfield of an unsigned integer data types."""
     unit: str = ""
-    """Optional unit for the object."""
+    """Optional engineering unit for the object."""
     scale_factor: float = 1
-    """Can be used to scale a integer value to a float."""
+    """Can be used to scale a integer value to a engineering (float) value."""
     low_limit: Optional[int] = None
     """
-    The lower limit for value. No need to set this if it limit is the lower limit of the data type.
+    The lower raw limit for value. No need to set this if it limit is the lower limit of the data
+    type.
     """
     high_limit: Optional[int] = None
     """
-    The higher limit for value. No need to set this if it limit is the higher limit of the data
+    The higher raw limit for value. No need to set this if it limit is the higher limit of the data
     type.
     """
 
 
 @dataclass
 class GenerateSubindex(ConfigObject):
     """
```

### Comparing `oresat_configs-0.7.0/oresat_configs/card_info.py` & `oresat_configs-0.7.1/oresat_configs/card_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     file_path = f"{os.path.dirname(os.path.abspath(__file__))}/cards.csv"
     with open(file_path, "r") as f:
         reader = csv.DictReader(f)
         cols = set(reader.fieldnames) if reader.fieldnames else set()
         expect = {f.name for f in fields(Card)}
         expect.add("name")  # the 'name' column is the keys of the returned dict; not in Card
         if cols - expect:
-            raise TypeError(f"cards.csv has excess columns: {cols-expect}. Update class Card?")
+            raise TypeError(f"cards.csv has excess columns: {cols - expect}. Update class Card?")
         if expect - cols:
-            raise TypeError(f"class Card expects more columns than cards.csv has: {expect-cols}")
+            raise TypeError(f"class Card expects more columns than cards.csv has: {expect - cols}")
 
         return {
             row["name"]: Card(
                 row["nice_name"],
                 int(row["node_id"], 16),
                 row["processor"],
                 int(row["opd_address"], 16),
```

### Comparing `oresat_configs-0.7.0/oresat_configs/cards.csv` & `oresat_configs-0.7.1/oresat_configs/cards.csv`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/constants.py` & `oresat_configs-0.7.1/oresat_configs/constants.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/oresat0/__init__.py` & `oresat_configs-0.7.1/oresat_configs/oresat0/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/oresat0/battery_overlay.yaml` & `oresat_configs-0.7.1/oresat_configs/oresat0/battery_overlay.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/oresat0/beacon.yaml` & `oresat_configs-0.7.1/oresat_configs/oresat0/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/oresat0_5/__init__.py` & `oresat_configs-0.7.1/oresat_configs/oresat0_5/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/oresat0_5/beacon.yaml` & `oresat_configs-0.7.1/oresat_configs/oresat0_5/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/oresat1/__init__.py` & `oresat_configs-0.7.1/oresat_configs/oresat1/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/gen_dbc.py` & `oresat_configs-0.7.1/oresat_configs/scripts/gen_dbc.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/gen_dcf.py` & `oresat_configs-0.7.1/oresat_configs/scripts/gen_dcf.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/gen_fw_files.py` & `oresat_configs-0.7.1/oresat_configs/scripts/gen_fw_files.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/gen_xtce.py` & `oresat_configs-0.7.1/oresat_configs/scripts/gen_xtce.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/list_cards.py` & `oresat_configs-0.7.1/oresat_configs/scripts/list_cards.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/pdo.py` & `oresat_configs-0.7.1/oresat_configs/scripts/pdo.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/print_od.py` & `oresat_configs-0.7.1/oresat_configs/scripts/print_od.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from argparse import ArgumentParser, Namespace
 from typing import Any, Optional
 
 import canopen
 
 from .. import Consts, OreSatConfig
-from .._yaml_to_od import OD_DATA_TYPES
+from .._yaml_to_od import STR_2_OD_DATA_TYPE
 
 PRINT_OD = "print the object dictionary out to stdout"
 
 
 def build_parser(parser: ArgumentParser) -> ArgumentParser:
     """Configures an ArgumentParser suitable for this script.
 
@@ -55,15 +55,15 @@
     """The print-od main"""
     if args is None:
         args = build_parser(ArgumentParser()).parse_args()
 
     config = OreSatConfig(args.oresat)
 
     inverted_od_data_types = {}
-    for key, value in OD_DATA_TYPES.items():
+    for key, value in STR_2_OD_DATA_TYPE.items():
         inverted_od_data_types[value] = key
 
     arg_card = args.card.lower().replace("-", "_")
 
     od = config.od_db[arg_card]
     for i in od:
         if isinstance(od[i], canopen.objectdictionary.Variable):
```

### Comparing `oresat_configs-0.7.0/oresat_configs/scripts/sdo_transfer.py` & `oresat_configs-0.7.1/oresat_configs/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs/standard_objects.yaml` & `oresat_configs-0.7.1/oresat_configs/standard_objects.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/oresat_configs.egg-info/PKG-INFO` & `oresat_configs-0.7.1/oresat_configs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.7.0
+Version: 0.7.1
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_configs-0.7.0/oresat_configs.egg-info/SOURCES.txt` & `oresat_configs-0.7.1/oresat_configs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/pyproject.toml` & `oresat_configs-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.7.0/tests/__init__.py` & `oresat_configs-0.7.1/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import unittest
 
 import canopen
 
 from oresat_configs import Consts, OreSatConfig
-from oresat_configs._yaml_to_od import OD_DATA_TYPE_SIZE, TPDO_COMM_START, TPDO_PARA_START
+from oresat_configs._yaml_to_od import OD_DATA_TYPES, TPDO_COMM_START, TPDO_PARA_START
 
 
 class TestConfig(unittest.TestCase):
     """Base class to test a OreSat OD databases."""
 
     def setUp(self) -> None:
         self.oresatid = Consts.ORESAT0
@@ -41,15 +41,15 @@
                     mapped_obj = od[mapped_index]
                     if not isinstance(mapped_obj, canopen.objectdictionary.Variable):
                         mapped_obj = mapped_obj[mapped_subindex]
                     self.assertTrue(
                         mapped_obj.pdo_mappable,
                         f"{self.oresatid.name} {name} {mapped_obj.name} is not pdo mappable",
                     )
-                    size += OD_DATA_TYPE_SIZE[mapped_obj.data_type]
+                    size += OD_DATA_TYPES[mapped_obj.data_type].size
                 self.assertLessEqual(
                     size, 64, f"{self.oresatid.name} {name} TPDO{i + 1} is more than 64 bits"
                 )
                 tpdos += 1
 
             # test the number of TPDOs
             if od.device_information.product_name == "c3":
@@ -73,15 +73,15 @@
                 length += len(obj.default)  # start_chars is required and static
             else:
                 self.assertNotIn(
                     obj.data_type,
                     dynamic_len_data_types,
                     f"{self.oresatid.name} {obj.name} is a dynamic length data type",
                 )
-                length += OD_DATA_TYPE_SIZE[obj.data_type] // 8  # bits to bytes
+                length += OD_DATA_TYPES[obj.data_type].size // 8  # bits to bytes
 
         # AX.25 payload max length = 255
         # CRC32 length = 4
         self.assertLessEqual(length, 255 - 4, f"{self.oresatid.name} beacon length too long")
 
     def test_record_array_length(self) -> None:
         """Test that array/record have is less than 255 objects in it."""
@@ -97,15 +97,15 @@
         regex_str = r"^[a-z][a-z0-9_]*[a-z0-9]*$"  # snake_case with no leading/trailing num or "_"
         self.assertIsNotNone(re.match(regex_str, string), f'"{string}" is not snake_case')
 
     def _test_variable(self, obj: canopen.objectdictionary.Variable) -> None:
         """Test that a variable is valid."""
 
         self.assertIsInstance(obj, canopen.objectdictionary.Variable)
-        self.assertIn(obj.data_type, OD_DATA_TYPE_SIZE.keys())
+        self.assertIn(obj.data_type, OD_DATA_TYPES.keys())
         self.assertIn(obj.access_type, ["ro", "wo", "rw", "rwr", "rww", "const"])
         self.assertIsInstance(obj.data_type, int)
         self._test_snake_case(obj.name)
 
         if not isinstance(obj.parent, canopen.ObjectDictionary):
             node_name = obj.parent.parent.device_information.product_name
         else:
```

### Comparing `oresat_configs-0.7.0/tests/test_config_types.py` & `oresat_configs-0.7.1/tests/test_config_types.py`

 * *Files identical despite different names*

