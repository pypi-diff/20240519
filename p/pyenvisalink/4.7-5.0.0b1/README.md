# Comparing `tmp/pyenvisalink-4.7.tar.gz` & `tmp/pyenvisalink-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenvisalink-4.7.tar", last modified: Sun May 19 03:43:43 2024, max compression
+gzip compressed data, was "pyenvisalink-5.0.0b1.tar", last modified: Sun Feb 26 23:45:01 2023, max compression
```

## Comparing `pyenvisalink-4.7.tar` & `pyenvisalink-5.0.0b1.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:43.920141 pyenvisalink-4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-19 03:43:40.000000 pyenvisalink-4.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-19 03:43:43.920141 pyenvisalink-4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-19 03:43:40.000000 pyenvisalink-4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:43.920141 pyenvisalink-4.7/pyenvisalink/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9476 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/alarm_panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/alarm_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/dsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/dsc_envisalinkdefs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/envisalink_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11146 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/honeywell_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/honeywell_envisalinkdefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-19 03:43:40.000000 pyenvisalink-4.7/pyenvisalink/test_harness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 03:43:43.920141 pyenvisalink-4.7/pyenvisalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-19 03:43:43.000000 pyenvisalink-4.7/pyenvisalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 03:43:43.000000 pyenvisalink-4.7/pyenvisalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 03:43:43.000000 pyenvisalink-4.7/pyenvisalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 03:43:43.000000 pyenvisalink-4.7/pyenvisalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-19 03:43:43.920141 pyenvisalink-4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-19 03:43:40.000000 pyenvisalink-4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 23:45:00.994551 pyenvisalink-5.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-26 23:45:00.994551 pyenvisalink-5.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 23:45:00.994551 pyenvisalink-5.0.0b1/pyenvisalink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18647 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/alarm_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/alarm_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/dsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/dsc_envisalinkdefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25132 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/envisalink_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/evl_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/honeywell_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20344 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/honeywell_envisalinkdefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/mock_server_dsc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/mock_server_honeywell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/pyenvisalink/test_harness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-26 23:45:00.994551 pyenvisalink-5.0.0b1/pyenvisalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-26 23:45:00.000000 pyenvisalink-5.0.0b1/pyenvisalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-26 23:45:00.000000 pyenvisalink-5.0.0b1/pyenvisalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-26 23:45:00.000000 pyenvisalink-5.0.0b1/pyenvisalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-26 23:45:00.000000 pyenvisalink-5.0.0b1/pyenvisalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-26 23:45:00.994551 pyenvisalink-5.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-02-26 23:44:51.000000 pyenvisalink-5.0.0b1/setup.py
```

### Comparing `pyenvisalink-4.7/LICENSE.txt` & `pyenvisalink-5.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyenvisalink-4.7/README.md` & `pyenvisalink-5.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pyenvisalink-4.7/pyenvisalink/dsc_client.py` & `pyenvisalink-5.0.0b1/pyenvisalink/dsc_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,287 +1,382 @@
 import asyncio
-import logging
+import datetime
 import json
+import logging
 import re
-import asyncio
-import datetime
-from pyenvisalink import EnvisalinkClient
-from pyenvisalink.dsc_envisalinkdefs import *
+import time
+
+from .const import (
+    STATE_CHANGE_KEYPAD,
+    STATE_CHANGE_PARTITION,
+    STATE_CHANGE_ZONE,
+    STATE_CHANGE_ZONE_BYPASS,
+)
+from .dsc_envisalinkdefs import (
+    evl_ArmModes,
+    evl_Commands,
+    evl_PanicTypes,
+    evl_ResponseTypes,
+    evl_TPI_Response_Codes,
+    evl_verboseTrouble,
+)
+from .envisalink_base_client import EnvisalinkClient
 
 _LOGGER = logging.getLogger(__name__)
 
-from asyncio import ensure_future
 
 class DSCClient(EnvisalinkClient):
     """Represents a dsc alarm client."""
 
-    def __init__(self, panel, loop):
-        self._refreshZoneByassState = False
-        self._zoneBypassRefreshTask = None
-        super().__init__(panel, loop)
+    def detect(prompt):
+        """Given the initial connection data, determine if this is a DSC panel."""
+        code = "505"
+        data = "3"
+        login = code + data + DSCClient.get_checksum(code, data)
+        return prompt == login
+
+    def __init__(self, panel):
+        super().__init__(panel)
+        self._loginEvent = asyncio.Event()
 
-    def to_chars(self, string):
+    def to_chars(string):
         chars = []
         for char in string:
             chars.append(ord(char))
         return chars
 
-    def get_checksum(self, code, data):
+    def get_checksum(code, data):
         """part of each command includes a checksum.  Calculate."""
-        return ("%02X" % sum(self.to_chars(code)+self.to_chars(data)))[-2:]
+        return ("%02X" % sum(DSCClient.to_chars(code) + DSCClient.to_chars(data)))[-2:]
 
-    def send_command(self, code, data):
+    async def send_command(self, code, data, logData=None):
         """Send a command in the proper honeywell format."""
-        to_send = code + data + self.get_checksum(code, data)
-        self.send_data(to_send)
+        to_send = code + data + DSCClient.get_checksum(code, data)
+        await self.send_data(to_send)
 
-    def dump_zone_timers(self):
+    async def dump_zone_timers(self):
         """Send a command to dump out the zone timers."""
-        self.send_command(evl_Commands['DumpZoneTimers'], '')
+        await self.queue_command(evl_Commands["DumpZoneTimers"], "")
 
-    def keypresses_to_partition(self, partitionNumber, keypresses):
+    async def keypresses_to_partition(self, partitionNumber, keypresses):
         """Send keypresses (max of 6) to a particular partition."""
-        self.send_command(evl_Commands['PartitionKeypress'], str.format("{0}{1}", partitionNumber, keypresses[:6]))
+        await self.queue_command(
+            evl_Commands["PartitionKeypress"],
+            str.format("{0}{1}", partitionNumber, keypresses[:6]),
+        )
 
     async def keep_alive(self):
         """Send a keepalive command to reset it's watchdog timer."""
-        while not self._shutdown:
-            if self._loggedin:
-                self.send_command(evl_Commands['KeepAlive'], '')
-            await asyncio.sleep(self._alarmPanel.keepalive_interval)
-
-    async def periodic_zone_timer_dump(self):
-        """Used to periodically get the zone timers to make sure our zones are updated."""
-        while not self._shutdown:
-            if self._loggedin:
-                self.dump_zone_timers()
-            await asyncio.sleep(self._alarmPanel.zone_timer_interval)
+        await self.queue_command(evl_Commands["KeepAlive"], "")
 
-    def arm_stay_partition(self, code, partitionNumber):
+    async def arm_stay_partition(self, code, partitionNumber):
         """Public method to arm/stay a partition."""
-        self._cachedCode = code
-        self.send_command(evl_Commands['ArmStay'], str(partitionNumber))
+        await self.queue_command(evl_Commands["ArmStay"], str(partitionNumber), code)
 
-    def arm_away_partition(self, code, partitionNumber):
+    async def arm_away_partition(self, code, partitionNumber):
         """Public method to arm/away a partition."""
-        self._cachedCode = code
-        self.send_command(evl_Commands['ArmAway'], str(partitionNumber))
+        await self.queue_command(evl_Commands["ArmAway"], str(partitionNumber), code)
 
-    def arm_max_partition(self, code, partitionNumber):
+    async def arm_max_partition(self, code, partitionNumber):
         """Public method to arm/max a partition."""
-        self._cachedCode = code
-        self.send_command(evl_Commands['ArmMax'], str(partitionNumber))
+        await self.queue_command(evl_Commands["ArmMax"], str(partitionNumber), code)
 
-    def arm_night_partition(self, code, partitionNumber):
+    async def arm_night_partition(self, code, partitionNumber, mode=None):
         """Public method to arm/max a partition."""
-        self.arm_max_partition(code, partitionNumber)
+        await self.arm_max_partition(code, partitionNumber)
 
-    def disarm_partition(self, code, partitionNumber):
+    async def disarm_partition(self, code, partitionNumber):
         """Public method to disarm a partition."""
-        self._cachedCode = code
-        self.send_command(evl_Commands['Disarm'], str(partitionNumber) + str(code))
+        await self.queue_command(evl_Commands["Disarm"], str(partitionNumber) + str(code), code)
 
-    def panic_alarm(self, panicType):
+    async def panic_alarm(self, panicType):
         """Public method to raise a panic alarm."""
-        self.send_command(evl_Commands['Panic'], evl_PanicTypes[panicType])
+        await self.queue_command(evl_Commands["Panic"], evl_PanicTypes[panicType])
 
-    def toggle_zone_bypass(self, zone):
+    async def toggle_zone_bypass(self, zone):
         """Public method to toggle a zone's bypass state."""
-        self.keypresses_to_partition(1, "*1%02d#" % zone)
+        await self.keypresses_to_partition(1, "*1%02d#" % zone)
 
-    def command_output(self, code, partitionNumber, outputNumber):
+    async def command_output(self, code, partitionNumber, outputNumber):
         """Used to activate the selected command output"""
-        self._cachedCode = code
-        self.send_command(evl_Commands['CommandOutput'], str.format("{0}{1}", partitionNumber, outputNumber))	
+        await self.queue_command(
+            evl_Commands["CommandOutput"],
+            str.format("{0}{1}", partitionNumber, outputNumber),
+            code,
+        )
 
     def parseHandler(self, rawInput):
         """When the envisalink contacts us- parse out which command and data."""
         cmd = {}
         dataoffset = 0
-        if rawInput != '':
-            if re.match(r'\d\d:\d\d:\d\d\s', rawInput):
+        if rawInput != "":
+            if re.match(r"\d\d:\d\d:\d\d\s", rawInput):
                 dataoffset = dataoffset + 9
-            code = rawInput[dataoffset:dataoffset+3]
-            cmd['code'] = code
-            cmd['data'] = rawInput[dataoffset+3:][:-2]
-            
-            try:
-                #Interpret the login command further to see what our handler is.
-                if evl_ResponseTypes[code]['handler'] == 'login':
-                    if cmd['data'] == '3':
-                      handler = 'login'
-                    elif cmd['data'] == '2':
-                      handler = 'login_timeout'
-                    elif cmd['data'] == '1':
-                      handler = 'login_success'
-                    elif cmd['data'] == '0':
-                      handler = 'login_failure'
+            code = rawInput[dataoffset : dataoffset + 3]
+            cmd["code"] = code
+            cmd["data"] = rawInput[dataoffset + 3 :][:-2]
 
-                    cmd['handler'] = "handle_%s" % handler
-                    cmd['callback'] = "callback_%s" % handler
+            try:
+                # Interpret the login command further to see what our handler is.
+                if evl_ResponseTypes[code]["handler"] == "login":
+                    if cmd["data"] == "3":
+                        handler = "login"
+                    elif cmd["data"] == "2":
+                        handler = "login_timeout"
+                    elif cmd["data"] == "1":
+                        handler = "login_success"
+                    elif cmd["data"] == "0":
+                        handler = "login_failure"
 
+                    cmd["handler"] = "handle_%s" % handler
                 else:
-                    cmd['handler'] = "handle_%s" % evl_ResponseTypes[code]['handler']
-                    cmd['callback'] = "callback_%s" % evl_ResponseTypes[code]['handler']
+                    cmd["handler"] = "handle_%s" % evl_ResponseTypes[code]["handler"]
+                cmd["state_change"] = evl_ResponseTypes[code].get("state_change", False)
             except KeyError:
-                _LOGGER.debug(str.format('No handler defined in config for {0}, skipping...', code))
-                
+                _LOGGER.debug(str.format("No handler defined in config for {0}, skipping...", code))
+
         return cmd
 
     def handle_login(self, code, data):
         """When the envisalink asks us for our password- send it."""
-        self.send_command(evl_Commands['Login'], self._alarmPanel.password) 
+        self.create_internal_task(self.queue_login_response(), name="queue_login_response")
+
+    async def queue_login_response(self):
+        self._loginEvent.clear()
+        await self.queue_command(evl_Commands["Login"], self._alarmPanel.password)
+
+        # Wait until the 505 resposnse is received
+        try:
+            await asyncio.wait_for(
+                self._loginEvent.wait(), timeout=self._alarmPanel.connection_timeout
+            )
+        except Exception:
+            pass
+
+        if not self._loggedin:
+            # Timed out waiting for login
+            await self.disconnect()
 
     def handle_login_success(self, code, data):
         """Handler for when the envisalink accepts our credentials."""
         super().handle_login_success(code, data)
-        dt = datetime.datetime.now().strftime('%H%M%m%d%y')
-        self.send_command(evl_Commands['SetTime'], dt)
-        self.send_command(evl_Commands['StatusReport'], '')
+
+        self._loginEvent.set()
+        self.create_internal_task(self.complete_login(), name="complete_login")
+
+    def handle_login_failure(self, code, data):
+        """Handler for when the envisalink rejects our credentials."""
+        super().handle_login_failure(code, data)
+        self._loginEvent.set()
+
+    async def complete_login(self):
+        dt = datetime.datetime.now().strftime("%H%M%m%d%y")
+        await self.queue_command(evl_Commands["SetTime"], dt)
+        await self.queue_command(evl_Commands["StatusReport"], "")
 
         if self._alarmPanel._zoneBypassEnabled:
-            """ Initiate request for zone bypass information """
-            self._refreshZoneBypassStatus = True
-            if self._zoneBypassRefreshTask == None:
-                self._zoneBypassRefreshTask = ensure_future(self.dump_zone_bypass_status(), loop=self._eventLoop)
+            """Initiate request for zone bypass information"""
+            await self.dump_zone_bypass_status()
 
     def handle_command_response(self, code, data):
         """Handle the envisalink's initial response to our commands."""
-        _LOGGER.debug("DSC ack recieved.")
+        if code == "500":
+            _LOGGER.debug("DSC ack recieved.")
+            self.command_succeeded(data)
+        elif code == "501":
+            _LOGGER.error("Issued command resulted in a checksum failure.")
+            self.command_failed(retry=True)
+        elif code == "502":
+            retry = False
+            if data in evl_TPI_Response_Codes:
+                errorInfo = evl_TPI_Response_Codes[data]
+                retry = errorInfo["retry"]
+                msg = f"System error received for issued command: {errorInfo['msg']} ({data})"
+                if retry:
+                    _LOGGER.warn(msg)
+                else:
+                    _LOGGER.error(msg)
 
-    def handle_command_response_error(self, code, data):
-        """Handle the case where the DSC passes back a checksum failure."""
-        _LOGGER.error("The previous command resulted in a checksum failure.")
-
-    def handle_poll_response(self, code, data):
-        """Handle the response to our keepalive messages."""
-        self.handle_command_response(code, data)
+            else:
+                _LOGGER.error(f"Unrecognized system error for issued command: '{data}'")
+            self.command_failed(retry=retry)
 
     def handle_zone_state_change(self, code, data):
         """Handle when the envisalink sends us a zone change."""
         """Event 601-610."""
-        parse = re.match('^[0-9]{3,4}$', data)
+        now = time.time()
+        parse = re.match("^[0-9]{3,4}$", data)
         if parse:
             zoneNumber = int(data[-3:])
-            self._alarmPanel.alarm_state['zone'][zoneNumber]['status'].update(evl_ResponseTypes[code]['status'])
-            _LOGGER.debug(str.format("(zone {0}) state has updated: {1}", zoneNumber, json.dumps(evl_ResponseTypes[code]['status'])))
-            return zoneNumber
+            self._alarmPanel.alarm_state["zone"][zoneNumber]["status"].update(
+                evl_ResponseTypes[code]["status"]
+            )
+            self._alarmPanel.alarm_state["zone"][zoneNumber]["updated"] = now
+            _LOGGER.debug(
+                str.format(
+                    "(zone {0}) state has updated: {1}",
+                    zoneNumber,
+                    json.dumps(evl_ResponseTypes[code]["status"]),
+                )
+            )
+            return {STATE_CHANGE_ZONE: [zoneNumber]}
         else:
             _LOGGER.error("Invalid data has been passed in the zone update.")
 
     def handle_partition_state_change(self, code, data):
-        """Handle when the envisalink sends us a partition change."""
-        """Event 650-674, 652 is an exception, because 2 bytes are passed for partition and zone type."""
-        if code == '652':
-            parse = re.match('^[0-9]{2}$', data)
+        """Handle when the envisalink sends us a partition change.
+        Event 650-674, 652 is an exception, because 2 bytes are passed for partition
+        and zone type."""
+        if code == "652":
+            parse = re.match("^[0-9]{2}$", data)
             if parse:
                 partitionNumber = int(data[0])
-                self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update(evl_ArmModes[data[1]]['status'])
-                _LOGGER.debug(str.format("(partition {0}) state has updated: {1}", partitionNumber, json.dumps(evl_ArmModes[data[1]]['status'])))
-                return partitionNumber
+                self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                    evl_ArmModes[data[1]]["status"]
+                )
+                _LOGGER.debug(
+                    str.format(
+                        "(partition {0}) state has updated: {1}",
+                        partitionNumber,
+                        json.dumps(evl_ArmModes[data[1]]["status"]),
+                    )
+                )
+                return {STATE_CHANGE_PARTITION: [partitionNumber]}
             else:
-                _LOGGER.error("Invalid data has been passed when arming the alarm.") 
+                _LOGGER.error("Invalid data has been passed when arming the alarm.")
         else:
-            parse = re.match('^[0-9]+$', data)
+            parse = re.match("^[0-9]+$", data)
             if parse:
                 partitionNumber = int(data[0])
-                self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update(evl_ResponseTypes[code]['status'])
-                _LOGGER.debug(str.format("(partition {0}) state has updated: {1}", partitionNumber, json.dumps(evl_ResponseTypes[code]['status'])))
-                
-                '''Log the user who last armed or disarmed the alarm'''
-                if code == '700':
-                    lastArmedBy = {'last_armed_by_user': int(data[1:5])}
-                    self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update(lastArmedBy)
-                elif code == '750':
-                    lastDisarmedBy = {'last_disarmed_by_user': int(data[1:5])}
-                    self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update(lastDisarmedBy)
-
-                if code == '655' and self._alarmPanel._zoneBypassEnabled:
-                    """Partition was disarmed which means the bypassed zones have likley been reset so force a zone bypass refresh"""
-                    self._refreshZoneBypassStatus = True
+                self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                    evl_ResponseTypes[code]["status"]
+                )
+                _LOGGER.debug(
+                    str.format(
+                        "(partition {0}) state has updated: {1}",
+                        partitionNumber,
+                        json.dumps(evl_ResponseTypes[code]["status"]),
+                    )
+                )
+
+                """Log the user who last armed or disarmed the alarm"""
+                if code == "700":
+                    lastArmedBy = {"last_armed_by_user": int(data[1:5])}
+                    self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                        lastArmedBy
+                    )
+                elif code == "750":
+                    lastDisarmedBy = {"last_disarmed_by_user": int(data[1:5])}
+                    self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                        lastDisarmedBy
+                    )
+
+                if code == "655" and self._alarmPanel._zoneBypassEnabled:
+                    """Partition was disarmed which means the bypassed zones have likley been
+                    reset so force a zone bypass refresh"""
+                    self.create_internal_task(
+                        self.dump_zone_bypass_status(), name="dump_zone_bypass_status"
+                    )
 
-                return partitionNumber
+                return {STATE_CHANGE_PARTITION: [partitionNumber]}
             else:
-                _LOGGER.error("Invalid data has been passed in the parition update.")
+                _LOGGER.error("Invalid data has been passed in the partition update.")
 
     def handle_send_code(self, code, data):
-        """The DSC will, depending upon settings, challenge us with the code.  If the user passed it in, we'll send it."""
+        """The DSC will, depending upon settings, challenge us with the code.  If the user
+        passed it in, we'll send it."""
+        self.create_internal_task(self.foo(), name="send_code")
+
+    async def send_code(self):
         if self._cachedCode is None:
             _LOGGER.error("The envisalink asked for a code, but we have no code in our cache.")
         else:
-            self.send_command(evl_Commands['SendCode'], self._cachedCode)
+            await self.send_command(evl_Commands["SendCode"], self._cachedCode)
             self._cachedCode = None
 
     def handle_keypad_update(self, code, data):
         """Handle general- non partition based info"""
-        if code == '849':
-            bits = "{0:016b}".format(int(data,16))
+        if code == "849":
+            bits = f"{int(data,16):016b}"
             trouble_description = ""
             ac_present = True
             for i in range(0, 7):
-                if bits[15-i] == '1':
-                    trouble_description += evl_verboseTrouble[i] + ', '
+                if bits[15 - i] == "1":
+                    trouble_description += evl_verboseTrouble[i] + ", "
                     if i == 1:
                         ac_present = False
-            new_status = {'alpha':trouble_description.strip(', '), 'ac_present': ac_present}
+            new_status = {
+                "alpha": trouble_description.strip(", "),
+                "ac_present": ac_present,
+            }
         else:
-            new_status = evl_ResponseTypes[code]['status']
-       
-        for part in self._alarmPanel.alarm_state['partition']:
-            self._alarmPanel.alarm_state['partition'][part]['status'].update(new_status)
+            new_status = evl_ResponseTypes[code]["status"]
+
+        updatedPartitions = []
+        for part in self._alarmPanel.alarm_state["partition"]:
+            self._alarmPanel.alarm_state["partition"][part]["status"].update(new_status)
+            updatedPartitions.append(part)
         _LOGGER.debug(str.format("(All partitions) state has updated: {0}", json.dumps(new_status)))
+        return {STATE_CHANGE_KEYPAD: updatedPartitions}
 
     def handle_zone_bypass_update(self, code, data):
-        """ Handle zone bypass update triggered when *1 is used on the keypad """
+        """Handle zone bypass update triggered when *1 is used on the keypad"""
         if not self._alarmPanel._zoneBypassEnabled:
             return
 
-        self._refreshZoneBypassStatus = False
         if len(data) == 16:
-            updates = {}
+            updates = []
             for byte in range(8):
-                bypassBitfield = int('0x' + data[byte * 2] + data[(byte * 2) + 1], 0)
+                bypassBitfield = int("0x" + data[byte * 2] + data[(byte * 2) + 1], 0)
 
                 for bit in range(8):
                     zoneNumber = (byte * 8) + bit + 1
-                    bypassed = (bypassBitfield & (1 << bit) != 0)
-                    if self._alarmPanel.alarm_state['zone'][zoneNumber]['bypassed'] != bypassed:
-                        updates[zoneNumber] = bypassed
-                    self._alarmPanel.alarm_state['zone'][zoneNumber]['bypassed'] = bypassed
-                    _LOGGER.debug(str.format("(zone {0}) bypass state has updated: {1}", zoneNumber, bypassed))
-
+                    bypassed = bypassBitfield & (1 << bit) != 0
+                    if self._alarmPanel.alarm_state["zone"][zoneNumber]["bypassed"] != bypassed:
+                        updates.append(zoneNumber)
+                    self._alarmPanel.alarm_state["zone"][zoneNumber]["bypassed"] = bypassed
+                    _LOGGER.debug(
+                        str.format(
+                            "(zone {0}) bypass state has updated: {1}",
+                            zoneNumber,
+                            bypassed,
+                        )
+                    )
 
             _LOGGER.debug(str.format("zone bypass updates: {0}", updates))
-            return updates
+            return {STATE_CHANGE_ZONE_BYPASS: updates}
         else:
-            _LOGGER.error(str.format("Invalid data length ({0}) has been received in the bypass update.", len(data)))
+            _LOGGER.error(
+                str.format(
+                    "Invalid data length ({0}) has been received in the bypass update.",
+                    len(data),
+                )
+            )
 
     async def dump_zone_bypass_status(self):
-        """ Loop requesting zone bypass status until the command succeeds.
-            This is necessary to deal with TPI/DSC buffer overrun errors.
-            Ideally all commands would be queued with a retry mechanism when BUSY or BUFFER_OVERRUN is received back"""
-        while not self._shutdown:
-            if self._loggedin and self._refreshZoneBypassStatus and not self.is_any_partition_armed():
-                """ Trigger a 616 'Bypassed Zones Bitfield Dump' to initialize the bypass state.
-                    There is unfortunately not a specific command to request a zone bypass dump so the *1# keypresses are sent instead.
-                    It appears that limitations in the envisalink API (or perhaps the panel itself) makes it impossible for this feature
-                    to work if the alarm panel is setup to require a code to bypass zones.
-
-                    Only issue the command if the alarm is not armed since the EVL will not send a 616 when in the armed state.
-                    """
-                self.keypresses_to_partition(1, "*1#")
-            await asyncio.sleep(5)
+        """Trigger a 616 'Bypassed Zones Bitfield Dump' to initialize the bypass state.
+        There is unfortunately not a specific command to request a zone bypass dump so
+        the *1# keypresses are sent instead.  It appears that limitations in the envisalink
+        API (or perhaps the panel itself) makes it impossible for this feature
+        to work if the alarm panel is setup to require a code to bypass zones."""
+
+        # The panel won't respond if this command is issued while armed.
+        if not self.is_any_partition_armed():
+            await self.keypresses_to_partition(1, "*1#")
+
+    def is_zone_open_from_zonedump(self, zone, ticks) -> bool:
+        # DSC seems to report accurately to 0 means open, anything else means closed
+        return ticks == 0
 
     def is_any_partition_armed(self) -> bool:
-        """ Check if any partition is either armed or arming/disarming """
-        for partition, state in self._alarmPanel.alarm_state['partition'].items():
-            status = state['status']
-            away = status.get('armed_away', False)
-            stay = status.get('armed_stay', False)
-            exit_delay = status.get('exit_delay', False)
-            entry_delay = status.get('entry_delay', False)
+        """Check if any partition is either armed or arming/disarming"""
+        for partition, state in self._alarmPanel.alarm_state["partition"].items():
+            status = state["status"]
+            away = status.get("armed_away", False)
+            stay = status.get("armed_stay", False)
+            exit_delay = status.get("exit_delay", False)
+            entry_delay = status.get("entry_delay", False)
             if away or stay or exit_delay or entry_delay:
-                _LOGGER.debug(f"is_any_partition_armed: partition {partition} status={status}")
+                _LOGGER.debug("is_any_partition_armed: partition %s status=%s", partition, status)
                 return True
         _LOGGER.debug("is_any_partition_armed: no partitions are armed")
         return False
-
```

### Comparing `pyenvisalink-4.7/pyenvisalink/honeywell_client.py` & `pyenvisalink-5.0.0b1/pyenvisalink/honeywell_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,406 @@
-import logging
 import json
+import logging
 import re
-import asyncio
-from pyenvisalink import EnvisalinkClient
-from pyenvisalink.honeywell_envisalinkdefs import *
+import time
+
+from .const import STATE_CHANGE_PARTITION, STATE_CHANGE_ZONE, STATE_CHANGE_ZONE_BYPASS
+from .envisalink_base_client import EnvisalinkClient
+from .honeywell_envisalinkdefs import (
+    IconLED_Flags,
+    evl_ArmDisarm_CIDs,
+    evl_CID_Events,
+    evl_CID_Qualifiers,
+    evl_Commands,
+    evl_PanicTypes,
+    evl_ResponseTypes,
+    evl_TPI_Response_Codes,
+    evl_Virtual_Keypad_How_To_Beep,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
+
 class HoneywellClient(EnvisalinkClient):
     """Represents a honeywell alarm client."""
 
+    def __init__(self, panel):
+        super().__init__(panel)
+        self._zoneTimers = {}
+
+    def detect(prompt):
+        """Given the initial connection data, determine if this is a Honeywell panel."""
+        return prompt == "Login:"
+
     async def keep_alive(self):
-        """Send a keepalive command to reset it's watchdog timer."""
-        while not self._shutdown:
-            if self._loggedin:
-                self.send_command(evl_Commands['KeepAlive'], '')
-            await asyncio.sleep(self._alarmPanel.keepalive_interval)
-
-    async def periodic_zone_timer_dump(self):
-        """Used to periodically get the zone timers to make sure our zones are updated."""
-        while not self._shutdown:
-            if self._loggedin:
-                self.dump_zone_timers()
-            await asyncio.sleep(self._alarmPanel.zone_timer_interval)
+        await self.queue_command(evl_Commands["KeepAlive"], "")
 
-    def send_command(self, code, data):
+    async def send_command(self, code, data, logData=None):
         """Send a command in the proper honeywell format."""
-        to_send = '^' + code + ',' + data + '$'
-        self.send_data(to_send)
+        to_send = "^" + code + "," + data + "$"
+        await self.send_data(to_send, logData)
 
-    def dump_zone_timers(self):
+    async def dump_zone_timers(self):
         """Send a command to dump out the zone timers."""
-        self.send_command(evl_Commands['DumpZoneTimers'], '')
+        await self.queue_command(evl_Commands["DumpZoneTimers"], "")
+
+    async def queue_keypresses_to_partition(self, partitionNumber, keypresses, logData):
+        commands = []
+        for idx, char in enumerate(keypresses):
+            log = data = f"{partitionNumber},{char}"
+            if logData:
+                log = f"{partitionNumber},{logData[idx]}"
+
+            commands.append(
+                {
+                    "cmd": evl_Commands["PartitionKeypress"],
+                    "data": data,
+                    "log": log,
+                }
+            )
+
+        # Queue up all the keypresses together to ensure an unrelated command cannot
+        # be inserted in the middle.
+        await self.queue_commands(commands)
 
-    def keypresses_to_partition(self, partitionNumber, keypresses):
+    async def keypresses_to_partition(self, partitionNumber, keypresses):
         """Send keypresses to a particular partition."""
-        for char in keypresses:
-            self.send_command(evl_Commands['PartitionKeypress'], str.format("{0},{1}", partitionNumber, char))
+        await self.queue_keypresses_to_partition(partitionNumber, keypresses, None)
 
-    def arm_stay_partition(self, code, partitionNumber):
+    async def arm_stay_partition(self, code, partitionNumber):
         """Public method to arm/stay a partition."""
-        self.keypresses_to_partition(partitionNumber, code + '3')
+        await self.queue_keypresses_to_partition(
+            partitionNumber,
+            code + "3",
+            ("*" * len(code)) + "3",
+        )
 
-    def arm_away_partition(self, code, partitionNumber):
+    async def arm_away_partition(self, code, partitionNumber):
         """Public method to arm/away a partition."""
-        self.keypresses_to_partition(partitionNumber, code + '2')
+        await self.queue_keypresses_to_partition(
+            partitionNumber,
+            code + "2",
+            ("*" * len(code)) + "2",
+        )
 
-    def arm_max_partition(self, code, partitionNumber):
+    async def arm_max_partition(self, code, partitionNumber):
         """Public method to arm/max a partition."""
-        self.keypresses_to_partition(partitionNumber, code + '4')
+        await self.queue_keypresses_to_partition(
+            partitionNumber,
+            code + "4",
+            ("*" * len(code)) + "4",
+        )
 
-    def arm_night_partition(self, code, partitionNumber):
+    async def arm_night_partition(self, code, partitionNumber, mode=None):
         """Public method to arm/max a partition."""
-        self.keypresses_to_partition(partitionNumber, code + '7')
+        mode_keys = "33"
+        if mode is not None:
+            mode_keys = mode
+        await self.queue_keypresses_to_partition(
+            partitionNumber,
+            code + mode_keys,
+            ("*" * len(code)) + mode_keys,
+        )
 
-    def disarm_partition(self, code, partitionNumber):
+    async def disarm_partition(self, code, partitionNumber):
         """Public method to disarm a partition."""
-        self.keypresses_to_partition(partitionNumber, code + '1')
+        await self.queue_keypresses_to_partition(
+            partitionNumber,
+            code + "1",
+            ("*" * len(code)) + "1",
+        )
 
-    def panic_alarm(self, panicType):
+    async def panic_alarm(self, panicType):
         """Public method to raise a panic alarm."""
-        self.keypresses_to_partition(1, evl_PanicTypes[panicType])
+        await self.keypresses_to_partition(1, evl_PanicTypes[panicType])
 
     def parseHandler(self, rawInput):
         """When the envisalink contacts us- parse out which command and data."""
         cmd = {}
         _LOGGER.debug(str.format("Data received:{0}", rawInput))
 
-        parse = re.match(r'([%\^].+)\$', rawInput)
+        parse = re.match(r"([%\^].+)\$", rawInput)
         if parse and parse.group(1):
             # keep first sentinel char to tell difference between tpi and
             # Envisalink command responses.  Drop the trailing $ sentinel.
-            inputList = parse.group(1).split(',')
+            inputList = parse.group(1).split(",")
             code = inputList[0]
-            cmd['code'] = code
-            cmd['data'] = ','.join(inputList[1:])
-            _LOGGER.debug(str.format("Code:{0} Data:{1}", code, cmd['data']))
+            cmd["code"] = code
+            cmd["data"] = ",".join(inputList[1:])
+            _LOGGER.debug(str.format("Code:{0} Data:{1}", code, cmd["data"]))
         elif not self._loggedin:
             # assume it is login info
             code = rawInput
-            cmd['code'] = code
-            cmd['data'] = ''
+            cmd["code"] = code
+            cmd["data"] = ""
         else:
-            _LOGGER.error("Unrecognized data recieved from the envisalink. Ignoring.")    
+            _LOGGER.error("Unrecognized data recieved from the envisalink. Ignoring.")
             return None
         try:
-            cmd['handler'] = "handle_%s" % evl_ResponseTypes[code]['handler']
-            cmd['callback'] = "callback_%s" % evl_ResponseTypes[code]['handler']
+            cmd["handler"] = "handle_%s" % evl_ResponseTypes[code]["handler"]
+            cmd["state_change"] = evl_ResponseTypes[code].get("state_change", False)
         except KeyError:
-            _LOGGER.warning(str.format('No handler defined in config for {0}, skipping...', code))
-                
+            _LOGGER.warning(str.format("No handler defined in config for {0}, skipping...", code))
+
         return cmd
 
     def handle_login(self, code, data):
         """When the envisalink asks us for our password- send it."""
-        self.send_data(self._alarmPanel.password) 
-        
+        self.create_internal_task(self.queue_login_response(), name="queue_login_response")
+
+    async def queue_login_response(self):
+        await self.send_data(self._alarmPanel.password)
+
     def handle_command_response(self, code, data):
         """Handle the envisalink's initial response to our commands."""
-        responseString = evl_TPI_Response_Codes[data]
-        _LOGGER.debug("Envisalink response: " + responseString)
-        if data != '00':
-            logging.error("error sending command to envisalink.  Response was: " + responseString)
-			
-    def handle_poll_response(self, code, data):
-        """Handle the response to our keepalive messages."""
-        self.handle_command_response(code, data)
-        
+        if data in evl_TPI_Response_Codes:
+            responseInfo = evl_TPI_Response_Codes[data]
+            _LOGGER.debug("Envisalink response: " + responseInfo["msg"])
+            if data == "00":
+                self.command_succeeded(code[1:])
+            else:
+                _LOGGER.error(
+                    "error sending command to envisalink.  Response was: " + responseInfo["msg"]
+                )
+                self.command_failed(retry=responseInfo["retry"])
+        else:
+            _LOGGER.error(str.format("Unrecognized response code ({0}) received", data))
+            self.command_failed(retry=False)
+
     def handle_keypad_update(self, code, data):
         """Handle the response to when the envisalink sends keypad updates our way."""
-        dataList = data.split(',')
+        partition_updates = []
+        zone_updates = []
+        bypass_updates = []
+
+        dataList = data.split(",")
         # Custom messages and alpha fields might contain unescaped commas, so we'll recombine them:
         if len(dataList) > 5:
             dataList[4] = ",".join(dataList[4:])
             del dataList[5:]
         # make sure data is in format we expect, current TPI seems to send bad data every so often
-        #TODO: Make this a regex...
+        # TODO: Make this a regex...
         if "%" in data:
             _LOGGER.error("Data format invalid from Envisalink, ignoring...")
             return
 
         partitionNumber = int(dataList[0])
+        if not (partitionNumber in self._zoneTimers.keys()):
+            self._zoneTimers[partitionNumber] = {}
+        partition_updates.append(partitionNumber)
         flags = IconLED_Flags()
         flags.asShort = int(dataList[1], 16)
-        beep = evl_Virtual_Keypad_How_To_Beep.get(dataList[3], 'unknown')
+        try:
+            user_zone_field = int(dataList[2])
+        except ValueError:
+            user_zone_field = None
+        beep = evl_Virtual_Keypad_How_To_Beep.get(dataList[3], "unknown")
         alpha = dataList[4]
-        _LOGGER.debug("Updating our local alarm state...")
-        self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update({'alarm': bool(flags.alarm), 'alarm_in_memory': bool(flags.alarm_in_memory), 'armed_away': bool(flags.armed_away),
-                                                                   'ac_present': bool(flags.ac_present), 'armed_bypass': bool(flags.bypass), 'chime': bool(flags.chime),
-                                                                   'armed_zero_entry_delay': bool(flags.armed_zero_entry_delay), 'alarm_fire_zone': bool(flags.alarm_fire_zone),
-                                                                   'trouble': bool(flags.system_trouble), 'ready': bool(flags.ready), 'fire': bool(flags.fire),
-                                                                   'armed_stay': bool(flags.armed_stay), 'bat_trouble': bool(flags.low_battery),
-                                                                   'alpha': alpha,
-                                                                   'beep': beep,
-                                                                   })
-        _LOGGER.debug(json.dumps(self._alarmPanel.alarm_state['partition'][partitionNumber]['status']))
+        partition_status = HoneywellClient.get_partition_state(flags, alpha)
+        zone_code = HoneywellClient.get_zone_report_type(flags, alpha)
+        prior_ready = self._alarmPanel.alarm_state["partition"][partitionNumber]["status"]["ready"]
+        prior_bypass = self._alarmPanel.alarm_state["partition"][partitionNumber]["status"][
+            "armed_bypass"
+        ]
+
+        # TODO "armed_bypass" is included in the state below but just passes the bypass flag.
+        # How is that used?
+        self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+            {
+                "alarm": bool(flags.alarm),
+                "alarm_in_memory": bool(flags.alarm_in_memory),
+                "armed_away": bool(flags.armed_away),
+                "ac_present": bool(flags.ac_present),
+                "armed_bypass": bool(flags.bypass),
+                "chime": bool(flags.chime),
+                "armed_zero_entry_delay": bool(flags.armed_zero_entry_delay),
+                "alarm_fire_zone": bool(flags.alarm_fire_zone),
+                "trouble": bool(flags.system_trouble),
+                "ready": bool(flags.ready),
+                "fire": bool(flags.fire),
+                "armed_stay": bool(flags.armed_stay),
+                "alpha": alpha,
+                "beep": beep,
+            }
+        )
+
+        if (partition_status == "ready") and not prior_ready:
+            # Clear all zones known to be in this partition
+            _LOGGER.debug(f"Clear partition {partitionNumber}")
+            for z in list(self._zoneTimers[partitionNumber]):
+                _LOGGER.debug(f"Timer {z} :: {self._zoneTimers[partitionNumber][z]} Closing")
+                timer = str.split(z, "|")
+                zone_updates.append(int(timer[0]))
+                if timer[1] == "state":
+                    self._alarmPanel.alarm_state["zone"][int(timer[0])]["status"].update(
+                        {"open": False, "fault": False}
+                    )
+                self._zoneTimers[partitionNumber].pop(z)
+
+        if prior_bypass and not bool(flags.bypass):
+            # Partition has switched from bypassed to not bypassed, so clear bypass flags
+            # TODO Need to know which bypassed zones are in which partition to handle this.
+            # No zone timers for these - either maintain a list or add partition to zone status
+            _LOGGER.debug("Clear bypassed zones")
+
+        if flags.not_used2 and flags.not_used3:
+            # Keypad update is giving partition status. Battery report applies to system battery
+            _LOGGER.debug(
+                f"Keypad update is giving partition {partitionNumber} status. "
+                f"Partition: {partition_status} Zonecode: {zone_code}"
+            )
+            self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                {"bat_trouble": bool(flags.low_battery)}
+            )
+
+        elif (partition_status == "arming") and (zone_code == "notready"):
+            # Keypad is counting down. Nothing to do
+            # TODO Add entry_delay to %00 update handler
+            _LOGGER.debug(f"Keypad is counting down to arm partition {partitionNumber}.")
+
+        elif user_zone_field is not None:
+            # Keypad is giving zone status. Update zone status and check zone timers
+            _LOGGER.debug(f"Keypad is giving zone status for partition {partitionNumber}.")
+
+            # Increment all existing zone timers by 1
+            for z in self._zoneTimers[partitionNumber]:
+                self._zoneTimers[partitionNumber][z] += 1
+
+            # Add a zone timer (if needed) of the appropriate type and update zone status
+            if zone_code in ["battery", "tamper"]:
+                # Battery or tamper report for a wireless zone. These are added to the keypad
+                # update queue separate from state changes, so need their own zone timers.
+                self._zoneTimers[partitionNumber][f"{user_zone_field}|{zone_code}"] = 1
+            elif zone_code == "bypass":
+                # Bypassed zones only show once in keypad updates and only clear when the
+                # partition is disarmed. No zone timer needed.
+                self._alarmPanel.alarm_state["zone"][user_zone_field]["bypassed"] = True
+                bypass_updates.append(user_zone_field)
+            elif zone_code in ["alarm", "alarmcleared", "notready"]:
+                # Zone is open
+                # TODO There is a "last_tripped_time" attribute that was previously populated
+                # based on zone timer dumps. Does that add enough value to merit reproducing?
+                self._alarmPanel.alarm_state["zone"][user_zone_field]["status"].update(
+                    {"open": True, "fault": True}
+                )
+                self._zoneTimers[partitionNumber][f"{user_zone_field}|state"] = 1
+                zone_updates.append(user_zone_field)
+
+            # Check and kill any overdue timers
+            active_timers = len(self._zoneTimers[partitionNumber])
+            # TODO Is this the right margin to add?
+            max_timer = round(active_timers * 2 + 2, 0)
+            for z in list(self._zoneTimers[partitionNumber]):
+                if self._zoneTimers[partitionNumber][z] > max_timer:
+                    _LOGGER.debug(f"Timer {z} :: {self._zoneTimers[partitionNumber][z]} Closing")
+                    timer = str.split(z, "|")
+                    zone_updates.append(int(timer[0]))
+                    if timer[1] == "state":
+                        self._alarmPanel.alarm_state["zone"][int(timer[0])]["status"].update(
+                            {"open": False, "fault": False}
+                        )
+                    # else:
+                    # TODO Clear tamper/battery status
+                    self._zoneTimers[partitionNumber].pop(z)
+                else:
+                    _LOGGER.debug(f"Timer {z} :: {self._zoneTimers[partitionNumber][z]}")
+            _LOGGER.debug(f"There are ({active_timers}) active timers")
+
+        _LOGGER.debug(
+            json.dumps(self._alarmPanel.alarm_state["partition"][partitionNumber]["status"])
+        )
+        results = {}
+        if partition_updates:
+            results[STATE_CHANGE_PARTITION] = partition_updates
+        if zone_updates:
+            results[STATE_CHANGE_ZONE] = zone_updates
+        if bypass_updates:
+            results[STATE_CHANGE_ZONE_BYPASS] = bypass_updates
+        return results
 
     def handle_zone_state_change(self, code, data):
         """Handle when the envisalink sends us a zone change."""
-        # Envisalink TPI is inconsistent at generating these
-        bigEndianHexString = ''
-        # every four characters
-        inputItems = re.findall('....', data)
-        for inputItem in inputItems:
-            # Swap the couples of every four bytes
-            # (little endian to big endian)
-            swapedBytes = []
-            swapedBytes.insert(0, inputItem[0:2])
-            swapedBytes.insert(0, inputItem[2:4])
-
-            # add swapped set of four bytes to our return items,
-            # converting from hex to int
-            bigEndianHexString += ''.join(swapedBytes)
-
-        # convert hex string to 64 bit bitstring TODO: THIS IS 128 for evl4
-        if self._alarmPanel.envisalink_version < 4:
-            bitfieldString = str(bin(int(bigEndianHexString, 16))[2:].zfill(64))
-        else:
-            bitfieldString = str(bin(int(bigEndianHexString, 16))[2:].zfill(128))
-
-        # reverse every 16 bits so "lowest" zone is on the left
-        zonefieldString = ''
-        inputItems = re.findall('.' * 16, bitfieldString)
-
-        for inputItem in inputItems:
-            zonefieldString += inputItem[::-1]
-
-        for zoneNumber, zoneBit in enumerate(zonefieldString, start=1):
-                self._alarmPanel.alarm_state['zone'][zoneNumber]['status'].update({'open': zoneBit == '1', 'fault': zoneBit == '1'})
-                if zoneBit == '1':
-                    self._alarmPanel.alarm_state['zone'][zoneNumber]['last_fault'] = 0
-
-                _LOGGER.debug("(zone %i) is %s", zoneNumber, "Open/Faulted" if zoneBit == '1' else "Closed/Not Faulted")
+        return None
 
     def handle_partition_state_change(self, code, data):
         """Handle when the envisalink sends us a partition change."""
-        for currentIndex in range(0, 8):
-            partitionStateCode = data[currentIndex * 2:(currentIndex * 2) + 2]
-            partitionState = evl_Partition_Status_Codes[str(partitionStateCode)]
-            partitionNumber = currentIndex + 1
-            previouslyArmed = self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].get('armed', False)
-            armed = partitionState['name'] in ('ARMED_STAY', 'ARMED_AWAY', 'ARMED_MAX')
-            self._alarmPanel.alarm_state.update({'arm': not armed, 'disarm': armed, 'cancel': bool(partitionState['name'] == 'EXIT_ENTRY_DELAY')})
-            self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update({'exit_delay': bool(partitionState['name'] == 'EXIT_ENTRY_DELAY' and not previouslyArmed),
-                                                                           'entry_delay': bool(partitionState['name'] == 'EXIT_ENTRY_DELAY' and previouslyArmed),
-                                                                           'armed': armed,
-                                                                           'ready': bool(partitionState['name'] == 'READY' or partitionState['name'] == 'READY_BYPASS')})
-
-            if partitionState['name'] == 'NOT_READY': self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update({'ready': False})
-            _LOGGER.debug('Parition ' + str(partitionNumber) + ' is in state ' + partitionState['name'])
-            _LOGGER.debug(json.dumps(self._alarmPanel.alarm_state['partition'][partitionNumber]['status']))
+        return None
 
     def handle_realtime_cid_event(self, code, data):
         """Handle when the envisalink sends us an alarm arm/disarm/trigger."""
         eventTypeInt = int(data[0])
         eventType = evl_CID_Qualifiers[eventTypeInt]
         cidEventInt = int(data[1:4])
         cidEvent = evl_CID_Events[cidEventInt]
         partitionNumber = int(data[4:6])
         zoneOrUser = int(data[6:9])
         if cidEventInt in evl_ArmDisarm_CIDs:
             if eventTypeInt == 1:
-                self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update({'last_disarmed_by_user': zoneOrUser})
+                self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                    {"last_disarmed_by_user": zoneOrUser}
+                )
             if eventTypeInt == 3:
-                self._alarmPanel.alarm_state['partition'][partitionNumber]['status'].update({'last_armed_by_user': zoneOrUser})
-        
-        _LOGGER.debug('Event Type is ' + eventType)
-        _LOGGER.debug('CID Type is ' + cidEvent['type'])
-        _LOGGER.debug('CID Description is ' + cidEvent['label'])
-        _LOGGER.debug('Partition is ' + str(partitionNumber))
-        _LOGGER.debug(cidEvent['type'] + ' value is ' + str(zoneOrUser))
-        
+                self._alarmPanel.alarm_state["partition"][partitionNumber]["status"].update(
+                    {"last_armed_by_user": zoneOrUser}
+                )
+
+        _LOGGER.debug("Event Type is " + eventType)
+        _LOGGER.debug("CID Type is " + cidEvent["type"])
+        _LOGGER.debug("CID Description is " + cidEvent["label"])
+        _LOGGER.debug("Partition is " + str(partitionNumber))
+        _LOGGER.debug(cidEvent["type"] + " value is " + str(zoneOrUser))
+
         return cidEvent
+
+    def is_zone_open_from_zonedump(self, zone, ticks) -> bool:
+        now = time.time()
+        last_zone_dump = now - self._alarmPanel.zone_timer_interval
+        last_update = self._alarmPanel.alarm_state["zone"][zone]["updated"]
+
+        if last_zone_dump < last_update:
+            # This zone has been explicitly updated since the last zone timer dump so honor
+            # its current state
+            return self._alarmPanel.alarm_state["zone"][zone]["status"]["open"]
+
+        # The envisalink never seems to report back exactly 0 seconds for an open zone.
+        # It always seems to be 1-3 ticks.  So 3 ticks or less will be considered open.
+        return ticks <= 3
+
+    def get_partition_state(flags, alpha):
+        if bool(flags.alarm) or bool(flags.alarm_fire_zone) or bool(flags.fire):
+            return "alarm"
+        elif bool(flags.alarm_in_memory):
+            return "alarmcleared"
+        elif alpha.find("You may exit now") != -1:
+            return "arming"
+        elif alpha.find("May Exit Now") != -1:
+            return "arming"
+        elif bool(flags.armed_stay) and bool(flags.armed_zero_entry_delay):
+            return "armedinstant"
+        elif bool(flags.armed_away) and bool(flags.armed_zero_entry_delay):
+            return "armedmax"
+        elif bool(flags.armed_stay):
+            return "armedstay"
+        elif bool(flags.armed_away):
+            return "armedaway"
+        elif bool(flags.ready):
+            return "ready"
+        elif not bool(flags.ready):
+            return "notready"
+        else:
+            return "unknown"
+
+    def get_zone_report_type(flags, alpha):
+        if bool(flags.alarm) or bool(flags.alarm_fire_zone) or bool(flags.fire):
+            return "alarm"
+        elif bool(flags.alarm_in_memory):
+            return "alarmcleared"
+        elif bool(flags.system_trouble):
+            return "tamper"
+        elif bool(flags.low_battery):
+            return "battery"
+        elif bool(flags.bypass) and (alpha.find("BYPAS") != -1):
+            return "bypass"
+        elif not bool(flags.ready):
+            return "notready"
+        else:
+            return "unknown"
```

### Comparing `pyenvisalink-4.7/pyenvisalink/honeywell_envisalinkdefs.py` & `pyenvisalink-5.0.0b1/pyenvisalink/honeywell_envisalinkdefs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,737 +1,838 @@
-## Alarm Server
-## Supporting Envisalink 2DS/3
-##
-## This code is under the terms of the GPL v3 license.
+# Alarm Server
+# Supporting Envisalink 2DS/3
+#
+# This code is under the terms of the GPL v3 license.
 import ctypes
+
 c_uint16 = ctypes.c_uint16
 
-class IconLED_Bitfield( ctypes.LittleEndianStructure ):
-    _fields_ = [
-                ("alarm",     c_uint16, 1 ),
-                ("alarm_in_memory", c_uint16, 1 ),
-                ("armed_away",    c_uint16, 1 ),
-                ("ac_present",       c_uint16, 1 ),
-                ("bypass",       c_uint16, 1 ),
-                ("chime",       c_uint16, 1 ),
-                ("not_used1",       c_uint16, 1 ),
-                ("armed_zero_entry_delay",       c_uint16, 1 ),
-                ("alarm_fire_zone",       c_uint16, 1 ),
-                ("system_trouble",       c_uint16, 1 ),
-                ("not_used2",       c_uint16, 1 ),
-                ("not_used3",       c_uint16, 1 ),
-                ("ready",       c_uint16, 1 ),
-                ("fire",       c_uint16, 1 ),
-                ("low_battery",       c_uint16, 1 ),
-                ("armed_stay",       c_uint16, 1 )
-               ]
 
-class IconLED_Flags( ctypes.Union ):
+class IconLED_Bitfield(ctypes.LittleEndianStructure):
     _fields_ = [
-                ("b",      IconLED_Bitfield ),
-                ("asShort", c_uint16    )
-               ]
-    _anonymous_ = ("b")
+        ("alarm", c_uint16, 1),
+        ("alarm_in_memory", c_uint16, 1),
+        ("armed_away", c_uint16, 1),
+        ("ac_present", c_uint16, 1),
+        ("bypass", c_uint16, 1),
+        ("chime", c_uint16, 1),
+        ("not_used1", c_uint16, 1),
+        ("armed_zero_entry_delay", c_uint16, 1),
+        ("alarm_fire_zone", c_uint16, 1),
+        ("system_trouble", c_uint16, 1),
+        ("not_used2", c_uint16, 1),
+        ("not_used3", c_uint16, 1),
+        ("ready", c_uint16, 1),
+        ("fire", c_uint16, 1),
+        ("low_battery", c_uint16, 1),
+        ("armed_stay", c_uint16, 1),
+    ]
+
+    def __str__(self) -> str:
+        b = bytes(self)
+        return f"{int((b[1] << 8) | b[0]):04x}"
+
+
+class IconLED_Flags(ctypes.Union):
+    _fields_ = [("b", IconLED_Bitfield), ("asShort", c_uint16)]
+    _anonymous_ = "b"
+
 
 evl_Commands = {
-    'KeepAlive' : '00',
-    'ChangeDefaultPartition' : '01',
-    'DumpZoneTimers' : '02',
-    'PartitionKeypress' : '03'
+    "KeepAlive": "00",
+    "ChangeDefaultPartition": "01",
+    "DumpZoneTimers": "02",
+    "PartitionKeypress": "03",
 }
 
-evl_PanicTypes = {
-    'Fire' : 'A',
-    'Ambulance' : 'B',
-    'Police' : 'C'
-}
+evl_PanicTypes = {"Fire": "A", "Ambulance": "B", "Police": "C"}
 
 evl_ResponseTypes = {
-    'Login:' :  {'name' : 'Login Prompt', 'description' : 'Sent During Session Login Only.', 'handler' : 'login'},
-    'OK' : {'name' : 'Login Success', 'description' : 'Send During Session Login Only, successful login', 'handler' : 'login_success'},
-    'FAILED' : {'name' : 'Login Failure', 'description' : 'Sent During Session Login Only, password not accepted', 'handler' : 'login_failure'},
-    'Timed Out!' : {'name' : 'Login Interaction Timed Out', 'description' : 'Sent during Session Login Only, socket connection is then closed', 'handler' : 'login_timeout'},
-    '%00' : {'name' : 'Virtual Keypad Update', 'description' : 'The panel wants to update the state of the keypad','handler' : 'keypad_update'},
-    '%01' : {'type' : 'zone', 'name' : 'Zone State Change', 'description' : 'A zone change-of-state has occurred', 'handler' : 'zone_state_change'},
-    '%02' : {'type' : 'partition', 'name' : 'Partition State Change', 'description' : 'A partition change-of-state has occured', 'handler' : 'partition_state_change'},
-    '%03' : {'type' : 'system', 'name' : 'Realtime CID Event', 'description' : 'A system event has happened that is signaled to either the Envisalerts servers or the central monitoring station', 'handler' : 'realtime_cid_event'},
-    '%FF' : {'name' : 'Envisalink Zone Timer Dump', 'description' : 'This command contains the raw zone timers used inside the Envisalink. The dump is a 256 character packed HEX string representing 64 UINT16 (little endian) zone timers. Zone timers count down from 0xFFFF (zone is open) to 0x0000 (zone is closed too long ago to remember). Each ''tick'' of the zone time is actually 5 seconds so a zone timer of 0xFFFE means ''5 seconds ago''. Remember, the zone timers are LITTLE ENDIAN so the above example would be transmitted as FEFF.', 'handler' : 'zone_timer_dump'},
-    '^00' : {'type' : 'envisalink', 'name': 'Poll', 'description' : 'Envisalink poll', 'handler' : 'poll_response'},
-    '^01' : {'type' : 'envisalink', 'name': 'Change Default Partition', 'description': 'Change the partition which keystrokes are sent to when using the virtual keypad.', 'handler' : 'command_response'},
-    '^02' : {'type' : 'envisalink', 'name': 'Dump Zone Timers', 'description' : 'This command contains the raw zone timers used inside the Envisalink. The dump is a 256 character packed HEX string representing 64 UINT16 (little endian) zone timers. Zone timers count down from 0xFFFF (zone is open) to 0x0000 (zone is closed too long ago to remember). Each ''tick'' of the zone time is actually 5 seconds so a zone timer of 0xFFFE means ''5 seconds ago''. Remember, the zone timers are LITTLE ENDIAN so the above example would be transmitted as FEFF.','handler' : 'command_response'},
-    '^03' : {'type' : 'envisalink', 'name': 'Keypress to Specific Partition', 'description' : 'This will send a keystroke to the panel from an arbitrary partition. Use this if you don''t want to change the TPI default partition.' ,'handler' : 'command_response'},
-    '^0C' : {'type' : 'envisalink', 'name': 'Response for Invalid Command', 'description' : 'This response is returned when an invalid command number is passed to Envisalink', 'handler': 'command_response'}
+    "Login:": {
+        "name": "Login Prompt",
+        "description": "Sent During Session Login Only.",
+        "handler": "login",
+    },
+    "OK": {
+        "name": "Login Success",
+        "description": "Send During Session Login Only, successful login",
+        "handler": "login_success",
+    },
+    "FAILED": {
+        "name": "Login Failure",
+        "description": "Sent During Session Login Only, password not accepted",
+        "handler": "login_failure",
+    },
+    "Timed Out!": {
+        "name": "Login Interaction Timed Out",
+        "description": "Sent during Session Login Only, socket connection is then closed",
+        "handler": "login_timeout",
+    },
+    "%00": {
+        "name": "Virtual Keypad Update",
+        "description": "The panel wants to update the state of the keypad",
+        "handler": "keypad_update",
+        "state_change": True,
+    },
+    "%01": {
+        "type": "zone",
+        "name": "Zone State Change",
+        "description": "A zone change-of-state has occurred",
+        "handler": "zone_state_change",
+        "state_change": True,
+    },
+    "%02": {
+        "type": "partition",
+        "name": "Partition State Change",
+        "description": "A partition change-of-state has occured",
+        "handler": "partition_state_change",
+        "state_change": True,
+    },
+    "%03": {
+        "type": "system",
+        "name": "Realtime CID Event",
+        "description": "A system event has happened that is signaled to either the Envisalerts servers or the central monitoring station",  # noqa: E501
+        "handler": "realtime_cid_event",
+    },
+    "%FF": {
+        "name": "Envisalink Zone Timer Dump",
+        "description": "This command contains the raw zone timers used inside the Envisalink. The dump is a 256 character packed HEX string representing 64 UINT16 (little endian) zone timers. Zone timers count down from 0xFFFF (zone is open) to 0x0000 (zone is closed too long ago to remember). Each 'tick' of the zone time is actually 5 seconds so a zone timer of 0xFFFE means '5 seconds ago'. Remember, the zone timers are LITTLE ENDIAN so the above example would be transmitted as FEFF.",  # noqa: E501
+        "handler": "zone_timer_dump",
+        "state_change": True,
+    },
+    "^00": {
+        "type": "envisalink",
+        "name": "Poll",
+        "description": "Envisalink poll",
+        "handler": "command_response",
+    },
+    "^01": {
+        "type": "envisalink",
+        "name": "Change Default Partition",
+        "description": "Change the partition which keystrokes are sent to when using the virtual keypad.",  # noqa: E501
+        "handler": "command_response",
+    },
+    "^02": {
+        "type": "envisalink",
+        "name": "Dump Zone Timers",
+        "description": "This command contains the raw zone timers used inside the Envisalink. The dump is a 256 character packed HEX string representing 64 UINT16 (little endian) zone timers. Zone timers count down from 0xFFFF (zone is open) to 0x0000 (zone is closed too long ago to remember). Each 'tick' of the zone time is actually 5 seconds so a zone timer of 0xFFFE means '5 seconds ago'. Remember, the zone timers are LITTLE ENDIAN so the above example would be transmitted as FEFF.",  # noqa: E501
+        "handler": "command_response",
+    },
+    "^03": {
+        "type": "envisalink",
+        "name": "Keypress to Specific Partition",
+        "description": "This will send a keystroke to the panel from an arbitrary partition. Use this if you don't want to change the TPI default partition.",  # noqa: E501
+        "handler": "command_response",
+    },
+    "^0C": {
+        "type": "envisalink",
+        "name": "Response for Invalid Command",
+        "description": "This response is returned when an invalid command number is passed to Envisalink",  # noqa: E501
+        "handler": "command_response",
+    },
 }
 
 evl_TPI_Response_Codes = {
-    '00' : 'Command Accepted',
-    '01' : 'Receive Buffer Overrun (a command is received while another is still being processed)',
-    '02' : 'Unknown Command',
-    '03' : 'Syntax Error. Data appended to the command is incorrect in some fashion',
-    '04' : 'Receive Buffer Overflow',
-    '05' : 'Receive State Machine Timeout (command not completed within 3 seconds)'
+    "00": {"retry": False, "msg": "Command Accepted"},
+    "01": {
+        "retry": True,
+        "msg": "Receive Buffer Overrun (a command is received while another is still being processed)",  # noqa: E501
+    },
+    "02": {"retry": False, "msg": "Unknown Command"},
+    "03": {
+        "retry": False,
+        "msg": "Syntax Error. Data appended to the command is incorrect in some fashion",
+    },
+    "04": {"retry": True, "msg": "Receive Buffer Overflow"},
+    "05": {
+        "retry": False,
+        "msg": "Receive State Machine Timeout (command not completed within 3 seconds)",
+    },
 }
 evl_Partition_Status_Codes = {
-    '00' : {'name' : 'NOT_USED', 'description' : 'Partition is not used or doesn''t exist'},
-    '01' : {'name' : 'READY', 'description' : 'Ready', 'pluginhandler' : 'disarmed'},
-    '02' : {'name' : 'READY_BYPASS', 'description' : 'Ready to Arm (Zones are Bypasses)', 'pluginhandler' : 'disarmed'},
-    '03' : {'name' : 'NOT_READY', 'description' : 'Not Ready', 'pluginhandler' : 'disarmed'},
-    '04' : {'name' : 'ARMED_STAY', 'description' : 'Armed in Stay Mode', 'pluginhandler' : 'armedHome'},
-    '05' : {'name' : 'ARMED_AWAY', 'description' : 'Armed in Away Mode', 'pluginhandler' : 'armedAway'},
-    '06' : {'name' : 'ARMED_MAX', 'description' : 'Armed in Away Mode', 'pluginhandler' : 'armedInstant'},
-    '07' : {'name' : 'EXIT_ENTRY_DELAY', 'description' : 'Entry or Exit Delay'},
-    '08' : {'name' : 'IN_ALARM', 'description' : 'Partition is in Alarm', 'pluginhandler' : 'alarmTriggered'},
-    '09' : {'name' : 'ALARM_IN_MEMORY', 'description' : 'Alarm Has Occurred (Alarm in Memory)', 'pluginhandler' : 'alarmCleared'}
+    "00": {
+        "name": "NOT_USED",
+        "description": "Partition is not used or doesn" "t exist",
+    },
+    "01": {"name": "READY", "description": "Ready", "pluginhandler": "disarmed"},
+    "02": {
+        "name": "READY_BYPASS",
+        "description": "Ready to Arm (Zones are Bypasses)",
+        "pluginhandler": "disarmed",
+    },
+    "03": {
+        "name": "NOT_READY",
+        "description": "Not Ready",
+        "pluginhandler": "disarmed",
+    },
+    "04": {
+        "name": "ARMED_STAY",
+        "description": "Armed in Stay Mode",
+        "pluginhandler": "armedHome",
+    },
+    "05": {
+        "name": "ARMED_AWAY",
+        "description": "Armed in Away Mode",
+        "pluginhandler": "armedAway",
+    },
+    "06": {
+        "name": "ARMED_MAX",
+        "description": "Armed in Away Mode",
+        "pluginhandler": "armedInstant",
+    },
+    "07": {"name": "EXIT_ENTRY_DELAY", "description": "Entry or Exit Delay"},
+    "08": {
+        "name": "IN_ALARM",
+        "description": "Partition is in Alarm",
+        "pluginhandler": "alarmTriggered",
+    },
+    "09": {
+        "name": "ALARM_IN_MEMORY",
+        "description": "Alarm Has Occurred (Alarm in Memory)",
+        "pluginhandler": "alarmCleared",
+    },
 }
 
 evl_Virtual_Keypad_How_To_Beep = {
-    '00' : 'off',
-    '01' : 'beep 1 time',
-    '02' : 'beep 2 times',
-    '03' : 'beep 3 times',
-    '04' : 'continous fast beep',
-    '05' : 'continuous slow beep'
+    "00": "off",
+    "01": "beep 1 time",
+    "02": "beep 2 times",
+    "03": "beep 3 times",
+    "04": "continous fast beep",
+    "05": "continuous slow beep",
 }
 
 evl_CID_Qualifiers = {
-    1 : 'New Event or Opening',
-    3 : 'New Restore or Closing',
-    6 : 'Previously Reported Condition Still Present'
+    1: "New Event or Opening",
+    3: "New Restore or Closing",
+    6: "Previously Reported Condition Still Present",
 }
 
 evl_ArmDisarm_CIDs = [401, 403, 407, 408, 409, 441, 442]
 
 evl_CID_Events = {
-    100 : {
-    "label" : "Medical Alert",
-    "type"  : "zone",
-    },
-    101 : {
-    "label" : "Personal Emergency",
-    "type"  : "zone",
-    },
-    102 : {
-    "label" : "Failure to Report In",
-    "type"  : "zone",
-    },
-    110 : {
-    "label" : "Fire Alarm",
-    "type"  : "zone",
-    },
-    111 : {
-    "label" : "Smoke Alarm",
-    "type"  : "zone",
-    },
-    112 : {
-    "label" : "Combustion Detected Alarm",
-    "type"  : "zone",
-    },
-    113 : {
-    "label" : "Water Flood Alarm",
-    "type"  : "zone",
-    },
-    114 : {
-    "label" : "Excessive Heat Alarm",
-    "type"  : "zone",
-    },
-    115 : {
-    "label" : "Fire Alarm Pulled",
-    "type"  : "zone",
-    },
-    116 : {
-    "label" : "Duct Alarm",
-    "type"  : "zone",
-    },
-    117 : {
-    "label" : "Flame Detected",
-    "type"  : "zone",
-    },
-    118 : {
-    "label" : "Near Alarm",
-    "type"  : "zone",
-    },
-    120 : {
-    "label" : "Panic Alarm",
-    "type"  : "zone",
-    },
-    121 : {
-    "label" : "Duress Alarm",
-    "type"  : "user",
-    },
-    122 : {
-    "label" : "Alarm, 24-hour Silent",
-    "type"  : "zone",
-    },
-    123 : {
-    "label" : "Alarm, 24-hour Audible",
-    "type"  : "zone",
-    },
-    124 : {
-    "label" : "Duress - Access granted",
-    "type"  : "zone",
-    },
-    125 : {
-    "label" : "Duress - Egress granted",
-    "type"  : "zone",
-    },
-    130 : {
-    "label" : "Burgalry in Progress",
-    "type"  : "zone",
-    },
-    131 : {
-    "label" : "Alarm, Perimeter",
-    "type"  : "zone",
-    },
-    132 : {
-    "label" : "Alarm, Interior",
-    "type"  : "zone",
-    },
-    133 : {
-    "label" : "24 Hour (Safe)",
-    "type"  : "zone",
-    },
-    134 : {
-    "label" : "Alarm, Entry/Exit",
-    "type"  : "zone",
-    },
-    135 : {
-    "label" : "Alarm, Day/Night",
-    "type"  : "zone",
-    },
-    136 : {
-    "label" : "Alarm, Outdoor",
-    "type"  : "zone",
-    },
-    137 : {
-    "label" : "Alarm, Tamper",
-    "type"  : "zone",
-    },
-    138 : {
-    "label" : "Near Alarm",
-    "type"  : "zone",
-    },
-    139 : {
-    "label" : "Intrusion Verifier",
-    "type"  : "zone",
-    },
-    140 : {
-    "label" : "Alarm, General Alarm",
-    "type"  : "zone",
-    },
-    141 : {
-    "label" : "Alarm, Polling Loop Open",
-    "type"  : "zone",
-    },
-    142 : {
-    "label" : "Alarm, Polling Loop Short",
-    "type"  : "zone",
-    },
-    143 : {
-    "label" : "Alarm, Expansion Module",
-    "type"  : "zone",
-    },
-    144 : {
-    "label" : "Alarm, Sensor Tamper",
-    "type"  : "zone",
-    },
-    145 : {
-    "label" : "Alarm, Expansion Module Tamper",
-    "type"  : "zone",
-    },
-    146 : {
-    "label" : "Silent Burglary",
-    "type"  : "zone",
-    },
-    147 : {
-    "label" : "Sensor Supervision failure",
-    "type"  : "zone",
-    },
-    150 : {
-    "label" : "Alarm, 24-Hour Auxiliary",
-    "type"  : "zone",
-    },
-    151 : {
-    "label" : "Alarm, Gas detected",
-    "type"  : "zone",
-    },
-    152 : {
-    "label" : "Alarm, Refrigeration",
-    "type"  : "zone",
-    },
-    153 : {
-    "label" : "Alarm, Loss of heat",
-    "type"  : "zone",
-    },
-    154 : {
-    "label" : "Alarm, Water leakage",
-    "type"  : "zone",
-    },
-    155 : {
-    "label" : "Alarm, foil break",
-    "type"  : "zone",
-    },
-    156 : {
-    "label" : "Day trouble",
-    "type"  : "zone",
-    },
-    157 : {
-    "label" : "Low bottled gas level",
-    "type"  : "zone",
-    },
-    158 : {
-    "label" : "Alarm, High temperature",
-    "type"  : "zone",
-    },
-    159 : {
-    "label" : "Alarm, Low temperature",
-    "type"  : "zone",
-    },
-    161 : {
-    "label" : "Alarm, Loss of air flow",
-    "type"  : "zone",
-    },
-    162 : {
-    "label" : "Alarm, Carbon Monoxide Detected",
-    "type"  : "zone",
-    },
-    163 : {
-    "label" : "Alarm, Tank Level",
-    "type"  : "zone",
-    },
-
-    300 : {
-    "label" : "System Trouble",
-    "type"  : "zone",
-    },
-    301 : {
-    "label" : "AC Power",
-    "type"  : "zone",
-    },
-    302 : {
-    "label" : "Low System Battery/Battery Test Fail",
-    "type"  : "zone",
-    },
-    303 : {
-    "label" : "RAM Checksum Bad",
-    "type"  : "zone",
-    },
-    304 : {
-    "label" : "ROM Checksum Bad",
-    "type"  : "zone",
-    },
-    305 : {
-    "label" : "System Reset",
-    "type"  : "zone",
-    },
-    306 : {
-    "label" : "Panel programming changed",
-    "type"  : "zone",
-    },
-    307 : {
-    "label" : "Self-test failure",
-    "type"  : "zone",
-    },
-    308 : {
-    "label" : "System shutdown",
-    "type"  : "zone",
-    },
-    309 : {
-    "label" : "Battery test failure",
-    "type"  : "zone",
-    },
-    310 : {
-    "label" : "Ground fault",
-    "type"  : "zone",
-    },
-    311 : {
-    "label" : "Battery Missing/Dead",
-    "type"  : "zone",
-    },
-    312 : {
-    "label" : "Power Supply Overcurrent",
-    "type"  : "zone",
-    },
-    313 : {
-    "label" : "Engineer Reset",
-    "type"  : "user",
-    },
-    321 : {
-    "label" : "Bell/Siren Trouble",
-    "type"  : "zone",
-    },
-    333 : {
-    "label" : "Trouble or Tamper Expansion Module",
-    "type"  : "zone",
-    },
-    341 : {
-    "label" : "Trouble, ECP Cover Tamper",
-    "type"  : "zone",
-    },
-    344 : {
-    "label" : "RF Receiver Jam",
-    "type"  : "zone",
-    },
-    351 : {
-    "label" : "Telco Line Fault",
-    "type"  : "zone",
-    },
-    353 : {
-    "label" : "Long Range Radio Trouble",
-    "type"  : "zone",
-    },
-    373 : {
-    "label" : "Fire Loop Trouble",
-    "type"  : "zone",
-    },
-    374 : {
-    "label" : "Exit Error Alarm",
-    "type"  : "zone",
-    },
-    380 : {
-    "label" : "Global Trouble, Trouble Day/Night",
-    "type"  : "zone",
-    },
-    381 : {
-    "label" : "RF Supervision Trouble",
-    "type"  : "zone",
-    },
-    382 : {
-    "label" : "Supervision Auxillary Wire Zone",
-    "type"  : "zone",
-    },
-    383 : {
-    "label" : "RF Sensor Tamper",
-    "type"  : "zone",
-    },
-    384 : {
-    "label" : "RF Sensor Low Battery",
-    "type"  : "zone",
-    },
-    393 : {
-    "label" : "Clean Me",
-    "type"  : "zone",
-    },
-
-    401 : {
-    "label" : "AWAY/MAX",
-    "type"  : "user",
-    },
-    403 : {
-    "label" : "Scheduled Arming",
-    "type"  : "user",
-    },
-    406 : {
-    "label" : "Cancel by User",
-    "type"  : "user",
-    },
-    407 : {
-    "label" : "Remote Arm/Disarm (Downloading)",
-    "type"  : "user",
-    },
-    408 : {
-    "label" : "Quick AWAY/MAX",
-    "type"  : "user",
-    },
-    409 : {
-    "label" : "AWAY/MAX Keyswitch",
-    "type"  : "user",
-    },
-    411 : {
-    "label" : "Callback Requested",
-    "type"  : "user",
-    },
-    412 : {
-    "label" : "Success-Download/Access",
-    "type"  : "user",
-    },
-    413 : {
-    "label" : "Unsuccessful Access",
-    "type"  : "user",
-    },
-    414 : {
-    "label" : "System Shutdown",
-    "type"  : "user",
-    },
-    415 : {
-    "label" : "Dialer Shutdown",
-    "type"  : "user",
-    },
-    416 : {
-    "label" : "Successful Upload",
-    "type"  : "user",
-    },
-    421 : {
-    "label" : "Access Denied",
-    "type"  : "user",
-    },
-    422 : {
-    "label" : "Access Granted",
-    "type"  : "user",
-    },
-    423 : {
-    "label" : "PANIC Forced Access",
-    "type"  : "zone",
-    },
-    424 : {
-    "label" : "Egress Denied",
-    "type"  : "user",
-    },
-    425 : {
-    "label" : "Egress Granted",
-    "type"  : "user",
-    },
-    426 : {
-    "label" : "Access Door Propped Open",
-    "type"  : "zone",
-    },
-    427 : {
-    "label" : "Access Point DSM Trouble",
-    "type"  : "zone",
-    },
-    428 : {
-    "label" : "Access Point RTE Trouble",
-    "type"  : "zone",
-    },
-    429 : {
-    "label" : "Access Program Mode Entry",
-    "type"  : "user",
-    },
-    430 : {
-    "label" : "Access Program Mode Exit",
-    "type"  : "user",
-    },
-    431 : {
-    "label" : "Access Threat Level Change",
-    "type"  : "user",
-    },
-    432 : {
-    "label" : "Access Relay/Triger Failure",
-    "type"  : "zone",
-    },
-    433 : {
-    "label" : "Access RTE Shunt",
-    "type"  : "zone",
-    },
-    434 : {
-    "label" : "Access DSM Shunt",
-    "type"  : "zone",
-    },
-    441 : {
-    "label" : "STAY/INSTANT",
-    "type"  : "user",
-    },
-    442 : {
-    "label" : "STAY/INSTANT Keyswitch",
-    "type"  : "user",
-    },
-
-    570 : {
-    "label" : "Zone Bypass",
-    "type"  : "zone",
-    },
-
-    574 : {
-    "label" : "Group Bypass",
-    "type"  : "user"
-    },
-
-    601 : {
-    "label" : "Operator Initiated Dialer Test",
-    "type"  : "user",
-    },
-    602 : {
-    "label" : "Periodic Test",
-    "type"  : "zone",
-    },
-    606 : {
-    "label" : "AAV to follow",
-    "type"  : "zone",
-    },
-    607 : {
-    "label" : "Walk Test",
-    "type"  : "user",
-    },
-    623 : {
-    "label" : "Event Log 80% Full",
-    "type"  : "zone",
-    },
-    625 : {
-    "label" : "Real-Time Clock Changed",
-    "type"  : "user",
-    },
-    627 : {
-    "label" : "Program Mode Entry",
-    "type"  : "zone",
-    },
-    628 : {
-    "label" : "Program Mode Exit",
-    "type"  : "zone",
-    },
-    629 : {
-    "label" : "1-1/3 Day No Event",
-    "type"  : "zone",
-    },
-    642 : {
-    "label" : "Latch Key",
-    "type"  : "user",
-    },
-    750 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    751 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    752 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    753 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    754 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    755 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    756 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    757 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    758 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    759 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    760 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    761 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    762 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    763 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    764 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    765 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    766 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    767 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    768 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    769 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    770 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    771 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    772 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    773 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    774 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    775 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    776 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    777 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    778 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    779 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    780 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    781 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    782 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    783 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    784 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    785 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    786 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    787 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    788 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
-    },
-    789 : {
-    "label" : "Configurable Zone Type",
-    "type"  : "zone",
+    100: {
+        "label": "Medical Alert",
+        "type": "zone",
+    },
+    101: {
+        "label": "Personal Emergency",
+        "type": "zone",
+    },
+    102: {
+        "label": "Failure to Report In",
+        "type": "zone",
+    },
+    110: {
+        "label": "Fire Alarm",
+        "type": "zone",
+    },
+    111: {
+        "label": "Smoke Alarm",
+        "type": "zone",
+    },
+    112: {
+        "label": "Combustion Detected Alarm",
+        "type": "zone",
+    },
+    113: {
+        "label": "Water Flood Alarm",
+        "type": "zone",
+    },
+    114: {
+        "label": "Excessive Heat Alarm",
+        "type": "zone",
+    },
+    115: {
+        "label": "Fire Alarm Pulled",
+        "type": "zone",
+    },
+    116: {
+        "label": "Duct Alarm",
+        "type": "zone",
+    },
+    117: {
+        "label": "Flame Detected",
+        "type": "zone",
+    },
+    118: {
+        "label": "Near Alarm",
+        "type": "zone",
+    },
+    120: {
+        "label": "Panic Alarm",
+        "type": "zone",
+    },
+    121: {
+        "label": "Duress Alarm",
+        "type": "user",
+    },
+    122: {
+        "label": "Alarm, 24-hour Silent",
+        "type": "zone",
+    },
+    123: {
+        "label": "Alarm, 24-hour Audible",
+        "type": "zone",
+    },
+    124: {
+        "label": "Duress - Access granted",
+        "type": "zone",
+    },
+    125: {
+        "label": "Duress - Egress granted",
+        "type": "zone",
+    },
+    130: {
+        "label": "Burgalry in Progress",
+        "type": "zone",
+    },
+    131: {
+        "label": "Alarm, Perimeter",
+        "type": "zone",
+    },
+    132: {
+        "label": "Alarm, Interior",
+        "type": "zone",
+    },
+    133: {
+        "label": "24 Hour (Safe)",
+        "type": "zone",
+    },
+    134: {
+        "label": "Alarm, Entry/Exit",
+        "type": "zone",
+    },
+    135: {
+        "label": "Alarm, Day/Night",
+        "type": "zone",
+    },
+    136: {
+        "label": "Alarm, Outdoor",
+        "type": "zone",
+    },
+    137: {
+        "label": "Alarm, Tamper",
+        "type": "zone",
+    },
+    138: {
+        "label": "Near Alarm",
+        "type": "zone",
+    },
+    139: {
+        "label": "Intrusion Verifier",
+        "type": "zone",
+    },
+    140: {
+        "label": "Alarm, General Alarm",
+        "type": "zone",
+    },
+    141: {
+        "label": "Alarm, Polling Loop Open",
+        "type": "zone",
+    },
+    142: {
+        "label": "Alarm, Polling Loop Short",
+        "type": "zone",
+    },
+    143: {
+        "label": "Alarm, Expansion Module",
+        "type": "zone",
+    },
+    144: {
+        "label": "Alarm, Sensor Tamper",
+        "type": "zone",
+    },
+    145: {
+        "label": "Alarm, Expansion Module Tamper",
+        "type": "zone",
+    },
+    146: {
+        "label": "Silent Burglary",
+        "type": "zone",
+    },
+    147: {
+        "label": "Sensor Supervision failure",
+        "type": "zone",
+    },
+    150: {
+        "label": "Alarm, 24-Hour Auxiliary",
+        "type": "zone",
+    },
+    151: {
+        "label": "Alarm, Gas detected",
+        "type": "zone",
+    },
+    152: {
+        "label": "Alarm, Refrigeration",
+        "type": "zone",
+    },
+    153: {
+        "label": "Alarm, Loss of heat",
+        "type": "zone",
+    },
+    154: {
+        "label": "Alarm, Water leakage",
+        "type": "zone",
+    },
+    155: {
+        "label": "Alarm, foil break",
+        "type": "zone",
+    },
+    156: {
+        "label": "Day trouble",
+        "type": "zone",
+    },
+    157: {
+        "label": "Low bottled gas level",
+        "type": "zone",
+    },
+    158: {
+        "label": "Alarm, High temperature",
+        "type": "zone",
+    },
+    159: {
+        "label": "Alarm, Low temperature",
+        "type": "zone",
+    },
+    161: {
+        "label": "Alarm, Loss of air flow",
+        "type": "zone",
+    },
+    162: {
+        "label": "Alarm, Carbon Monoxide Detected",
+        "type": "zone",
+    },
+    163: {
+        "label": "Alarm, Tank Level",
+        "type": "zone",
+    },
+    300: {
+        "label": "System Trouble",
+        "type": "zone",
+    },
+    301: {
+        "label": "AC Power",
+        "type": "zone",
+    },
+    302: {
+        "label": "Low System Battery/Battery Test Fail",
+        "type": "zone",
+    },
+    303: {
+        "label": "RAM Checksum Bad",
+        "type": "zone",
+    },
+    304: {
+        "label": "ROM Checksum Bad",
+        "type": "zone",
+    },
+    305: {
+        "label": "System Reset",
+        "type": "zone",
+    },
+    306: {
+        "label": "Panel programming changed",
+        "type": "zone",
+    },
+    307: {
+        "label": "Self-test failure",
+        "type": "zone",
+    },
+    308: {
+        "label": "System shutdown",
+        "type": "zone",
+    },
+    309: {
+        "label": "Battery test failure",
+        "type": "zone",
+    },
+    310: {
+        "label": "Ground fault",
+        "type": "zone",
+    },
+    311: {
+        "label": "Battery Missing/Dead",
+        "type": "zone",
+    },
+    312: {
+        "label": "Power Supply Overcurrent",
+        "type": "zone",
+    },
+    313: {
+        "label": "Engineer Reset",
+        "type": "user",
+    },
+    321: {
+        "label": "Bell/Siren Trouble",
+        "type": "zone",
+    },
+    333: {
+        "label": "Trouble or Tamper Expansion Module",
+        "type": "zone",
+    },
+    341: {
+        "label": "Trouble, ECP Cover Tamper",
+        "type": "zone",
+    },
+    344: {
+        "label": "RF Receiver Jam",
+        "type": "zone",
+    },
+    351: {
+        "label": "Telco Line Fault",
+        "type": "zone",
+    },
+    353: {
+        "label": "Long Range Radio Trouble",
+        "type": "zone",
+    },
+    373: {
+        "label": "Fire Loop Trouble",
+        "type": "zone",
+    },
+    374: {
+        "label": "Exit Error Alarm",
+        "type": "zone",
+    },
+    380: {
+        "label": "Global Trouble, Trouble Day/Night",
+        "type": "zone",
+    },
+    381: {
+        "label": "RF Supervision Trouble",
+        "type": "zone",
+    },
+    382: {
+        "label": "Supervision Auxillary Wire Zone",
+        "type": "zone",
+    },
+    383: {
+        "label": "RF Sensor Tamper",
+        "type": "zone",
+    },
+    384: {
+        "label": "RF Sensor Low Battery",
+        "type": "zone",
+    },
+    393: {
+        "label": "Clean Me",
+        "type": "zone",
+    },
+    401: {
+        "label": "AWAY/MAX",
+        "type": "user",
+    },
+    403: {
+        "label": "Scheduled Arming",
+        "type": "user",
+    },
+    406: {
+        "label": "Cancel by User",
+        "type": "user",
+    },
+    407: {
+        "label": "Remote Arm/Disarm (Downloading)",
+        "type": "user",
+    },
+    408: {
+        "label": "Quick AWAY/MAX",
+        "type": "user",
+    },
+    409: {
+        "label": "AWAY/MAX Keyswitch",
+        "type": "user",
+    },
+    411: {
+        "label": "Callback Requested",
+        "type": "user",
+    },
+    412: {
+        "label": "Success-Download/Access",
+        "type": "user",
+    },
+    413: {
+        "label": "Unsuccessful Access",
+        "type": "user",
+    },
+    414: {
+        "label": "System Shutdown",
+        "type": "user",
+    },
+    415: {
+        "label": "Dialer Shutdown",
+        "type": "user",
+    },
+    416: {
+        "label": "Successful Upload",
+        "type": "user",
+    },
+    421: {
+        "label": "Access Denied",
+        "type": "user",
+    },
+    422: {
+        "label": "Access Granted",
+        "type": "user",
+    },
+    423: {
+        "label": "PANIC Forced Access",
+        "type": "zone",
+    },
+    424: {
+        "label": "Egress Denied",
+        "type": "user",
+    },
+    425: {
+        "label": "Egress Granted",
+        "type": "user",
+    },
+    426: {
+        "label": "Access Door Propped Open",
+        "type": "zone",
+    },
+    427: {
+        "label": "Access Point DSM Trouble",
+        "type": "zone",
+    },
+    428: {
+        "label": "Access Point RTE Trouble",
+        "type": "zone",
+    },
+    429: {
+        "label": "Access Program Mode Entry",
+        "type": "user",
+    },
+    430: {
+        "label": "Access Program Mode Exit",
+        "type": "user",
+    },
+    431: {
+        "label": "Access Threat Level Change",
+        "type": "user",
+    },
+    432: {
+        "label": "Access Relay/Triger Failure",
+        "type": "zone",
+    },
+    433: {
+        "label": "Access RTE Shunt",
+        "type": "zone",
+    },
+    434: {
+        "label": "Access DSM Shunt",
+        "type": "zone",
+    },
+    441: {
+        "label": "STAY/INSTANT",
+        "type": "user",
+    },
+    442: {
+        "label": "STAY/INSTANT Keyswitch",
+        "type": "user",
+    },
+    570: {
+        "label": "Zone Bypass",
+        "type": "zone",
+    },
+    574: {"label": "Group Bypass", "type": "user"},
+    601: {
+        "label": "Operator Initiated Dialer Test",
+        "type": "user",
+    },
+    602: {
+        "label": "Periodic Test",
+        "type": "zone",
+    },
+    606: {
+        "label": "AAV to follow",
+        "type": "zone",
+    },
+    607: {
+        "label": "Walk Test",
+        "type": "user",
+    },
+    623: {
+        "label": "Event Log 80% Full",
+        "type": "zone",
+    },
+    625: {
+        "label": "Real-Time Clock Changed",
+        "type": "user",
+    },
+    627: {
+        "label": "Program Mode Entry",
+        "type": "zone",
+    },
+    628: {
+        "label": "Program Mode Exit",
+        "type": "zone",
+    },
+    629: {
+        "label": "1-1/3 Day No Event",
+        "type": "zone",
+    },
+    642: {
+        "label": "Latch Key",
+        "type": "user",
+    },
+    750: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    751: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    752: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    753: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    754: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    755: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    756: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    757: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    758: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    759: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    760: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    761: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    762: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    763: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    764: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    765: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    766: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    767: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    768: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    769: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    770: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    771: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    772: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    773: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    774: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    775: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    776: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    777: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    778: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    779: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    780: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    781: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    782: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    783: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    784: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    785: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    786: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    787: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    788: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
+    },
+    789: {
+        "label": "Configurable Zone Type",
+        "type": "zone",
     },
 }
```

### Comparing `pyenvisalink-4.7/setup.py` & `pyenvisalink-5.0.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 from setuptools import setup
 
 setup(
     name="pyenvisalink",
-    version="4.7",
+    version="5.0.0b1",
     description=(
         "A python3 library for running asynchronus communications with envisalink "
         "alarm control panel modules."
     ),
     long_description=(
         "A python3 library for running asynchronus communications with envisalink "
         "alarm control panel modules."
```

