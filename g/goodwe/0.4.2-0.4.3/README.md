# Comparing `tmp/goodwe-0.4.2.tar.gz` & `tmp/goodwe-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.4.2.tar", last modified: Thu May 16 21:30:15 2024, max compression
+gzip compressed data, was "goodwe-0.4.3.tar", last modified: Sun May 19 18:21:52 2024, max compression
```

## Comparing `goodwe-0.4.2.tar` & `goodwe-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 21:30:06.000000 goodwe-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 21:30:15.670645 goodwe-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-16 21:30:06.000000 goodwe-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 21:30:12.000000 goodwe-0.4.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    43890 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27703 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    37679 2024-05-16 21:30:06.000000 goodwe-0.4.2/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 21:30:15.000000 goodwe-0.4.2/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 21:30:06.000000 goodwe-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 21:30:15.674645 goodwe-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:30:15.670645 goodwe-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-16 21:30:06.000000 goodwe-0.4.2/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.662389 goodwe-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 18:21:40.000000 goodwe-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 18:21:52.662389 goodwe-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-19 18:21:40.000000 goodwe-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 18:21:48.000000 goodwe-0.4.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.658389 goodwe-0.4.3/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43890 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28306 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37679 2024-05-19 18:21:40.000000 goodwe-0.4.3/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.662389 goodwe-0.4.3/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 18:21:52.000000 goodwe-0.4.3/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 18:21:40.000000 goodwe-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-19 18:21:52.662389 goodwe-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:21:52.662389 goodwe-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29883 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73945 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14244 2024-05-19 18:21:40.000000 goodwe-0.4.3/tests/test_sensor.py
```

### Comparing `goodwe-0.4.2/LICENSE` & `goodwe-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/PKG-INFO` & `goodwe-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.2
+Version: 0.4.3
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.2/README.md` & `goodwe-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/__init__.py` & `goodwe-0.4.3/goodwe/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 ET_FAMILY = ["ET", "EH", "BT", "BH"]
 ES_FAMILY = ["ES", "EM", "BP"]
 DT_FAMILY = ["DT", "MS", "NS", "XS"]
 
 # Initial discovery command
 DISCOVERY_COMMAND = Aa55ProtocolCommand("010200", "0182")
 
-# supported inverter protocols
-_SUPPORTED_PROTOCOLS = [ET, DT, ES]
-
 
 async def connect(host: str, port: int = GOODWE_UDP_PORT, family: str = None, comm_addr: int = 0, timeout: int = 1,
                   retries: int = 3, do_discover: bool = True) -> Inverter:
     """Contact the inverter at the specified host/port and answer appropriate Inverter instance.
 
     The specific inverter family/type will be detected automatically, but it can be passed explicitly.
     Supported inverter family names are ET, EH, BT, BH, ES, EM, BP, DT, MS, D-NS and XS.
@@ -37,15 +34,15 @@
     will be used (0xf7 for ET/EH/BT/BH/ES/EM/BP inverters, 0x7f for DT/MS/D-NS/XS inverters).
 
     Since the UDP communication is by definition unreliable, when no (valid) response is received by the specified
     timeout, it is considered lost and the command will be re-tried up to retries times.
 
     Raise InverterError if unable to contact or recognise supported inverter.
     """
-    if family in ET_FAMILY or port == GOODWE_TCP_PORT:
+    if family in ET_FAMILY:
         inv = ET(host, port, comm_addr, timeout, retries)
     elif family in ES_FAMILY:
         inv = ES(host, port, comm_addr, timeout, retries)
     elif family in DT_FAMILY:
         inv = DT(host, port, comm_addr, timeout, retries)
     elif do_discover:
         return await discover(host, port, timeout, retries)
@@ -61,50 +58,51 @@
 async def discover(host: str, port: int = GOODWE_UDP_PORT, timeout: int = 1, retries: int = 3) -> Inverter:
     """Contact the inverter at the specified value and answer appropriate Inverter instance
 
     Raise InverterError if unable to contact or recognise supported inverter
     """
     failures = []
 
-    # Try the common AA55C07F0102000241 command first and detect inverter type from serial_number
-    try:
-        logger.debug("Probing inverter at %s:%s.", host, port)
-        response = await DISCOVERY_COMMAND.execute(UdpInverterProtocol(host, port, timeout, retries))
-        response = response.response_data()
-        model_name = response[5:15].decode("ascii").rstrip()
-        serial_number = response[31:47].decode("ascii")
-
-        i: Inverter | None = None
-        for model_tag in ET_MODEL_TAGS:
-            if model_tag in serial_number:
-                logger.debug("Detected ET/EH/BT/BH/GEH inverter %s, S/N:%s.", model_name, serial_number)
-                i = ET(host, port, 0, timeout, retries)
-                break
-        if not i:
-            for model_tag in ES_MODEL_TAGS:
-                if model_tag in serial_number:
-                    logger.debug("Detected ES/EM/BP inverter %s, S/N:%s.", model_name, serial_number)
-                    i = ES(host, port, 0, timeout, retries)
-                    break
-        if not i:
-            for model_tag in DT_MODEL_TAGS:
+    if port == GOODWE_UDP_PORT:
+        # Try the common AA55C07F0102000241 command first and detect inverter type from serial_number
+        try:
+            logger.debug("Probing inverter at %s:%s.", host, port)
+            response = await DISCOVERY_COMMAND.execute(UdpInverterProtocol(host, port, timeout, retries))
+            response = response.response_data()
+            model_name = response[5:15].decode("ascii").rstrip()
+            serial_number = response[31:47].decode("ascii")
+
+            i: Inverter | None = None
+            for model_tag in ET_MODEL_TAGS:
                 if model_tag in serial_number:
-                    logger.debug("Detected DT/MS/D-NS/XS/GEP inverter %s, S/N:%s.", model_name, serial_number)
-                    i = DT(host, port, 0, timeout, retries)
+                    logger.debug("Detected ET/EH/BT/BH/GEH inverter %s, S/N:%s.", model_name, serial_number)
+                    i = ET(host, port, 0, timeout, retries)
                     break
-        if i:
-            await i.read_device_info()
-            logger.debug("Connected to inverter %s, S/N:%s.", i.model_name, i.serial_number)
-            return i
+            if not i:
+                for model_tag in ES_MODEL_TAGS:
+                    if model_tag in serial_number:
+                        logger.debug("Detected ES/EM/BP inverter %s, S/N:%s.", model_name, serial_number)
+                        i = ES(host, port, 0, timeout, retries)
+                        break
+            if not i:
+                for model_tag in DT_MODEL_TAGS:
+                    if model_tag in serial_number:
+                        logger.debug("Detected DT/MS/D-NS/XS/GEP inverter %s, S/N:%s.", model_name, serial_number)
+                        i = DT(host, port, 0, timeout, retries)
+                        break
+            if i:
+                await i.read_device_info()
+                logger.debug("Connected to inverter %s, S/N:%s.", i.model_name, i.serial_number)
+                return i
 
-    except InverterError as ex:
-        failures.append(ex)
+        except InverterError as ex:
+            failures.append(ex)
 
     # Probe inverter specific protocols
-    for inv in _SUPPORTED_PROTOCOLS:
+    for inv in [ET, DT, ES]:
         i = inv(host, port, 0, timeout, retries)
         try:
             logger.debug("Probing %s inverter at %s.", inv.__name__, host)
             await i.read_device_info()
             await i.read_runtime_data()
             logger.debug("Detected %s family inverter %s, S/N:%s.", inv.__name__, i.model_name, i.serial_number)
             return i
```

### Comparing `goodwe-0.4.2/goodwe/const.py` & `goodwe-0.4.3/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/dt.py` & `goodwe-0.4.3/goodwe/dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/es.py` & `goodwe-0.4.3/goodwe/es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/et.py` & `goodwe-0.4.3/goodwe/et.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/exceptions.py` & `goodwe-0.4.3/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/inverter.py` & `goodwe-0.4.3/goodwe/inverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     Common superclass for various inverter models implementations.
     Represents the inverter state and its basic behavior
     """
 
     def __init__(self, host: str, port: int, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
         self._protocol: InverterProtocol = self._create_protocol(host, port, comm_addr, timeout, retries)
         self._consecutive_failures_count: int = 0
-        self.keep_alive: bool = True
 
         self.model_name: str | None = None
         self.serial_number: str | None = None
         self.rated_power: int = 0
         self.ac_output_type: int | None = None
         self.firmware: str | None = None
         self.arm_firmware: str | None = None
@@ -126,17 +125,17 @@
         except MaxRetriesException:
             self._consecutive_failures_count += 1
             raise RequestFailedException(f'No valid response received even after {self._protocol.retries} retries',
                                          self._consecutive_failures_count) from None
         except RequestFailedException as ex:
             self._consecutive_failures_count += 1
             raise RequestFailedException(ex.message, self._consecutive_failures_count) from None
-        finally:
-            if not self.keep_alive:
-                self._protocol.close_transport()
+
+    def set_keep_alive(self, keep_alive: bool) -> None:
+        self._protocol.keep_alive = keep_alive
 
     @abstractmethod
     async def read_device_info(self):
         """
         Request the device information from the inverter.
         The inverter instance variables will be loaded with relevant data.
         """
```

### Comparing `goodwe-0.4.2/goodwe/modbus.py` & `goodwe-0.4.3/goodwe/modbus.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,18 +218,22 @@
     data[7] is command return type
     data[8] is response payload length (for read commands)
     """
     if len(data) <= 8:
         logger.debug("Response is too short.")
         return False
     expected_length = int.from_bytes(data[4:6], byteorder='big', signed=False) + 6
-    if len(data) < expected_length:
+    # The weird expected_length != 12 is work around Goodwe bug answering wrong (hardcoded 6) length.
+    if len(data) < expected_length and expected_length != 12:
         raise PartialResponseException(len(data), expected_length)
 
     if data[7] == MODBUS_READ_CMD:
+        expected_length = data[8] + 9
+        if len(data) < expected_length:
+            raise PartialResponseException(len(data), expected_length)
         if data[8] != value * 2:
             logger.debug("Response has unexpected length: %d, expected %d.", data[8], value * 2)
             return False
     elif data[7] in (MODBUS_WRITE_CMD, MODBUS_WRITE_MULTI_CMD):
         if len(data) < 12:
             logger.debug("Response has unexpected length: %d, expected %d.", len(data), 14)
             raise PartialResponseException(len(data), expected_length)
```

### Comparing `goodwe-0.4.2/goodwe/model.py` & `goodwe-0.4.3/goodwe/model.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe/protocol.py` & `goodwe-0.4.3/goodwe/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self._port: int = port
         self._comm_addr: int = comm_addr
         self._running_loop: asyncio.AbstractEventLoop | None = None
         self._lock: asyncio.Lock | None = None
         self._timer: asyncio.TimerHandle | None = None
         self.timeout: int = timeout
         self.retries: int = retries
+        self.keep_alive: bool = True
         self.protocol: asyncio.Protocol | None = None
         self.response_future: Future | None = None
         self.command: ProtocolCommand | None = None
         self._partial_data: bytes | None = None
 
     def _ensure_lock(self) -> asyncio.Lock:
         """Validate (or create) asyncio Lock.
@@ -53,18 +54,18 @@
         """
         if self._lock and self._running_loop == asyncio.get_event_loop():
             return self._lock
         else:
             logger.debug("Creating lock instance for current event loop.")
             self._lock = asyncio.Lock()
             self._running_loop = asyncio.get_event_loop()
-            self.close_transport()
+            self._close_transport()
             return self._lock
 
-    def close_transport(self) -> None:
+    async def close(self) -> None:
         """Close the underlying transport/connection."""
         raise NotImplementedError()
 
     async def send_request(self, command: ProtocolCommand) -> Future:
         """Convert command to request and send it to inverter."""
         raise NotImplementedError()
 
@@ -112,15 +113,15 @@
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
         """On connection lost"""
         if exc:
             logger.debug("Socket closed with error: %s.", exc)
         else:
             logger.debug("Socket closed.")
-        self.close_transport()
+        self._close_transport()
 
     def datagram_received(self, data: bytes, addr: Tuple[str, int]) -> None:
         """On datagram received"""
         if self._timer:
             self._timer.cancel()
             self._timer = None
         try:
@@ -142,21 +143,21 @@
             self._partial_data = data
             return
         except asyncio.InvalidStateError:
             logger.debug("Response already handled: %s", data.hex())
         except RequestRejectedException as ex:
             logger.debug("Received exception response: %s", data.hex())
             self.response_future.set_exception(ex)
-            self.close_transport()
+            self._close_transport()
 
     def error_received(self, exc: Exception) -> None:
         """On error received"""
         logger.debug("Received error: %s", exc)
         self.response_future.set_exception(exc)
-        self.close_transport()
+        self._close_transport()
 
     async def send_request(self, command: ProtocolCommand) -> Future:
         """Send message via transport"""
         async with self._ensure_lock():
             await self._connect()
             response_future = asyncio.get_running_loop().create_future()
             self._retry = 0
@@ -184,27 +185,30 @@
             if self._timer:
                 logger.debug("Failed to receive response to %s in time (%ds).", self.command, self.timeout)
             self._retry += 1
             self._send_request(self.command, self.response_future)
         else:
             logger.debug("Max number of retries (%d) reached, request %s failed.", self.retries, self.command)
             self.response_future.set_exception(MaxRetriesException)
-            self.close_transport()
+            self._close_transport()
 
-    def close_transport(self) -> None:
+    def _close_transport(self) -> None:
         if self._transport:
             try:
                 self._transport.close()
             except RuntimeError:
                 logger.debug("Failed to close transport.")
             self._transport = None
         # Cancel Future on connection close
         if self.response_future and not self.response_future.done():
             self.response_future.cancel()
 
+    async def close(self):
+        self._close_transport()
+
 
 class TcpInverterProtocol(InverterProtocol, asyncio.Protocol):
     def __init__(self, host: str, port: int, comm_addr: int, timeout: int = 1, retries: int = 0):
         super().__init__(host, port, comm_addr, timeout, retries)
         self._transport: asyncio.transports.Transport | None = None
         self._retry: int = 0
 
@@ -223,39 +227,43 @@
     async def _connect(self) -> None:
         if not self._transport or self._transport.is_closing():
             logger.debug("Opening connection.")
             self._transport, self.protocol = await asyncio.get_running_loop().create_connection(
                 lambda: self,
                 host=self._host, port=self._port,
             )
-            sock = self._transport.get_extra_info('socket')
-            if sock is not None:
-                sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
-                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, 10)
-                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, 10)
-                sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPCNT, 3)
-                if platform.system() == 'Windows':
-                    sock.ioctl(socket.SIO_KEEPALIVE_VALS, (1, 10000, 10000))
+            if self.keep_alive:
+                try:
+                    sock = self._transport.get_extra_info('socket')
+                    if sock is not None:
+                        sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+                        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, 10)
+                        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, 10)
+                        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPCNT, 3)
+                        if platform.system() == 'Windows':
+                            sock.ioctl(socket.SIO_KEEPALIVE_VALS, (1, 10000, 10000))
+                except AttributeError as ex:
+                    logger.debug("Failed to apply KEEPALIVE: %s", ex)
 
     def connection_made(self, transport: asyncio.DatagramTransport) -> None:
         """On connection made"""
         logger.debug("Connection opened.")
         pass
 
     def eof_received(self) -> None:
         logger.debug("EOF received.")
-        self.close_transport()
+        self._close_transport()
 
     def connection_lost(self, exc: Optional[Exception]) -> None:
         """On connection lost"""
         if exc:
             logger.debug("Connection closed with error: %s.", exc)
         else:
             logger.debug("Connection closed.")
-        self.close_transport()
+        self._close_transport()
 
     def data_received(self, data: bytes) -> None:
         """On data received"""
         if self._timer:
             self._timer.cancel()
         try:
             if self._partial_data:
@@ -268,31 +276,31 @@
                     logger.debug("Received: %s", data.hex())
                 self._retry = 0
                 self._partial_data = None
                 self.response_future.set_result(data)
             else:
                 logger.debug("Received invalid response: %s", data.hex())
                 self.response_future.set_exception(RequestRejectedException())
-                self.close_transport()
+                self._close_transport()
         except PartialResponseException:
             logger.debug("Received response fragment: %s", data.hex())
             self._partial_data = data
             return
         except asyncio.InvalidStateError:
             logger.debug("Response already handled: %s", data.hex())
         except RequestRejectedException as ex:
             logger.debug("Received exception response: %s", data.hex())
             self.response_future.set_exception(ex)
-            # self.close_transport()
+            # self._close_transport()
 
     def error_received(self, exc: Exception) -> None:
         """On error received"""
         logger.debug("Received error: %s", exc)
         self.response_future.set_exception(exc)
-        self.close_transport()
+        self._close_transport()
 
     async def send_request(self, command: ProtocolCommand) -> Future:
         """Send message via transport"""
         await self._ensure_lock().acquire()
         try:
             await asyncio.wait_for(self._connect(), timeout=5)
             response_future = asyncio.get_running_loop().create_future()
@@ -302,15 +310,15 @@
         except asyncio.CancelledError:
             if self._retry < self.retries:
                 if self._timer:
                     logger.debug("Connection broken error.")
                 self._retry += 1
                 if self._lock and self._lock.locked():
                     self._lock.release()
-                self.close_transport()
+                self._close_transport()
                 return await self.send_request(command)
             else:
                 return self._max_retries_reached()
         except (ConnectionRefusedError, TimeoutError, OSError, asyncio.TimeoutError):
             if self._retry < self.retries:
                 logger.debug("Connection refused error.")
                 self._retry += 1
@@ -339,34 +347,42 @@
         """Retry mechanism to prevent hanging transport"""
         if self.response_future.done():
             self._retry = 0
         else:
             if self._timer:
                 logger.debug("Failed to receive response to %s in time (%ds).", self.command, self.timeout)
                 self._timer = None
-            self.close_transport()
+            self._close_transport()
 
     def _max_retries_reached(self) -> Future:
         logger.debug("Max number of retries (%d) reached, request %s failed.", self.retries, self.command)
-        self.close_transport()
+        self._close_transport()
         self.response_future = asyncio.get_running_loop().create_future()
         self.response_future.set_exception(MaxRetriesException)
         return self.response_future
 
-    def close_transport(self) -> None:
+    def _close_transport(self) -> None:
         if self._transport:
             try:
                 self._transport.close()
             except RuntimeError:
                 logger.debug("Failed to close transport.")
             self._transport = None
         # Cancel Future on connection lost
         if self.response_future and not self.response_future.done():
             self.response_future.cancel()
 
+    async def close(self):
+        await self._ensure_lock().acquire()
+        try:
+            self._close_transport()
+        finally:
+            if self._lock and self._lock.locked():
+                self._lock.release()
+
 
 class ProtocolResponse:
     """Definition of response to protocol command"""
 
     def __init__(self, raw_data: bytes, command: Optional[ProtocolCommand]):
         self.raw_data: bytes = raw_data
         self.command: ProtocolCommand = command
@@ -437,14 +453,17 @@
                 raise RequestFailedException(
                     "No response received to '" + self.request.hex() + "' request."
                 )
         except (asyncio.CancelledError, ConnectionRefusedError):
             raise RequestFailedException(
                 "No valid response received to '" + self.request.hex() + "' request."
             ) from None
+        finally:
+            if not protocol.keep_alive:
+                await protocol.close()
 
 
 class Aa55ProtocolCommand(ProtocolCommand):
     """
     Inverter communication protocol seen mostly on older generations of inverters.
     Quite probably it is some variation of the protocol used on RS-485 serial link,
     extended/adapted to UDP transport layer.
@@ -481,16 +500,15 @@
         Validate the response.
         data[0:3] is header
         data[4:5] is response type
         data[6] is response payload length
         data[-2:] is checksum (plain sum of response data incl. header)
         """
         if len(data) <= 8 or len(data) != data[6] + 9:
-            logger.debug("Response has unexpected length: %d, expected %d.", len(data), data[6] + 9)
-            return False
+            raise PartialResponseException(len(data), data[6] + 9)
         elif response_type:
             data_rt_int = int.from_bytes(data[4:6], byteorder="big", signed=True)
             if int(response_type, 16) != data_rt_int:
                 logger.debug("Response type unexpected: %04x, expected %s.", data_rt_int, response_type)
                 return False
         checksum = 0
         for each in data[:-2]:
```

### Comparing `goodwe-0.4.2/goodwe/sensor.py` & `goodwe-0.4.3/goodwe/sensor.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/goodwe.egg-info/PKG-INFO` & `goodwe-0.4.3/goodwe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.4.2
+Version: 0.4.3
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.4.2/setup.cfg` & `goodwe-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/tests/test_dt.py` & `goodwe-0.4.3/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/tests/test_es.py` & `goodwe-0.4.3/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/tests/test_et.py` & `goodwe-0.4.3/tests/test_et.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/tests/test_modbus.py` & `goodwe-0.4.3/tests/test_modbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,16 @@
     def test_create_modbus_tcp_multi_request(self):
         request = create_modbus_tcp_multi_request(0xf7, 0x10, 0x88b8, b'\x01\x02\x03\x04\x05\x06')
         self.assertEqual('00010000000df71088b8000306010203040506', request.hex())
 
     def test_validate_modbus_tcp_read_response(self):
         self.assert_tcp_response_ok('000100000007b4030445565345', 0x3, 310, 2)
         self.assert_tcp_response_ok('000100000007b4030400000002', 0x3, 331, 2)
+        # technically illegal, but work around Goodwe bug
+        self.assert_tcp_response_ok('000100000006f703020000', 0x3, 47510, 1)
         # length too short
         self.assert_tcp_response_partial('000100000007b403040000', 0x03, 331, 2)
         # failure code
         self.assert_tcp_response_rejected('000100000007b4830400000002', 0x03, 331, 2)
 
     def test_validate_modbus_tcp_write_response(self):
         self.assert_tcp_response_ok('000100000006b40601364556', 0x06, 310, 0x4556)
```

### Comparing `goodwe-0.4.2/tests/test_protocol.py` & `goodwe-0.4.3/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.4.2/tests/test_sensor.py` & `goodwe-0.4.3/tests/test_sensor.py`

 * *Files identical despite different names*

