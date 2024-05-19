# Comparing `tmp/govee_local_api-1.4.5.tar.gz` & `tmp/govee_local_api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govee_local_api-1.4.5.tar", max compression
+gzip compressed data, was "govee_local_api-1.5.0.tar", max compression
```

## Comparing `govee_local_api-1.4.5.tar` & `govee_local_api-1.5.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/LICENSE
--rw-r--r--   0        0        0      464 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/README.md
--rw-r--r--   0        0        0     1252 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/pyproject.toml
--rw-r--r--   0        0        0      219 2024-04-28 15:13:17.435687 govee_local_api-1.4.5/src/govee_local_api/__init__.py
--rw-r--r--   0        0        0    13573 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/controller.py
--rw-r--r--   0        0        0     4062 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/device.py
--rw-r--r--   0        0        0    11156 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/light_capabilities.py
--rw-r--r--   0        0        0     3755 2024-04-28 15:13:17.439687 govee_local_api-1.4.5/src/govee_local_api/message.py
--rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 govee_local_api-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/LICENSE
+-rw-r--r--   0        0        0      464 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/README.md
+-rw-r--r--   0        0        0     1295 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0      219 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/src/govee_local_api/__init__.py
+-rw-r--r--   0        0        0    14069 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/src/govee_local_api/controller.py
+-rw-r--r--   0        0        0     4062 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/src/govee_local_api/device.py
+-rw-r--r--   0        0        0    11472 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/src/govee_local_api/light_capabilities.py
+-rw-r--r--   0        0        0     3778 2024-05-19 16:06:58.790463 govee_local_api-1.5.0/src/govee_local_api/message.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 govee_local_api-1.5.0/PKG-INFO
```

### Comparing `govee_local_api-1.4.5/LICENSE` & `govee_local_api-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govee_local_api-1.4.5/pyproject.toml` & `govee_local_api-1.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "govee-local-api"
-version = "1.4.5"
+version = "1.5.0"
 description = "Library to communicate with Govee local API"
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/Galorhallen/govee-local-api"
 
 authors = ["Galorhallen <andrea.ponte1987@gmail.com>"]
 
@@ -46,8 +46,9 @@
 pythonpath = "src"
 addopts = [
     "--import-mode=importlib",
     "-v",
 ]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `govee_local_api-1.4.5/src/govee_local_api/controller.py` & `govee_local_api-1.5.0/src/govee_local_api/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import socket
 from datetime import datetime, timedelta
 from typing import Callable, Tuple, Any, cast
+import ipaddress
 
 from .device import GoveeDevice
 from .light_capabilities import GOVEE_LIGHT_CAPABILITIES, GoveeLightCapability
 from .message import (
     BrightnessMessage,
     ColorMessage,
     GoveeMessage,
@@ -72,14 +73,15 @@
         self._broadcast_address = broadcast_address
         self._broadcast_port = broadcast_port
         self._listening_address = listening_address
         self._listening_port = listening_port
         self._device_command_port = device_command_port
 
         self._loop = loop or asyncio.get_running_loop()
+        self._cleanup_done: asyncio.Event = asyncio.Event()
         self._message_factory = MessageResponseFactory()
         self._devices: dict[str, GoveeDevice] = {}
 
         self._discovery_enabled = discovery_enabled
         self._discovery_interval = discovery_interval
         self._update_enabled = update_enabled
         self._update_interval = update_interval
@@ -100,21 +102,23 @@
         )
 
         if self._discovery_enabled:
             self.send_discovery_message()
         if self._update_enabled:
             self.send_update_message()
 
-    def cleanup(self):
+    def cleanup(self) -> asyncio.Event:
+        self._cleanup_done.clear()
         self.set_update_enabled(False)
         self.set_discovery_enabled(False)
 
         if self._transport:
             self._transport.close()
         self._devices.clear()
+        return self._cleanup_done
 
     def add_device(
         self,
         ip: str,
         sku: str,
         fingerprint,
         capabilities: set[GoveeLightCapability] | None,
@@ -240,37 +244,44 @@
 
     def connection_made(self, transport):
         self._transport = transport
         sock = self._transport.get_extra_info("socket")
 
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
-        sock.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, 2)
 
-        sock.setsockopt(
-            socket.SOL_IP,
-            socket.IP_MULTICAST_IF,
-            socket.inet_aton(self._listening_address),
-        )
-        sock.setsockopt(
-            socket.SOL_IP,
-            socket.IP_ADD_MEMBERSHIP,
-            socket.inet_aton(self._broadcast_address)
-            + socket.inet_aton(self._listening_address),
-        )
+        broadcast_ip = ipaddress.ip_address(self._broadcast_address)
 
-    def connection_lost(self, *args, **kwargs):
-        if self._transport:
-            sock = self._transport.get_extra_info("socket")
+        if broadcast_ip.is_multicast:
+            sock.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, 2)
+
+            sock.setsockopt(
+                socket.SOL_IP,
+                socket.IP_MULTICAST_IF,
+                socket.inet_aton(self._listening_address),
+            )
             sock.setsockopt(
                 socket.SOL_IP,
-                socket.IP_DROP_MEMBERSHIP,
+                socket.IP_ADD_MEMBERSHIP,
                 socket.inet_aton(self._broadcast_address)
                 + socket.inet_aton(self._listening_address),
             )
+
+    def connection_lost(self, *args, **kwargs):
+        if self._transport:
+            broadcast_ip = ipaddress.ip_address(self._broadcast_address)
+            if broadcast_ip.is_multicast:
+                sock = self._transport.get_extra_info("socket")
+                sock.setsockopt(
+                    socket.SOL_IP,
+                    socket.IP_DROP_MEMBERSHIP,
+                    socket.inet_aton(self._broadcast_address)
+                    + socket.inet_aton(self._listening_address),
+                )
+        self._cleanup_done.set()
         self._logger.debug("Disconnected")
 
     def datagram_received(self, data: bytes, addr: tuple):
         if not data:
             return
         message = self._message_factory.create_message(data)
         if not message:
```

### Comparing `govee_local_api-1.4.5/src/govee_local_api/device.py` & `govee_local_api-1.5.0/src/govee_local_api/device.py`

 * *Files identical despite different names*

### Comparing `govee_local_api-1.4.5/src/govee_local_api/light_capabilities.py` & `govee_local_api-1.5.0/src/govee_local_api/light_capabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,8 +353,18 @@
         GoveeLightCapability.BRIGHTNESS,
     },
     "H61C3": {
         GoveeLightCapability.COLOR_RGB,
         GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
         GoveeLightCapability.BRIGHTNESS,
     },
+    "H61D3": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
+    "H608B": {
+        GoveeLightCapability.COLOR_RGB,
+        GoveeLightCapability.COLOR_KELVIN_TEMPERATURE,
+        GoveeLightCapability.BRIGHTNESS,
+    },
 }
```

### Comparing `govee_local_api-1.4.5/src/govee_local_api/message.py` & `govee_local_api-1.5.0/src/govee_local_api/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, data: dict[str, Any]) -> None:
         self._data = data
 
     def as_dict(self) -> dict[str, Any]:
         return {"msg": {"cmd": self.command, "data": self.data}}
 
     def as_json(self) -> str:
-        return json.dumps(self.as_dict())
+        return json.dumps(self.as_dict(), separators=(",", ":"))
 
     def __bytes__(self) -> bytearray | bytes:
         return self.as_json().encode("utf-8")
 
     def __str__(self) -> str:
         return self.as_json()
```

### Comparing `govee_local_api-1.4.5/PKG-INFO` & `govee_local_api-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govee-local-api
-Version: 1.4.5
+Version: 1.5.0
 Summary: Library to communicate with Govee local API
 Home-page: https://github.com/Galorhallen/govee-local-api
 License: Apache Software License 2.0
 Author: Galorhallen
 Author-email: andrea.ponte1987@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

