# Comparing `tmp/gink-0.20240516.1715898271.tar.gz` & `tmp/gink-0.20240518.1716010702.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gink-0.20240516.1715898271.tar", last modified: Thu May 16 22:24:37 2024, max compression
+gzip compressed data, was "gink-0.20240518.1716010702.tar", last modified: Sat May 18 05:38:25 2024, max compression
```

## Comparing `gink-0.20240516.1715898271.tar` & `gink-0.20240518.1716010702.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 22:24:23.000000 gink-0.20240516.1715898271/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.404682 gink-0.20240516.1715898271/gink/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.408682 gink-0.20240516.1715898271/gink/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/behavior_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/change_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/claim_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/clearance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/entry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/header_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/key_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/log_file_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/movement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/muid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/pair_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/sync_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/gink/builders/value_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.416683 gink-0.20240516.1715898271/gink/impl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/abstract_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/addressable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/attribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/bundle_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/bundle_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/container.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19740 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/deferred.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    56480 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/lmdb_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/log_backed_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    21698 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/selectable_console.py
--rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/tuples.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/wsgi_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/impl/wsgi_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/gink/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_chain_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_change_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_code_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_key_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_lmdb_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_logbackedstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_muid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_pair_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_pair_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_websocket_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 22:24:24.000000 gink-0.20240516.1715898271/gink/tests/test_wsgi_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/gink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-16 22:24:37.000000 gink-0.20240516.1715898271/gink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:24:37.420683 gink-0.20240516.1715898271/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 22:24:31.000000 gink-0.20240516.1715898271/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:25.832673 gink-0.20240518.1716010702/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-18 05:38:25.832673 gink-0.20240518.1716010702/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:25.812673 gink-0.20240518.1716010702/gink/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5932 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:25.816673 gink-0.20240518.1716010702/gink/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/behavior_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/change_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/claim_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/clearance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/entry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/header_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/key_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/log_file_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/movement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/muid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/pair_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/sync_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40439 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/gink/builders/value_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:25.824673 gink-0.20240518.1716010702/gink/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/abstract_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/bundle_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/bundle_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/bundle_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21568 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13163 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/container.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17826 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/deferred.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57125 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/lmdb_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/log_backed_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22134 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/selectable_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12612 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/wsgi_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/impl/wsgi_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:25.828673 gink-0.20240518.1716010702/gink/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_chain_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_change_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_code_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10116 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_key_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_lmdb_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_logbackedstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_muid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_pair_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_pair_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_websocket_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-18 05:38:20.000000 gink-0.20240518.1716010702/gink/tests/test_wsgi_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 05:38:25.828673 gink-0.20240518.1716010702/gink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11194 2024-05-18 05:38:25.000000 gink-0.20240518.1716010702/gink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-18 05:38:25.000000 gink-0.20240518.1716010702/gink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 05:38:25.000000 gink-0.20240518.1716010702/gink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-18 05:38:25.000000 gink-0.20240518.1716010702/gink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 05:38:25.000000 gink-0.20240518.1716010702/gink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 05:38:25.832673 gink-0.20240518.1716010702/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-18 05:38:22.000000 gink-0.20240518.1716010702/setup.py
```

### Comparing `gink-0.20240516.1715898271/LICENSE` & `gink-0.20240518.1716010702/LICENSE`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/PKG-INFO` & `gink-0.20240518.1716010702/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240516.1715898271
+Version: 0.20240518.1716010702
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240516.1715898271/README.md` & `gink-0.20240518.1716010702/README.md`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/__init__.py` & `gink-0.20240518.1716010702/gink/__init__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/__main__.py` & `gink-0.20240518.1716010702/gink/__main__.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/behavior_pb2.py` & `gink-0.20240518.1716010702/gink/builders/behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/bundle_pb2.py` & `gink-0.20240518.1716010702/gink/builders/bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/change_pb2.py` & `gink-0.20240518.1716010702/gink/builders/change_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/claim_pb2.py` & `gink-0.20240518.1716010702/gink/builders/claim_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/clearance_pb2.py` & `gink-0.20240518.1716010702/gink/builders/clearance_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/container_pb2.py` & `gink-0.20240518.1716010702/gink/builders/container_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/entry_pb2.py` & `gink-0.20240518.1716010702/gink/builders/entry_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/header_pb2.py` & `gink-0.20240518.1716010702/gink/builders/header_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/key_pb2.py` & `gink-0.20240518.1716010702/gink/builders/key_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/log_file_pb2.py` & `gink-0.20240518.1716010702/gink/builders/log_file_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/movement_pb2.py` & `gink-0.20240518.1716010702/gink/builders/movement_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/muid_pb2.py` & `gink-0.20240518.1716010702/gink/builders/muid_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/pair_pb2.py` & `gink-0.20240518.1716010702/gink/builders/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/sync_message_pb2.py` & `gink-0.20240518.1716010702/gink/builders/sync_message_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/builders/value_pb2.py` & `gink-0.20240518.1716010702/gink/builders/value_pb2.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/abstract_store.py` & `gink-0.20240518.1716010702/gink/impl/abstract_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """Contains AbstractStore class."""
 
 # standard python modules
-from typing import Tuple, Callable, Optional, Iterable, List, Union, Mapping, TypeVar, Generic
-from abc import ABC, abstractmethod
+from typing import Tuple, Optional, Iterable, List, Union, Mapping, TypeVar, Generic, Callable
+from abc import abstractmethod
 
 from pathlib import Path
 
 # Gink specific modules
 from .builders import ContainerBuilder, ChangeBuilder, EntryBuilder, ClaimBuilder
 from .bundle_info import BundleInfo
 from .chain_tracker import ChainTracker
-from .typedefs import UserKey, MuTimestamp, Medallion
+from .typedefs import UserKey, MuTimestamp, Medallion, Limit
 from .tuples import FoundEntry, Chain, PositionedEntry, FoundContainer
 from .muid import Muid
 from .bundle_wrapper import BundleWrapper
 from .utilities import is_certainly_gone
 from .watcher import Watcher
-BundleCallback = Callable[[bytes, BundleInfo], None]
+from .bundle_store import BundleStore
 Lock = TypeVar('Lock')
 
 
-class AbstractStore(ABC, Generic[Lock]):
+class AbstractStore(BundleStore, Generic[Lock]):
     """ abstract base class for the gink data store
 
         Stores both the bundles received and the contents of those
         bundles unpacked so that you can examine entries, container definitions, etc.
 
         Warning! Since data stores are viewed as part of the internal implementation,
         this interface may change at any time without warning on a minor version change.
@@ -110,21 +110,21 @@
     def get_entry(self, muid: Muid) -> Optional[EntryBuilder]:
         """ Return the entry builder for a entry if it's visible in the store. """
 
     def close(self):
         """Safely releases resources."""
 
     @abstractmethod
-    def _refresh_helper(self, lock: Lock, callback: Optional[BundleCallback] = None, /) -> int:
+    def _refresh_helper(self, lock: Lock, callback: Optional[Callable[[BundleWrapper], None]]=None, /) -> int:
         """ do a refresh using a lock/transaction """
 
     def maybe_reuse_chain(
             self,
             identity: str,
-            callback: Optional[BundleCallback] = None) -> Optional[BundleInfo]:
+            callback: Optional[Callable[[BundleWrapper], None]]=None) -> Optional[BundleInfo]:
         """ Tries to find a chain for reuse.  The callback is used for refresh.
         """
         lock: Lock = self._acquire_lock()
         try:
             self._refresh_helper(lock, callback)
             claims = self._get_claims(lock)
             for old_claim in claims.values():
@@ -153,55 +153,43 @@
     def _release_lock(self, lock: Lock, /):
         """ Finalize Transaction """
 
     @abstractmethod
     def apply_bundle(
             self,
             bundle: Union[BundleWrapper, bytes],
-            callback: Optional[BundleCallback]=None,
+            callback: Optional[Callable[[BundleWrapper], None]]=None,
             claim_chain: bool=False) -> bool:
         """ Tries to add data from a particular bundle to this store.
 
             Returns true if the data is actually added, false if data already exists,
             and will throw an exception in the case of an invalid extension.
         """
 
-    def refresh(self, callback: Optional[BundleCallback] = None) -> int:
+    def refresh(self, callback: Optional[Callable[[BundleWrapper], None]]=None) -> int:
         """ Checks the source file for bundles that haven't come from this process and calls the callback.
 
             Intended to allow the process to send bundles to peers and otherwise get the model in line with the file.
 
             Returns the number of transactions processed.
         """
         lock = self._acquire_lock()
         if count := self._refresh_helper(lock, callback):
             self._clear_notifications()
         self._release_lock(lock)
         return count
 
-    @abstractmethod
-    def get_bundles(self, callback: BundleCallback, since: MuTimestamp=0):
-        """ Calls the callback with each bundle currently in the store since the `since` argument (default 0).
-
-            Calls in order received by this store, which may not correspond to the bundle creation times.
-            But we still expect dependency order to be respected, that is if B1 references objects from B0,
-            then B0 should come before B1.
-
-            This is done callback style because we don't want to leave dangling transactions
-            in the store, which could easily happen if we offered up an iterator interface instead.
-        """
-
-    def get_bundle_infos(self) -> List[BundleInfo]:
+    def get_bundle_infos(self, limit_to: Mapping[Chain, Limit] | None = None) -> List[BundleInfo]:
         """ Gets a list of bundle infos; mostly for testing. """
         result = []
 
-        def callback(_, info: BundleInfo):
-            result.append(info)
+        def callback(bundle_wrapper: BundleWrapper):
+            result.append(bundle_wrapper.get_info())
 
-        self.get_bundles(callback)
+        self.get_bundles(callback, limit_to=limit_to)
         return result
 
     @abstractmethod
     def list_containers(self) -> Iterable[Tuple[Muid, ContainerBuilder]]:
         """ Gets the address and definition of each regular container.
 
             Does not include the instance/medallion containers or the global containers.
@@ -229,15 +217,15 @@
             returning = thing
         if actual == expected:
             return returning
         else:
             return None
 
     @abstractmethod
-    def get_chain_tracker(self) -> ChainTracker:
+    def get_chain_tracker(self, limit_to: Optional[Mapping[Chain, Limit]]=None) -> ChainTracker:
         """Returns a tracker showing what this store has at the time this function is called."""
 
     @abstractmethod
     def get_last(self, chain: Chain) -> BundleInfo:
         """ Returns metadata for the last bundle in a specified chain. """
 
     @abstractmethod
```

### Comparing `gink-0.20240516.1715898271/gink/impl/addressable.py` & `gink-0.20240518.1716010702/gink/impl/addressable.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/attribution.py` & `gink-0.20240518.1716010702/gink/impl/attribution.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/box.py` & `gink-0.20240518.1716010702/gink/impl/box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/builders.py` & `gink-0.20240518.1716010702/gink/impl/builders.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         movement: MovementBuilder
 
 
     class BundleBuilder(Message):
         header: HeaderBuilder
         changes: List[ChangeBuilder]
 
-    class SyncMessage(Message):
-        pass
 
+    class SyncMessage(Message):
+        bundle: bytes
 
 
     class Pair:
         left: MuidBuilder
         rite: MuidBuilder
```

### Comparing `gink-0.20240516.1715898271/gink/impl/bundle_info.py` & `gink-0.20240518.1716010702/gink/impl/bundle_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
-""" Contains the ChangeSetInfo class. """
+""" Contains the BundleInfo class. """
+from __future__ import annotations
 from typing import Optional
 from struct import Struct
 
 from .builders import SyncMessage, HeaderBuilder
 from .typedefs import Medallion, MuTimestamp
 from .tuples import Chain
 
@@ -62,15 +63,15 @@
             chain_start=ack.chain_start,
             medallion=ack.medallion,
             timestamp=ack.timestamp,
             previous=ack.previous,
         )
 
     @staticmethod
-    def from_bytes(data: bytes):
+    def from_bytes(data: bytes) -> BundleInfo:
         """ the opposite of __bytes__ """
         if not (isinstance(data, bytes) and len(data) >= 32):
             raise ValueError("bad argument to BundleInfo.from_bytes: %r" % data)
         return BundleInfo(encoded=data)
 
     def get_chain(self) -> Chain:
         """Gets a Chain tuple saying which chain this change set came from."""
```

### Comparing `gink-0.20240516.1715898271/gink/impl/bundler.py` & `gink-0.20240518.1716010702/gink/impl/bundler.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/chain_tracker.py` & `gink-0.20240518.1716010702/gink/impl/chain_tracker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Defines the ChainTracker class.
 """
-
-from typing import Union, Optional
+from __future__ import annotations
+from typing import Union, Optional, Iterable
 
 from sortedcontainers import SortedDict  # type: ignore
 
 from .builders import SyncMessage
-from .typedefs import MuTimestamp, Medallion
+from .typedefs import MuTimestamp, Medallion, Limit
 from .muid import Muid
 from .tuples import Chain
 from .bundle_info import BundleInfo
 
 
 class ChainTracker:
     """
@@ -27,17 +27,27 @@
             greeting = sync_message.greeting  # type: ignore
             for greeting_entry in greeting.entries:
                 chain = Chain(
                     medallion=greeting_entry.medallion,
                     chain_start=greeting_entry.chain_start)
                 self._data[chain] = greeting_entry.seen_through
 
-    def get_seen_to(self, chain: Chain) -> Optional[MuTimestamp]:
-        """ Says how far along a giving chain the given instance has seen. """
-        return self._data.get(chain)
+    def get_subset(self, chains=Iterable[Chain]) -> ChainTracker:
+        result = ChainTracker()
+        for chain in chains:
+            i_have = self._data.get(chain)
+            if i_have is not None:
+                result._data[chain] = i_have
+        return result
+
+    def is_valid_extension(self, bundle_info: BundleInfo) -> bool:
+        if bundle_info.timestamp == bundle_info.chain_start:
+            return True
+        seen_to = self._data.get(bundle_info.get_chain())
+        return seen_to == bundle_info.previous
 
     def mark_as_having(self, bundle_info: BundleInfo):
         """ Indicates has everything along the chain in bundle_info up to its timestamp. """
         chain = bundle_info.get_chain()
         have_so_far = self._data.get(chain, 0)
         if have_so_far < bundle_info.timestamp:
             self._data[chain] = bundle_info.timestamp
```

### Comparing `gink-0.20240516.1715898271/gink/impl/coding.py` & `gink-0.20240518.1716010702/gink/impl/coding.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/container.py` & `gink-0.20240518.1716010702/gink/impl/container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/database.py` & `gink-0.20240518.1716010702/gink/impl/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     _lock: Lock
     _last_time: Optional[MuTimestamp]
     _store: AbstractStore
     _connections: Set[Connection]
     _wsgi_connections: Set[WsgiConnection]
     _listeners: Set[Listener]
     _sent_but_not_acked: Set[BundleInfo]
-    _trackers: Dict[Connection, ChainTracker]  # tracks what we know a peer has
     _last_link: Optional[BundleInfo]
     _container_types: dict = {}
 
     def __init__(self,
                  store: Union[AbstractStore, str, None] = None,
                  identity = get_identity(),
                  web_server = None,
@@ -63,15 +62,14 @@
         self._store = store
         self._last_link = None
         self._lock = Lock()
         self._last_time = None
         self._connections = set()
         self._wsgi_connections = set()
         self._listeners = set()
-        self._trackers = {}
         self._identity = identity
         self._logger = getLogger(self.__class__.__name__)
         self._wsgi_listener: Optional[WsgiListener] = None
         # Web server would be a Flask app or other WSGI compatible app
         if web_server:
             self._wsgi_listener = WsgiListener(app=web_server, address=web_server_addr)
         self._sent_but_not_acked = set()
@@ -182,66 +180,33 @@
             added = self._store.apply_bundle(wrap, self._on_bundle, False)
             assert added
             info = wrap.get_info()
             self._last_link = info
             self._logger.debug("locally committed bundle: %r", info)
             return info
 
-    def _on_bundle(self, bundle_bytes: bytes, bundle_info: BundleInfo) -> None:
+    def _on_bundle(self, bundle_wrapper: BundleWrapper) -> None:
         """ Sends a bundle either created locally or received from a peer to other peers.
         """
-        outbound_message_with_bundle = SyncMessage()
-        outbound_message_with_bundle.bundle = bundle_bytes
         for peer in self._connections:
-            tracker = self._trackers.get(peer)
-            if tracker is None:
-                # In this case we haven't received a greeting from the peer, and so don't want to
-                # send any bundles because it might result in gaps in their chain.
-                continue
-            if tracker.has(bundle_info):
-                # peer already has or has been previously sent this bundle
-                continue
-            self._logger.debug("sending %r to %r", bundle_info, peer)
-            peer.send(outbound_message_with_bundle)
-            tracker.mark_as_having(bundle_info)
+            peer.send_bundle(bundle_wrapper)
         for callback in self._callbacks:
-            callback(bundle_info)
+            callback(bundle_wrapper.get_info())
 
-    def _receive_data(self, sync_message: SyncMessage, from_peer: Connection):
+    def _on_peer_ready(self, peer: Connection):
         with self._lock:
-            if sync_message.HasField("bundle"):
-                bundle_bytes = sync_message.bundle
-                wrap = BundleWrapper(bundle_bytes)
-                info = wrap.get_info()
-                if (tracker := self._trackers.get(from_peer)):
-                    tracker.mark_as_having(info)
-                self._store.apply_bundle(wrap, self._on_bundle)
-                from_peer.send(info.as_acknowledgement())
-            elif sync_message.HasField("greeting"):
-                self._logger.debug("received greeting from %s", from_peer)
-                chain_tracker = ChainTracker(sync_message=sync_message)
-                self._trackers[from_peer] = chain_tracker
-
-                def callback(bundle_bytes: bytes, info: BundleInfo):
-                    if not chain_tracker.has(info):
-                        outgoing_builder = SyncMessage()
-                        outgoing_builder.bundle = bundle_bytes
-                        from_peer.send(outgoing_builder)
-
-                self._store.get_bundles(callback=callback)
-                from_peer.set_replied_to_greeting()
-            elif sync_message.HasField("ack"):
-                acked_info = BundleInfo.from_ack(sync_message)
-                tracker = self._trackers.get(from_peer)
-                if tracker is not None:
-                    tracker.mark_as_having(acked_info)
-                if acked_info in self._sent_but_not_acked:
-                    self._sent_but_not_acked.remove(acked_info)
-            else:
-                self._logger.warning("got binary message without ack, bundle, or greeting")
+            for thing in peer.receive_objects():
+                if isinstance(thing, BundleWrapper):  # some data
+                    self._store.apply_bundle(thing, self._on_bundle)
+                elif isinstance(thing, ChainTracker):  # greeting message
+                    self._store.get_bundles(peer.send_bundle, peer_has=thing)
+                elif isinstance(thing, BundleInfo):  # an ack:
+                    self._sent_but_not_acked.discard(thing)
+                else:
+                    raise AssertionError("unexpected object")
 
     def start_listening(self, ip_addr="", port: Union[str, int] = "8080"):
         """ Listen for incoming connections on the given port.
 
             Note that you'll still need to call "run" to actually accept those connections.
         """
         port = int(port)
@@ -296,16 +261,15 @@
                     readers.append(conn)
                 if isinstance(console, SelectableConsole):
                     readers.append(console)
                     console.refresh()
                 ready_readers, _, _ = select(readers, [], [], 0.1)
                 for ready_reader in ready_readers:
                     if isinstance(ready_reader, Connection):
-                        for data in ready_reader.receive():
-                            self._receive_data(data, ready_reader)
+                        self._on_peer_ready(ready_reader)
                         if ready_reader.is_closed():
                             self._connections.remove(ready_reader)
                             readers.remove(ready_reader)
                     elif isinstance(ready_reader, WsgiListener) and self._wsgi_listener:
                         conn = self._wsgi_listener.accept()
                         if conn:
                             self._wsgi_connections.add(conn)
```

### Comparing `gink-0.20240516.1715898271/gink/impl/deferred.py` & `gink-0.20240518.1716010702/gink/impl/deferred.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/directory.py` & `gink-0.20240518.1716010702/gink/impl/directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/graph.py` & `gink-0.20240518.1716010702/gink/impl/graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/group.py` & `gink-0.20240518.1716010702/gink/impl/group.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/key_set.py` & `gink-0.20240518.1716010702/gink/impl/key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/listener.py` & `gink-0.20240518.1716010702/gink/impl/listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/lmdb_store.py` & `gink-0.20240518.1716010702/gink/impl/lmdb_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Contains the LmdbStore class."""
 
 # Standard Python Stuff
 from os import unlink
 from os.path import exists
 from logging import getLogger
 import uuid
-from typing import Tuple, Iterable, Optional, Set, Union, Mapping
+from typing import Tuple, Iterable, Optional, Set, Union, Mapping, Callable
 from struct import pack
 from pathlib import Path
 from lmdb import open as ldmbopen, Transaction as Trxn, Cursor # type: ignore
 
 # Gink Implementation
 from .builders import (BundleBuilder, ChangeBuilder, EntryBuilder, MovementBuilder,
                        ContainerBuilder, ClearanceBuilder, Message, Behavior, ClaimBuilder)
-from .typedefs import MuTimestamp, UserKey, Medallion
+from .typedefs import MuTimestamp, UserKey, Medallion, Limit
 from .tuples import Chain, FoundEntry, PositionedEntry, FoundContainer
 from .muid import Muid
 from .bundle_info import BundleInfo
-from .abstract_store import AbstractStore, BundleWrapper, BundleCallback
+from .abstract_store import AbstractStore, BundleWrapper
 from .chain_tracker import ChainTracker
 from .lmdb_utilities import to_last_with_prefix
 from .utilities import generate_timestamp, create_claim
 from .coding import (encode_key, create_deleting_entry, PlacementBuilderPair, decode_muts, wrap_change,
                      Placement, encode_muts, QueueMiddleKey, DIRECTORY, SEQUENCE, serialize,
                      ensure_entry_is_valid, deletion, Deletion, decode_entry_occupant, RemovalKey,
                      LocationKey, PROPERTY, BOX, GROUP, decode_value, EDGE_TYPE, PAIR_MAP, PAIR_SET, KEY_SET,
-                     normalize_entry_builder, VERTEX)
+                     normalize_entry_builder, VERTEX, FLOAT_INF)
 
 
 class LmdbStore(AbstractStore):
     """
     """
 
     def __init__(
@@ -717,37 +717,37 @@
                     ckey = to_last_with_prefix(cursor, container_prefix, ckey[16:-24])
                     continue
                 entry_builder = EntryBuilder()
                 entry_builder.ParseFromString(txn.get(cursor.value(), db=self._entries))  # type: ignore
                 yield FoundEntry(address=placement_key.placer, builder=entry_builder)
                 ckey = to_last_with_prefix(cursor, container_prefix, ckey[16:-24])
 
-    def refresh(self, callback: Optional[BundleCallback] = None) -> int:
+    def refresh(self, callback: Optional[Callable[[BundleWrapper], None]]=None) -> int:
         with self._handle.begin(write=False) as trxn:
             count = self._refresh_helper(trxn=trxn, callback=callback)
         if count:
             self._clear_notifications()
         return count
 
-    def _refresh_helper(self, trxn: Trxn, callback: Optional[BundleCallback] = None) -> int:
+    def _refresh_helper(self, trxn: Trxn, callback: Optional[Callable[[BundleWrapper], None]]=None) -> int:
         cursor = trxn.cursor(self._bundles)
         count = 0
         while cursor.set_range(encode_muts(self._seen_through + 1)):
             byte_key = cursor.key()
             wrapper = BundleWrapper(cursor.value())
             if callback is not None:
-                callback(wrapper.get_bytes(), wrapper.get_info())
+                callback(wrapper)
                 count += 1
             self._seen_through = decode_muts(byte_key) or 0
         return count
 
     def apply_bundle(
             self,
             bundle: Union[BundleWrapper, bytes],
-            callback: Optional[BundleCallback]=None,
+            callback: Optional[Callable[[BundleWrapper], None]]=None,
             claim_chain: bool=False
             ) -> bool:
         wrapper = BundleWrapper(bundle) if isinstance(bundle, bytes) else bundle
         builder = wrapper.get_builder()
         new_info = wrapper.get_info()
         chain_key = bytes(new_info.get_chain())
         # Note: LMDB supports only one write transaction, so we don't need to explicitly lock.
@@ -784,15 +784,15 @@
                         continue
                     if change.HasField("clearance"):
                         self._apply_clearance(new_info, trxn, offset, change.clearance)
                         continue
                     raise AssertionError(f"Can't process change: {new_info} {offset} {change}")
         self._clear_notifications()
         if needed and callback is not None:
-            callback(wrapper.get_bytes(), wrapper.get_info())
+            callback(wrapper)
         return needed
 
     def get_identity(self, chain: Chain, trxn: Optional[Trxn]=None, /) -> str:
         if trxn is None:
             with self._handle.begin() as trxn:
                 result = trxn.get(bytes(chain), db=self._identities)
         else:
@@ -974,39 +974,49 @@
         if container_muid == Muid(-1, -1, Behavior.PROPERTY):
             if entry_builder.HasField("value") and entry_builder.HasField("describing"):
                 name = decode_value(entry_builder.value)
                 if isinstance(name, str):
                     by_name_key = name.encode() + b"\x00" + bytes(entry_muid)
                     trxn.delete(by_name_key, db=self._by_name)
 
-    def get_bundles(self, callback: BundleCallback, since: MuTimestamp = 0):
+    def get_bundles(
+        self,
+        callback: Callable[[BundleWrapper], None], *,
+        limit_to: Optional[Mapping[Chain, Limit]] = None,
+        **_
+    ):
         with self._handle.begin() as txn:
             retention = decode_muts(txn.get(b"bundles", db=self._retentions))
-            if retention is None or (retention != 1 and retention > since):
-                raise ValueError("haven't been retaining bundles that long")
-            bundles_cursor = txn.cursor(self._bundles)
-            data_remaining = bundles_cursor.set_range(encode_muts(since))
+            if retention is None or retention != 1:
+                # TODO: handle the case of partial bundle retention, which would require computing the
+                # minimum lookback time necessary to service the request.
+                raise ValueError("don't have full bundle retention")
+            bundle_infos_cursor = txn.cursor(self._bundle_infos)
+            start_scan_at_time: MuTimestamp = 0  # would need to put the minimum lookback time here
+            data_remaining = bundle_infos_cursor.set_range(encode_muts(start_scan_at_time))
             while data_remaining:
-                bundle_bytes = bundles_cursor.value()
-                bundle_builder = BundleBuilder()
-                bundle_builder.ParseFromString(bundle_bytes)
-                bundle_info = BundleInfo(builder=bundle_builder.header)
-                callback(bundle_bytes, bundle_info)
-                data_remaining = bundles_cursor.next()
+                bundle_info = BundleInfo(encoded=bundle_infos_cursor.key())
+                if limit_to is None or bundle_info.timestamp <= limit_to.get(bundle_info.get_chain(), 0):
+                    bundle_bytes = txn.get(bundle_infos_cursor.value(), db=self._bundles)
+                    bundle_wrapper = BundleWrapper(bundle_bytes=bundle_bytes, bundle_info=bundle_info)
+                    callback(bundle_wrapper)
+                data_remaining = bundle_infos_cursor.next()
 
-    def get_chain_tracker(self) -> ChainTracker:
+    def get_chain_tracker(self, limit_to: Optional[Mapping[Chain, Limit]]=None) -> ChainTracker:
         chain_tracker = ChainTracker()
         with self._handle.begin() as txn:
             infos_cursor = txn.cursor(self._chains)
             data_remaining = infos_cursor.first()
             while data_remaining:
                 info_bytes = infos_cursor.value()
                 bundle_info = BundleInfo(encoded=info_bytes)
                 chain_tracker.mark_as_having(bundle_info)
                 data_remaining = infos_cursor.next()
+        if limit_to is not None:
+            chain_tracker = chain_tracker.get_subset(limit_to.keys())
         return chain_tracker
 
     def get_by_describing(self, desc: Muid, as_of: MuTimestamp = -1) -> Iterable[FoundEntry]:
         prefix = bytes(desc)
         with self._handle.begin() as trxn:
             retaining_entries = decode_muts(trxn.get(b"entries", db=self._retentions))  # type: ignore
             by_describing_cursor = trxn.cursor(self._by_describing)
```

### Comparing `gink-0.20240516.1715898271/gink/impl/lmdb_utilities.py` & `gink-0.20240518.1716010702/gink/impl/lmdb_utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/log_backed_store.py` & `gink-0.20240518.1716010702/gink/impl/log_backed_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ implementation of the LogBackedStore class """
-from typing import Optional, Union, Dict
+from typing import Optional, Union, Callable
 from fcntl import flock, LOCK_EX, LOCK_NB, LOCK_UN, LOCK_SH
 from pathlib import Path
 from .builders import LogFileBuilder, ClaimBuilder
 from .memory_store import MemoryStore
 from .bundle_wrapper import BundleWrapper
-from .abstract_store import BundleCallback, Lock
-from .typedefs import Medallion
+from .abstract_store import Lock
 from .tuples import Chain
 from .utilities import create_claim
 
 class LogBackedStore(MemoryStore):
     """A Store backed by a simple append-only file."""
 
     def __init__(self, filepath: Union[Path, str], *, exclusive=False, reset=False):
@@ -50,30 +49,30 @@
         data: bytes = self._log_file_builder.SerializeToString()  # type: ignore
         self._handle.write(data)
         self._handle.flush()
 
     def _get_file_path(self) -> Optional[Path]:
         return self._filepath
 
-    def _refresh_helper(self, _: Lock, callback: Optional[BundleCallback] = None, /) -> int:
+    def _refresh_helper(self, _: Lock, callback: Optional[Callable[[BundleWrapper], None]]=None, /) -> int:
         file_bytes = self._handle.read()
         self._log_file_builder.ParseFromString(file_bytes)  # type: ignore
         count = 0
         for bundle_bytes in self._log_file_builder.bundles:  # type: ignore # pylint: disable=maybe-no-member
             MemoryStore.apply_bundle(self, bundle_bytes, callback=callback)
             count += 1
         for claim_builder in self._log_file_builder.claims:
             self._claims[claim_builder.medallion] = claim_builder
         self._processed_to += len(file_bytes)
         return count
 
     def apply_bundle(
             self,
             bundle: Union[BundleWrapper, bytes],
-            callback: Optional[BundleCallback]=None,
+            callback: Optional[Callable[[BundleWrapper], None]]=None,
             claim_chain: bool=False,
             ) -> bool:
         if self._handle.closed:
             raise AssertionError("attempt to write to closed LogBackStore")
         if isinstance(bundle, bytes):
             bundle = BundleWrapper(bundle)
         flocked_by_apply = False
@@ -89,15 +88,15 @@
                 claim_builder: ClaimBuilder = create_claim(bundle.get_info().get_chain())
                 self._log_file_builder.claims.append(claim_builder)
                 self._claims[bundle.get_info().medallion] = claim_builder
             data: bytes = self._log_file_builder.SerializeToString()  # type: ignore
             self._handle.write(data)
             self._handle.flush()
             if callback is not None:
-                callback(bundle.get_bytes(), bundle.get_info())
+                callback(bundle)
         if flocked_by_apply:
             flock(self._handle, LOCK_UN)
             self._flocked = False
         self._clear_notifications()
         return added
 
     def close(self):
```

### Comparing `gink-0.20240516.1715898271/gink/impl/memory_store.py` & `gink-0.20240518.1716010702/gink/impl/memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from typing import Tuple, Callable, Optional, Iterable, Union, Dict, Mapping
 from sortedcontainers import SortedDict  # type: ignore
 from pathlib import Path
 
 # gink modules
 from .builders import (BundleBuilder, EntryBuilder, MovementBuilder, ClearanceBuilder,
                        ContainerBuilder, Message, ChangeBuilder, ClaimBuilder)
-from .typedefs import UserKey, MuTimestamp, Medallion, Deletion
+from .typedefs import UserKey, MuTimestamp, Medallion, Deletion, Limit
 from .tuples import Chain, FoundEntry, PositionedEntry
 from .bundle_info import BundleInfo
-from .abstract_store import AbstractStore, BundleWrapper, BundleCallback, Lock
+from .abstract_store import AbstractStore, BundleWrapper, Lock
 from .chain_tracker import ChainTracker
 from .muid import Muid
 from .coding import (DIRECTORY, encode_muts, QueueMiddleKey, RemovalKey,
                      SEQUENCE, LocationKey, create_deleting_entry, wrap_change,
                      Placement, decode_key, decode_entry_occupant)
 from .utilities import create_claim
 
@@ -174,15 +174,15 @@
                 return None
             return FoundEntry(address=entry_storage_key.placer, builder=builder)
         return None
 
     def _get_claims(self, _: Lock, /) -> Mapping[Medallion, ClaimBuilder]:
         return self._claims
 
-    def _refresh_helper(self, lock: Lock, callback: Optional[BundleCallback] = None, /) -> int:
+    def _refresh_helper(self, lock: Lock, callback: Optional[Callable[[BundleWrapper], None]]=None, /) -> int:
         return 0
 
     def get_ordered_entries(
             self,
             container: Muid,
             as_of: MuTimestamp,
             limit: Optional[int] = None,
@@ -228,16 +228,16 @@
                 builder=entry_builder)
             if limit is not None:
                 limit -= 1
 
     def apply_bundle(
             self,
             bundle: Union[BundleWrapper, bytes],
-            callback: Optional[Callable]=None,
-            claim_chain: bool=False
+            callback: Optional[Callable[[BundleWrapper], None]]=None,
+            claim_chain: bool=False,
             ) -> bool:
         if isinstance(bundle, bytes):
             bundle = BundleWrapper(bundle)
         bundle_builder = bundle.get_builder()
         new_info = bundle.get_info()
         chain_key = new_info.get_chain()
         old_info = self._chain_infos.get(new_info.get_chain())
@@ -262,15 +262,15 @@
                     self._add_movement(new_info=new_info, offset=offset, builder=change.movement)
                     continue
                 if change.HasField("clearance"):
                     self._add_clearance(new_info=new_info, offset=offset, builder=change.clearance)
                     continue
                 raise AssertionError(f"Can't process change: {new_info} {offset} {change}")
         if needed and callback is not None:
-            callback(bundle.get_bytes(), bundle.get_info())
+            callback(bundle)
         return needed
 
     def _acquire_lock(self) -> bool:
         return False
 
     def _release_lock(self, _, /):
         pass
@@ -331,27 +331,36 @@
         encoded_placement_key = bytes(placement)
         self._entries[entry_muid] = entry_builder
         self._placements[encoded_placement_key] = entry_muid
         # entries_location_key = bytes(placement.placer) + bytes(placement.placer)
         entries_location_key = LocationKey(placement.placer, placement.placer)
         self._locations[entries_location_key] = encoded_placement_key
 
-    def get_bundles(self, callback: Callable[[bytes, BundleInfo], None], since: MuTimestamp = 0):
-        for bundle_info_key in self._bundles.irange(minimum=encode_muts(since)):
+    def get_bundles(
+        self,
+        callback: Callable[[BundleWrapper], None], *,
+        limit_to: Optional[Mapping[Chain, Limit]] = None,
+        **_
+    ):
+        start_scan_at: MuTimestamp = 0
+        for bundle_info_key in self._bundles.irange(minimum=encode_muts(start_scan_at)):
             bundle_info = BundleInfo.from_bytes(bundle_info_key)
-            assert isinstance(bundle_info, BundleInfo)
-            data = self._bundles[bundle_info]
-            assert isinstance(data, bytes)
-            callback(data, bundle_info)
+            if limit_to is None or bundle_info.timestamp <= limit_to.get(bundle_info.get_chain(), 0):
+                bundle_bytes = self._bundles[bundle_info]
+                assert isinstance(bundle_bytes, bytes)
+                bundle_wrapper = BundleWrapper(bundle_bytes=bundle_bytes, bundle_info=bundle_info)
+                callback(bundle_wrapper)
 
-    def get_chain_tracker(self) -> ChainTracker:
+    def get_chain_tracker(self, limit_to: Optional[Mapping[Chain, Limit]]=None) -> ChainTracker:
         chain_tracker = ChainTracker()
         for bundle_info in self._chain_infos.values():
             assert isinstance(bundle_info, BundleInfo)
             chain_tracker.mark_as_having(bundle_info)
+        if limit_to is not None:
+            chain_tracker = chain_tracker.get_subset(limit_to.keys())
         return chain_tracker
 
     def get_last(self, chain: Chain) -> BundleInfo:
         return self._chain_infos[chain]
 
     def _get_entry_location(self, entry_muid: Muid, as_of: MuTimestamp = -1) -> Optional[bytes]:
         # bkey = bytes(entry_muid)
```

### Comparing `gink-0.20240516.1715898271/gink/impl/muid.py` & `gink-0.20240518.1716010702/gink/impl/muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/pair_map.py` & `gink-0.20240518.1716010702/gink/impl/pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/pair_set.py` & `gink-0.20240518.1716010702/gink/impl/pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/property.py` & `gink-0.20240518.1716010702/gink/impl/property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/selectable_console.py` & `gink-0.20240518.1716010702/gink/impl/selectable_console.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/sequence.py` & `gink-0.20240518.1716010702/gink/impl/sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/tuples.py` & `gink-0.20240518.1716010702/gink/impl/tuples.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/typedefs.py` & `gink-0.20240518.1716010702/gink/impl/typedefs.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 MuTimestamp = int
 Offset = NewType('Offset', int)
 GenericTimestamp = Union[datetime, timedelta, date, int, float, str, None]
 Destination = GenericTimestamp
 UserKey = Union[str, int, bytes]
 UserValue = Union[str, int, float, datetime, bytes, bool, list, tuple, dict, None]
 EPOCH = 0
-
+Limit = Union[int, float]
 
 class Deletion: # pylint: disable=too-few-public-methods
     """ Used internally to indicate that a key/value assocation has been removed. """
 
 class Inclusion:
     """ Used to indicate adding something to a set or group. """
```

### Comparing `gink-0.20240516.1715898271/gink/impl/utilities.py` & `gink-0.20240518.1716010702/gink/impl/utilities.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/watcher.py` & `gink-0.20240518.1716010702/gink/impl/watcher.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/websocket_connection.py` & `gink-0.20240518.1716010702/gink/impl/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/wsgi_connection.py` & `gink-0.20240518.1716010702/gink/impl/wsgi_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/impl/wsgi_listener.py` & `gink-0.20240518.1716010702/gink/impl/wsgi_listener.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_box.py` & `gink-0.20240518.1716010702/gink/tests/test_box.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_chain_tracker.py` & `gink-0.20240518.1716010702/gink/tests/test_chain_tracker.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_change_set_info.py` & `gink-0.20240518.1716010702/gink/tests/test_change_set_info.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_code_values.py` & `gink-0.20240518.1716010702/gink/tests/test_code_values.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_container.py` & `gink-0.20240518.1716010702/gink/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_database.py` & `gink-0.20240518.1716010702/gink/tests/test_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """ tests that the add_bundle works """
     store = MemoryStore()
     database = Database(store=store)
     started = database.get_now()
     bundler = Bundler("just a test")
     database.bundle(bundler)
     bundles: List[BundleInfo] = []
-    store.get_bundles(lambda _, info: bundles.append(info))
+    store.get_bundles(lambda _: bundles.append(_.get_info()))
     assert len(bundles) == 2
     assert bundles[-1].comment == "just a test"
     assert bundles[-1].timestamp > started
 
 
 def test_negative_as_of():
     for store in [MemoryStore(), LmdbStore()]:
```

### Comparing `gink-0.20240516.1715898271/gink/tests/test_demo.py` & `gink-0.20240518.1716010702/gink/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_directory.py` & `gink-0.20240518.1716010702/gink/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_graph.py` & `gink-0.20240518.1716010702/gink/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_key_set.py` & `gink-0.20240518.1716010702/gink/tests/test_key_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_lmdb_store.py` & `gink-0.20240518.1716010702/gink/tests/test_lmdb_store.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_logbackedstore.py` & `gink-0.20240518.1716010702/gink/tests/test_logbackedstore.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_muid.py` & `gink-0.20240518.1716010702/gink/tests/test_muid.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_names.py` & `gink-0.20240518.1716010702/gink/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_pair_map.py` & `gink-0.20240518.1716010702/gink/tests/test_pair_map.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_pair_set.py` & `gink-0.20240518.1716010702/gink/tests/test_pair_set.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_property.py` & `gink-0.20240518.1716010702/gink/tests/test_property.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_role.py` & `gink-0.20240518.1716010702/gink/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_sequence.py` & `gink-0.20240518.1716010702/gink/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_store.py` & `gink-0.20240518.1716010702/gink/tests/test_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 # gink generated proto modules
 from ..impl.builders import BundleBuilder
 from google.protobuf.text_format import Parse  # type: ignore
 
 # gink stuff
 from ..impl.abstract_store import AbstractStore
 from ..impl.bundle_info import BundleInfo
+from ..impl.bundle_wrapper import BundleWrapper
 from ..impl.muid import Muid
+from ..impl.tuples import Chain
 
 StoreMaker = Callable[[], AbstractStore]
 
 
 def curried(a_function, some_data) -> Callable[[], None]:
     """ returns a function with the first argument applied to the second """
 
@@ -76,14 +78,40 @@
 
         result_ext_second = store.apply_bundle(ext_bytes)
         assert not result_ext_second
     finally:
         store.close()
 
 
+def generic_limit_to(store_maker: StoreMaker):
+    """ Ensures that chains with missing links throw exceptions. """
+    with closing(store_maker()) as store:
+        store.apply_bundle(make_empty_bundle(BundleInfo(medallion=123, chain_start=456, timestamp=456, comment="a1")))
+        store.apply_bundle(make_empty_bundle(
+            BundleInfo(medallion=123, chain_start=456, timestamp=456, previous=456, comment="a2")))
+
+        store.apply_bundle(make_empty_bundle(BundleInfo(medallion=775, chain_start=456, timestamp=456, comment="b1")))
+        store.apply_bundle(make_empty_bundle(
+            BundleInfo(medallion=775, chain_start=456, timestamp=456, previous=456, comment="b2")))
+
+        store.apply_bundle(make_empty_bundle(BundleInfo(medallion=137, chain_start=456, timestamp=456, comment="c1")))
+        store.apply_bundle(make_empty_bundle(
+            BundleInfo(medallion=137, chain_start=456, timestamp=456, previous=456, comment="c2")))
+
+        limit_to = {
+            Chain(123, 456): float("inf"),
+            Chain(775, 456): 456,
+        }
+
+        infos = store.get_bundle_infos(limit_to=limit_to)
+        assert len(infos) == 3
+        comments = [info.comment for info in infos]
+        assert comments == ["a1", "b1", "a2"], comments
+
+
 def generic_test_rejects_gap(store_maker: StoreMaker):
     """ Ensures that chains with missing links throw exceptions. """
     with closing(store_maker()) as store:
         start_info = BundleInfo(medallion=123, chain_start=456, timestamp=456, comment="start")
         start_bytes = make_empty_bundle(start_info)
         store.apply_bundle(start_bytes)
 
@@ -143,16 +171,16 @@
         store.apply_bundle(cs1)
         store.apply_bundle(cs2)
         store.apply_bundle(cs3)
         store.apply_bundle(cs4)
 
         ordered = []
 
-        def appender(bundle, info):
-            ordered.append((bundle, info))
+        def appender(wrapper: BundleWrapper):
+            ordered.append((wrapper.get_bytes(), wrapper.get_info()))
 
         store.get_bundles(appender)
         assert len(ordered) == 4
         assert ordered[0] == (cs1, info1)
         assert ordered[1] == (cs3, info3) or ordered[1] == (cs2, info2)
         assert ordered[2] == (cs2, info2) or ordered[2] == (cs3, info3)
         assert ordered[3] == (cs4, info4)
```

### Comparing `gink-0.20240516.1715898271/gink/tests/test_websocket_connection.py` & `gink-0.20240518.1716010702/gink/tests/test_websocket_connection.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink/tests/test_wsgi_server.py` & `gink-0.20240518.1716010702/gink/tests/test_wsgi_server.py`

 * *Files identical despite different names*

### Comparing `gink-0.20240516.1715898271/gink.egg-info/PKG-INFO` & `gink-0.20240518.1716010702/gink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gink
-Version: 0.20240516.1715898271
+Version: 0.20240518.1716010702
 Summary: a system for storing data structures in lmdb
 Home-page: https://github.com/x5e/gink
 Author: Darin McGill
 Author-email: gink@darinmcgill.com
 Keywords: gink lmdb crdt history versioned
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `gink-0.20240516.1715898271/gink.egg-info/SOURCES.txt` & `gink-0.20240518.1716010702/gink.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 gink/impl/__init__.py
 gink/impl/abstract_store.py
 gink/impl/addressable.py
 gink/impl/attribution.py
 gink/impl/box.py
 gink/impl/builders.py
 gink/impl/bundle_info.py
+gink/impl/bundle_store.py
 gink/impl/bundle_wrapper.py
 gink/impl/bundler.py
 gink/impl/chain_tracker.py
 gink/impl/coding.py
 gink/impl/connection.py
 gink/impl/container.py
 gink/impl/database.py
```

### Comparing `gink-0.20240516.1715898271/setup.py` & `gink-0.20240518.1716010702/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='gink',
-    version='0.20240516.1715898271',
+    version='0.20240518.1716010702',
     description='a system for storing data structures in lmdb',
     url='https://github.com/x5e/gink',
     author='Darin McGill',
     author_email="gink@darinmcgill.com",
     classifiers=[
         'Development Status :: 4 - Beta',
         "Intended Audience :: Developers",
```

