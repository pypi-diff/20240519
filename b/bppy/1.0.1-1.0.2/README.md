# Comparing `tmp/bppy-1.0.1.tar.gz` & `tmp/bppy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bppy-1.0.1.tar", last modified: Thu Jan 11 12:57:33 2024, max compression
+gzip compressed data, was "bppy-1.0.2.tar", last modified: Sun May 19 09:47:03 2024, max compression
```

## Comparing `bppy-1.0.1.tar` & `bppy-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.893583 bppy-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-11 12:57:25.000000 bppy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-11 12:57:25.000000 bppy-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-01-11 12:57:33.893583 bppy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-01-11 12:57:25.000000 bppy-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.885583 bppy-1.0.1/bppy/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.885583 bppy-1.0.1/bppy/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/analysis/bprogram_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/analysis/dfs_bprogram_verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/analysis/symbolic_bprogram_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.885583 bppy-1.0.1/bppy/execution/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.885583 bppy-1.0.1/bppy/execution/listeners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/execution/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/execution/listeners/b_program_runner_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/execution/listeners/print_b_program_runner_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.889582 bppy-1.0.1/bppy/gym/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/gym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/gym/bp_action_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/gym/bp_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/gym/bp_observation_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/gym/simple_bp_observation_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.889582 bppy-1.0.1/bppy/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/b_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/b_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/bprogram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.889582 bppy-1.0.1/bppy/model/event_selection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/experimental_smt_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/priority_based_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/rich_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/simple_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/smt_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_selection/solver_based_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/event_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/model/sync_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.893583 bppy-1.0.1/bppy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/utils/dfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/utils/weighted_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-11 12:57:25.000000 bppy-1.0.1/bppy/utils/z3helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.893583 bppy-1.0.1/bppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-01-11 12:57:33.000000 bppy-1.0.1/bppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-01-11 12:57:33.000000 bppy-1.0.1/bppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 12:57:33.000000 bppy-1.0.1/bppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-11 12:57:33.000000 bppy-1.0.1/bppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-11 12:57:33.000000 bppy-1.0.1/bppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 12:57:33.893583 bppy-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-11 12:57:25.000000 bppy-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 12:57:33.893583 bppy-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-01-11 12:57:25.000000 bppy-1.0.1/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-11 12:57:25.000000 bppy-1.0.1/tests/test_bprogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-11 12:57:25.000000 bppy-1.0.1/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-01-11 12:57:25.000000 bppy-1.0.1/tests/test_dfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-01-11 12:57:25.000000 bppy-1.0.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-01-11 12:57:25.000000 bppy-1.0.1/tests/test_gym.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.435443 bppy-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 09:46:59.000000 bppy-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-19 09:46:59.000000 bppy-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-19 09:47:03.435443 bppy-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-19 09:46:59.000000 bppy-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.427443 bppy-1.0.2/bppy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.427443 bppy-1.0.2/bppy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/analysis/bprogram_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/analysis/dfs_bprogram_verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/analysis/symbolic_bprogram_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.427443 bppy-1.0.2/bppy/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.427443 bppy-1.0.2/bppy/execution/listeners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/execution/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/execution/listeners/b_program_runner_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/execution/listeners/print_b_program_runner_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.427443 bppy-1.0.2/bppy/gym/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/gym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/gym/bp_action_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/gym/bp_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/gym/bp_observation_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/gym/simple_bp_observation_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.431444 bppy-1.0.2/bppy/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/b_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/b_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/bprogram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.431444 bppy-1.0.2/bppy/model/event_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/experimental_smt_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/priority_based_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/rich_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/simple_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/smt_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_selection/solver_based_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/event_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/model/sync_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.431444 bppy-1.0.2/bppy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/utils/dfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/utils/weighted_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-19 09:46:59.000000 bppy-1.0.2/bppy/utils/z3helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.431444 bppy-1.0.2/bppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-19 09:47:03.000000 bppy-1.0.2/bppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-19 09:47:03.000000 bppy-1.0.2/bppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:47:03.000000 bppy-1.0.2/bppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-19 09:47:03.000000 bppy-1.0.2/bppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 09:47:03.000000 bppy-1.0.2/bppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:47:03.435443 bppy-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-19 09:46:59.000000 bppy-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:47:03.431444 bppy-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-19 09:46:59.000000 bppy-1.0.2/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-19 09:46:59.000000 bppy-1.0.2/tests/test_bprogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-19 09:46:59.000000 bppy-1.0.2/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-19 09:46:59.000000 bppy-1.0.2/tests/test_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12315 2024-05-19 09:46:59.000000 bppy-1.0.2/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-19 09:46:59.000000 bppy-1.0.2/tests/test_gym.py
```

### Comparing `bppy-1.0.1/LICENSE` & `bppy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/PKG-INFO` & `bppy-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bppy
-Version: 1.0.1
+Version: 1.0.2
 Summary: BPpy: Behavioral Programming In Python
 Home-page: https://github.com/bThink-BGU/BPpy
 Author: Tom Yaacov
 Author-email: tomyaacov1210@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: z3-solver>=4.8.5.0
 Provides-Extra: gym
 Requires-Dist: gymnasium>=0.28.1; extra == "gym"
 Requires-Dist: stable-baselines3>=2.0.0; extra == "gym"
 Provides-Extra: develop
```

### Comparing `bppy-1.0.1/README.md` & `bppy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/__init__.py` & `bppy-1.0.2/bppy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from os import listdir
 from os.path import dirname, basename, isfile, join, isdir
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 # TODO: find a smarter way to import all submodules
 from bppy.execution.listeners.b_program_runner_listener import *
 from bppy.execution.listeners.print_b_program_runner_listener import *
 from bppy.model.event_selection.event_selection_strategy import *
 from bppy.model.event_selection.simple_event_selection_strategy import *
 from bppy.model.event_selection.solver_based_event_selection_strategy import *
 from bppy.model.event_selection.smt_event_selection_strategy import *
```

### Comparing `bppy-1.0.1/bppy/analysis/bprogram_converter.py` & `bppy-1.0.2/bppy/analysis/bprogram_converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
 		names = [x.name for x in dfs.event_list]
 		events = {e: BEvent(e) for e in names}
 		bp_states = {self.bt_names[i]:v for i, v in mapper.items()}
 
 		return names, events, bp_states
 
+	#def 
+
 	def to_prism(self, output_file=None):
 		"""
 		Converts the behavioral program to a PRISM model of a markov decision process, with each bthread corresponding to a module.
 		Returns the resulting text content.
 
 		Parameters
 		----------
@@ -62,80 +64,67 @@
 		"""
 
 		event_names, events, bp_states = self.collect_structure()
 
 		rule_template = "formula {}_{} = {};"
 		bt_condition = "({}_{}_{}={})"
 
-		header = 'mdp\n\n'
-
-		req = [rule_template.format(e, "req",
-				' | '.join([bt_condition.format(bt,'req',e,'true')
-				for bt in self.bt_names]))
-			for e in event_names]
-
-		block = [rule_template.format(e, "block",
-				' | '.join([bt_condition.format(bt,'block',e,'true')
-				for bt in self.bt_names]))
-			for e in event_names]
-
-		enable = [rule_template.format(e, "enabled",
-				' & '.join([f'({e}_req=true)',
-							f'({e}_block=false)']))
-			for e in event_names]
-
-		labels = ["//event {} = {};".format(i, e)
-			for i, e in enumerate(event_names)]
-		
-		event_transition = '[{}] ({}_enabled=true) -> 1: (event\'={});'
-		guards = '\n\t'.join([event_transition.format(e, e, i)
-						for i, e in enumerate(event_names)])
-		module_main = f'\nmodule main\n\tevent: [-1..{len(event_names)}] init -1;'+\
-						f'\n\t{guards}\nendmodule\n'
-
-		header += '\n\n'.join(
-			['\n'.join(sec) for sec in [req,block,enable,
-				labels]])
-		
-		header += module_main
-		header += '\n//-----------------------\n\n'
-
-		def format_bt_module(name, event_names, bt_states):
+		header = 'dtmc\n\n'
 
-			node_to_s = {s: i for i, s in enumerate(bp_states[name])}
+		def map_bt_states(event_names, bt_states):
+			node_to_s = {s: i for i, s in enumerate(bt_states)}
+			relevant_events = {e: False for e in event_names}
 
 			bt_req = {e: [] for e in event_names}
 			bt_block = {e: [] for e in event_names}
 			bt_trans = {}
 			bt_probs = {}
 
 			for node, n in node_to_s.items():
 				if isinstance(node.data, sync):
 					bt_trans[n] = {}
+					if ('request' in node.data):
+						if isinstance(node.data['request'], Iterable):
+							for e in node.data['request']:
+								bt_req[e.name].append(n)
+						elif isinstance(node.data['request'], BEvent):
+							bt_req[node.data['request'].name].append(n)
+						else:
+							raise BPAssertionError("Request of an unknown type")
+					if ('block' in node.data):
+						if isinstance(node.data['block'], Iterable):
+							for e in node.data['block']:
+								bt_block[e.name].append(n)
+						elif isinstance(node.data['block'], BEvent):
+							bt_block[node.data['block'].name].append(n)
+						else:
+							raise BPAssertionError("Block of an unknown type")
 					for e in event_names:
-						if ('request' in node.data):
-							if (isinstance(node.data['request'], Iterable) and
-									events[e] in node.data['request']):
-								bt_req[e].append(n)
-							elif (isinstance(node.data['request'], BEvent) and
-									events[e] == node.data['request']):
-								bt_req[e].append(n)
-						if ('block' in node.data):
-							if (isinstance(node.data['block'], Iterable) and
-									events[e] in node.data['block']):
-								bt_block[e].append(n)
-							elif (isinstance(node.data['block'], BEvent) and
-									events[e] == node.data['block']):
-								bt_block[e].append(n)
 						bt_trans[n][e] = (node_to_s[node.transitions[events[e]]] if
-										events[e] in node.transitions else n)
+								events[e] in node.transitions else n)
+					for t in node.transitions:
+						if node.transitions[t] != node: 
+							relevant_events[t.name] = True
 				if isinstance(node.data, choice):
 					bt_probs[n] = {choice_outcome: (node_to_s[node.transitions[choice_outcome][0]],
 												choice_prob) for choice_outcome, choice_prob in node.data.options()}
 
+			for e, n in bt_req.items():
+				if not relevant_events[e] and len(n) > 0:
+					relevant_events[e] = True
+			for e, n in bt_block.items():
+				if not relevant_events[e] and len(n) > 0:
+					relevant_events[e] = True
+
+			return bt_req, bt_block, bt_trans, bt_probs, relevant_events
+
+		def format_bt_module(name, event_names, bt_states):
+			bt_req, bt_block, bt_trans, bt_probs, relevant_events = map_bt_states(event_names, bt_states)
+			event_names = [e for e in event_names if relevant_events[e]]
+
 			module_template = '\nmodule {}\n\t{}\n\n\t{}\nendmodule\n'
 			state_template = "formula {}_{}_{} = {};"
 			state_name = f's_{name}'
 			state_init = f'{state_name}: [0..{len(bt_states)-1}] init 0;'
 			event_transition = '[{}] ({}={}) -> 1: ({}\'={});'
 			prob_transition = '[] ({}={}) -> {};'
 			prob_format = '{}: ({}\'={})'
@@ -149,15 +138,16 @@
 					' | '.join([('({}={})').format(state_name, n)
 					for n in bt_block[e]]) if len(bt_block[e]) > 0 else 'false')
 				for e in event_names]
 
 			transitions = []
 			for n, tr in bt_trans.items():
 				string_tr = [event_transition.format(e, state_name,
-								n, state_name, s_tag) for e, s_tag in tr.items()]
+								n, state_name, s_tag) for e, s_tag in tr.items()
+								if e in event_names]
 				transitions.append('\n\t'.join(string_tr))
 			
 			probabilities = []
 			for n, c in bt_probs.items():
 				string_prob = [prob_format.format(p, state_name, next_state)
 								for next_state, p in c.values()]
 				probabilities.append(prob_transition.format(state_name, n,
@@ -166,18 +156,51 @@
 			module = ''
 			module += '\n\n'.join(
 				['\n'.join(sec) for sec in [req,block]])
 
 			module += module_template.format(name,
 									state_init, '\n\t\n\t'.join(transitions + probabilities))
 
-			return module
+			return module, event_names
 
-
-		content = '\n\n'.join([format_bt_module(bt_name, event_names,
+		text, bt_events = zip(*[format_bt_module(bt_name, event_names,
 								bp_states[bt_name]) for bt_name in self.bt_names])
+		content = '\n\n'.join([t for t in text])
+		
+		# header regulating which events are enabled + main module
 		
+		req = [rule_template.format(e, "req",
+				' | '.join([bt_condition.format(bt,'req',e,'true')
+				for i, bt in enumerate(self.bt_names) if e in bt_events[i]]))
+			for e in event_names]
+
+		block = [rule_template.format(e, "block",
+				' | '.join([bt_condition.format(bt,'block',e,'true')
+				for i, bt in enumerate(self.bt_names) if e in bt_events[i]]))
+			for e in event_names]
+
+		enable = [rule_template.format(e, "enabled",
+				' & '.join([f'({e}_req=true)',
+							f'({e}_block=false)']))
+			for e in event_names]
+
+		labels = ["label \"{}\" = ({}_enabled=true);".format(e, e)
+					for e in event_names]
+		
+		event_transition = '[{}] ({}_enabled=true) -> 1: (event\'={});'
+		guards = '\n\t'.join([event_transition.format(e, e, i)
+						for i, e in enumerate(event_names)])
+		module_main = f'\nmodule main\n\tevent: [-1..{len(event_names)}] init -1;'+\
+						f'\n\t{guards}\nendmodule\n'
+
+		header += '\n\n'.join(
+			['\n'.join(sec) for sec in [req,block,enable,
+				labels]])
+		
+		header += module_main
+		header += '\n//-----------------------\n\n'
+
 		if output_file:
 			with open(output_file, "w") as f:
 				f.write(header + content)
 		return header + content
```

### Comparing `bppy-1.0.1/bppy/analysis/dfs_bprogram_verifier.py` & `bppy-1.0.2/bppy/analysis/dfs_bprogram_verifier.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/analysis/symbolic_bprogram_verifier.py` & `bppy-1.0.2/bppy/analysis/symbolic_bprogram_verifier.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/execution/listeners/b_program_runner_listener.py` & `bppy-1.0.2/bppy/execution/listeners/b_program_runner_listener.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/execution/listeners/print_b_program_runner_listener.py` & `bppy-1.0.2/bppy/execution/listeners/print_b_program_runner_listener.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/gym/bp_action_space.py` & `bppy-1.0.2/bppy/gym/bp_action_space.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/gym/bp_env.py` & `bppy-1.0.2/bppy/gym/bp_env.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/gym/bp_observation_space.py` & `bppy-1.0.2/bppy/gym/bp_observation_space.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/gym/simple_bp_observation_space.py` & `bppy-1.0.2/bppy/gym/simple_bp_observation_space.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/b_event.py` & `bppy-1.0.2/bppy/model/b_event.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/b_thread.py` & `bppy-1.0.2/bppy/model/b_thread.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/bprogram.py` & `bppy-1.0.2/bppy/model/bprogram.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/event_selection/event_selection_strategy.py` & `bppy-1.0.2/bppy/model/event_selection/event_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/event_selection/priority_based_event_selection_strategy.py` & `bppy-1.0.2/bppy/model/event_selection/priority_based_event_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/event_selection/rich_event_selection_strategy.py` & `bppy-1.0.2/bppy/model/event_selection/rich_event_selection_strategy.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,9 +6,9 @@
     """
     A solver-based implementation of EventSelectionStrategy using z3 SMT solver. The strategy used is the one
     presented in the paper `Executing Scenario-Based Specification with Dynamic Generation of Rich Events
     <https://www.wisdom.weizmann.ac.il/~dharel/papers/CCIS2019RichEvents.pdf>`_.
     """
 
     def is_satisfied(self, event, statement):
-        return is_true(event.eval(statement.get('waitFor', true)))
+        return is_true(event.eval(statement.get('waitFor', true), model_completion=True))
```

### Comparing `bppy-1.0.1/bppy/model/event_selection/simple_event_selection_strategy.py` & `bppy-1.0.2/bppy/model/event_selection/simple_event_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/event_selection/smt_event_selection_strategy.py` & `bppy-1.0.2/bppy/model/event_selection/smt_event_selection_strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     A solver-based implementation of EventSelectionStrategy using z3 SMT solver. The strategy used is the one
     presented in the paper `Executing Scenario-Based Specification with Dynamic Generation of Rich Events
     <https://www.wisdom.weizmann.ac.il/~dharel/papers/CCIS2019RichEvents.pdf>`_, with the difference that
     b-threads are continued if the selected assignment is either requested or waited for.
     For the original strategy, see :class:`RichEventSelectionStrategy<bppy.model.event_selection.rich_event_selection_strategy.RichEventSelectionStrategy>`.
     """
     def is_satisfied(self, event, statement):
-        return is_true(event.eval(statement.get('waitFor', false)) or event.eval(statement.get('request', false)))
+        return is_true(event.eval(statement.get('waitFor', false), model_completion=True) or event.eval(statement.get('request', false), model_completion=True))
 
     # TODO: implement a way to set additional_statement
     def select(self, statements, additional_statement=None):
         if isinstance(additional_statement, list) and len(additional_statement) > 0:
             raise NotImplementedError("SMTEventSelectionStrategy does not support external events.")
         (request, block) = (false, false)
```

### Comparing `bppy-1.0.1/bppy/model/event_selection/solver_based_event_selection_strategy.py` & `bppy-1.0.2/bppy/model/event_selection/solver_based_event_selection_strategy.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/event_set.py` & `bppy-1.0.2/bppy/model/event_set.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/model/sync_statement.py` & `bppy-1.0.2/bppy/model/sync_statement.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/utils/dfs.py` & `bppy-1.0.2/bppy/utils/dfs.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/utils/weighted_sampling.py` & `bppy-1.0.2/bppy/utils/weighted_sampling.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy/utils/z3helper.py` & `bppy-1.0.2/bppy/utils/z3helper.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/bppy.egg-info/PKG-INFO` & `bppy-1.0.2/bppy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: bppy
-Version: 1.0.1
+Version: 1.0.2
 Summary: BPpy: Behavioral Programming In Python
 Home-page: https://github.com/bThink-BGU/BPpy
 Author: Tom Yaacov
 Author-email: tomyaacov1210@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: z3-solver>=4.8.5.0
 Provides-Extra: gym
 Requires-Dist: gymnasium>=0.28.1; extra == "gym"
 Requires-Dist: stable-baselines3>=2.0.0; extra == "gym"
 Provides-Extra: develop
```

### Comparing `bppy-1.0.1/bppy.egg-info/SOURCES.txt` & `bppy-1.0.2/bppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/setup.py` & `bppy-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,9 +42,9 @@
     install_requires=[
         "z3-solver>=4.8.5.0"
     ],
     extras_require={
         "gym": gym_dependencies,
         "develop": gym_dependencies + develop_dependencies
     },
-    python_requires='>=3.4'
+    python_requires='>=3.9'
 )
```

### Comparing `bppy-1.0.1/tests/test_analysis.py` & `bppy-1.0.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/tests/test_bprogram.py` & `bppy-1.0.2/tests/test_bprogram.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/tests/test_conversion.py` & `bppy-1.0.2/tests/test_conversion.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import unittest
 import bppy as bp
 from bppy.analysis.bprogram_converter import BProgramConverter
 
 class TestBProgram(unittest.TestCase):
 
 	def test_prism_conversion(self):
-		@bp.thread
+		@bp.analysis_thread
 		def main():
 			r = yield bp.choice({'a': 0.2, 'b': 0.3, 'c': 0.5})
-			yield bp.sync(request=bp.BEvent(f'event_{r}'))
+			yield bp.sync(request=bp.BEvent(r))
 
 		def bp_gen():
 			return bp.BProgram(bthreads=[main()],
 							event_selection_strategy=bp.SimpleEventSelectionStrategy())
 
 		converter = BProgramConverter(bp_gen, [bp.BEvent('a'), bp.BEvent('b'), bp.BEvent('c')])
 		output = converter.to_prism(None)
```

### Comparing `bppy-1.0.1/tests/test_dfs.py` & `bppy-1.0.2/tests/test_dfs.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/tests/test_examples.py` & `bppy-1.0.2/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `bppy-1.0.1/tests/test_gym.py` & `bppy-1.0.2/tests/test_gym.py`

 * *Files identical despite different names*

