# Comparing `tmp/ha_mqtt_discoverable_cli-0.4.1.tar.gz` & `tmp/ha_mqtt_discoverable_cli-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha_mqtt_discoverable_cli-0.4.1.tar", max compression
+gzip compressed data, was "ha_mqtt_discoverable_cli-0.5.0.tar", max compression
```

## Comparing `ha_mqtt_discoverable_cli-0.4.1.tar` & `ha_mqtt_discoverable_cli-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-01-01 20:21:45.749179 ha_mqtt_discoverable_cli-0.4.1/LICENSE
--rw-r--r--   0        0        0     3849 2024-01-01 20:21:45.749179 ha_mqtt_discoverable_cli-0.4.1/README.md
--rw-r--r--   0        0        0     1150 2024-01-01 20:21:45.749179 ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/__init__.py
--rw-r--r--   0        0        0     2948 2024-01-01 20:21:45.749179 ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/device_driver.py
--rw-r--r--   0        0        0     1516 2024-01-01 20:21:45.749179 ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/hmd.py
--rw-r--r--   0        0        0     1739 2024-01-01 20:21:45.749179 ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/sensor_driver.py
--rw-r--r--   0        0        0      948 2024-01-01 20:21:55.589100 ha_mqtt_discoverable_cli-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4410 1970-01-01 00:00:00.000000 ha_mqtt_discoverable_cli-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-13 02:51:17.000000 ha_mqtt_discoverable_cli-0.5.0/LICENSE
+-rwxr-xr-x   0        0        0     3849 2023-03-13 02:51:32.861066 ha_mqtt_discoverable_cli-0.5.0/README.md
+-rw-r--r--   0        0        0     1150 2023-03-27 13:54:42.000000 ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/__init__.py
+-rw-r--r--   0        0        0     2948 2023-03-10 02:58:45.000000 ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/device_driver.py
+-rw-r--r--   0        0        0     1516 2023-03-10 02:58:45.000000 ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/hmd.py
+-rw-r--r--   0        0        0     1739 2023-03-10 02:58:45.000000 ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/sensor_driver.py
+-rw-r--r--   0        0        0      955 2024-05-19 05:29:04.774066 ha_mqtt_discoverable_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 ha_mqtt_discoverable_cli-0.5.0/PKG-INFO
```

### Comparing `ha_mqtt_discoverable_cli-0.4.1/LICENSE` & `ha_mqtt_discoverable_cli-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable_cli-0.4.1/README.md` & `ha_mqtt_discoverable_cli-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/__init__.py` & `ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/device_driver.py` & `ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/device_driver.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/hmd.py` & `ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/hmd.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable_cli-0.4.1/ha_mqtt_discoverable_cli/sensor_driver.py` & `ha_mqtt_discoverable_cli-0.5.0/ha_mqtt_discoverable_cli/sensor_driver.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable_cli-0.4.1/pyproject.toml` & `ha_mqtt_discoverable_cli-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ha-mqtt-discoverable-cli"
-version = "0.4.1"
+version = "0.5.0"
 description = "CLI tools for the ha-mqtt-discoverable module"
 authors = ["Joe Block <jpb@unixorn.net>"]
 readme = "README.md"
 packages = [{include = "ha_mqtt_discoverable_cli"}]
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0.0"
-ha-mqtt-discoverable = "0.13.0"
+ha-mqtt-discoverable = "^0.14.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.1.0"
-flake8 = "^6.0.0"
+flake8 = ">=6,<8"
 pre-commit = "^3.1.1"
-pytest = "^7.2.2"
+pytest = ">=7.2.2,<9.0.0"
+ruff = "^0.4.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 hmd = 'ha_mqtt_discoverable_cli.hmd:hmd_driver'
```

### Comparing `ha_mqtt_discoverable_cli-0.4.1/PKG-INFO` & `ha_mqtt_discoverable_cli-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ha-mqtt-discoverable-cli
-Version: 0.4.1
+Version: 0.5.0
 Summary: CLI tools for the ha-mqtt-discoverable module
 License: Apache 2.0
 Author: Joe Block
 Author-email: jpb@unixorn.net
 Requires-Python: >=3.10,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ha-mqtt-discoverable (==0.13.0)
+Requires-Dist: ha-mqtt-discoverable (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # ha-mqtt-discoverable-cli
 
 [![License](https://img.shields.io/github/license/unixorn/ha-mqtt-discoverable-cli.svg)](https://opensource.org/license/apache-2-0/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub last commit (branch)](https://img.shields.io/github/last-commit/unixorn/ha-mqtt-discoverable-cli/main.svg)](https://github.com/unixorn/ha-mqtt-discoverable-cli)
```

