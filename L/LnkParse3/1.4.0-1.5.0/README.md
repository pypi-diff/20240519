# Comparing `tmp/LnkParse3-1.4.0.tar.gz` & `tmp/lnkparse3-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LnkParse3-1.4.0.tar", last modified: Tue Mar 19 18:12:35 2024, max compression
+gzip compressed data, was "lnkparse3-1.5.0.tar", last modified: Sun May 19 11:36:46 2024, max compression
```

## Comparing `LnkParse3-1.4.0.tar` & `lnkparse3-1.5.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.888342 LnkParse3-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.880342 LnkParse3-1.4.0/LnkParse3/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.884342 LnkParse3-1.4.0/LnkParse3/extra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/code_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/darwin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/distributed_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/known_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/lnk_extra_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/shell_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/shim_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/special_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/extra_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.884342 LnkParse3-1.4.0/LnkParse3/info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/info/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/info/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/info_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21952 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/lnk_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/lnk_header.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/lnk_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/lnk_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/string_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.888342 LnkParse3-1.4.0/LnkParse3/target/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/common_places_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/compressed_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/control_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/internet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/lnk_target_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/my_computer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/network_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/printers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/root_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/shell_fs_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target/users_files_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/target_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/text_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/LnkParse3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.888342 LnkParse3-1.4.0/LnkParse3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-03-19 18:12:35.000000 LnkParse3-1.4.0/LnkParse3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-19 18:12:35.000000 LnkParse3-1.4.0/LnkParse3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 18:12:35.000000 LnkParse3-1.4.0/LnkParse3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-19 18:12:35.000000 LnkParse3-1.4.0/LnkParse3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 18:12:35.000000 LnkParse3-1.4.0/LnkParse3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-03-19 18:12:35.888342 LnkParse3-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7562 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 18:12:35.888342 LnkParse3-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:12:35.888342 LnkParse3-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-03-19 18:12:27.000000 LnkParse3-1.4.0/tests/test_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.596823 lnkparse3-1.5.0/LnkParse3/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/LnkParse3/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/code_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/darwin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/distributed_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/known_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/lnk_extra_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17056 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/shell_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/shim_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/special_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/extra_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/LnkParse3/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/info/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/info/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/info_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15029 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/lnk_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19807 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/lnk_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/lnk_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/lnk_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/string_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/LnkParse3/target/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/common_places_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/compressed_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/control_panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/internet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/lnk_target_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/my_computer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/network_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/printers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/root_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/shell_fs_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target/users_files_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/target_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/text_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/LnkParse3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/LnkParse3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-19 11:36:46.000000 lnkparse3-1.5.0/LnkParse3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-19 11:36:46.000000 lnkparse3-1.5.0/LnkParse3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:36:46.000000 lnkparse3-1.5.0/LnkParse3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 11:36:46.000000 lnkparse3-1.5.0/LnkParse3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 11:36:46.000000 lnkparse3-1.5.0/LnkParse3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 11:36:46.000000 lnkparse3-1.5.0/LnkParse3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:36:46.600823 lnkparse3-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-05-19 11:36:38.000000 lnkparse3-1.5.0/tests/test_samples.py
```

### Comparing `LnkParse3-1.4.0/LICENSE` & `lnkparse3-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/decorators.py` & `lnkparse3-1.5.0/LnkParse3/decorators.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/code_page.py` & `lnkparse3-1.5.0/LnkParse3/extra/code_page.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/console.py` & `lnkparse3-1.5.0/LnkParse3/extra/console.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/darwin.py` & `lnkparse3-1.5.0/LnkParse3/extra/darwin.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/distributed_tracker.py` & `lnkparse3-1.5.0/LnkParse3/extra/distributed_tracker.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/environment.py` & `lnkparse3-1.5.0/LnkParse3/extra/environment.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/icon.py` & `lnkparse3-1.5.0/LnkParse3/extra/icon.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/known_folder.py` & `lnkparse3-1.5.0/LnkParse3/extra/known_folder.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/lnk_extra_base.py` & `lnkparse3-1.5.0/LnkParse3/extra/lnk_extra_base.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/metadata.py` & `lnkparse3-1.5.0/LnkParse3/extra/metadata.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/shell_item.py` & `lnkparse3-1.5.0/LnkParse3/extra/shell_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from LnkParse3.extra.lnk_extra_base import LnkExtraBase
 from LnkParse3.lnk_targets import LnkTargets
 from LnkParse3.lnk_targets import TargetFactory
 
 """
 ------------------------------------------------------------------
 |     0-7b     |     8-15b     |     16-23b     |     24-31b     |
```

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/shim_layer.py` & `lnkparse3-1.5.0/LnkParse3/extra/shim_layer.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/special_folder.py` & `lnkparse3-1.5.0/LnkParse3/extra/special_folder.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/terminal.py` & `lnkparse3-1.5.0/LnkParse3/extra/terminal.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra/unknown.py` & `lnkparse3-1.5.0/LnkParse3/extra/unknown.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra_data.py` & `lnkparse3-1.5.0/LnkParse3/extra_data.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/extra_factory.py` & `lnkparse3-1.5.0/LnkParse3/extra_factory.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/info/local.py` & `lnkparse3-1.5.0/LnkParse3/info/local.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/info/network.py` & `lnkparse3-1.5.0/LnkParse3/info/network.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/info_factory.py` & `lnkparse3-1.5.0/LnkParse3/info_factory.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/lnk_header.py` & `lnkparse3-1.5.0/LnkParse3/lnk_header.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/lnk_info.py` & `lnkparse3-1.5.0/LnkParse3/lnk_info.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/lnk_targets.py` & `lnkparse3-1.5.0/LnkParse3/lnk_targets.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/string_data.py` & `lnkparse3-1.5.0/LnkParse3/string_data.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target/control_panel.py` & `lnkparse3-1.5.0/LnkParse3/target/control_panel.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target/lnk_target_base.py` & `lnkparse3-1.5.0/LnkParse3/target/lnk_target_base.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target/my_computer.py` & `lnkparse3-1.5.0/LnkParse3/target/my_computer.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target/network_location.py` & `lnkparse3-1.5.0/LnkParse3/target/network_location.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target/root_folder.py` & `lnkparse3-1.5.0/LnkParse3/target/root_folder.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target/shell_fs_folder.py` & `lnkparse3-1.5.0/LnkParse3/target/shell_fs_folder.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/target_factory.py` & `lnkparse3-1.5.0/LnkParse3/target_factory.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3/text_processor.py` & `lnkparse3-1.5.0/LnkParse3/text_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,22 @@
     def read_strings(self, binary):
         chars = []
 
         def _chars_to_string(lst):
             bin_string = b"".join(lst)
             try:
                 string = bin_string.decode(self.cp)
-            except UnicodeDecodeError as e:
-                string = bin_string.decode(self.cp, errors="replace")
-                msg = f"Error while decoding string `{string}` ({e})"
-                warnings.warn(msg)
+            except UnicodeDecodeError:
+                # Fallback to UTF-8 before giving up.
+                try:
+                    string = bin_string.decode("utf-8")
+                except UnicodeDecodeError as e:
+                    string = bin_string.decode(self.cp, errors="replace")
+                    msg = f"Error while decoding string `{string}` ({e})"
+                    warnings.warn(msg)
             yield string
 
         for char in binary:
             if char == 0x00:
                 yield from _chars_to_string(chars)
                 chars = []
             else:
```

### Comparing `LnkParse3-1.4.0/LnkParse3/utils.py` & `lnkparse3-1.5.0/LnkParse3/utils.py`

 * *Files identical despite different names*

### Comparing `LnkParse3-1.4.0/LnkParse3.egg-info/PKG-INFO` & `lnkparse3-1.5.0/LnkParse3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: LnkParse3
-Version: 1.4.0
+Version: 1.5.0
 Summary: Windows Shortcut file (LNK) parser
 Home-page: https://github.com/Matmaus/LnkParse
 Author: Matmaus
 Author-email: matusjas.work@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 # LnkParse3
 
 Windows Shortcut file (LNK) parser
 
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](http://makeapullrequest.com)
 [![PyPI license](https://img.shields.io/pypi/l/LnkParse3.svg?style=for-the-badge)](https://github.com/Matmaus/LnkParse3/blob/master/LICENSE)
@@ -69,31 +70,30 @@
 ```
 
 ## CLI tool
 
 ```console
 $ lnkparse tests/samples/microsoft_example
 Windows Shortcut Information:
-   Link CLSID: 00021401-0000-0000-C000-000000000046
-   Link Flags: HasTargetIDList | HasLinkInfo | HasRelativePath | HasWorkingDir | IsUnicode | E
-nableTargetMetadata - (524443)
-   File Flags: FILE_ATTRIBUTE_ARCHIVE - (32)
-
-   Creation Timestamp: 2008-09-12 20:27:17.101000+00:00
-   Modified Timestamp: 2008-09-12 20:27:17.101000+00:00
-   Accessed Timestamp: 2008-09-12 20:27:17.101000+00:00
-
-   Icon Index: 0
-   Window Style: SW_SHOWNORMAL
-   HotKey: UNSET - UNSET {0x0000}
+   Guid: 00021401-0000-0000-C000-000000000046
+   Link flags: HasTargetIDList | HasLinkInfo | HasRelativePath | HasWorkingDir | IsUnicode | EnableTargetMetadata - (524443)
+   File flags: FILE_ATTRIBUTE_ARCHIVE - (32)
+   Creation time: 2008-09-12 20:27:17.101000+00:00
+   Accessed time: 2008-09-12 20:27:17.101000+00:00
+   Modified time: 2008-09-12 20:27:17.101000+00:00
+   File size: 0
+   Icon index: 0
+   Windowstyle: SW_SHOWNORMAL
+   Hotkey: UNSET - UNSET {0x0000}
 
    ...more data...
 
-   EXTRA BLOCKS:
-      DISTRIBUTED_LINK_TRACKER_BLOCK
+   EXTRA:
+      DISTRIBUTED LINK TRACKER BLOCK:
+         Size: 96
          Length: 88
          Version: 0
          Machine identifier: chris-xps
          Droid volume identifier: 94C77840-FA47-46C7-B356-5C2DC6B6D115
          Droid file identifier: 7BCD46EC-7F22-11DD-9499-00137216874A
          Birth droid volume identifier: 94C77840-FA47-46C7-B356-5C2DC6B6D115
          Birth droid file identifier: 7BCD46EC-7F22-11DD-9499-00137216874A
@@ -156,14 +156,16 @@
   - [x] **IconEnvironmentDataBlock** [`icon.py`]
   - [x] **KnownFolderDataBlock** [`known_folder.py`]
   - [ ] **PropertyStoreDataBlock** [`metadata.py`] (incomplete)
   - [x] **ShimDataBlock** [`shim_layer.py`]
   - [x] **SpecialFolderDataBlock** [`special_folder.py`]
   - [x] **TrackerDataBlock** [`distributed_tracker.py`]
   - [x] **VistaAndAboveIDListDataBlock** [`shell_item.py`]
+  - [x] *Unknown (undefined) block* [`unknown.py`]
+  - [x] **TerminalBlock** [`terminal.py`]
 
 # Contributing
 
 Any contribution is welcome. There are still several uncovered parts of LNK Structure. Just fork the project and open a new PR.
 
 ## Tests
```

### Comparing `LnkParse3-1.4.0/LnkParse3.egg-info/SOURCES.txt` & `lnkparse3-1.5.0/LnkParse3.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 LnkParse3/target_factory.py
 LnkParse3/text_processor.py
 LnkParse3/utils.py
 LnkParse3.egg-info/PKG-INFO
 LnkParse3.egg-info/SOURCES.txt
 LnkParse3.egg-info/dependency_links.txt
 LnkParse3.egg-info/entry_points.txt
+LnkParse3.egg-info/requires.txt
 LnkParse3.egg-info/top_level.txt
 LnkParse3/extra/__init__.py
 LnkParse3/extra/code_page.py
 LnkParse3/extra/console.py
 LnkParse3/extra/darwin.py
 LnkParse3/extra/distributed_tracker.py
 LnkParse3/extra/environment.py
```

### Comparing `LnkParse3-1.4.0/PKG-INFO` & `lnkparse3-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: LnkParse3
-Version: 1.4.0
+Version: 1.5.0
 Summary: Windows Shortcut file (LNK) parser
 Home-page: https://github.com/Matmaus/LnkParse
 Author: Matmaus
 Author-email: matusjas.work@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyyaml
 
 # LnkParse3
 
 Windows Shortcut file (LNK) parser
 
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=for-the-badge)](http://makeapullrequest.com)
 [![PyPI license](https://img.shields.io/pypi/l/LnkParse3.svg?style=for-the-badge)](https://github.com/Matmaus/LnkParse3/blob/master/LICENSE)
@@ -69,31 +70,30 @@
 ```
 
 ## CLI tool
 
 ```console
 $ lnkparse tests/samples/microsoft_example
 Windows Shortcut Information:
-   Link CLSID: 00021401-0000-0000-C000-000000000046
-   Link Flags: HasTargetIDList | HasLinkInfo | HasRelativePath | HasWorkingDir | IsUnicode | E
-nableTargetMetadata - (524443)
-   File Flags: FILE_ATTRIBUTE_ARCHIVE - (32)
-
-   Creation Timestamp: 2008-09-12 20:27:17.101000+00:00
-   Modified Timestamp: 2008-09-12 20:27:17.101000+00:00
-   Accessed Timestamp: 2008-09-12 20:27:17.101000+00:00
-
-   Icon Index: 0
-   Window Style: SW_SHOWNORMAL
-   HotKey: UNSET - UNSET {0x0000}
+   Guid: 00021401-0000-0000-C000-000000000046
+   Link flags: HasTargetIDList | HasLinkInfo | HasRelativePath | HasWorkingDir | IsUnicode | EnableTargetMetadata - (524443)
+   File flags: FILE_ATTRIBUTE_ARCHIVE - (32)
+   Creation time: 2008-09-12 20:27:17.101000+00:00
+   Accessed time: 2008-09-12 20:27:17.101000+00:00
+   Modified time: 2008-09-12 20:27:17.101000+00:00
+   File size: 0
+   Icon index: 0
+   Windowstyle: SW_SHOWNORMAL
+   Hotkey: UNSET - UNSET {0x0000}
 
    ...more data...
 
-   EXTRA BLOCKS:
-      DISTRIBUTED_LINK_TRACKER_BLOCK
+   EXTRA:
+      DISTRIBUTED LINK TRACKER BLOCK:
+         Size: 96
          Length: 88
          Version: 0
          Machine identifier: chris-xps
          Droid volume identifier: 94C77840-FA47-46C7-B356-5C2DC6B6D115
          Droid file identifier: 7BCD46EC-7F22-11DD-9499-00137216874A
          Birth droid volume identifier: 94C77840-FA47-46C7-B356-5C2DC6B6D115
          Birth droid file identifier: 7BCD46EC-7F22-11DD-9499-00137216874A
@@ -156,14 +156,16 @@
   - [x] **IconEnvironmentDataBlock** [`icon.py`]
   - [x] **KnownFolderDataBlock** [`known_folder.py`]
   - [ ] **PropertyStoreDataBlock** [`metadata.py`] (incomplete)
   - [x] **ShimDataBlock** [`shim_layer.py`]
   - [x] **SpecialFolderDataBlock** [`special_folder.py`]
   - [x] **TrackerDataBlock** [`distributed_tracker.py`]
   - [x] **VistaAndAboveIDListDataBlock** [`shell_item.py`]
+  - [x] *Unknown (undefined) block* [`unknown.py`]
+  - [x] **TerminalBlock** [`terminal.py`]
 
 # Contributing
 
 Any contribution is welcome. There are still several uncovered parts of LNK Structure. Just fork the project and open a new PR.
 
 ## Tests
```

### Comparing `LnkParse3-1.4.0/README.md` & `lnkparse3-1.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,31 +55,30 @@
 ```
 
 ## CLI tool
 
 ```console
 $ lnkparse tests/samples/microsoft_example
 Windows Shortcut Information:
-   Link CLSID: 00021401-0000-0000-C000-000000000046
-   Link Flags: HasTargetIDList | HasLinkInfo | HasRelativePath | HasWorkingDir | IsUnicode | E
-nableTargetMetadata - (524443)
-   File Flags: FILE_ATTRIBUTE_ARCHIVE - (32)
-
-   Creation Timestamp: 2008-09-12 20:27:17.101000+00:00
-   Modified Timestamp: 2008-09-12 20:27:17.101000+00:00
-   Accessed Timestamp: 2008-09-12 20:27:17.101000+00:00
-
-   Icon Index: 0
-   Window Style: SW_SHOWNORMAL
-   HotKey: UNSET - UNSET {0x0000}
+   Guid: 00021401-0000-0000-C000-000000000046
+   Link flags: HasTargetIDList | HasLinkInfo | HasRelativePath | HasWorkingDir | IsUnicode | EnableTargetMetadata - (524443)
+   File flags: FILE_ATTRIBUTE_ARCHIVE - (32)
+   Creation time: 2008-09-12 20:27:17.101000+00:00
+   Accessed time: 2008-09-12 20:27:17.101000+00:00
+   Modified time: 2008-09-12 20:27:17.101000+00:00
+   File size: 0
+   Icon index: 0
+   Windowstyle: SW_SHOWNORMAL
+   Hotkey: UNSET - UNSET {0x0000}
 
    ...more data...
 
-   EXTRA BLOCKS:
-      DISTRIBUTED_LINK_TRACKER_BLOCK
+   EXTRA:
+      DISTRIBUTED LINK TRACKER BLOCK:
+         Size: 96
          Length: 88
          Version: 0
          Machine identifier: chris-xps
          Droid volume identifier: 94C77840-FA47-46C7-B356-5C2DC6B6D115
          Droid file identifier: 7BCD46EC-7F22-11DD-9499-00137216874A
          Birth droid volume identifier: 94C77840-FA47-46C7-B356-5C2DC6B6D115
          Birth droid file identifier: 7BCD46EC-7F22-11DD-9499-00137216874A
@@ -142,14 +141,16 @@
   - [x] **IconEnvironmentDataBlock** [`icon.py`]
   - [x] **KnownFolderDataBlock** [`known_folder.py`]
   - [ ] **PropertyStoreDataBlock** [`metadata.py`] (incomplete)
   - [x] **ShimDataBlock** [`shim_layer.py`]
   - [x] **SpecialFolderDataBlock** [`special_folder.py`]
   - [x] **TrackerDataBlock** [`distributed_tracker.py`]
   - [x] **VistaAndAboveIDListDataBlock** [`shell_item.py`]
+  - [x] *Unknown (undefined) block* [`unknown.py`]
+  - [x] **TerminalBlock** [`terminal.py`]
 
 # Contributing
 
 Any contribution is welcome. There are still several uncovered parts of LNK Structure. Just fork the project and open a new PR.
 
 ## Tests
```

### Comparing `LnkParse3-1.4.0/setup.py` & `lnkparse3-1.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='LnkParse3',
-    version='1.4.0',
+    version='1.5.0',
     description='Windows Shortcut file (LNK) parser',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/Matmaus/LnkParse',
     author='Matmaus',
     author_email='matusjas.work@gmail.com',
     license='MIT',
     packages=find_packages(exclude=["tests*"]),
+    install_requires=['pyyaml'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `LnkParse3-1.4.0/tests/test_samples.py` & `lnkparse3-1.5.0/tests/test_samples.py`

 * *Files identical despite different names*

