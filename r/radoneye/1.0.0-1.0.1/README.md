# Comparing `tmp/radoneye-1.0.0.tar.gz` & `tmp/radoneye-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radoneye-1.0.0.tar", last modified: Mon Dec 25 02:57:02 2023, max compression
+gzip compressed data, was "radoneye-1.0.1.tar", last modified: Sun May 19 03:57:00 2024, max compression
```

## Comparing `radoneye-1.0.0.tar` & `radoneye-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-12-25 02:57:02.330357 radoneye-1.0.0/
--rw-r--r--   0 artem      (501) staff       (20)     1070 2023-12-25 01:06:24.000000 radoneye-1.0.0/LICENSE
--rw-r--r--   0 artem      (501) staff       (20)     4619 2023-12-25 02:57:02.330157 radoneye-1.0.0/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)     2732 2023-12-25 02:56:44.000000 radoneye-1.0.0/README.md
--rw-r--r--   0 artem      (501) staff       (20)      838 2023-12-25 02:56:11.000000 radoneye-1.0.0/pyproject.toml
--rw-r--r--   0 artem      (501) staff       (20)       46 2023-12-25 01:46:37.000000 radoneye-1.0.0/requirements.txt
--rw-r--r--   0 artem      (501) staff       (20)       38 2023-12-25 02:57:02.330391 radoneye-1.0.0/setup.cfg
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-12-25 02:57:02.327657 radoneye-1.0.0/src/
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-12-25 02:57:02.329142 radoneye-1.0.0/src/radoneye/
--rw-r--r--   0 artem      (501) staff       (20)      173 2023-12-25 01:16:49.000000 radoneye-1.0.0/src/radoneye/__init__.py
--rw-r--r--   0 artem      (501) staff       (20)      140 2023-12-25 01:29:51.000000 radoneye-1.0.0/src/radoneye/__main__.py
--rw-r--r--   0 artem      (501) staff       (20)     4925 2023-12-25 02:18:45.000000 radoneye-1.0.0/src/radoneye/cli.py
--rw-r--r--   0 artem      (501) staff       (20)     2051 2023-12-25 02:42:16.000000 radoneye-1.0.0/src/radoneye/client.py
--rw-r--r--   0 artem      (501) staff       (20)     1235 2023-12-25 01:02:27.000000 radoneye-1.0.0/src/radoneye/interface.py
--rw-r--r--   0 artem      (501) staff       (20)      830 2023-12-25 01:22:51.000000 radoneye-1.0.0/src/radoneye/interface_factory.py
--rw-r--r--   0 artem      (501) staff       (20)     4009 2023-12-25 01:01:07.000000 radoneye-1.0.0/src/radoneye/interface_v1.py
--rw-r--r--   0 artem      (501) staff       (20)     6538 2023-12-25 01:19:24.000000 radoneye-1.0.0/src/radoneye/interface_v2.py
--rw-r--r--   0 artem      (501) staff       (20)        0 2023-12-25 01:01:15.000000 radoneye-1.0.0/src/radoneye/py.typed
--rw-r--r--   0 artem      (501) staff       (20)      468 2023-12-25 01:01:23.000000 radoneye-1.0.0/src/radoneye/scanner.py
-drwxr-xr-x   0 artem      (501) staff       (20)        0 2023-12-25 02:57:02.329963 radoneye-1.0.0/src/radoneye.egg-info/
--rw-r--r--   0 artem      (501) staff       (20)     4619 2023-12-25 02:57:02.000000 radoneye-1.0.0/src/radoneye.egg-info/PKG-INFO
--rw-r--r--   0 artem      (501) staff       (20)      524 2023-12-25 02:57:02.000000 radoneye-1.0.0/src/radoneye.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (501) staff       (20)        1 2023-12-25 02:57:02.000000 radoneye-1.0.0/src/radoneye.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (501) staff       (20)       52 2023-12-25 02:57:02.000000 radoneye-1.0.0/src/radoneye.egg-info/entry_points.txt
--rw-r--r--   0 artem      (501) staff       (20)       46 2023-12-25 02:57:02.000000 radoneye-1.0.0/src/radoneye.egg-info/requires.txt
--rw-r--r--   0 artem      (501) staff       (20)        9 2023-12-25 02:57:02.000000 radoneye-1.0.0/src/radoneye.egg-info/top_level.txt
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2024-05-19 03:57:00.392111 radoneye-1.0.1/
+-rw-r--r--   0 artem      (501) staff       (20)     1070 2023-12-25 01:06:24.000000 radoneye-1.0.1/LICENSE
+-rw-r--r--   0 artem      (501) staff       (20)     4328 2024-05-19 03:57:00.391913 radoneye-1.0.1/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)     2473 2024-05-19 03:39:39.000000 radoneye-1.0.1/README.md
+-rw-r--r--   0 artem      (501) staff       (20)      870 2024-05-19 03:53:27.000000 radoneye-1.0.1/pyproject.toml
+-rw-r--r--   0 artem      (501) staff       (20)       29 2024-05-19 03:27:34.000000 radoneye-1.0.1/requirements.txt
+-rw-r--r--   0 artem      (501) staff       (20)       38 2024-05-19 03:57:00.392155 radoneye-1.0.1/setup.cfg
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2024-05-19 03:57:00.389151 radoneye-1.0.1/src/
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2024-05-19 03:57:00.390866 radoneye-1.0.1/src/radoneye/
+-rw-r--r--   0 artem      (501) staff       (20)      173 2023-12-25 01:16:49.000000 radoneye-1.0.1/src/radoneye/__init__.py
+-rw-r--r--   0 artem      (501) staff       (20)      140 2023-12-25 01:29:51.000000 radoneye-1.0.1/src/radoneye/__main__.py
+-rw-r--r--   0 artem      (501) staff       (20)     4925 2023-12-25 02:18:45.000000 radoneye-1.0.1/src/radoneye/cli.py
+-rw-r--r--   0 artem      (501) staff       (20)     2051 2023-12-25 02:42:16.000000 radoneye-1.0.1/src/radoneye/client.py
+-rw-r--r--   0 artem      (501) staff       (20)     1235 2023-12-25 01:02:27.000000 radoneye-1.0.1/src/radoneye/interface.py
+-rw-r--r--   0 artem      (501) staff       (20)      830 2023-12-25 01:22:51.000000 radoneye-1.0.1/src/radoneye/interface_factory.py
+-rw-r--r--   0 artem      (501) staff       (20)     4264 2024-05-19 03:56:34.000000 radoneye-1.0.1/src/radoneye/interface_v1.py
+-rw-r--r--   0 artem      (501) staff       (20)     6502 2024-05-19 03:37:55.000000 radoneye-1.0.1/src/radoneye/interface_v2.py
+-rw-r--r--   0 artem      (501) staff       (20)        0 2023-12-25 01:01:15.000000 radoneye-1.0.1/src/radoneye/py.typed
+-rw-r--r--   0 artem      (501) staff       (20)      468 2023-12-25 01:01:23.000000 radoneye-1.0.1/src/radoneye/scanner.py
+drwxr-xr-x   0 artem      (501) staff       (20)        0 2024-05-19 03:57:00.391713 radoneye-1.0.1/src/radoneye.egg-info/
+-rw-r--r--   0 artem      (501) staff       (20)     4328 2024-05-19 03:57:00.000000 radoneye-1.0.1/src/radoneye.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (501) staff       (20)      524 2024-05-19 03:57:00.000000 radoneye-1.0.1/src/radoneye.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (501) staff       (20)        1 2024-05-19 03:57:00.000000 radoneye-1.0.1/src/radoneye.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (501) staff       (20)       52 2024-05-19 03:57:00.000000 radoneye-1.0.1/src/radoneye.egg-info/entry_points.txt
+-rw-r--r--   0 artem      (501) staff       (20)       29 2024-05-19 03:57:00.000000 radoneye-1.0.1/src/radoneye.egg-info/requires.txt
+-rw-r--r--   0 artem      (501) staff       (20)        9 2024-05-19 03:57:00.000000 radoneye-1.0.1/src/radoneye.egg-info/top_level.txt
```

### Comparing `radoneye-1.0.0/LICENSE` & `radoneye-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radoneye-1.0.0/PKG-INFO` & `radoneye-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radoneye
-Version: 1.0.0
+Version: 1.0.1
 Summary: API and CLI for Ecosense RadonEye devices
 Author-email: Artem Butusov <art.sormy@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Artem Butusov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,29 +32,28 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio~=3.4.3
 Requires-Dist: bleak~=0.21.1
-Requires-Dist: paho-mqtt~=1.6.1
 
 # Ecosense RadonEye CLI and API for Python
 
 Provides simple and convinient Python API to communicate with RadonEye bluetooth devices.
 
 Supported devices:
 
-- RD200 (version 1) - not tested
-- RD200N (version 2) - tested
-- RD200P (version 2) - should work, never tested
+-   RD200 (version 1) - ok (but no history support, no counts/version in status)
+-   RD200N (version 2) - ok (full support)
+-   RD200P (version 2) - should work, not tested
 
 Version 1 support is implemented using publicly available information. I have no device to test on,
-if you have old RD200 device and are willing to help to build better support (beeps, history etc),
-then let me know.
+if you have old RD200 device and are willing to help to build better support (history etc), then let
+me know.
 
 ## Usage (API)
 
 Scan for all available devices, beep, read status and history:
 
 ```py
 import asyncio
@@ -135,31 +134,12 @@
 7	5	0.14
 8	3	0.08
 9	10	0.27
 10	10	0.27
 ...
 ```
 
-NOTE: On macOS bluetooth addresses are obfuscated to UUID.
-
-## Publishing
-
-```sh
-# install dependencices
-pip3 install twine
-# install locally
-pip3 install -e .
-# test using cli
-radoneye --help
-# build
-python3 -m build
-# view what is included into wheel
-unzip -l dist/*.whl
-# check wheel
-twine check dist/*.whl
-# upload to pypi
-twine upload --repository radoneye dist/*
-```
+NOTE: On macOS bluetooth addresses are obfuscated to UUIDs.
 
 ## License
 
 MIT
```

### Comparing `radoneye-1.0.0/README.md` & `radoneye-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # Ecosense RadonEye CLI and API for Python
 
 Provides simple and convinient Python API to communicate with RadonEye bluetooth devices.
 
 Supported devices:
 
-- RD200 (version 1) - not tested
-- RD200N (version 2) - tested
-- RD200P (version 2) - should work, never tested
+-   RD200 (version 1) - ok (but no history support, no counts/version in status)
+-   RD200N (version 2) - ok (full support)
+-   RD200P (version 2) - should work, not tested
 
 Version 1 support is implemented using publicly available information. I have no device to test on,
-if you have old RD200 device and are willing to help to build better support (beeps, history etc),
-then let me know.
+if you have old RD200 device and are willing to help to build better support (history etc), then let
+me know.
 
 ## Usage (API)
 
 Scan for all available devices, beep, read status and history:
 
 ```py
 import asyncio
@@ -95,31 +95,12 @@
 7	5	0.14
 8	3	0.08
 9	10	0.27
 10	10	0.27
 ...
 ```
 
-NOTE: On macOS bluetooth addresses are obfuscated to UUID.
-
-## Publishing
-
-```sh
-# install dependencices
-pip3 install twine
-# install locally
-pip3 install -e .
-# test using cli
-radoneye --help
-# build
-python3 -m build
-# view what is included into wheel
-unzip -l dist/*.whl
-# check wheel
-twine check dist/*.whl
-# upload to pypi
-twine upload --repository radoneye dist/*
-```
+NOTE: On macOS bluetooth addresses are obfuscated to UUIDs.
 
 ## License
 
 MIT
```

### Comparing `radoneye-1.0.0/pyproject.toml` & `radoneye-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,21 @@
 description = "API and CLI for Ecosense RadonEye devices"
 dynamic = ["dependencies"]
 keywords = ["Ecosense", "RadonEye", "RD200", "RD200N", "RD200P"]
 license = {file = "LICENSE"}
 name = "radoneye"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Homepage = "https://github.com/sormy/radoneye"
 Issues = "https://github.com/sormy/radoneye/issues"
 
 [project.scripts]
 radoneye = "radoneye.__main__:main"
+
+[tool.black]
+line-length = 100
```

### Comparing `radoneye-1.0.0/src/radoneye/cli.py` & `radoneye-1.0.1/src/radoneye/cli.py`

 * *Files identical despite different names*

### Comparing `radoneye-1.0.0/src/radoneye/client.py` & `radoneye-1.0.1/src/radoneye/client.py`

 * *Files identical despite different names*

### Comparing `radoneye-1.0.0/src/radoneye/interface.py` & `radoneye-1.0.1/src/radoneye/interface.py`

 * *Files identical despite different names*

### Comparing `radoneye-1.0.0/src/radoneye/interface_factory.py` & `radoneye-1.0.1/src/radoneye/interface_factory.py`

 * *Files identical despite different names*

### Comparing `radoneye-1.0.0/src/radoneye/interface_v1.py` & `radoneye-1.0.1/src/radoneye/interface_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from radoneye.interface import RadonEyeHistory, RadonEyeInterfaceBase, RadonEyeStatus
 
 SERVICE_V1 = "00001523-1212-efde-1523-785feabcd123"
 CHARACTERISTIC_V1_COMMAND = "00001524-1212-efde-1523-785feabcd123"
 CHARACTERISTIC_V1_STATUS = "00001525-1212-efde-1523-785feabcd123"
 COMMAND_V1_STATUS1 = [0x50]
 COMMAND_V1_STATUS2 = [0x51]
+COMMAND_V1_BEEP = [0xA1, 0x11]
+
+BEEP_DELAY = 0.2  # sec
 
 
 class RadonEyeMessageParserV1:
     @classmethod
     def parse_status(cls, data: bytearray, data2: bytearray, addr: str) -> RadonEyeStatus:
         latest_value = float(unpack("<f", data[2:6])[0])
         latest_pci_l = round(latest_value, 2)
@@ -95,8 +98,10 @@
         await client.stop_notify(CHARACTERISTIC_V1_STATUS)
         return result
 
     async def history(self, client: BleakClient) -> RadonEyeHistory:
         raise NotImplementedError
 
     async def beep(self, client: BleakClient) -> None:
-        raise NotImplementedError
+        await client.write_gatt_char(CHARACTERISTIC_V1_COMMAND, bytearray(COMMAND_V1_BEEP))
+        # there is some delay needed before you can do next beep, otherwise it will be just one beep
+        await asyncio.sleep(BEEP_DELAY)
```

### Comparing `radoneye-1.0.0/src/radoneye/interface_v2.py` & `radoneye-1.0.1/src/radoneye/interface_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 SERVICE_V2 = "00001523-0000-1000-8000-00805f9b34fb"
 CHARACTERISTIC_V2_COMMAND = "00001524-0000-1000-8000-00805f9b34fb"
 CHARACTERISTIC_V2_STATUS = "00001525-0000-1000-8000-00805f9b34fb"
 CHARACTERISTIC_V2_HISTORY = "00001526-0000-1000-8000-00805f9b34fb"
 COMMAND_V2_STATUS = [0x40]
 COMMAND_V2_HISTORY = [0x41]
-COMMAND_V2_BEEP = [0xA1, 0x11, 0x17, 0x0C, 0x0B, 0x01, 0x25, 0x28]
+COMMAND_V2_BEEP = [0xA1, 0x11]
 
 BEEP_DELAY = 0.2  # sec
 
 
 class RadonEyeMessageParserV2:
     @classmethod
     def read_short(cls, data: bytearray, start: int) -> int:
```

### Comparing `radoneye-1.0.0/src/radoneye.egg-info/PKG-INFO` & `radoneye-1.0.1/src/radoneye.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radoneye
-Version: 1.0.0
+Version: 1.0.1
 Summary: API and CLI for Ecosense RadonEye devices
 Author-email: Artem Butusov <art.sormy@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Artem Butusov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -32,29 +32,28 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: asyncio~=3.4.3
 Requires-Dist: bleak~=0.21.1
-Requires-Dist: paho-mqtt~=1.6.1
 
 # Ecosense RadonEye CLI and API for Python
 
 Provides simple and convinient Python API to communicate with RadonEye bluetooth devices.
 
 Supported devices:
 
-- RD200 (version 1) - not tested
-- RD200N (version 2) - tested
-- RD200P (version 2) - should work, never tested
+-   RD200 (version 1) - ok (but no history support, no counts/version in status)
+-   RD200N (version 2) - ok (full support)
+-   RD200P (version 2) - should work, not tested
 
 Version 1 support is implemented using publicly available information. I have no device to test on,
-if you have old RD200 device and are willing to help to build better support (beeps, history etc),
-then let me know.
+if you have old RD200 device and are willing to help to build better support (history etc), then let
+me know.
 
 ## Usage (API)
 
 Scan for all available devices, beep, read status and history:
 
 ```py
 import asyncio
@@ -135,31 +134,12 @@
 7	5	0.14
 8	3	0.08
 9	10	0.27
 10	10	0.27
 ...
 ```
 
-NOTE: On macOS bluetooth addresses are obfuscated to UUID.
-
-## Publishing
-
-```sh
-# install dependencices
-pip3 install twine
-# install locally
-pip3 install -e .
-# test using cli
-radoneye --help
-# build
-python3 -m build
-# view what is included into wheel
-unzip -l dist/*.whl
-# check wheel
-twine check dist/*.whl
-# upload to pypi
-twine upload --repository radoneye dist/*
-```
+NOTE: On macOS bluetooth addresses are obfuscated to UUIDs.
 
 ## License
 
 MIT
```

### Comparing `radoneye-1.0.0/src/radoneye.egg-info/SOURCES.txt` & `radoneye-1.0.1/src/radoneye.egg-info/SOURCES.txt`

 * *Files identical despite different names*

