# Comparing `tmp/oresat_olaf-3.5.0.tar.gz` & `tmp/oresat_olaf-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_olaf-3.5.0.tar", last modified: Sat Apr 27 22:21:52 2024, max compression
+gzip compressed data, was "oresat_olaf-3.6.0.tar", last modified: Sun May 19 21:16:41 2024, max compression
```

## Comparing `oresat_olaf-3.5.0.tar` & `oresat_olaf-3.6.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.036912 oresat_olaf-3.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.040912 oresat_olaf-3.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.040912 oresat_olaf-3.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/adc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/app.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/cpufreq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/daemon.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/ecss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/gpio.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/node.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/oresat_file.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/oresat_file_cache.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/pru.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/resource.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/rest_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/service.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/timer_loop.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/api/updater.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/rest_api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/docs/updater/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/updater/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/docs/updater/update_archive.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/daemons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/resources/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)    13228 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.044912 oresat_olaf-3.5.0/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/daemons.html
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/reset.html
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/updater.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/_internals/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/os_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/services/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/_internals/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 22:21:51.000000 oresat_olaf-3.5.0/olaf/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/board/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/adc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/board/pru.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/canopen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/master_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/canopen/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.048912 oresat_olaf-3.5.0/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 22:21:52.000000 oresat_olaf-3.5.0/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/run.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_pru.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/common/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/resources/test_fwrite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/services/
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/services/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/test_rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.052912 oresat_olaf-3.5.0/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:21:52.056913 oresat_olaf-3.5.0/tests/internals/updater/test_files/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test-script.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611941111.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611947777.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611948888.tar.xz
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-04-27 22:21:47.000000 oresat_olaf-3.5.0/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.473163 oresat_olaf-3.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.477163 oresat_olaf-3.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.477163 oresat_olaf-3.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.481163 oresat_olaf-3.6.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/adc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/app.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/cpufreq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/daemon.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/ecss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/gpio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/node.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/oresat_file.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/oresat_file_cache.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/pru.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/rest_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/service.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/timer_loop.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/api/updater.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/rest_api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.481163 oresat_olaf-3.6.0/docs/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/updater/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/docs/updater/update_archive.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.481163 oresat_olaf-3.6.0/olaf/
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.481163 oresat_olaf-3.6.0/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.485163 oresat_olaf-3.6.0/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/resources/daemons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/resources/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.485163 oresat_olaf-3.6.0/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.485163 oresat_olaf-3.6.0/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.485163 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/daemons.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/reset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/updater.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.485163 oresat_olaf-3.6.0/olaf/_internals/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/services/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/services/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/services/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/_internals/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 21:16:41.000000 oresat_olaf-3.6.0/olaf/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.485163 oresat_olaf-3.6.0/olaf/board/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/board/adc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/board/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/board/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/board/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/board/pru.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.489163 oresat_olaf-3.6.0/olaf/canopen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/canopen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/canopen/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/canopen/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/canopen/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21489 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/canopen/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.489163 oresat_olaf-3.6.0/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-19 21:16:41.000000 oresat_olaf-3.6.0/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-19 21:16:41.000000 oresat_olaf-3.6.0/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:16:41.000000 oresat_olaf-3.6.0/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 21:16:41.000000 oresat_olaf-3.6.0/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 21:16:41.000000 oresat_olaf-3.6.0/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      398 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.489163 oresat_olaf-3.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.489163 oresat_olaf-3.6.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/common/test_oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/common/test_pru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/common/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.489163 oresat_olaf-3.6.0/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/resources/test_fwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/tests/internals/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/services/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/test_rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:16:41.493163 oresat_olaf-3.6.0/tests/internals/updater/test_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test-script.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611941111.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611947777.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611948888.tar.xz
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-19 21:16:36.000000 oresat_olaf-3.6.0/tests/internals/updater/test_updater.py
```

### Comparing `oresat_olaf-3.5.0/.github/workflows/pypi.yaml` & `oresat_olaf-3.6.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/.github/workflows/tests.yaml` & `oresat_olaf-3.6.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/.gitignore` & `oresat_olaf-3.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/LICENSE` & `oresat_olaf-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/PKG-INFO` & `oresat_olaf-3.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 3.5.0
+Version: 3.6.0
 Summary: Application framework for all OreSat Linux boards
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: canopen
 Requires-Dist: flask
 Requires-Dist: loguru
-Requires-Dist: natsort
 Requires-Dist: psutil
 Requires-Dist: python-can>=4.3.0
 Requires-Dist: oresat-configs
 
 OLAF (OreSat Linux App Framework)
 =================================
```

### Comparing `oresat_olaf-3.5.0/README.rst` & `oresat_olaf-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/Makefile` & `oresat_olaf-3.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/api/ecss.rst` & `oresat_olaf-3.6.0/docs/api/ecss.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/api/oresat_file.rst` & `oresat_olaf-3.6.0/docs/api/oresat_file.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/api/rest_api.rst` & `oresat_olaf-3.6.0/docs/api/rest_api.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/conf.py` & `oresat_olaf-3.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/glossary.rst` & `oresat_olaf-3.6.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/index.rst` & `oresat_olaf-3.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/make.bat` & `oresat_olaf-3.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/rest_api.rst` & `oresat_olaf-3.6.0/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/updater/index.rst` & `oresat_olaf-3.6.0/docs/updater/index.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/docs/updater/update_archive.rst` & `oresat_olaf-3.6.0/docs/updater/update_archive.rst`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/__init__.py` & `oresat_olaf-3.6.0/olaf/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/app.py` & `oresat_olaf-3.6.0/olaf/_internals/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,20 +134,23 @@
 
         for service in self._services:
             service.start(self._node)
 
         for resource in self._resources:
             resource.start(self._node)
 
-        if self._node:
-            try:
-                reset = self._node.run()
-            except Exception as e:  # pylint: disable=W0718
-                logger.exception(f"unexpected error was raised by app node: {e}")
-                reset = NodeStop.SOFT_RESET
+        if self.node is None:
+            logger.critical("node was not set")
+            return
+
+        try:
+            reset = self._node.run()
+        except Exception as e:  # pylint: disable=W0718
+            logger.exception(f"unexpected error was raised by app node: {e}")
+            reset = NodeStop.SOFT_RESET
 
         for service in self._services:
             service.stop()
 
         for resource in self._resources:
             resource.end()
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/resources/daemons.py` & `oresat_olaf-3.6.0/olaf/_internals/resources/daemons.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/resources/ecss.py` & `oresat_olaf-3.6.0/olaf/_internals/resources/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/resources/fread.py` & `oresat_olaf-3.6.0/olaf/_internals/resources/fread.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/resources/fwrite.py` & `oresat_olaf-3.6.0/olaf/_internals/resources/fwrite.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 f.write(data)
             logger.info(f"receive new file: {basename(self.file_path)}")
             self.node.fwrite_cache.add(self.file_path, consume=True)
         except Exception as e:  # pylint: disable=W0718
             logger.exception(e)
 
         # clear file data OD obj value to not waste memory
-        self.node.od["fwrite_cache"]["file_data"].value = b""
+        self.node.od_write("fwrite_cache", "file_data", b"")
 
     def on_write_delete(self, value: bool):
         """SDO read callback to delete the selected file."""
 
         if not value:
             return
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/resources/system.py` & `oresat_olaf-3.6.0/olaf/_internals/resources/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Resource for the system."""
 
 from time import monotonic, time
 
 import psutil
-
-from olaf import logger
+from loguru import logger
 
 from ...board.eeprom import Eeprom
 from ...canopen.node import NodeStop
 from ...common.resource import Resource
 
 
 class SystemResource(Resource):
     """Resource for the system."""
 
     def on_start(self):
-        self.node.od["system"]["reset"].value = 0
+        self.node.od_write("system", "reset", 0)
 
         self.node.add_sdo_callbacks("system", "ram_percent", self.on_read_ram, None)
         self.node.add_sdo_callbacks("system", "storage_percent", self.on_read_storage, None)
         self.node.add_sdo_callbacks("system", "uptime", self.on_read_uptime, None)
         self.node.add_sdo_callbacks("system", "unix_time", self.on_read_unix_time, None)
         self.node.add_sdo_callbacks("system", "reset", None, self.on_write_reset)
 
         try:
             eeprom = Eeprom()
-            self.node.od["versions"]["hw_version"].value = f"{eeprom.major}.{eeprom.minor}"
+            self.node.od_write("versions", "hw_version", f"{eeprom.major}.{eeprom.minor}")
         except (PermissionError, FileNotFoundError):
             logger.warning("could not read hardware info from eeprom")
 
     def on_read_ram(self):
         """SDO read callback for getting the RAM usage percent."""
 
         return int(psutil.virtual_memory().percent)
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/__init__.py` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from pathlib import Path
 from threading import Thread
 from typing import Union
 
 import canopen
 from flask import Flask, jsonify, render_template, request, send_from_directory
 from loguru import logger
-from natsort import natsorted
 from oresat_configs import OreSatId
 from werkzeug.serving import make_server
 
+from ...common import natsorted
 from ..app import app
 
 DATA_TYPE_NAMES = {
     canopen.objectdictionary.BOOLEAN: "BOOLEAN",
     canopen.objectdictionary.INTEGER8: "INTEGER8",
     canopen.objectdictionary.INTEGER16: "INTEGER16",
     canopen.objectdictionary.INTEGER32: "INTEGER32",
@@ -364,14 +364,16 @@
             data["bit_definitions"] = obj.bit_definitions
             data["value_descriptions"] = obj.value_descriptions
             data["scale_factor"] = obj.factor
             if add_values:
                 data["eng_value"] = obj.factor * value
         data["subindex"] = obj.subindex
         data["unit"] = obj.unit
+        data["low_limit"] = obj.min or ""
+        data["high_limit"] = obj.max or ""
     elif isinstance(obj, canopen.objectdictionary.Array):
         data["object_type"] = "ARRAY"
         data["subindexes"] = {sub: _object_to_dict(index, sub, add_values) for sub in obj}
     else:
         data["object_type"] = "RECORD"
         data["subindexes"] = {sub: _object_to_dict(index, sub, add_values) for sub in obj}
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/static/favicon.ico` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/_base.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/_base.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/base.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "_base.html" %}
 
 {% block baseContent %}
   <style>
     #headerGrid {
       display: grid;
-      grid-template-columns: 35% 30% 35%;
+      grid-template-columns: 40% 20% 40%;
     }
     #headerCenter {
       text-align: center;
     }
     #headerRight {
       text-align: right;
     }
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/daemons.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/daemons.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fread.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/fwrite.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/logs.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/logs.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/od.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/od.html`

 * *Files 18% similar despite different names*

```diff
@@ -48,34 +48,38 @@
         <td>Access Type *</td>
         <td><span id="varAccessType"></span></td>
       </tr>
       <tr>
         <td>Value</td>
         <td><span id="varValue"></span></td>
       </tr>
-      <tr>
+      <tr id="varLowLimitRow">
+        <td>Low Limit</td>
+        <td><span id="varLowLimit"></span></td>
+      </tr>
+      <tr id="varHighLimitRow">
+        <td>High Limit</td>
+        <td><span id="varHighLimit"></span></td>
+      </tr>
+      <tr id="varScalingRow">
         <td>Scale Factor</td>
-        <td><span id="varScaling"></span></td>
+      <td><span id="varScaling"></span></td>
       </tr>
-      <tr>
+      <tr id="varEngValueRow">
         <td>Engineering Value</td>
         <td><span id="varEngValue"></span></td>
       </tr>
-      <tr>
-        <td>Unit</td>
-        <td><span id="varUnit"></span></td>
-      </tr>
     </table>
     <br/>
     <label for="objNewValue">New Value:</label>
     <input type="text" id="objNewValue" name="objNewValue"/>
     <button id="setObjectValueButton" onclick="setObjectValue()">Change</button>
     <br/>
     <br/>
-    <small>* Access premissions are be bypassed by REST API for testing/integration purposes. They are inforce over the CAN bus.</small>
+    <small>* Access premissions are be bypassed by REST API for testing/integration purposes. They are inforced over the CAN bus.</small>
   </div>
   <div id="arrayRecordObj">
     <table>
       <tr>
         <td>Object Type</td>
         <td><span id="objType"></span></td>
       </tr>
@@ -134,26 +138,41 @@
             desc += `- ${val}: ${obj.bit_definitions[val]}\n`;
           }
         }
         document.getElementById("varDesc").textContent = desc;
         document.getElementById("varDataType").textContent = obj.data_type;
         document.getElementById("varAccessType").textContent = obj.access_type;
         document.getElementById("varValue").textContent = obj.value;
-        document.getElementById("varScaling").textContent = obj.scale_factor;
-        document.getElementById("varEngValue").textContent = obj.eng_value;
-        document.getElementById("varUnit").textContent = obj.unit;
+        document.getElementById("varEngValueRow").style.display = "none";
+        document.getElementById("varScalingRow").style.display = "none";
+        document.getElementById("varLowLimitRow").style.display = "none";
+        document.getElementById("varHighLimitRow").style.display = "none";
+        if (obj.data_type.startsWith("INTEGER") || obj.data_type.startsWith("UNSIGNED")) {
+          document.getElementById("varScaling").textContent = obj.scale_factor;
+          document.getElementById("varEngValue").textContent = `${obj.eng_value} ${obj.unit}`;
+          document.getElementById("varLowLimit").textContent = obj.low_limit;
+          document.getElementById("varHighLimit").textContent = obj.high_limit;
+          document.getElementById("varEngValueRow").style.display = "";
+          document.getElementById("varScalingRow").style.display = "";
+          document.getElementById("varLowLimitRow").style.display = "";
+          document.getElementById("varHighLimitRow").style.display = "";
+        } else if (obj.data_type.startsWith("REAL")) {
+          document.getElementById("varValue").textContent = `${obj.value} ${obj.unit}`;
+        }
         document.getElementById("objNewValue").value = obj.value;
+        localStorage.setItem("subindex", obj.name);
       } else {
         document.getElementById("variableObj").style.display = "none";
         document.getElementById("arrayRecordObj").style.display = "inline";
 
         document.getElementById("objType").textContent = obj.object_type;
         document.getElementById("objName").textContent = obj.name;
         document.getElementById("objDesc").textContent = obj.description;
         document.getElementById("objSubindexes").textContent = Object.keys(obj.subindexes).length;
+        localStorage.removeItem("subindex");
       }
     }
 
     async function setObjectValue() {
       const indexSelect = document.getElementById("indexSelect");
       const subindexSelect = document.getElementById("subindexSelect");
       const value = document.getElementById("objNewValue").value;
@@ -176,14 +195,16 @@
     function updateSubindexSelect() {
 
       const indexSelect = document.getElementById("indexSelect");
       const subindexSelect = document.getElementById("subindexSelect");
       const index = parseInt(indexSelect.value, 16);
       const obj = objects[index];
 
+      localStorage.setItem("index", obj.name);
+
       // clear select options
       subindexSelect.options.length = 0
 
       let opt = document.createElement("option");
       opt.value = "";
       opt.innerHTML = "None";
       subindexSelect.appendChild(opt);
@@ -194,14 +215,17 @@
         document.getElementById("subindexSelect").disabled = false;
         for (const subindex in objects[index].subindexes) {
           let subindexHex = "0x" + parseInt(subindex).toString(16).toUpperCase();
           let opt = document.createElement("option");
           opt.value = subindexHex;
           opt.innerHTML = `${subindexHex} - ${objects[index].subindexes[subindex].name}`;
           subindexSelect.appendChild(opt);
+          if (objects[index].subindexes[subindex].name === localStorage.getItem("subindex")) {
+            subindexSelect.value = subindexHex;
+          }
         }
       }
       updateData();
     }
 
     let objects;
 
@@ -217,25 +241,28 @@
     }
 
     async function updateIndexSelect() {
 
       await readAllObjects();
 
       const indexSelect = document.getElementById("indexSelect");
-      indexSelect.onchange = updateSubindexSelect
+      indexSelect.onchange = updateSubindexSelect;
       for (const index in objects) {
         let indexHex = "0x" + parseInt(index).toString(16).toUpperCase();
         let opt = document.createElement("option");
         opt.value = indexHex;
         opt.innerHTML = `${indexHex} - ${objects[index].name}`;
         indexSelect.appendChild(opt);
+        if (objects[index].name === localStorage.getItem("index")) {
+          indexSelect.value = indexHex;
+        }
       }
 
       const subindexSelect = document.getElementById("subindexSelect");
-      subindexSelect.onchange = updateData
+      subindexSelect.onchange = updateData;
 
       updateSubindexSelect();
     }
 
     updateIndexSelect();
   </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,20 +3,21 @@
 
 Object Type       VARIABLE
 Name
 Description
 Data Type
 Access Type *
 Value
+Low Limit
+High Limit
 Scale Factor
 Engineering Value
-Unit
 
 New Value: [objNewValue         ]Change
 
 * Access premissions are be bypassed by REST API for testing/integration
-purposes. They are inforce over the CAN bus.
+purposes. They are inforced over the CAN bus.
 Object Type
 Name
 Description
 Subindexes
 {% endblock %}
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/os_command.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/os_command.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/reset.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/reset.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/root.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/root.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% extends "_base.html" %}
 
 {% block baseContent %}
   <style>
     #headerGrid {
       display: grid;
-      grid-template-columns: 35% 30% 35%;
+      grid-template-columns: 40% 20% 40%;
     }
     #headerCenter {
       text-align: center;
     }
     #headerRight {
       text-align: right;
     }
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/rest_api/templates/updater.html` & `oresat_olaf-3.6.0/olaf/_internals/rest_api/templates/updater.html`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/_internals/services/logs.py` & `oresat_olaf-3.6.0/olaf/_internals/services/logs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,52 @@
-"""Service for getting system logs"""
+"""Service for the getting system logs over CAN."""
 
 import os
 import tarfile
 
 from loguru import logger
 
 from ...common.oresat_file import new_oresat_file
 from ...common.service import Service
 
 TMP_LOGS_FILE = "/tmp/olaf.log"
 
 
 def logger_tmp_file_setup(level: str):
-    """Congfigure logger to save to tmp file for LogsService"""
-
-    # log file for log service (overrides each time app starts)
+    """Get the boot log file handler and clean up temp log file used by LogsService."""
     if os.path.isfile(TMP_LOGS_FILE):
         os.remove(TMP_LOGS_FILE)
     logger.add(TMP_LOGS_FILE, level=level, backtrace=True)
 
 
 class LogsService(Service):
     """Service for getting system logs"""
 
     def __init__(self):
         super().__init__()
 
         self.logs_dir_path = "/var/log/journal/"
-        self.make_file_obj = None
 
     def on_start(self):
-        self.make_file_obj = self.node.od["logs"]["make_file"]
-        self.make_file_obj.value = False  # make sure this is False by default
+        self.node.od_write("logs", "make_file", False)  # make sure this is False by default
 
         self.node.add_sdo_callbacks("logs", "since_boot", self.on_read_since_boot, None)
 
     def on_loop(self):
-        if self.make_file_obj.value:
+        if self.node.od_read("logs", "make_file"):
             logger.info("Making a copy of logs")
 
             tar_file_path = "/tmp/" + new_oresat_file("logs", ext=".tar.xz")
 
             with tarfile.open(tar_file_path, "w:xz") as t:
                 for i in os.listdir(self.logs_dir_path):
                     t.add(self.logs_dir_path + "/" + i, arcname=i)
 
             self.node.fread_cache.add(tar_file_path, consume=True)
-            self.make_file_obj.value = False
+            self.node.od_write("logs", "make_file", False)
 
         self.sleep(0.1)
 
     def on_read_since_boot(self) -> str:
         """SDO callback to get a copy of logs since boot."""
 
         if not os.path.isfile(TMP_LOGS_FILE):
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/services/os_command.py` & `oresat_olaf-3.6.0/olaf/_internals/services/os_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Service for running OS (bash) commands over CAN bus."""
 
 import subprocess
-from enum import IntEnum
+from enum import Enum
 
 from loguru import logger
 
 from ...common.service import Service
 
 
-class OsCommandState(IntEnum):
+class OsCommandState(Enum):
     """Valid states for OS command as defined by CiA 301 specs."""
 
     NO_ERROR_NO_REPLY = 0x00
     NO_ERROR_REPLY = 0x01
     ERROR_NO_REPLY = 0x02
     ERROR_REPLY = 0x03
     EXECUTING = 0xFF
@@ -23,66 +23,66 @@
 
     def __init__(self):
         super().__init__()
 
         self.command = ""  # internal to prevent overwriting it when running a command
         self.reply_obj_max_len = 10000
         self.failed = False
-        self.state_obj = None
-        self.reply_obj = None
 
     def on_start(self):
-        self.state_obj = self.node.od["os_command"]["status"]
-        self.state_obj.value = OsCommandState.NO_ERROR_NO_REPLY.value
-        self.reply_obj = self.node.od["os_command"]["reply"]
-        self.reply_obj.value = b""
+        self._set_status_and_reply(OsCommandState.ERROR_NO_REPLY.value, b"")
         self.node.add_sdo_callbacks(
             "os_command", "command", self.on_command_read, self.on_command_write
         )
 
     def on_loop(self):
-        if self.state_obj.value == OsCommandState.EXECUTING:
+        if self.node.od_read("os_command", "status") == OsCommandState.EXECUTING.value:
             logger.info("running os command: " + self.command)
 
             out = subprocess.run(self.command, capture_output=True, shell=True, check=False)
             if out.returncode != 0:  # error
-                self.reply_obj.value = out.stderr[: self.reply_obj_max_len]
-                if self.reply_obj.value:
-                    self.state_obj.value = OsCommandState.ERROR_REPLY.value
+                reply = out.stderr[: self.reply_obj_max_len]
+                if reply:
+                    status = OsCommandState.ERROR_REPLY.value
                 else:
-                    self.state_obj.value = OsCommandState.ERROR_NO_REPLY.value
+                    status = OsCommandState.ERROR_NO_REPLY.value
             else:  # no error
-                self.reply_obj.value = out.stdout[: self.reply_obj_max_len]
-                if self.reply_obj.value:
-                    self.state_obj.value = OsCommandState.NO_ERROR_REPLY.value
+                reply = out.stdout[: self.reply_obj_max_len]
+                if reply:
+                    status = OsCommandState.NO_ERROR_REPLY.value
                 else:
-                    self.state_obj.value = OsCommandState.NO_ERROR_NO_REPLY.value
+                    status = OsCommandState.NO_ERROR_NO_REPLY.value
+
+            self._set_status_and_reply(status, reply)
 
             logger.info(f"os command has completed; ret code: {out.returncode}")
 
         self.sleep(0.1)
 
     def on_loop_error(self, error: Exception):
         """On loop error set obj back to default."""
 
         self.failed = True
-        self.command = b""
-        self.state_obj.value = OsCommandState.ERROR_NO_REPLY
-        self.reply_obj.value = b""
+        self.command = ""
+        self._set_status_and_reply(OsCommandState.ERROR_NO_REPLY.value, b"")
         logger.exception(error)
 
     def on_command_read(self) -> bytes:
         """SDO read callback for command read."""
         return self.command.encode()
 
     def on_command_write(self, command: bytes):
         """SDO write callback for command write."""
-        if self.state_obj.value == OsCommandState.EXECUTING:
+        logger.error("hi")
+        if self.node.od_read("os_command", "status") == OsCommandState.EXECUTING.value:
             logger.error("cannot start another os command when one is running")
             return
         if self.failed:
             logger.error("cannot run os command as service has errored")
             return
 
         self.command = command.decode()
-        self.state_obj.value = OsCommandState.EXECUTING.value
-        self.reply_obj.value = b""
+        self._set_status_and_reply(OsCommandState.EXECUTING.value, b"")
+
+    def _set_status_and_reply(self, status: int, reply: bytes):
+        self.node.od_write("os_command", "status", status)
+        self.node.od_write("os_command", "reply", reply)
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/services/updater.py` & `oresat_olaf-3.6.0/olaf/_internals/services/updater.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 """Service for interacting with the updater"""
 
-import canopen
 from loguru import logger
 
 from ...common.service import Service
 from ..updater import Updater, UpdaterError
 
 
 class UpdaterService(Service):
     """Service for interacting with the updater"""
 
     def __init__(self, updater: Updater):
         super().__init__()
-
         self._updater = updater
-        self.update_obj: canopen.objectdictionary.Variable = None
-        self.make_status_obj: canopen.objectdictionary.Variable = None
 
     def on_start(self):
-        record = self.node.od["updater"]
-        self.update_obj = record["update"]
-        self.make_status_obj = record["make_status_file"]
 
         # make sure defaults are set correctly
-        self.update_obj.value = False
-        self.make_status_obj.value = False
+        self.node.od_write("updater", "update", False)
+        self.node.od_write("updater", "make_status_file", False)
 
         self.node.add_sdo_callbacks("updater", "status", self.on_read_status, None)
         self.node.add_sdo_callbacks("updater", "cache_files_json", self.on_read_cache_json, None)
         self.node.add_sdo_callbacks("updater", "cache_length", self.on_read_cache_len, None)
 
     def on_loop(self):
         # check for update files in fwrite cache
         for i in self.node.fwrite_cache.files("update"):
             self._updater.add_update_archive(self.node.fwrite_cache.dir + "/" + i.name)
             self.node.fwrite_cache.remove(i.name)
             logger.info(f"updater moved {i.name} into update cache")
 
         # check for flag to start a update
-        if self.update_obj.value:
+        if self.node.od_read("updater", "update"):
             try:
                 self._updater.update()
             except UpdaterError as e:
                 logger.exception(e)
-            self.update_obj.value = False
+            self.node.od_write("updater", "update", False)
 
         # check for flag to make a status archive
-        if self.make_status_obj.value:
+        if self.node.od_read("updater", "make_status_file"):
             status_archive_file_path = self._updater.make_status_archive()
             self.node.fread_cache.add(status_archive_file_path, consume=True)
-            self.make_status_obj.value = False
+            self.node.od_write("updater", "make_status_file", False)
 
         self.sleep(0.1)
 
     def on_read_status(self) -> int:
         """SDO read callback to get the status of update"""
         return self._updater.status.value
```

### Comparing `oresat_olaf-3.5.0/olaf/_internals/updater.py` & `oresat_olaf-3.6.0/olaf/_internals/updater.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/board/adc.py` & `oresat_olaf-3.6.0/olaf/board/adc.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/board/cpufreq.py` & `oresat_olaf-3.6.0/olaf/board/cpufreq.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/board/eeprom.py` & `oresat_olaf-3.6.0/olaf/board/eeprom.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/board/gpio.py` & `oresat_olaf-3.6.0/olaf/board/gpio.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/board/pru.py` & `oresat_olaf-3.6.0/olaf/board/pru.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/canopen/ecss.py` & `oresat_olaf-3.6.0/olaf/canopen/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/canopen/network.py` & `oresat_olaf-3.6.0/olaf/canopen/network.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/canopen/node.py` & `oresat_olaf-3.6.0/olaf/canopen/node.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,25 +4,38 @@
 import struct
 from enum import IntEnum
 from pathlib import Path
 from threading import Event
 from time import monotonic
 from typing import Any, Callable, Dict, Union
 
-import canopen
+from canopen import LocalNode, ObjectDictionary
+from canopen.objectdictionary import (
+    DOMAIN,
+    FLOAT_TYPES,
+    INTEGER_TYPES,
+    OCTET_STRING,
+    VISIBLE_STRING,
+    ODArray,
+    ODRecord,
+    ODVariable,
+)
 from loguru import logger
 
 from ..canopen.network import CanNetwork, CanNetworkState
 from ..common.daemon import Daemon
 from ..common.oresat_file_cache import OreSatFileCache
+from . import EmcyCode
 
 
 class NodeStop(IntEnum):
     """Node stop commands."""
 
+    NO_STOP = 0
+    """Default value for no stop."""
     SOFT_RESET = 1
     """Just stop the app and exit. Systemd will restart the app."""
     HARD_RESET = 2
     """Reboot system after app has stopped"""
     FACTORY_RESET = 3
     """Clear all file cachces and reboot system after app has stopped"""
     POWER_OFF = 4
@@ -30,40 +43,41 @@
 
 
 class Node:
     """
     OreSat CANopen Node class
 
     Jobs:
+
     - It abstracts away the canopen.LocalNode and canopen.Network from Resources and Services.
     - Provides access to the OD for Resources and Services.
     - Lets Resources and Services send TPDOs.
     - Lets Resources and Services send EMCY messages.
     - Set up the file transfer caches.
     - Starts/stops all Resources and Services.
     - Sets up all timer-base TPDOs.
     - Sets up all RPDO callbacks.
 
     Basically it tries to abstract all the CANopen things as much a possible, while providing a
     basic API for CANopen things.
     """
 
-    def __init__(self, network: CanNetwork, od: canopen.ObjectDictionary):
+    def __init__(self, network: CanNetwork, od: ObjectDictionary):
         """
         Parameters
         ----------
         network: CanNetwork
             The CAN network
         od: canopen.ObjectDictionary
             The CANopen ObjectDictionary
         """
 
         self._event = Event()
         self._od = od
-        self._node: canopen.LocalNode = None
+        self._node: LocalNode = None
         self._network: CanNetwork = network
         self._read_cbs = {}  # type: ignore
         self._write_cbs = {}  # type: ignore
         self._syncs = 0
         self._reset = NodeStop.SOFT_RESET
         self._daemons = {}  # type: ignore
 
@@ -124,94 +138,28 @@
                 break  # nothing todo
 
             pdo_map_bytes = pdo_map.to_bytes(4, "big")
             index, subindex, size = struct.unpack(">HBB", pdo_map_bytes)
             size //= 8
 
             # call sdo callback(s) and convert data to bytes
-            if isinstance(self.od[index], canopen.objectdictionary.Variable):
+            if isinstance(self.od[index], ODVariable):
                 self._node.sdo[index].raw = data[offset : offset + size]
             else:  # record or array
                 self._node.sdo[index][subindex].raw = data[offset : offset + size]
 
             offset += size
 
-    def send_tpdo(self, tpdo: int):
-        """
-        Send a TPDO. Will not be sent if not node is not in operational state.
-
-        Parameters
-        ----------
-        tpdo: int
-            TPDO number to send, should be between 1 and 16.
-        """
-
-        if tpdo < 1:
-            raise ValueError("TPDO number must be greather than 1")
-
-        if self._network.status != CanNetworkState.NETWORK_UP:
-            logger.debug("network is down cannot send an TPDO message")
-            return
-
-        tpdo -= 1  # number to offset
-
-        # PDOs should not be sent if CAN bus not in 'OPERATIONAL' state as defined by spec
-        if self._node is None or self._node.nmt.state != "OPERATIONAL":
-            return
-
-        cob_id = self.od[0x1800 + tpdo][1].value & 0x3F_FF_FF_FF
-        maps = self.od[0x1A00 + tpdo][0].value
-
-        data = b""
-        for i in range(maps):
-            pdo_map = self.od[0x1A00 + tpdo][i + 1].value
-
-            if pdo_map == 0:
-                break  # nothing todo
-
-            pdo_map_bytes = pdo_map.to_bytes(4, "big")
-            index, subindex, _ = struct.unpack(">HBB", pdo_map_bytes)
-
-            # call sdo callback(s) and convert data to bytes
-            if isinstance(self.od[index], canopen.objectdictionary.Variable):
-                value = self._node.sdo[index].phys
-                value_bytes = self.od[index].encode_raw(value)
-            else:  # record or array
-                value = self._node.sdo[index][subindex].phys
-                value_bytes = self.od[index][subindex].encode_raw(value)
-
-            # pack pdo with bytes
-            data += value_bytes
-
-        self._network.send_message(cob_id, data, False)
-
-    def _on_rpdo_update_od(self, mapping: canopen.pdo.base.Map):
-        """Handle parsering an RPDO"""
-
-        for i in mapping.map_array:
-            if i == 0:
-                continue
-
-            value = mapping.map_array[i].raw
-            if value == 0:
-                break  # no more mapping
-
-            index, subindex, _ = struct.unpack(">HBB", value.to_bytes(4, "big"))
-            if isinstance(self.od[index], canopen.objectdictionary.Variable):
-                self._node.sdo[index].raw = mapping.map[i - 1].get_data()
-            else:
-                self._node.sdo[index][subindex].raw = mapping.map[i - 1].get_data()
-
     def _setup_node(self):
         """Create the CANopen node."""
 
         if self._od.node_id is None:
             self._od.node_id = 0x7C
 
-        self._node = canopen.LocalNode(self._od.node_id, self._od)
+        self._node = LocalNode(self._od.node_id, self._od)
         self._network.add_node(self._node)
         self._node.nmt.state = "OPERATIONAL"
 
         self._node.add_read_callback(self._on_sdo_read)
         self._node.add_write_callback(self._on_sdo_write)
 
         if not self._first_network_reset or monotonic() - self._start_time > 5:
@@ -327,59 +275,130 @@
                 return
 
         if read_cb is not None:
             self._read_cbs[index, subindex] = read_cb
         if write_cb is not None:
             self._write_cbs[index, subindex] = write_cb
 
-    def send_emcy(self, code: int, data: bytes = b""):
+    def _send_pdo(self, comm_index: int, map_index: int, raise_error: bool = True):
+        """Send a PDO. Will not be sent if not node is not in operational state."""
+
+        # PDOs should not be sent if CANopen node not in 'OPERATIONAL' state
+        if self._node.nmt.state != "OPERATIONAL":
+            return
+
+        cob_id = self.od[comm_index][1].value & 0x3F_FF_FF_FF
+        maps = self.od[map_index][0].value
+
+        data = b""
+        for i in range(maps):
+            pdo_map = self.od[map_index][i + 1].value
+
+            if pdo_map == 0:
+                break  # nothing todo
+
+            pdo_map_bytes = pdo_map.to_bytes(4, "big")
+            index, subindex, _ = struct.unpack(">HBB", pdo_map_bytes)
+
+            # call sdo callback(s) and convert data to bytes
+            if isinstance(self.od[index], ODVariable):
+                value = self._node.sdo[index].phys
+                value_bytes = self.od[index].encode_raw(value)
+            else:  # record or array
+                value = self._node.sdo[index][subindex].phys
+                value_bytes = self.od[index][subindex].encode_raw(value)
+
+            # pack pdo with bytes
+            data += value_bytes
+
+        if len(data) > 8:
+            self.send_emcy(EmcyCode.PROTOCOL_PDO_LEN_EXCEEDED, b"", False)
+            return
+
+        self._network.send_message(cob_id, data, raise_error)
+
+    def send_tpdo(self, tpdo: int, raise_error: bool = True):
+        """
+        Send a TPDO. Will not be sent if not node is not in operational state.
+
+        Parameters
+        ----------
+        tpdo: int
+            TPDO number to send, should be between 1 and 16.
+        raise_error: bool
+            Set to False to not raise NetworkError.
+
+        Raises
+        ------
+        NetworkError
+            Cannot send a TPDO message when the network is down.
+        """
+        if tpdo < 1:
+            raise ValueError("TPDO number must be greater than 1")
+
+        tpdo -= 1  # number to offset
+        comm_index = 0x1800 + tpdo
+        map_index = 0x1A00 + tpdo
+        self._send_pdo(comm_index, map_index, raise_error)
+
+    def send_emcy(self, code: Union[EmcyCode, int], data: bytes = b"", raise_error: bool = True):
         """
         Send a EMCY message.
 
         Parameters
         ----------
-        code: int
+        code: Emcy, int
             The EMCY code.
         data: bytes
-            Optional manufacturer error code/data (up to 5 bytes).
+            Optional data to add to the message (up to 5 bytes).
+        raise_error: bool
+            Set to False to not raise NetworkError.
+
+        Raises
+        ------
+        NetworkError
+            Cannot send a EMCY message when the network is down.
         """
 
+        if isinstance(code, EmcyCode):
+            code = code.value
+
         if len(data) > 5:
             raise ValueError("data must be 5 or less bytes")
 
         frame = code.to_bytes(2, "little") + self.od[0x1001].value.to_bytes(1, "little") + data
         frame += b"\x00" * (5 - len(data))
-        self._network.send_message(self.od.node_id + 0x80, frame)
+        self._network.send_message(self.od.node_id + 0x80, frame, raise_error)
         logger.error(f"sent emcy 0x{code:04X} {data.hex()}")
 
-    def _on_sdo_read(self, index: int, subindex: int, od: canopen.objectdictionary.Variable):
+    def _on_sdo_read(self, index: int, subindex: int, od: ODVariable):
         """
         SDO read callback function. Allows overriding the data being sent on a SDO read. Return
         valid datatype for object, if overriding read data, or :py:data:`None` to use the the value
         on object dictionary.
 
         Parameters
         ----------
         index: int
             The index the SDO is reading to.
         subindex: int
             The subindex the SDO is reading to.
-        od: canopen.objectdictionary.Variable
+        od: canopen.objectdictionary.ODVariable
             The variable object being read to. Badly named. And not appart of the actual OD.
 
         Returns
         -------
         Any
             The value to return for that index / subindex.
         """
 
         ret = None
 
         # convert any ints to strs
-        if isinstance(self.od[index], canopen.objectdictionary.Variable) and od == self.od[index]:
+        if isinstance(self.od[index], ODVariable) and od == self.od[index]:
             index = od.name
             subindex = None  # type: ignore
         else:
             index = self.od[index].name
             subindex = od.name
 
         if (index, subindex) in self._read_cbs:
@@ -387,44 +406,42 @@
 
         # get value from OD
         if ret is None:
             ret = od.value
 
         return ret
 
-    def _on_sdo_write(
-        self, index: int, subindex: int, od: canopen.objectdictionary.Variable, data: bytes
-    ):
+    def _on_sdo_write(self, index: int, subindex: int, od: ODVariable, data: bytes):
         """
         SDO write callback function. Gives access to the data being received on a SDO write.
 
         *Note:* data is still written to object dictionary before call.
 
         Parameters
         ----------
         index: int
             The index the SDO being written to.
         subindex: int
             The subindex the SDO being written to.
-        od: canopen.objectdictionary.Variable
+        od: canopen.objectdictionary.ODVariable
             The variable object being written to. Badly named.
         data: bytes
             The raw data being written.
         """
 
-        binary_types = [canopen.objectdictionary.DOMAIN, canopen.objectdictionary.OCTET_STRING]
+        binary_types = [DOMAIN, OCTET_STRING]
 
         # set value in OD before callback
         if od.data_type in binary_types:
             od.value = data
         else:
             od.value = od.decode_raw(data)
 
         # convert any ints to strs
-        if isinstance(self.od[index], canopen.objectdictionary.Variable) and od == self.od[index]:
+        if isinstance(self.od[index], ODVariable) and od == self.od[index]:
             index = od.name
             subindex = None  # type: ignore
         else:
             index = self.od[index].name
             subindex = od.name
 
         if (index, subindex) in self._write_cbs:
@@ -445,15 +462,15 @@
     @property
     def name(self) -> str:
         """str: The nodes name."""
 
         return self._od.device_information.product_name
 
     @property
-    def od(self) -> canopen.ObjectDictionary:
+    def od(self) -> ObjectDictionary:
         """canopen.ObjectDictionary: Access to the object dictionary."""
 
         return self._od
 
     @property
     def fread_cache(self) -> OreSatFileCache:
         """OreSatFile: Cache the CANopen master node can read to."""
@@ -473,7 +490,202 @@
         return not self._event.is_set()
 
     @property
     def daemons(self) -> Dict[str, Daemon]:
         """dict: The dictionary of external daemons that are monitored and/or controllable"""
 
         return self._daemons
+
+    def od_get_obj(
+        self, index: Union[int, str], subindex: Union[int, str, None] = None
+    ) -> Union[ODVariable, ODArray, ODRecord]:
+        """
+        Quick helper function to get an object from the od.
+
+        Returns
+        -------
+        ODVariable | ODArray | ODRecord
+            The object from the OD.
+        """
+
+        if subindex is None:
+            return self._od[index]
+        return self._od[index][subindex]
+
+    def od_read(
+        self, index: Union[int, str], subindex: Union[int, str, None]
+    ) -> Union[int, str, float, bytes, bool]:
+        """
+        Read a value from the OD.
+
+        Parameters
+        ----------
+        index: int or str
+            The index to read from.
+        subindex: int, str, or None
+            The subindex to read from or None.
+
+        Returns
+        -------
+        int | str | float | bytes | bool
+            The value read.
+        """
+
+        obj = self.od_get_obj(index, subindex)
+        return obj.value
+
+    def od_read_bitfield(
+        self, index: Union[int, str], subindex: Union[int, str, None], field: str
+    ) -> int:
+        """
+        Read a field from a object from the OD.
+
+        Parameters
+        ----------
+        index: int or str
+            The index to read from.
+        subindex: int, str, or None
+            The subindex to read from or None.
+
+        Returns
+        -------
+        int:
+            The field value.
+        """
+
+        obj = self.od_get_obj(index, subindex)
+        bits = obj.bit_definitions[field]
+
+        value = 0
+        for i in bits:
+            tmp = obj.value & (1 << bits[i])
+            value |= tmp >> bits[i]
+        return value
+
+    def od_read_enum(self, index: Union[int, str], subindex: Union[int, str, None]) -> str:
+        """
+        Read a enum str from the OD.
+
+        Parameters
+        ----------
+        index: int or str
+            The index to read from.
+        subindex: int, str, or None
+            The subindex to read from or None.
+
+        Returns
+        -------
+        str
+            The enum str value.
+        """
+
+        obj = self.od_get_obj(index, subindex)
+        return obj.value_descriptions[obj.value]
+
+    def _var_write(self, obj: ODVariable, value: Union[int, str, float, bytes, bool]):
+
+        value_type = type(value)
+
+        def make_error_value(data_type) -> str:
+            return f"cannot write {value!r} ({data_type}) to object {obj.name} ({obj.data_type})"
+
+        if obj.data_type in INTEGER_TYPES:
+            if value_type != int:
+                raise TypeError(make_error_value("int"))
+            if obj.max is not None and value > obj.max:
+                raise ValueError(f"value {value!r} too high (high limit {obj.max})")
+            if obj.min is not None and value < obj.min:
+                raise ValueError(f"value {value!r} too low (low limit {obj.min})")
+        elif obj.data_type in FLOAT_TYPES:
+            if not isinstance(value, int):
+                raise TypeError(make_error_value("float"))
+            if obj.max is not None and value > obj.max:
+                raise ValueError(f"value {value!r} too high (high limit {obj.max})")
+            if obj.min is not None and value < obj.min:
+                raise ValueError(f"value {value!r} too low (low limit {obj.min})")
+        elif obj.data_type == VISIBLE_STRING and not isinstance(value, str):
+            raise TypeError(make_error_value("str"))
+        elif obj.data_type == OCTET_STRING and not isinstance(value, bytes):
+            raise TypeError(make_error_value("bytes"))
+
+        obj.value = value
+
+    def od_write(
+        self,
+        index: Union[int, str],
+        subindex: Union[int, str, None],
+        value: Union[int, str, float, bytes, bool],
+    ):
+        """
+        Write an value to the OD.
+
+        Parameters
+        ----------
+        index: int | str
+            The index to read from.
+        subindex: int | str | None
+            The subindex to read from or None.
+        value: int | str | float | bytes | bool
+            The value to write.
+
+        Raises
+        ------
+        ValueError
+            An invalid value.
+        """
+
+        obj = self.od_get_obj(index, subindex)
+        self._var_write(obj, value)
+
+    def od_write_bitfield(
+        self, index: Union[int, str], subindex: Union[int, str, None], field: str, value: int
+    ):
+        """
+        Write a bit field value to a object to the OD.
+
+        Parameters
+        ----------
+        index: int | str
+            The index to read from.
+        subindex: int | str | None
+            The subindex to read from or None.
+        field: str
+            Name of field to write to.
+        value: int
+            The value to write.
+
+        Raises
+        ------
+        ValueError
+            An invalid value.
+        """
+
+        obj = self.od_get_obj(index, subindex)
+        bits = obj.bit_definitions[field]
+        offset = min(bits)
+
+        mask = 0
+        for i in bits:
+            mask |= 1 << bits[i]
+
+        new_value = obj.value
+        new_value ^= mask
+        new_value |= value << offset
+        obj.value = new_value
+
+    def od_write_enum(self, index: Union[int, str], subindex: Union[int, str, None], value: str):
+        """
+        Write a enum str to the OD.
+
+        Parameters
+        ----------
+        index: int | str
+            The index to read from.
+        subindex: int | str | None
+            The subindex to read from or None.
+        value: str
+            The enum string to write.
+        """
+
+        obj = self.od_get_obj(index, subindex)
+        tmp = {d: v for v, d in obj.value_descriptions}
+        obj.value = tmp[value.lower()]
```

### Comparing `oresat_olaf-3.5.0/olaf/common/daemon.py` & `oresat_olaf-3.6.0/olaf/common/daemon.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/common/oresat_file.py` & `oresat_olaf-3.6.0/olaf/common/oresat_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import uname
 from os.path import basename
 from time import time
 
 
 def new_oresat_file(keyword: str, card: str = "", date: float = -1.0, ext: str = "") -> str:
     """
-    Convience function for making valid oresat file_names
+    Convenience function for making valid oresat file_names
 
     Parameters
     ----------
     keyword: str
         The keyword for the new file_name
     card: str
         The card name for the file_name. If not set, the hostname will be
```

### Comparing `oresat_olaf-3.5.0/olaf/common/oresat_file_cache.py` & `oresat_olaf-3.6.0/olaf/common/oresat_file_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import shutil
 from copy import deepcopy
 from os import listdir, remove
 from os.path import abspath, basename, isfile
 from pathlib import Path
 from threading import Lock
 
-from natsort import natsorted
-
 from .oresat_file import OreSatFile
 
 
 class OreSatFileCache:
     """File cache for OreSat files (by use of :py:class:`OresatFile`). Thread safe."""
 
     def __init__(self, dir_path: str):
@@ -34,15 +32,15 @@
 
         for f in listdir(self._dir):
             try:
                 oresat_file = OreSatFile(self._dir + f)
                 self._data.append(oresat_file)
             except Exception:  # pylint: disable=W0718
                 remove(self._dir + f)  # invalid file name
-        self._data = natsorted(self._data)
+        self._data = sorted(self._data)
 
     def __len__(self) -> int:
         with self._lock:
             length = len(self._data)
 
         return length
 
@@ -75,15 +73,15 @@
             overwrite = False
             for i in self._data:
                 if i.name == oresat_file.name:
                     overwrite = True
 
             if not overwrite:
                 self._data.append(oresat_file)
-                self._data = natsorted(self._data)
+                self._data = sorted(self._data)
 
     def remove(self, file_name: str):
         """Remove a file from cache
 
         Parameters
         ----------
         file_name: str
```

### Comparing `oresat_olaf-3.5.0/olaf/common/resource.py` & `oresat_olaf-3.6.0/olaf/common/resource.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/common/service.py` & `oresat_olaf-3.6.0/olaf/common/service.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/olaf/common/timer_loop.py` & `oresat_olaf-3.6.0/olaf/common/timer_loop.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/oresat_olaf.egg-info/PKG-INFO` & `oresat_olaf-3.6.0/oresat_olaf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 3.5.0
+Version: 3.6.0
 Summary: Application framework for all OreSat Linux boards
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: canopen
 Requires-Dist: flask
 Requires-Dist: loguru
-Requires-Dist: natsort
 Requires-Dist: psutil
 Requires-Dist: python-can>=4.3.0
 Requires-Dist: oresat-configs
 
 OLAF (OreSat Linux App Framework)
 =================================
```

### Comparing `oresat_olaf-3.5.0/oresat_olaf.egg-info/SOURCES.txt` & `oresat_olaf-3.6.0/oresat_olaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/pyproject.toml` & `oresat_olaf-3.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 dependencies = [
     "canopen",
     "flask",
     "loguru",
-    "natsort",
     "psutil",
     "python-can>=4.3.0",
     "oresat-configs",
 ]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
@@ -60,15 +59,16 @@
 # W1514:    Using open without explicitly specifying an encoding
 # R0902:    Too many instance attributes
 # R0913:    Too many arguments
 # W0707:    Consider explicitly re-raising
 # W0102:    Dangerous default value as argument
 # W0107:    Unnecessary pass statement
 # R0903:    Too few public methods
-ignore = "E402,C901,C0103,E203,R0912,R0915,R901,R901,R0914,C0413,C0206,R1716,W1514,R0902,R0913,W0707,W0102,W0107,R0903"
+# R0904:    Too many public methods
+ignore = "E402,C901,C0103,E203,R0912,R0915,R901,R901,R0914,C0413,C0206,R1716,W1514,R0902,R0913,W0707,W0102,W0107,R0903,R0904"
 max_line_length = 100
 
 [[tool.pylama.files]]
 path = "*/__init__.py"
 # W0611:    Imported but unused
 ignore = "W0611"
 
@@ -79,13 +79,13 @@
 
 [[tool.pylama.files]]
 path = "*/_version.py"
 # C0114:    Missing module docstring
 ignore = "C0114"
 
 [[tool.mypy.overrides]]
-module = "canopen,oresat_configs,psutil"
+module = "canopen,oresat_configs,psutil,canopen.sdo,canopen.sdo.exceptions,canopen.objectdictionary"
 ignore_missing_imports = true
 
 [tool.isort]
 profile = "black"
 line_length = 100
```

### Comparing `oresat_olaf-3.5.0/tests/common/test_ecss.py` & `oresat_olaf-3.6.0/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/common/test_oresat_file.py` & `oresat_olaf-3.6.0/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/common/test_oresat_file_cache.py` & `oresat_olaf-3.6.0/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/common/test_pru.py` & `oresat_olaf-3.6.0/tests/common/test_pru.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/common/test_resources.py` & `oresat_olaf-3.6.0/tests/common/test_resources.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/resources/__init__.py` & `oresat_olaf-3.6.0/tests/internals/resources/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._fread_cache = OreSatFileCache("/tmp/fread")
         self._fread_cache.clear()
         self._fwrite_cache = OreSatFileCache("/tmp/fwrite")
         self._fwrite_cache.clear()
 
         self._setup_node()
 
-    def send_tpdo(self, tpdo: int):
+    def send_tpdo(self, tpdo: int, raise_error: bool = True):
         pass  # override to do nothing
 
 
 class MockApp:
     """Mock app for testing Resources."""
 
     def __init__(self):
```

### Comparing `oresat_olaf-3.5.0/tests/internals/resources/test_ecss.py` & `oresat_olaf-3.6.0/tests/internals/resources/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/resources/test_fread.py` & `oresat_olaf-3.6.0/tests/internals/resources/test_fread.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/resources/test_fwrite.py` & `oresat_olaf-3.6.0/tests/internals/resources/test_fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/services/__init__.py` & `oresat_olaf-3.6.0/tests/internals/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._fread_cache = OreSatFileCache("/tmp/fread")
         self._fread_cache.clear()
         self._fwrite_cache = OreSatFileCache("/tmp/fwrite")
         self._fwrite_cache.clear()
 
         self._setup_node()
 
-    def send_tpdo(self, tpdo: int):
+    def send_tpdo(self, tpdo: int, raise_error: bool = True):
         pass  # override to do nothing
 
 
 class MockApp:
     """Mock app for testing services."""
 
     def __init__(self):
```

### Comparing `oresat_olaf-3.5.0/tests/internals/services/test_os_command.py` & `oresat_olaf-3.6.0/tests/internals/services/test_os_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 
         self.assertIsNotNone(self.app.sdo_read(self.index, self.subindex_command))
         self.assertIn(
             self.app.sdo_read(self.index, self.subindex_status), [e.value for e in OsCommandState]
         )
         self.assertIsNotNone(self.app.sdo_read(self.index, self.subindex_reply))
 
-        self.run_os_command("ls".encode())
-        self.assertEqual(
-            self.app.sdo_read(self.index, self.subindex_status), OsCommandState.NO_ERROR_REPLY
-        )
-        self.assertIsNotNone(self.app.sdo_read(self.index, self.subindex_reply))
+        self.run_os_command(b"ls")
+        status = self.app.sdo_read(self.index, self.subindex_status)
+        self.assertEqual(OsCommandState(status), OsCommandState.NO_ERROR_REPLY)
+        reply = self.app.sdo_read(self.index, self.subindex_reply)
+        self.assertIsNotNone(reply)
 
-        self.run_os_command("invalid-bash-command".encode())
-        self.assertEqual(
-            self.app.sdo_read(self.index, self.subindex_status), OsCommandState.ERROR_REPLY
-        )
-        self.assertIsNotNone(self.app.sdo_read(self.index, self.subindex_reply))
+        self.run_os_command(b"invalid-bash-command")
+        status = self.app.sdo_read(self.index, self.subindex_status)
+        self.assertEqual(OsCommandState(status), OsCommandState.ERROR_REPLY)
+        reply = self.app.sdo_read(self.index, self.subindex_reply)
+        self.assertIsNotNone(reply)
```

### Comparing `oresat_olaf-3.5.0/tests/internals/test_rest_api.py` & `oresat_olaf-3.6.0/tests/internals/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/README.md` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/README.md`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test-package1_0.1.0-0_all.deb`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test-package2_0.1.0-0_all.deb`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611940000.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611942222.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611943333.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611944444.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611945555.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz` & `oresat_olaf-3.6.0/tests/internals/updater/test_files/test_update_1611946666.tar.xz`

 * *Files identical despite different names*

### Comparing `oresat_olaf-3.5.0/tests/internals/updater/test_updater.py` & `oresat_olaf-3.6.0/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

