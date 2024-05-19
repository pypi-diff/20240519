# Comparing `tmp/pyperf-2.6.3.tar.gz` & `tmp/pyperf-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperf-2.6.3.tar", last modified: Wed Mar  6 12:02:13 2024, max compression
+gzip compressed data, was "pyperf-2.7.0.tar", last modified: Sun May 19 01:57:01 2024, max compression
```

## Comparing `pyperf-2.6.3.tar` & `pyperf-2.7.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:02:13.784664 pyperf-2.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-06 12:02:05.000000 pyperf-2.6.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-06 12:02:05.000000 pyperf-2.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-06 12:02:13.784664 pyperf-2.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-06 12:02:05.000000 pyperf-2.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-06 12:02:05.000000 pyperf-2.6.3/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:02:13.772664 pyperf-2.6.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/analyze.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26258 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    28583 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/developer_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:02:13.772664 pyperf-2.6.3/doc/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/bench_async_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/bench_async_func_with_loop_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      145 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/bench_command.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      145 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/bench_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/bench_time_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/bench_timeit.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/export_csv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1345 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/hist_scipy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2487 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)    38613 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/hist_scipy_telco.png
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/outliers.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/py2.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/py3.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/run_benchmark.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/timeit_strip.json.gz
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-06 12:02:05.000000 pyperf-2.6.3/doc/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:02:13.776664 pyperf-2.6.3/pyperf/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26482 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27934 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    19725 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13104 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_collect_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    16008 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_cpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_linux_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_process_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_psutil_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27478 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    34176 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_timeit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_timeit_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_win_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:02:13.784664 pyperf-2.6.3/pyperf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/mult_list_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    35289 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/mult_list_py36.json
--rw-r--r--   0 runner    (1001) docker     (127)    72828 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/mult_list_py36_tags.json
--rw-r--r--   0 runner    (1001) docker     (127)    34915 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/mult_list_py37.json
--rw-r--r--   0 runner    (1001) docker     (127)    72454 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/mult_list_py37_tags.json
--rw-r--r--   0 runner    (1001) docker     (127)    35370 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/mult_list_py38.json
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    40602 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/telco.json
--rw-r--r--   0 runner    (1001) docker     (127)    19149 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    34088 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_perf_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)    16620 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_timeit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyperf/tests/track_memory.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 12:02:13.784664 pyperf-2.6.3/pyperf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-03-06 12:02:13.000000 pyperf-2.6.3/pyperf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-06 12:02:13.000000 pyperf-2.6.3/pyperf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 12:02:13.000000 pyperf-2.6.3/pyperf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-06 12:02:13.000000 pyperf-2.6.3/pyperf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-06 12:02:13.000000 pyperf-2.6.3/pyperf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-06 12:02:13.000000 pyperf-2.6.3/pyperf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-06 12:02:05.000000 pyperf-2.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 12:02:13.784664 pyperf-2.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-06 12:02:05.000000 pyperf-2.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:01.751436 pyperf-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 01:56:56.000000 pyperf-2.7.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-19 01:56:56.000000 pyperf-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-19 01:57:01.751436 pyperf-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-19 01:56:56.000000 pyperf-2.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-19 01:56:56.000000 pyperf-2.7.0/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:01.743436 pyperf-2.7.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/analyze.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26257 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28936 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24133 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/developer_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:01.743436 pyperf-2.7.0/doc/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      175 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/bench_async_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      260 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/bench_async_func_with_loop_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      145 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/bench_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      145 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/bench_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      599 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/bench_time_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/bench_timeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/export_csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1345 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/hist_scipy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2487 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    38613 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/hist_scipy_telco.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7243 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/outliers.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/py2.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/py3.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/run_benchmark.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6232 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/timeit_strip.json.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-19 01:56:56.000000 pyperf-2.7.0/doc/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:01.747436 pyperf-2.7.0/pyperf/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26482 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27908 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19725 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13291 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_collect_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_cpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_linux_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_process_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_psutil_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27477 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34285 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_timeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_timeit_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_win_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12794 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:01.751436 pyperf-2.7.0/pyperf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/mult_list_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35289 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/mult_list_py36.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72828 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/mult_list_py36_tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34915 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/mult_list_py37.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72454 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/mult_list_py37_tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35370 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/mult_list_py38.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40602 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/telco.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19149 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34080 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_perf_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18864 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16620 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_timeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyperf/tests/track_memory.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 01:57:01.751436 pyperf-2.7.0/pyperf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-19 01:57:01.000000 pyperf-2.7.0/pyperf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-19 01:57:01.000000 pyperf-2.7.0/pyperf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 01:57:01.000000 pyperf-2.7.0/pyperf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 01:57:01.000000 pyperf-2.7.0/pyperf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-19 01:57:01.000000 pyperf-2.7.0/pyperf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 01:57:01.000000 pyperf-2.7.0/pyperf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-19 01:56:56.000000 pyperf-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 01:57:01.751436 pyperf-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-19 01:56:56.000000 pyperf-2.7.0/tox.ini
```

### Comparing `pyperf-2.6.3/COPYING` & `pyperf-2.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/PKG-INFO` & `pyperf-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf
-Version: 2.6.3
+Version: 2.7.0
 Summary: Python module to run and analyze benchmarks
 Author-email: Victor Stinner <vstinner@redhat.com>
 Maintainer-email: Dong-hee Na <donghee.na@python.org>
 License: MIT
 Project-URL: Homepage, https://github.com/psf/pyperf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pyperf-2.6.3/README.rst` & `pyperf-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/TODO.rst` & `pyperf-2.7.0/TODO.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/Makefile` & `pyperf-2.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/analyze.rst` & `pyperf-2.7.0/doc/analyze.rst`

 * *Files 4% similar despite different names*

```diff
@@ -219,13 +219,19 @@
 pyperf determines whether two samples differ significantly using a `Student's
 two-sample, two-tailed t-test
 <https://en.wikipedia.org/wiki/Student's_t-test>`_ with alpha equals to
 ``0.95``.
 
 Render a table using ``--table`` option::
 
-    $ python3 -m pyperf compare_to py36.json py38.json --table
-    +-----------+---------+------------------------------+
-    | Benchmark | py36    | py38                         |
-    +===========+=========+==============================+
-    | timeit    | 4.70 us | 4.22 us: 1.11x faster (-10%) |
-    +-----------+---------+------------------------------+
+    $ python3 -m pyperf compare_to mult_list_py36.json mult_list_py38.json --table
+    +----------------+----------------+-----------------------+
+    | Benchmark      | mult_list_py36 | mult_list_py38        |
+    +================+================+=======================+
+    | [1,2]*1000     | 3.70 us        | 3.18 us: 1.16x faster |
+    +----------------+----------------+-----------------------+
+    | [1,2,3]*1000   | 4.61 us        | 4.17 us: 1.11x faster |
+    +----------------+----------------+-----------------------+
+    | Geometric mean | (ref)          | 1.09x faster          |
+    +----------------+----------------+-----------------------+
+
+    Benchmark hidden because not significant (1): [1]*1000
```

### Comparing `pyperf-2.6.3/doc/api.rst` & `pyperf-2.7.0/doc/api.rst`

 * *Files 0% similar despite different names*

```diff
@@ -675,15 +675,15 @@
 * ``date`` (str): date when the benchmark run started, formatted as ISO 8601
 * ``duration`` (int or float >= 0): total duration of the benchmark run in seconds (``float``)
 * ``name`` (non-empty str): benchmark name
 * ``loops`` (``int >= 1``): number of outer-loops per value (``int``)
 * ``inner_loops`` (``int >= 1``): number of inner-loops of the benchmark (``int``)
 * ``timer``: Implementation of ``time.perf_counter()``, and also resolution if
   available
-* ``tags``: (list of str, optional): A list of tags associated with the benchmark. If provided, the results output will be aggreggated by each tag.
+* ``tags``: (list of str, optional): A list of tags associated with the benchmark. If provided, the results output will be aggregated by each tag.
 
 Python metadata:
 
 * ``python_compiler``: Compiler name and version.
 * ``python_cflags``: Compiler flags used to compile Python.
 * ``python_executable``: path to the Python executable
 * ``python_hash_seed``: value of the ``PYTHONHASHSEED`` environment variable
```

### Comparing `pyperf-2.6.3/doc/changelog.rst` & `pyperf-2.7.0/doc/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog
 =========
 
+Version 2.7.0 (2024-05-18)
+---------------------------
+
+* Fix logic in MSR availability test.
+  Patch by Mike Droettboom.
+* Disable tuning TurboBoost setting on non-Intel device.
+  Patch by Mike Droettboom.
+* Include CONFIG_ARGS in Metadata.
+  Patch by Jeff Glass.
+* Support environment variables PYTHON_GIL / PYTHON_CPU_COUNT.
+  Patch by Donghee Na.
+
 Version 2.6.3 (2024-03-05)
 ---------------------------
 
 * Support Free-threading CPython (PEP-703) by disabling psutil related features.
   Relevant issue: https://github.com/python/cpython/issues/116024.
   Patch by Donghee Na.
 * Fix mem_max_rss measurement on macOS.
@@ -84,15 +96,15 @@
 --------------------------
 
 * The :ref:`compare_to command <compare_to_cmd>` now computes the geometric
   mean.
 * The :ref:`compare_to command <compare_to_cmd>` no longer displays
   percentages: display less numbers to make the output easier to read. Also,
   percentage were almost the same values than the xxx faster or xxx slower
-  values, but rounded differenly which introduced confusion.
+  values, but rounded differently which introduced confusion.
 * Project moved to https://github.com/psf/pyperf/
 * system command now only emits a warning rather than failing with a hard error
   if it fails to get or set the frequency of a CPU.
 * The pyperf project is now covered by the `PSF Code of Conduct
   <https://www.python.org/psf/codeofconduct/>`_.
 
 Version 2.0.0 (2020-03-19)
```

### Comparing `pyperf-2.6.3/doc/cli.rst` & `pyperf-2.7.0/doc/cli.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/conf.py` & `pyperf-2.7.0/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # pyperf documentation build configuration file, created by
 # sphinx-quickstart on Wed Jun  1 15:28:03 2016.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
@@ -38,24 +37,24 @@
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'pyperf'
-copyright = u'2016, Victor Stinner'
-author = u'Victor Stinner'
+project = 'pyperf'
+copyright = '2016, Victor Stinner'
+author = 'Victor Stinner'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = release = '2.6.3'
+version = release = '2.7.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
@@ -212,16 +211,16 @@
 #'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-  (master_doc, 'pyperf.tex', u'pyperf Documentation',
-   u'Victor Stinner', 'manual'),
+  (master_doc, 'pyperf.tex', 'pyperf Documentation',
+   'Victor Stinner', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -242,29 +241,29 @@
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'pyperf', u'pyperf Documentation',
+    (master_doc, 'pyperf', 'pyperf Documentation',
      [author], 1)
 ]
 
 # If true, show URL addresses after external links.
 #man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  (master_doc, 'pyperf', u'pyperf Documentation',
+  (master_doc, 'pyperf', 'pyperf Documentation',
    author, 'pyperf', 'One line description of project.',
    'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
```

### Comparing `pyperf-2.6.3/doc/examples/bench_time_func.py` & `pyperf-2.7.0/doc/examples/bench_time_func.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/examples/export_csv.py` & `pyperf-2.7.0/doc/examples/export_csv.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/examples/hist_scipy.py` & `pyperf-2.7.0/doc/examples/hist_scipy.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/examples/plot.py` & `pyperf-2.7.0/doc/examples/plot.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/examples.rst` & `pyperf-2.7.0/doc/examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 
 
 .. _timeit_example:
 
 timeit() method
 ---------------
 
-Benchmark using the :meth:`Runner.timeit` method to performance of sorting a
-sorted list of 1000 numbers using a ``key`` function (which does nothing):
+Benchmark using the :meth:`Runner.timeit` method to measure the performance of
+sorting a sorted list of 1000 numbers using a ``key`` function (which does
+nothing):
 
 .. literalinclude:: examples/bench_timeit.py
 
 
 .. _bench_command_example:
 
 bench_command() method
```

### Comparing `pyperf-2.6.3/doc/hist_scipy_telco.png` & `pyperf-2.7.0/doc/hist_scipy_telco.png`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/index.rst` & `pyperf-2.7.0/doc/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ++++++++++++++++++++
 Python pyperf module
 ++++++++++++++++++++
 
 The Python ``pyperf`` module is a toolkit to write, run and analyze benchmarks.
 
-Documenation:
+Documentation:
 
 .. toctree::
    :maxdepth: 2
 
    user_guide
    developer_guide
```

### Comparing `pyperf-2.6.3/doc/make.bat` & `pyperf-2.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/outliers.json.gz` & `pyperf-2.7.0/doc/outliers.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/py2.json.gz` & `pyperf-2.7.0/doc/py2.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/py3.json.gz` & `pyperf-2.7.0/doc/py3.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/run_benchmark.rst` & `pyperf-2.7.0/doc/run_benchmark.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/runner.rst` & `pyperf-2.7.0/doc/runner.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/system.rst` & `pyperf-2.7.0/doc/system.rst`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/doc/timeit_strip.json.gz` & `pyperf-2.7.0/doc/timeit_strip.json.gz`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/__init__.py` & `pyperf-2.7.0/pyperf/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from time import perf_counter
 
-VERSION = (2, 6, 3)
+VERSION = (2, 7, 0)
 __version__ = '.'.join(map(str, VERSION))
 
 # Export pyperf.perf_counter for backward compatibility with pyperf 1.7
 # which supports Python 2 and Python 3
 __all__ = ['perf_counter']
 
 from pyperf._utils import python_implementation, python_has_jit  # noqa
```

### Comparing `pyperf-2.6.3/pyperf/__main__.py` & `pyperf-2.7.0/pyperf/__main__.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_bench.py` & `pyperf-2.7.0/pyperf/_bench.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         value = func(self)
         setattr(self, attr, value)
         return value
 
     return method
 
 
-class Run(object):
+class Run:
     # Run is immutable, so it can be shared/exchanged between two benchmarks
 
     __slots__ = ('_warmups', '_values', '_metadata')
 
     def __init__(self, values, warmups=None,
                  metadata=None, collect_metadata=True):
         if any(not (isinstance(value, NUMBER_TYPES) and value > 0)
@@ -315,15 +315,15 @@
                 raise ValueError("inner_loops metadata cannot be modified")
 
         metadata2 = dict(self._metadata)
         metadata2.update(metadata)
         return self._replace(metadata=metadata2)
 
 
-class Benchmark(object):
+class Benchmark:
     def __init__(self, runs):
         self._runs = []   # list of Run objects
         self._clear_runs_cache()
 
         if not runs:
             raise ValueError("runs must be a non-empty sequence of Run objects")
 
@@ -623,15 +623,15 @@
         if not metadata:
             return self
 
         new_runs = [run._update_metadata(metadata) for run in self._runs]
         self._replace_runs(new_runs)
 
 
-class BenchmarkSuite(object):
+class BenchmarkSuite:
     def __init__(self, benchmarks, filename=None):
         if not benchmarks:
             raise ValueError("benchmarks must be a non-empty "
                              "sequence of Benchmark objects")
 
         self.filename = filename
         self._benchmarks = []
@@ -723,15 +723,15 @@
         return suite
 
     @staticmethod
     def _load_open(filename):
         if isinstance(filename, bytes):
             suffix = b'.gz'
         else:
-            suffix = u'.gz'
+            suffix = '.gz'
 
         if filename.endswith(suffix):
             # Use lazy import to limit imports on 'import pyperf'
             import gzip
             return gzip.open(filename, "rt", encoding="utf-8")
         else:
             return open(filename, "r", encoding="utf-8")
@@ -766,15 +766,15 @@
         return cls._json_load(None, data)
 
     @staticmethod
     def _dump_open(filename, replace):
         if isinstance(filename, bytes):
             suffix = b'.gz'
         else:
-            suffix = u'.gz'
+            suffix = '.gz'
 
         if not replace and os.path.exists(filename):
             raise OSError(errno.EEXIST, "File already exists")
 
         if filename.endswith(suffix):
             # Use lazy import to limit imports on 'import pyperf'
             import gzip
```

### Comparing `pyperf-2.6.3/pyperf/_cli.py` & `pyperf-2.7.0/pyperf/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,20 +600,20 @@
 
         yield
 
         # Flush files to be able to catch a broken pipe error if the pipe
         # was closed by the consumer
         for file in files:
             file.flush()
-    except IOError as exc:
+    except OSError as exc:
         if exc.errno != errno.EPIPE:
             raise
         # got a broken pipe error: ignore it
 
         # explicitly close files to prevent broken pipe error on implicit
         # close at exit which would log the error:
         # "Exception ignored in: ... BrokenPipeError: ..."
         for file in files:
             try:
                 file.close()
-            except IOError:
+            except OSError:
                 pass
```

### Comparing `pyperf-2.6.3/pyperf/_collect_metadata.py` & `pyperf-2.7.0/pyperf/_collect_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,19 @@
         pass
     else:
         cflags = sysconfig.get_config_var('CFLAGS')
         if cflags:
             cflags = normalize_text(cflags)
             metadata['python_cflags'] = cflags
 
+        config_args = sysconfig.get_config_var('CONFIG_ARGS')
+        if config_args:
+            config_args = normalize_text(config_args)
+            metadata['python_config_args'] = config_args
+
     # GC disabled?
     try:
         import gc
     except ImportError:
         pass
     else:
         if not gc.isenabled():
@@ -127,15 +132,15 @@
 
 def read_proc(path):
     path = proc_path(path)
     try:
         with open_text(path) as fp:
             for line in fp:
                 yield line.rstrip()
-    except (OSError, IOError):
+    except OSError:
         return
 
 
 def collect_linux_metadata(metadata):
     # ASLR
     for line in read_proc('sys/kernel/randomize_va_space'):
         if line == '0':
@@ -323,15 +328,15 @@
 
     index = 1
     while True:
         template = os.path.join(path, "temp%s_%%s" % index)
 
         try:
             temp_label = read_first_line(template % 'label', error=True)
-        except IOError:
+        except OSError:
             break
 
         temp_input = read_first_line(template % 'input', error=True)
         temp_input = float(temp_input) / 1000
         # On Python 2, u"%.0f\xb0C" introduces unicode errors if the
         # locale encoding is ASCII, so use a space.
         temp_input = "%.0f C" % temp_input
```

### Comparing `pyperf-2.6.3/pyperf/_command.py` & `pyperf-2.7.0/pyperf/_command.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_compare.py` & `pyperf-2.7.0/pyperf/_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     return format_normalized_mean(geo_mean)
 
 
 def get_tags_for_result(result):
     return result.ref.benchmark.get_metadata().get("tags", [])
 
 
-class CompareResult(object):
+class CompareResult:
     def __init__(self, ref, changed, min_speed=None):
         # CompareData object
         self.ref = ref
         # CompareData object
         self.changed = changed
         self._min_speed = min_speed
         self._significant = None
```

### Comparing `pyperf-2.6.3/pyperf/_cpu_utils.py` & `pyperf-2.7.0/pyperf/_cpu_utils.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_formatter.py` & `pyperf-2.7.0/pyperf/_formatter.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_linux_memory.py` & `pyperf-2.7.0/pyperf/_linux_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         return self.peak_usage
 
 
 def check_tracking_memory():
     mem_thread = PeakMemoryUsageThread()
     try:
         mem_thread.get()
-    except IOError as exc:
+    except OSError as exc:
         path = proc_path("self/smaps")
         return "unable to read %s: %s" % (path, exc)
 
     if not mem_thread.peak_usage:
         return "memory usage is zero"
 
     # it seems to work
```

### Comparing `pyperf-2.6.3/pyperf/_manager.py` & `pyperf-2.7.0/pyperf/_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 # Limit to 5 calibration processes
 # (10 if calibration is needed for loops and warmups)
 MAX_CALIBRATION = 5
 
 
-class Manager(object):
+class Manager:
     """
     Manager process which spawns worker processes to:
     - calibrate warmups
     - calibrate loops
     - compute values
 
     It uses a state machine with next_run attribute and the choose_next_run()
```

### Comparing `pyperf-2.6.3/pyperf/_metadata.py` & `pyperf-2.7.0/pyperf/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 
 def format_metadata(name, value):
     info = get_metadata_info(name)
     return info.formatter(value)
 
 
-class Metadata(object):
+class Metadata:
     def __init__(self, name, value):
         self._name = name
         self._value = value
 
     @property
     def name(self):
         return self._name
```

### Comparing `pyperf-2.6.3/pyperf/_process_time.py` & `pyperf-2.7.0/pyperf/_process_time.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_psutil_memory.py` & `pyperf-2.7.0/pyperf/_psutil_memory.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_runner.py` & `pyperf-2.7.0/pyperf/_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 class CLIError(Exception):
     pass
 
 
 class Runner:
     _created = set()
 
-    # Default parameters are chosen to have approximatively a run of 0.5 second
+    # Default parameters are chosen to have approximately a run of 0.5 second
     # and so a total duration of 5 seconds by default
     def __init__(self, values=None, processes=None,
                  loops=0, min_time=0.1, metadata=None,
                  show_name=True,
                  program_args=None, add_cmdline_args=None,
                  _argparser=None):
 
@@ -81,15 +81,15 @@
         try:
             sys._stats_off()
             sys._stats_clear()
         except AttributeError:
             pass
 
         # Watchdog: ensure that only once instance of Runner (or a Runner
-        # subclass) is created per process to prevent bad suprises
+        # subclass) is created per process to prevent bad surprises
         cls = self.__class__
         key = id(cls)
         if key in cls._created:
             raise RuntimeError("only one %s instance must be created "
                                "per process: use the same instance to run "
                                "all benchmarks" % cls.__name__)
         cls._created.add(key)
```

### Comparing `pyperf-2.6.3/pyperf/_system.py` & `pyperf-2.7.0/pyperf/_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import errno
 import os.path
+import platform
 import re
 import struct
 import subprocess
 import sys
 
 from pyperf._cli import display_title
 from pyperf._cpu_utils import (parse_cpu_list,
@@ -70,15 +71,15 @@
 def use_intel_pstate():
     cpu = 0
     path = sysfs_path("devices/system/cpu/cpu%s/cpufreq/scaling_driver" % cpu)
     scaling_driver = read_first_line(path)
     return (scaling_driver == 'intel_pstate')
 
 
-class Operation(object):
+class Operation:
     @staticmethod
     def available():
         return True
 
     def __init__(self, name, system):
         self.name = name
         self.system = system
@@ -103,15 +104,15 @@
     def check_permission_error(self, exc):
         if is_permission_error(exc):
             self.permission_error = True
 
     def read_first_line(self, path):
         try:
             return read_first_line(path, error=True)
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             return ''
 
     def show(self):
         pass
 
     def write(self, tune):
@@ -121,15 +122,19 @@
 class TurboBoostMSR(Operation):
     """
     Get/Set Turbo Boost mode of Intel CPUs using /dev/cpu/N/msr.
     """
 
     @staticmethod
     def available():
-        return (OS_LINUX and not use_intel_pstate())
+        return (
+            OS_LINUX and 
+            not use_intel_pstate() and 
+            platform.machine() in ('x86', 'x86_64', 'amd64')
+        )
 
     def __init__(self, system):
         Operation.__init__(self, 'Turbo Boost (MSR)', system)
         self.cpu_states = {}
         self.have_device = True
 
     def read_msr(self, cpu, reg_num, use_warnings=False):
@@ -215,15 +220,15 @@
                 if hasattr(os, 'pwrite'):
                     os.pwrite(fd, data, reg_num)
                 else:
                     os.lseek(fd, reg_num, os.SEEK_SET)
                     os.write(fd, data)
             finally:
                 os.close(fd)
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             self.error("Failed to write %#x into MSR %#x using %s: %s"
                        % (value, reg_num, path, exc))
             return False
 
         return True
 
@@ -304,15 +309,15 @@
         if self.enabled == enable:
             # no_turbo already set to the expected value
             return
 
         content = '0' if enable else '1'
         try:
             write_text(self.path, content)
-        except IOError as exc:
+        except OSError as exc:
             # don't log a permission error if the user is root: permission
             # error as root means that Turbo Boost is disabled in the BIOS
             if not is_root():
                 self.check_permission_error(exc)
 
             action = 'enable' if enable else 'disable'
             msg = "Failed to %s Turbo Boost" % action
@@ -372,23 +377,23 @@
             return
 
         new_governor = 'performance' if tune else 'powersave'
         if new_governor == self.governor:
             return
         try:
             write_text(self.path, new_governor)
-        except IOError as exc:
+        except OSError as exc:
             self.error("Failed to set the CPU scaling governor: %s" % exc)
         else:
             self.log_action("CPU scaling governor set to %s" % new_governor)
 
 
 class LinuxScheduler(Operation):
     """
-    Check isolcpus=cpus and rcu_nocbs=cpus paramaters of the Linux kernel
+    Check isolcpus=cpus and rcu_nocbs=cpus parameters of the Linux kernel
     command line.
     """
 
     @staticmethod
     def available():
         return OS_LINUX
 
@@ -491,15 +496,15 @@
 
         new_value = '2'
         if new_value == value:
             return
 
         try:
             write_text(self.path, new_value)
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             self.error("Failed to write into %s: %s" % (self.path, exc))
         else:
             self.log_action("Full randomization enabled: %r written into %s"
                             % (new_value, self.path))
 
 
@@ -548,15 +553,15 @@
             return
         self.log_state('; '.join(infos))
 
     def read_freq(self, filename):
         try:
             with open(filename, "rb") as fp:
                 return fp.readline()
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             return None
 
     def write_freq(self, filename, new_freq):
         with open(filename, "rb") as fp:
             freq = fp.readline()
 
@@ -575,15 +580,15 @@
         if not freq:
             self.warning("Unable to read %s of CPU %s" % (name, cpu))
             return False
 
         filename = os.path.join(cpu_path, "scaling_min_freq")
         try:
             return self.write_freq(filename, freq)
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             self.error("Unable to write scaling_max_freq of CPU %s: %s"
                        % (cpu, exc))
 
     def write(self, tune):
         modified = []
         for cpu in self.system.cpus:
@@ -764,29 +769,29 @@
         default_smp_affinity = self.read_default_affinity()
         if new_affinity == default_smp_affinity:
             return
 
         mask = format_cpus_as_mask(new_affinity)
         try:
             write_text(self.default_affinity_path, mask)
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             self.error("Failed to write %r into %s: %s"
                        % (mask, self.default_affinity_path, exc))
         else:
             self.log_action("Set default affinity to CPU %s"
                             % format_cpu_list(new_affinity))
 
     def write_irq(self, irq, cpus):
         path = self.irq_affinity_path % irq
         mask = format_cpus_as_mask(cpus)
         try:
             write_text(path, mask)
             return True
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             # EIO means that the IRQ doesn't support SMP affinity:
             # ignore the error
             if exc.errno != errno.EIO:
                 self.error("Failed to write %r into %s: %s"
                            % (mask, path, exc))
             return False
@@ -933,15 +938,15 @@
 
         max_sample_rate = self.read_max_sample_rate()
         if max_sample_rate == new_rate:
             return
 
         try:
             write_text(self.path, str(new_rate))
-        except IOError as exc:
+        except OSError as exc:
             self.check_permission_error(exc)
             self.error("Failed to write into %s: %s" % (self.path, exc))
         else:
             self.log_action("Max sample rate set to %s per second" % new_rate)
 
 
 OPERATIONS = [
```

### Comparing `pyperf-2.6.3/pyperf/_timeit.py` & `pyperf-2.7.0/pyperf/_timeit.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_timeit_cli.py` & `pyperf-2.7.0/pyperf/_timeit_cli.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_utils.py` & `pyperf-2.7.0/pyperf/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
 
 def read_first_line(path, error=False):
     try:
         with open_text(path) as fp:
             line = fp.readline()
         return line.rstrip()
-    except IOError:
+    except OSError:
         if error:
             raise
         else:
             return ''
 
 
 def proc_path(path):
@@ -262,31 +262,32 @@
     return os.path.normpath(python)
 
 
 def create_environ(inherit_environ, locale, copy_all):
     if copy_all:
         return os.environ
     env = {}
-
-    copy_env = ["PATH", "PYTHONPATH", "HOME", "TEMP", "COMSPEC", "SystemRoot", "SystemDrive"]
+    copy_env = ["PATH", "HOME", "TEMP", "COMSPEC", "SystemRoot", "SystemDrive",
+                # Python specific variables
+                "PYTHONPATH", "PYTHON_CPU_COUNT", "PYTHON_GIL"]
     if locale:
         copy_env.extend(('LANG', 'LC_ADDRESS', 'LC_ALL', 'LC_COLLATE',
                          'LC_CTYPE', 'LC_IDENTIFICATION', 'LC_MEASUREMENT',
                          'LC_MESSAGES', 'LC_MONETARY', 'LC_NAME', 'LC_NUMERIC',
                          'LC_PAPER', 'LC_TELEPHONE', 'LC_TIME'))
     if inherit_environ:
         copy_env.extend(inherit_environ)
 
     for name in copy_env:
         if name in os.environ:
             env[name] = os.environ[name]
     return env
 
 
-class _Pipe(object):
+class _Pipe:
     _OPEN_MODE = "r"
 
     def __init__(self, fd):
         self._fd = fd
         self._file = None
         if MS_WINDOWS:
             self._handle = msvcrt.get_osfhandle(fd)
```

### Comparing `pyperf-2.6.3/pyperf/_win_memory.py` & `pyperf-2.7.0/pyperf/_win_memory.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/_worker.py` & `pyperf-2.7.0/pyperf/_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         if args.calibrate_warmups or args.recalibrate_warmups:
             self.calibrate_warmups()
         elif args.calibrate_loops or args.recalibrate_loops:
             self.calibrate_loops()
         else:
             self.compute_warmups_values()
 
-        # collect metatadata
+        # collect metadata
         metadata2 = self.collect_metadata()
         metadata2.update(self.metadata)
         self.metadata = metadata2
 
         self.metadata['loops'] = self.loops
 
     def create_run(self):
```

### Comparing `pyperf-2.6.3/pyperf/tests/__init__.py` & `pyperf-2.7.0/pyperf/tests/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     finally:
         shutil.rmtree(tmpdir)
 
 
 def benchmark_as_json(benchmark, compact=True):
     with temporary_file() as tmp_name:
         benchmark.dump(tmp_name, compact=compact)
-        with io.open(tmp_name, 'r', encoding='utf-8') as tmp:
+        with open(tmp_name, 'r', encoding='utf-8') as tmp:
             return tmp.read()
 
 
 def compare_benchmarks(testcase, bench1, bench2):
     json1 = benchmark_as_json(bench1, compact=False)
     json2 = benchmark_as_json(bench2, compact=False)
     testcase.assertEqual(json1, json2)
```

### Comparing `pyperf-2.6.3/pyperf/tests/mult_list_py36.json` & `pyperf-2.7.0/pyperf/tests/mult_list_py36.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/mult_list_py36_tags.json` & `pyperf-2.7.0/pyperf/tests/mult_list_py36_tags.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/mult_list_py37.json` & `pyperf-2.7.0/pyperf/tests/mult_list_py37.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/mult_list_py37_tags.json` & `pyperf-2.7.0/pyperf/tests/mult_list_py37_tags.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/mult_list_py38.json` & `pyperf-2.7.0/pyperf/tests/mult_list_py38.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/replay.py` & `pyperf-2.7.0/pyperf/tests/replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     raw_values = [value * (loops * inner_loops)
                   for loops, value in run.warmups]
     total_loops = run.get_total_loops()
     raw_values.extend(value * total_loops for value in run.values)
     return (run, raw_values)
 
 
-class Replay(object):
+class Replay:
     def __init__(self, runner, filename):
         self.runner = runner
         self.args = runner.args
         self.filename = filename
         self.value_id = 0
         self.init()
```

### Comparing `pyperf-2.6.3/pyperf/tests/telco.json` & `pyperf-2.7.0/pyperf/tests/telco.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_bench.py` & `pyperf-2.7.0/pyperf/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_cli.py` & `pyperf-2.7.0/pyperf/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_examples.py` & `pyperf-2.7.0/pyperf/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_metadata.py` & `pyperf-2.7.0/pyperf/tests/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             if filename == '/sys/devices/system/cpu/cpu0/cpufreq/scaling_driver':
                 data = 'DRIVER\n'
             elif filename == '/sys/devices/system/cpu/cpu0/cpufreq/scaling_governor':
                 data = 'GOVERNOR\n'
             elif filename.startswith('/sys/devices/system/cpu/nohz_full'):
                 data = nohz_full
             elif filename.startswith('/sys/devices/system/cpu/cpu2'):
-                raise IOError
+                raise OSError
             elif filename == '/sys/devices/system/cpu/cpuidle/current_driver':
                 data = 'IDLE_DRV\n'
             else:
                 raise ValueError("unexpect open: %r" % filename)
             return io.StringIO(data)
 
         with mock.patch('pyperf._collect_metadata.get_isolated_cpus', return_value=[2]):
@@ -190,15 +190,15 @@
             if filename == '/proc/cpuinfo':
                 data = self.INTEL_CPU_INFO
             elif filename == '/sys/devices/system/cpu/cpu0/cpufreq/scaling_driver':
                 data = 'DRIVER\n'
             elif filename == '/sys/devices/system/cpu/cpu0/cpufreq/scaling_governor':
                 data = 'GOVERNOR\n'
             elif filename.startswith('/sys/devices/system/cpu/cpu2'):
-                raise IOError
+                raise OSError
             else:
                 raise ValueError("unexpect open: %r" % filename)
             return io.StringIO(data)
 
         with mock.patch('pyperf._utils.open', create=True, side_effect=mock_open):
             metadata = {}
             perf_metadata.collect_cpu_freq(metadata, [0, 2])
```

### Comparing `pyperf-2.6.3/pyperf/tests/test_misc.py` & `pyperf-2.7.0/pyperf/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_perf_cli.py` & `pyperf-2.7.0/pyperf/tests/test_perf_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pyperf import tests
 
 
 TESTDIR = os.path.dirname(__file__)
 TELCO = os.path.join(TESTDIR, 'telco.json')
 
 
-class BaseTestCase(object):
+class BaseTestCase:
     maxDiff = 100 * 80
 
     def create_bench(self, values, metadata=None):
         if metadata is None:
             metadata = {'name': 'bench'}
         elif 'name' not in metadata:
             metadata['name'] = 'bench'
```

### Comparing `pyperf-2.6.3/pyperf/tests/test_runner.py` & `pyperf-2.7.0/pyperf/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_system.py` & `pyperf-2.7.0/pyperf/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_timeit.py` & `pyperf-2.7.0/pyperf/tests/test_timeit.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/test_utils.py` & `pyperf-2.7.0/pyperf/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf/tests/track_memory.json` & `pyperf-2.7.0/pyperf/tests/track_memory.json`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyperf.egg-info/PKG-INFO` & `pyperf-2.7.0/pyperf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf
-Version: 2.6.3
+Version: 2.7.0
 Summary: Python module to run and analyze benchmarks
 Author-email: Victor Stinner <vstinner@redhat.com>
 Maintainer-email: Dong-hee Na <donghee.na@python.org>
 License: MIT
 Project-URL: Homepage, https://github.com/psf/pyperf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pyperf-2.6.3/pyperf.egg-info/SOURCES.txt` & `pyperf-2.7.0/pyperf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyperf-2.6.3/pyproject.toml` & `pyperf-2.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -57,7 +57,14 @@
 pyperf = "pyperf.__main__:main"
 
 [tool.setuptools]
 packages = ["pyperf", "pyperf.tests"]
 
 [tool.setuptools.dynamic]
 version = {attr = "pyperf.__version__"}
+
+[tool.ruff.lint]
+extend-select = ["C90", "UP"]
+extend-ignore = ["UP015", "UP031"]
+
+[tool.ruff.lint.mccabe]
+max-complexity = 31
```

