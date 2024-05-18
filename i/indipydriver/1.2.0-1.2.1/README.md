# Comparing `tmp/indipydriver-1.2.0.tar.gz` & `tmp/indipydriver-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipydriver-1.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipydriver-1.2.0.tar` & `indipydriver-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.2.0/LICENSE
--rw-r--r--   0        0        0     2469 2024-04-18 11:52:22.000000 indipydriver-1.2.0/README.md
--rw-r--r--   0        0        0      573 2024-04-17 19:58:31.000000 indipydriver-1.2.0/indipydriver/__init__.py
--rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.2.0/indipydriver/comms.py
--rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.2.0/indipydriver/events.py
--rw-r--r--   0        0        0    21349 2024-04-05 12:04:08.000000 indipydriver-1.2.0/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    11951 2024-04-18 08:46:27.000000 indipydriver-1.2.0/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.2.0/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.2.0/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2024-04-17 19:57:42.000000 indipydriver-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 indipydriver-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2469 2024-04-18 11:52:22.000000 indipydriver-1.2.1/README.md
+-rw-r--r--   0        0        0      573 2024-05-18 22:07:32.000000 indipydriver-1.2.1/indipydriver/__init__.py
+-rw-r--r--   0        0        0    21484 2024-05-18 21:58:43.000000 indipydriver-1.2.1/indipydriver/comms.py
+-rw-r--r--   0        0        0    24981 2024-05-16 20:54:58.000000 indipydriver-1.2.1/indipydriver/events.py
+-rw-r--r--   0        0        0    21236 2024-05-16 20:30:24.000000 indipydriver-1.2.1/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    11494 2024-05-18 21:50:05.000000 indipydriver-1.2.1/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    12256 2024-05-16 20:34:45.000000 indipydriver-1.2.1/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    43286 2024-04-25 22:33:51.000000 indipydriver-1.2.1/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2024-05-18 22:07:10.000000 indipydriver-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 indipydriver-1.2.1/PKG-INFO
```

### Comparing `indipydriver-1.2.0/LICENSE` & `indipydriver-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.0/README.md` & `indipydriver-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-1.2.0/indipydriver/__init__.py` & `indipydriver-1.2.1/indipydriver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.2.0"
+version = "1.2.1"
```

### Comparing `indipydriver-1.2.0/indipydriver/comms.py` & `indipydriver-1.2.1/indipydriver/comms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
-import asyncio, sys, os, time
+import asyncio, sys, os, time, copy
 
 import xml.etree.ElementTree as ET
 
 import fcntl
 
 from base64 import standard_b64encode
 
+import logging
+logger = logging.getLogger(__name__)
 
 # All xml data received from the client, or from snooped devices should be contained in one of the following tags
 TAGS = (b'getProperties',
         b'newTextVector',
         b'newNumberVector',
         b'newSwitchVector',
         b'newBLOBVector',
@@ -76,63 +78,81 @@
 
 
 class STDOUT_TX:
     "An object that transmits data on stdout, used by STDINOUT as one half of the communications path"
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on stdout"""
+        if logger.isEnabledFor(logging.DEBUG):
+            logenabled = True
+        else:
+            logenabled = False
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit down stdout
             txdata = await writerque.get()
             writerque.task_done()
             if (txdata.tag == "setBLOBVector") and len(txdata):
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # transmit the data
                     sys.stdout.buffer.write(binarydata)
                     sys.stdout.buffer.flush()
                     await asyncio.sleep(0)
+                if logenabled:
+                    copytx = copy.deepcopy(txdata)
+                    for element in copytx:
+                        element.text = "NOT LOGGED"
+                    binarydata = ET.tostring(copytx)
+                    logger.debug(f"TX:{binarydata.decode('utf-8')}")
             else:
                 # its straight xml, send it out on stdout
                 binarydata = ET.tostring(txdata)
                 binarydata += b"\n"
                 sys.stdout.buffer.write(binarydata)
                 sys.stdout.buffer.flush()
+                if logenabled:
+                    logger.debug(f"TX:{binarydata.decode('utf-8')}")
 
 
 class STDIN_RX:
     """An object that receives data, parses it to ElementTree elements
        and passes it to the driver by appending it to the driver's readerque"""
 
     async def run_rx(self, readerque):
         "pass data to readerque"
         source = self.datasource()
-        while True:
-            await asyncio.sleep(0)
-            if readerque is None:
-                continue
+        if logger.isEnabledFor(logging.DEBUG):
+            logenabled = True
+        else:
+            logenabled = False
+        async for rxdata in source:
             # get block of xml.etree.ElementTree data
             # from source and append it to  readerque
-            rxdata = await anext(source)
-            if rxdata is not None:
-                await readerque.put(rxdata)
+            await readerque.put(rxdata)
+            if logenabled:
+                if (rxdata.tag == "setBLOBVector" or rxdata.tag == "newBLOBVector") and len(rxdata):
+                    # rxdata contains blobs
+                    copyrx = copy.deepcopy(rxdata)
+                    for element in copyrx:
+                        element.text = "NOT LOGGED"
+                    binarydata = ET.tostring(copyrx)
+                    logger.debug(f"RX:{binarydata.decode('utf-8')}")
+                else:
+                    binarydata = ET.tostring(rxdata)
+                    logger.debug(f"RX:{binarydata.decode('utf-8')}")
+
 
     async def datasource(self):
         # get received data, parse it, and yield it as xml.etree.ElementTree object
         data_in = self.datainput()
         message = b''
         messagetagnumber = None
-        while True:
-            await asyncio.sleep(0)
-            # get blocks of data from stdin
-            data = await anext(data_in)
-            if not data:
-                continue
+        async for data in data_in:
             if not message:
                 # data is expected to start with <tag, first strip any newlines
                 data = data.strip()
                 for index, st in enumerate(_STARTTAGS):
                     if data.startswith(st):
                         messagetagnumber = index
                         break
@@ -211,26 +231,32 @@
         # Set stdin to non-blocking mode
         flags = fcntl.fcntl(sys.stdin.fileno(), fcntl.F_GETFL)
         fcntl.fcntl(sys.stdin.fileno(), fcntl.F_SETFL, flags | os.O_NONBLOCK)
 
         rx = STDIN_RX()
         tx = STDOUT_TX()
 
+        logger.warning("Listening on STDIN")
+
         await asyncio.gather(rx.run_rx(readerque),
                              tx.run_tx(writerque)
                              )
 
 class Port_TX():
     "An object that transmits data on a port, used by Portcomms as one half of the communications path"
 
     def __init__(self, blobstatus, writer, timer):
         self.blobstatus = blobstatus
         self.writer = writer
         self.timer = timer
-
+        self.addr = writer.get_extra_info('peername')
+        if logger.isEnabledFor(logging.DEBUG):
+            self.logenabled = True
+        else:
+            self.logenabled = False
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on the port writer"""
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit
             txdata = await writerque.get()
@@ -245,48 +271,67 @@
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # Send to the port
                     self.timer.update()
                     self.writer.write(binarydata)
                     await self.writer.drain()
+                if self.logenabled:
+                    copytx = copy.deepcopy(txdata)
+                    for element in copytx:
+                        element.text = "NOT LOGGED"
+                    binarydata = ET.tostring(copytx)
+                    logger.debug(f"TX:{self.addr}:{binarydata.decode('utf-8')}")
             else:
                 # its straight xml, send it out on the port
                 binarydata = ET.tostring(txdata)
+                if self.logenabled:
+                    logger.debug(f"TX:{self.addr}:{binarydata.decode('utf-8')}")
                 # Send to the port
                 self.timer.update()
                 self.writer.write(binarydata)
                 await self.writer.drain()
 
 
 class Port_RX(STDIN_RX):
     """Produces xml.etree.ElementTree data from data received on the port,
        this is used by Portcomms as one half of the communications path.
        This overwrites methods of the STDIN_RX parent class."""
 
-    def __init__(self, blobstatus, reader):
+    def __init__(self, blobstatus, reader, addr):
         self.blobstatus = blobstatus
         self.reader = reader
+        self.addr = addr
+        if logger.isEnabledFor(logging.DEBUG):
+            self.logenabled = True
+        else:
+            self.logenabled = False
 
     async def run_rx(self, readerque):
         "pass data to readerque"
         source = self.datasource()
-        while True:
-            await asyncio.sleep(0)
-            if readerque is None:
-                continue
+        async for rxdata in source:
             # get block of xml.etree.ElementTree data
             # from source and append it to  readerque
-            rxdata = await anext(source)
-            if rxdata is not None:
-                if rxdata.tag == "enableBLOB":
-                    # set permission flags in the blobstatus object
-                    self.blobstatus.setpermissions(rxdata)
-                # and place rxdata into readerque
-                await readerque.put(rxdata)
+            if rxdata.tag == "enableBLOB":
+                # set permission flags in the blobstatus object
+                self.blobstatus.setpermissions(rxdata)
+            # and place rxdata into readerque
+            await readerque.put(rxdata)
+            if self.logenabled:
+                if (rxdata.tag == "setBLOBVector" or rxdata.tag == "newBLOBVector") and len(rxdata):
+                    # rxdata contains blobs
+                    copyrx = copy.deepcopy(rxdata)
+                    for element in copyrx:
+                        element.text = "NOT LOGGED"
+                    binarydata = ET.tostring(copyrx)
+                    logger.debug(f"RX:{self.addr}:{binarydata.decode('utf-8')}")
+                else:
+                    binarydata = ET.tostring(rxdata)
+                    logger.debug(f"RX:{self.addr}:{binarydata.decode('utf-8')}")
 
 
     async def datainput(self):
         "Generator producing binary string of data from the port"
         binarydata = b""
         while True:
             await asyncio.sleep(0)
@@ -345,59 +390,61 @@
         # the connection
         self.timer = TXTimer(timeout = 15)
 
     async def __call__(self, readerque, writerque):
         "Called from indipydriver.asyncrun() to run the communications"
         self.readerque = readerque
         self.writerque = writerque
+        logger.warning(f"Listening on {self.host} : {self.port}")
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
-        try:
-            await server.serve_forever()
-        except KeyboardInterrupt as e:
-            server.close()
-            raise e
+        await server.serve_forever()
 
 
     async def _monitor_connection(self):
         """If connected and not transmitting, send def vectors every self.timeout seconds
            This ensures that if the connection has failed, due to the client disconnecting, the write
            to the port operation will cause a failure exception which will close the connection"""
         while True:
             await asyncio.sleep(5)
             # this is tested every five seconds
             if self.connected and self.writerque.empty() and self.readerque.empty():
                 # only need to test if the queue are empty
                 if self.timer.elapsed():
                     # no transmission in timeout seconds so send defVectors
                     for device in self.devices.values():
+                        if not device.enable:
+                            continue
                         for vector in device.values():
                             await vector.send_defVector()
 
 
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
         if self.connected:
             # already connected, can only handle one connection
             writer.close()
             await writer.wait_closed()
             return
         self.connected = True
-        rx = Port_RX(self.blobstatus, reader)
+        addr = writer.get_extra_info('peername')
+        rx = Port_RX(self.blobstatus, reader, addr)
         tx = Port_TX(self.blobstatus, writer, self.timer)
+        logger.info(f"Connection received from {addr}")
         try:
             txtask = asyncio.create_task(tx.run_tx(self.writerque))
             rxtask = asyncio.create_task(rx.run_rx(self.readerque))
             montask = asyncio.create_task(self._monitor_connection())
             await asyncio.gather(txtask, rxtask, montask)
         except Exception as e:
             self.connected = False
             txtask.cancel()
             rxtask.cancel()
             montask.cancel()
             cleanque(self.writerque)
+        logger.info(f"Connection from {addr} closed")
 
 
 def cleanque(que):
     "Clears out a que"
     try:
         while True:
             xmldata = que.get_nowait()
```

### Comparing `indipydriver-1.2.0/indipydriver/events.py` & `indipydriver-1.2.1/indipydriver/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                     remainder = remainder[:6]
                 remainder = int(remainder)
                 timestamp = datetime.fromisoformat(timestamp_string)
                 timestamp = timestamp.replace(microsecond=remainder, tzinfo=timezone.utc)
             else:
                 timestamp = datetime.fromisoformat(timestamp_string)
                 timestamp = timestamp.replace(tzinfo=timezone.utc)
-        except:
+        except Exception:
             timestamp = None
     else:
         timestamp = datetime.now(tz=timezone.utc)
     return timestamp
 
 
 class Event:
@@ -63,15 +63,15 @@
     def __init__(self, devicename, vectorname, vector, root):
         super().__init__(devicename, vectorname, vector, root)
         value = root.text.strip()
         if value in ("Never", "Also", "Only"):
             self.value = value
         else:
             # unrecognised value
-            raise EventException
+            raise EventException("Invalid value for enableBLOB")
 
 
 class newVector(Event, UserDict):
     "Parent to new vectors, adds dictionary and self.timestamp"
     def __init__(self, devicename, vectorname, vector, root):
         Event.__init__(self, devicename, vectorname, vector, root)
         UserDict.__init__(self)
@@ -95,21 +95,22 @@
                 if membername in self.vector:
                     value = member.text.strip()
                     if value == "On":
                         self.data[membername] = "On"
                     elif value == "Off":
                         self.data[membername] = "Off"
                     else:
-                        raise EventException
+                        raise EventException("Received invalid value for newSwitchVector")
                 else:
-                    raise EventException
+                    raise EventException("Received membername not known for newSwitchVector")
             else:
-                raise EventException
+                raise EventException("Received tag not known for newSwitchVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents received for newSwitchVector")
+
 
 class newTextVector(newVector):
     """An event indicating a newTextVector has been received, this is a mapping
        of membername:value, where each value is a text string"""
 
 
     def __init__(self, devicename, vectorname, vector, root):
@@ -117,19 +118,19 @@
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneText":
                 membername = member.get("name")
                 if membername in self.vector:
                     self.data[membername] = member.text
                 else:
-                    raise EventException
+                    raise EventException("Received membername not known for newTextVector")
             else:
-                raise EventException
+                raise EventException("Received tag not known for newTextVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents received for newTextVector")
 
 
 class newNumberVector(newVector):
     """An event indicating a newNumberVector has been received, this is a mapping
        of membername:value, where each value is a string number, which may be in
        sexagesimal format, and may have newlines appended or prepended. If desired,
        the driver method indi_number_to_float() can be used to convert this to a float."""
@@ -139,19 +140,19 @@
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneNumber":
                 membername = member.get("name")
                 if membername in self.vector:
                     self.data[membername] = member.text.strip()
                 else:
-                    raise EventException
+                    raise EventException("Received membername not known for newNumberVector")
             else:
-                raise EventException
+                raise EventException("Received tag not known for newNumberVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents received for newNumberVector")
 
 
 class newBLOBVector(newVector):
     """An event indicating a newBLOBVector has been received, this is a mapping
        of membername:value, where each value is a bytes string.
 
        This contains a further attribute 'sizeformat' which is a dictionary
@@ -167,26 +168,26 @@
         for member in root:
             if member.tag == "oneBLOB":
                 membername = member.get("name")
                 if membername in self.vector:
                     try:
                         self.data[membername] = standard_b64decode(member.text.encode('ascii'))
                         membersize = int(member.get("size"))
-                    except:
-                        raise EventException
+                    except Exception:
+                        raise EventException("Unable to decode BLOB")
                     memberformat = member.get("format")
                     if not memberformat:
-                        raise EventException
+                        raise EventException("No format received in oneBLOB")
                     self.sizeformat[membername] = (membersize, memberformat)
                 else:
-                    raise EventException
+                    raise EventException("Received tag not known for newBLOBVector")
             else:
-                raise EventException
+                raise EventException("Received tag not known for newBLOBVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents received for newBLOBVector")
 
 
 class SnoopEvent:
     "Parent class for snoop events"
     def __init__(self, root):
         self.devicename = root.get("device")
         self.root = root
@@ -207,34 +208,34 @@
     """The remote driver is instructing the client to delete either a device or a vector property.
        This contains attribute vectorname, if it is None, then the whole device is to be deleted.
        A 'message' attribute contains any message sent by the client with this instruction."""
 
     def __init__(self, root):
         super().__init__(root)
         if self.devicename is None:
-            raise EventException
+            raise EventException("No devicename given in snooped delProperty")
         self.vectorname = root.get("name")
         self.message = root.get("message", "")
 
 
 class defVector(SnoopEvent, UserDict):
     "Parent to def vectors, adds a mapping of membername:value"
     def __init__(self, root):
         SnoopEvent.__init__(self, root)
         UserDict.__init__(self)
         self.vectorname = root.get("name")
         if self.vectorname is None:
-            raise EventException
+            raise EventException("No vectorname given in snooped defVector")
         self.label = root.get("label", self.vectorname)
         self.group = root.get("group", "")
         state = root.get("state")
         if not state:
-            raise EventException
+            raise EventException("No state given in snooped defVector")
         if not state in ('Idle','Ok','Busy','Alert'):
-            raise EventException
+            raise EventException("Invalid state given in snooped defVector")
         self.state = state
         self.message = root.get("message", "")
 
     def __setitem__(self, membername):
         raise KeyError
 
 
@@ -244,119 +245,119 @@
        attributes perm, rule, timeout, and memberlabels which is a dictionary of
        membername:label."""
 
     def __init__(self, root):
         defVector.__init__(self, root)
         self.perm = root.get("perm")
         if self.perm is None:
-            raise EventException
+            raise EventException("No perm value given in snooped defSwitchVector")
         if self.perm not in ('ro', 'wo', 'rw'):
-            raise EventException
+            raise EventException("Invalid perm value given in snooped defSwitchVector")
         self.rule = root.get("rule")
         if self.rule is None:
-            raise EventException
+            raise EventException("No rule value given in snooped defSwitchVector")
         if self.rule not in ('OneOfMany', 'AtMostOne', 'AnyOfMany'):
-            raise EventException
+            raise EventException("Invalid rule value given in snooped defSwitchVector")
         self.timeout = root.get("timeout", "0")
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defSwitch":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped defSwitchVector")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
                 value = member.text.strip()
                 if value == "On":
                     self.data[membername] = "On"
                 elif value == "Off":
                     self.data[membername] = "Off"
                 else:
-                    raise EventException
+                    raise EventException("Invalid member value given in snooped defSwitchVector")
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped defSwitchVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped defSwitchVector")
 
 
 class defTextVector(defVector):
 
     """The remote driver has sent this to define a text vector property, it has further
        attributes perm, timeout, and memberlabels which is a dictionary of
        membername:label."""
 
     def __init__(self, root):
         defVector.__init__(self, root)
         self.perm = root.get("perm")
         if self.perm is None:
-            raise EventException
+            raise EventException("No perm value given in snooped defTextVector")
         if self.perm not in ('ro', 'wo', 'rw'):
-            raise EventException
+            raise EventException("Invalid perm value given in snooped defTextVector")
         self.timeout = root.get("timeout", "0")
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defText":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped defTextVector")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
                 self.data[membername] = member.text
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped defTextVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped defTextVector")
 
 
 class defNumberVector(defVector):
 
     """The remote driver has sent this to define a number vector property, it has further
        attributes perm, timeout, and memberlabels which is a dictionary of
        membername:(label, format, min, max, step)."""
 
     def __init__(self, root):
         defVector.__init__(self, root)
         self.perm = root.get("perm")
         if self.perm is None:
-            raise EventException
+            raise EventException("No perm value given in snooped defNumberVector")
         if self.perm not in ('ro', 'wo', 'rw'):
-            raise EventException
+            raise EventException("Invalid perm value given in snooped defNumberVector")
         self.timeout = root.get("timeout", "0")
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and
         # value being a tuple of (label, format, min, max, step)
         self.memberlabels = {}
         for member in root:
             if member.tag == "defNumber":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped defNumberVector")
                 label = member.get("label", membername)
                 memberformat = member.get("format")
                 if not memberformat:
-                    raise EventException
+                    raise EventException("No format string given in snooped defNumberVector")
                 membermin = member.get("min")
                 if not membermin:
-                    raise EventException
+                    raise EventException("No minimum given in snooped defNumberVector")
                 membermax = member.get("max")
                 if not membermax:
-                    raise EventException
+                    raise EventException("No maximum given in snooped defNumberVector")
                 memberstep = member.get("step")
                 if not memberstep:
-                    raise EventException
+                    raise EventException("No step given in snooped defNumberVector")
                 self.memberlabels[membername] = (label, memberformat, membermin, membermax, memberstep)
                 self.data[membername] = member.text.strip()
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped defNumberVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped defNumberVector")
 
 
 class defLightVector(defVector):
 
     """The remote driver has sent this to define a light vector property, it has further
        attribute memberlabels which is a dictionary of membername:label."""
 
@@ -365,83 +366,83 @@
         # create object dictionary of member name to value
         # and another dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defLight":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped defLightVector")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
                 value = member.text.strip()
                 if not value in ('Idle','Ok','Busy','Alert'):
-                    raise EventException
+                    raise EventException("Invalid value given in snooped defLightVector")
                 self.data[membername] = value
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped defLightVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped defLightVector")
 
 
 class defBLOBVector(SnoopEvent):
 
     """The remote driver has sent this to define a BLOB vector property, it has further
        attributes perm, timeout, and memberlabels which is a dictionary of
        membername:label.
 
        However this class does not have an object mapping of member name to value, since
        values are not given in defBLOBVectors"""
 
     def __init__(self, root):
         SnoopEvent.__init__(self, root)
         if self.devicename is None:
-            raise EventException
+            raise EventException("No devicename given in snooped defBLOBVector")
         self.vectorname = root.get("name")
         if self.vectorname is None:
-            raise EventException
+            raise EventException("No vectorname given in snooped defBLOBVector")
         self.label = root.get("label", self.vectorname)
         self.group = root.get("group", "")
         state = root.get("state")
         if not state:
-            raise EventException
+            raise EventException("No state given in snooped defBLOBVector")
         if not state in ('Idle','Ok','Busy','Alert'):
-            raise EventException
+            raise EventException("Invalid state given in snooped defBLOBVector")
         self.state = state
         self.message = root.get("message", "")
         self.perm = root.get("perm")
         if self.perm is None:
-            raise EventException
+            raise EventException("No perm value given in snooped defBLOBVector")
         if self.perm not in ('ro', 'wo', 'rw'):
-            raise EventException
+            raise EventException("Invalid perm value given in snooped defBLOBVector")
         self.timeout = root.get("timeout", "0")
         # create a dictionary of self.memberlabels with key member name and value being label
         self.memberlabels = {}
         for member in root:
             if member.tag == "defBLOB":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped defBLOBVector")
                 label = member.get("label", membername)
                 self.memberlabels[membername] = label
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped defBLOBVector")
         if not self.memberlabels:
-            raise EventException
+            raise EventException("No member labels given in snooped defBLOBVector")
 
 
 class setVector(SnoopEvent, UserDict):
     "Parent to set vectors, adds dictionary"
     def __init__(self, root):
         SnoopEvent.__init__(self, root)
         UserDict.__init__(self)
         if self.devicename is None:
-            raise EventException
+            raise EventException("No device name given in snooped setVector")
         self.vectorname = root.get("name")
         if self.vectorname is None:
-            raise EventException
+            raise EventException("No vector name given in snooped setVector")
         state = root.get("state")
         if state and (state in ('Idle','Ok','Busy','Alert')):
             self.state = state
         else:
             self.state = None
         self.message = root.get("message", "")
 
@@ -457,26 +458,26 @@
         setVector.__init__(self, root)
         self.timeout = root.get("timeout", "0")
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneSwitch":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped setSwitchVector")
                 value = member.text.strip()
                 if value == "On":
                     self.data[membername] = "On"
                 elif value == "Off":
                     self.data[membername] = "Off"
                 else:
-                    raise EventException
+                    raise EventException("Invalid value given in snooped setSwitchVector")
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped setSwitchVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped setSwitchVector")
 
 
 class setTextVector(setVector):
 
     """The remote driver is setting a Text vector property, this
        has further attribute timeout."""
 
@@ -484,20 +485,20 @@
         setVector.__init__(self, root)
         self.timeout = root.get("timeout", "0")
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneText":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped setTextVector")
                 self.data[membername] = member.text
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped setTextVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped setTextVector")
 
 
 class setNumberVector(setVector):
 
     """The remote driver is setting a Number vector property, this
        has further attribute timeout. The number values of the
        membername:membervalue are string values."""
@@ -506,41 +507,42 @@
         setVector.__init__(self, root)
         self.timeout = root.get("timeout", "0")
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneNumber":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped setNumberVector")
                 self.data[membername] = member.text.strip()
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped setNumberVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped setNumberVector")
+
 
 class setLightVector(setVector):
 
     """The remote driver is setting a Light vector property."""
 
     def __init__(self, root):
         setVector.__init__(self, root)
         # create a dictionary of member name to value
         for member in root:
             if member.tag == "oneLight":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
+                    raise EventException("No member name given in snooped setLightVector")
                 value = member.text.strip()
                 if not value in ('Idle','Ok','Busy','Alert'):
                     raise EventException
                 self.data[membername] = value
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped setLightVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped setLightVector")
 
 
 class setBLOBVector(setVector):
 
     """The remote driver is setting a BLOB vector property, this
        has further attributes timeout and sizeformat which is a dictionary
        of membername:(size, format)."""
@@ -552,24 +554,23 @@
         # and dictionary sizeformat
         # with key member name and value being a tuple of size, format
         self.sizeformat = {}
         for member in root:
             if member.tag == "oneBLOB":
                 membername = member.get("name")
                 if not membername:
-                    raise EventException
-                membersize = member.get("size")
-                if not membersize:
-                    raise EventException
+                    raise EventException("No member name given in snooped setBLOBVector")
+                if not member.get("size"):
+                    raise EventException("No member size given in snooped setBLOBVector")
                 memberformat = member.get("format")
                 if not memberformat:
-                    raise EventException
+                    raise EventException("No member format given in snooped setBLOBVector")
                 try:
                     self.data[membername] = standard_b64decode(member.text.encode('ascii'))
                     memberize = int(member.get("size"))
-                except:
-                    raise EventException
+                except Exception:
+                    raise EventException("Unable to decode snooped setBLOBVector")
                 self.sizeformat[membername] = (membersize, memberformat)
             else:
-                raise EventException
+                raise EventException("Invalid tag given in snooped setBLOBVector")
         if not self.data:
-            raise EventException
+            raise EventException("No contents given in snooped setBLOBVector")
```

### Comparing `indipydriver-1.2.0/indipydriver/ipydriver.py` & `indipydriver-1.2.1/indipydriver/ipydriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 import collections, asyncio, sys
 
 from datetime import datetime, timezone
 
 import xml.etree.ElementTree as ET
 
+import logging
+logger = logging.getLogger(__name__)
+
 from .comms import STDINOUT, Portcomms
 from . import events
 from .propertyvectors import timestamp_string
 
 
 class IPyDriver(collections.UserDict):
 
@@ -65,15 +68,15 @@
                 parts.append("0")
             assert len(parts) == 3
             # a part could be empty string, ie if 2:5: is given
             numbers = list(float(x) if x else 0.0 for x in parts)
             floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
             if negative:
                 floatvalue = -1 * floatvalue
-        except:
+        except Exception:
             raise TypeError("Error: Unable to parse number value")
         return floatvalue
 
 
     def __init__(self, devices, tasks=[], **driverdata):
         super().__init__()
 
@@ -111,18 +114,14 @@
         # initially the driver is not snooping anything, until it sends
         # a getProperties
         self.snoopall = False           # gets set to True if it is snooping everything
         self.snoopdevices = set()       # gets set to a set of device names
         self.snoopvectors = set()       # gets set to a set of (devicename,vectorname) tuples
 
 
-    def _reporterror(self, message):
-        "Prints message to stderr"
-        print(message, file=sys.stderr)
-
     def listen(self, host="localhost", port=7624):
         """If called, listens on the given host and port. Only one connection is accepted,
            further connection attempts while a client is already connected will be refused.
            This method also checks for enableBLOB instructions, and implements them.
            In general, using IPyServer is preferred."""
         if not self.comms is None:
              raise RuntimeError("A communications method has already been set, there can only be one")
@@ -186,15 +185,15 @@
             await asyncio.sleep(0)
             root = await self.snoopque.get()
             devicename = root.get("device")
             if devicename is not None:
                 # if a device name is given, check
                 # it is not in this drivers devices
                 if devicename in self.devices:
-                    self._reporterror("Cannot snoop on a device already controlled by this driver")
+                    logger.error("Cannot snoop on a device already controlled by this driver")
                     self.snoopque.task_done()
                     continue
             try:
                 if root.tag == "message":
                     # create event
                     event = events.message(root)
                     await self.snoopevent(event)
@@ -238,25 +237,25 @@
                     # create event
                     event = events.defBLOBVector(root)
                     await self.snoopevent(event)
                 elif root.tag == "setBLOBVector":
                     # create event
                     event = events.setBLOBVector(root)
                     await self.snoopevent(event)
-            except events.EventException:
+            except events.EventException as ex:
                 # if an EventException is raised, it is because received data is malformed
-                # so ignore it, and just pass
-                pass
+                # so log it
+                logger.error(str(ex))
             self.snoopque.task_done()
 
     async def send_message(self, message="", timestamp=None):
         "Send system wide message - without device name"
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("The timestamp given in send_message must be a datetime.datetime UTC object")
+            logger.error("The timestamp given in send_message must be a datetime.datetime UTC object")
             return
         xmldata = ET.Element('message')
         xmldata.set("timestamp", tstring)
         if message:
             xmldata.set("message", message)
         await self.send(xmldata)
 
@@ -267,15 +266,15 @@
         xmldata = ET.Element('getProperties')
         xmldata.set("version", "1.7")
         if devicename is None:
             await self.send(xmldata)
             self.snoopall = True
             return
         if devicename in self.devices:
-            self._reporterror("Cannot snoop on a device already controlled by this driver")
+            logger.error("Cannot snoop on a device already controlled by this driver")
             return
         xmldata.set("device", devicename)
         if vectorname is None:
             await self.send(xmldata)
             self.snoopdevices.add(devicename)
             return
         xmldata.set("name", vectorname)
@@ -311,14 +310,17 @@
            On receiving snoop data, this is called, and should handle
            any necessary actions.
            event is an object with attributes according to the data received."""
         pass
 
     async def asyncrun(self):
         """Gathers tasks to be run simultaneously"""
+
+        logger.warning(f"Driver {self.__class__.__name__} started")
+
         # set an object for communicating, as default this is stdin and stdout
         if self.comms is None:
             self.comms = STDINOUT()
 
         # get all tasks into a list
         self._tasks.append( self.comms(self.readerque, self.writerque) )    # run communications
         self._tasks.append( self.hardware() )                               # task to operate device hardware, and transmit updates
@@ -373,28 +375,24 @@
             p.devicename = self.devicename
             self.propertyvectors[p.name] = p
 
         self.data = self.propertyvectors
         # self.data is used by UserDict, it is an alias of self.propertyvectors
         # simply because 'propertyvectors' is more descriptive
 
-    def _reporterror(self, message):
-        "Prints message to stderr"
-        print(message, file=sys.stderr)
-
     async def send_device_message(self, message="", timestamp=None):
         """Send a message associated with this device, which the client could display.
            The timestamp should be either None or a datetime.datetime object. If the
            timestamp is None a UTC value will be inserted."""
         if not self.enable:
             # messages only sent if self.enable is True
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("The timestamp given in send_device_message must be a datetime.datetime UTC object")
+            logger.error("The timestamp given in send_device_message must be a datetime.datetime UTC object")
             return
         xmldata = ET.Element('message')
         xmldata.set("device", self.devicename)
         xmldata.set("timestamp", tstring)
         if message:
             xmldata.set("message", message)
         await self.driver.send(xmldata)
@@ -405,15 +403,15 @@
            False, which stops any data being transmitted between the client and this device.
            Setting device.enable to True re-enables communications.
            The message argument is any appropriate string which the client could display to the user.
            The timestamp should be either None or a datetime.datetime object. If the timestamp is None
            a UTC value will be inserted."""
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("The timestamp given in send_delProperty must be a datetime.datetime UTC object")
+            logger.error("The timestamp given in send_delProperty must be a datetime.datetime UTC object")
             return
         xmldata = ET.Element('delProperty')
         xmldata.set("device", self.devicename)
         xmldata.set("timestamp", tstring)
         if message:
             xmldata.set("message", message)
         await self.driver.send(xmldata)
```

### Comparing `indipydriver-1.2.0/indipydriver/ipyserver.py` & `indipydriver-1.2.1/indipydriver/ipyserver.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
 import collections, asyncio, sys
 
 import xml.etree.ElementTree as ET
 
 from functools import partialmethod
 
+import logging
+logger = logging.getLogger(__name__)
+
 from .ipydriver import IPyDriver
 
 from .comms import Port_RX, Port_TX, cleanque, BLOBSstatus, TXTimer
 
 
 class IPyServer:
 
@@ -65,22 +68,20 @@
             otherdrivers = [ d for d in drivers if not d is driver]
             driver.comms = _DriverComms(self.serverwriterque, self.connectionpool, otherdrivers)
 
         self.drivers = drivers
         self.host = host
         self.port = port
 
-    async def runserver(self):
+    async def _runserver(self):
         "Runs the server on the given host and port"
+        logger.warning(f"{self.__class__.__name__} listening on {self.host} : {self.port}")
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
-        try:
-            await server.serve_forever()
-        except KeyboardInterrupt as e:
-            server.close()
-            raise e
+        await server.serve_forever()
+
 
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
 
         for clientconnection in self.connectionpool:
             if not clientconnection.connected:
                 # this clientconnection is available
@@ -91,49 +92,48 @@
             writer.close()
             await writer.wait_closed()
 
     async def asyncrun(self):
         """Runs the server together with its drivers."""
         driverruns = [ driver.asyncrun() for driver in self.drivers ]
         await asyncio.gather(*driverruns,
-                             self.runserver(),
+                             self._runserver(),
                              self.copyreceivedtodriversrxque(),
                              self.copytransmittedtoclienttxque()
                              )
 
 
     async def copyreceivedtodriversrxque(self):
-        "For every driver, get rxque and copy data into it from serverreaderque"
+        "For every driver, get readerque and copy data into it from serverreaderque"
         while True:
             await asyncio.sleep(0)
             xmldata = await self.serverreaderque.get()
             devicename = xmldata.get("device")
             propertyname = xmldata.get("name")
             if devicename is None:
                 # if no devicename - goes to every driver (getproperties)
                 for driver in self.drivers:
-                    await driver.comms.rxque.put(xmldata)
+                    await driver.readerque.put(xmldata)
             elif devicename in self.devices:
                 # self.devices is a dictionary of device name to device
-                driver = self.devices[devicename].driver
-                # data is intended for this driver
-                await driver.comms.rxque.put(xmldata)
+                # data is intended for the driver this device belongs to
+                await self.devices[devicename].driver.readerque.put(xmldata)
             else:
                 # devicename is unknown, check if driver is snooping on this device, vector
                 for driver in self.drivers:
                     if driver.snoopall:
-                        await driver.comms.rxque.put(xmldata)
+                        await driver.readerque.put(xmldata)
                     elif devicename in driver.snoopdevices:
-                        await driver.comms.rxque.put(xmldata)
+                        await driver.readerque.put(xmldata)
                     elif not propertyname is None:
                         if (devicename, propertyname) in driver.snoopvectors:
-                            await driver.comms.rxque.put(xmldata)
+                            await driver.readerque.put(xmldata)
                     # else not snooping, so don't bother sending it to the driver
             self.serverreaderque.task_done()
-            # now every driver.comms object which needs it has this xmldata in its rxque
+            # now every driver which needs it has this xmldata in its readerque
 
 
     async def copytransmittedtoclienttxque(self):
         "For every clientconnection, get txque and copy data into it from serverwriterque"
         while True:
             await asyncio.sleep(0)
             xmldata = await self.serverwriterque.get()
@@ -144,73 +144,55 @@
             self.serverwriterque.task_done()
 
 
 
 class _DriverComms:
 
     """An instance of this is created for each driver, which calls the __call__
-       method, expecting xmldata to be received from the client and placed
-       in readerque, and any data the driver wishes to be sent should
-       be taken from the writerque and transmitted to the client by placing it
+       method.  Any data the driver wishes to be send will be taken
+       from the drivers writerque and transmitted to the client by placing it
        into the serverwriterque"""
 
     def __init__(self, serverwriterque, connectionpool, otherdrivers):
 
-        # self.rxque will have data received from the network
-        # inserted into it from the IPyServer.copyreceivedtodriversrxque()
-        # method
-        self.rxque = asyncio.Queue(6)
         self.serverwriterque = serverwriterque
         # connectionpool is a list of ClientConnection objects, which is used
         # to test if a client is connected
         self.connectionpool = connectionpool
         # self.connected is read by the driver, and in this case is always True
         # as the driver is connected to IPyServer, which handles snooping traffic,
         # even if no client is connected
         self.connected = True
         # self.otherdrivers is set to a list of drivers, not including the driver
         # this object is attached to.
         self.otherdrivers = otherdrivers
 
 
     async def __call__(self, readerque, writerque):
-        "Called by the driver, should run continuously to add and read the queues"
-        await asyncio.gather(self.handleread(readerque),
-                             self.handlewrite(writerque))
-
-    async def handleread(self, readerque):
-        "reads rxque, and sends xml data to the driver"
-        while True:
-            await asyncio.sleep(0)
-            xmldata = await self.rxque.get()
-            await readerque.put(xmldata)
-            # task completed
-            self.rxque.task_done()
-
-    async def handlewrite(self, writerque):
-        "reads writerque from the driver, and sends xml data to the network"
+        """Called by the driver, should run continuously.
+           reads writerque from the driver, and sends xml data to the network"""
         while True:
             await asyncio.sleep(0)
             xmldata = await writerque.get()
             # Check if other drivers wants to snoop this traffic
             devicename = xmldata.get("device")
             propertyname = xmldata.get("name")
             if devicename is None:
                 # if no devicename - goes to every other driver (getproperties)
                 for driver in self.otherdrivers:
-                    await driver.comms.rxque.put(xmldata)
+                    await driver.readerque.put(xmldata)
             else:
                 for driver in self.otherdrivers:
                     if driver.snoopall:
-                        await driver.comms.rxque.put(xmldata)
+                        await driver.readerque.put(xmldata)
                     elif devicename in driver.snoopdevices:
-                        await driver.comms.rxque.put(xmldata)
+                        await driver.readerque.put(xmldata)
                     elif not propertyname is None:
                         if (devicename, propertyname) in driver.snoopvectors:
-                            await driver.comms.rxque.put(xmldata)
+                            await driver.readerque.put(xmldata)
             # traffic from one driver has been sent to other drivers if they want to snoop
             # the traffic must also now be sent to the clients
             # If no clients are connected, do not put this data into
             # the serverwriterque
             for clientconnection in self.connectionpool:
                 if clientconnection.connected:
                     # at least one is connected, so this data is put into
@@ -252,29 +234,35 @@
             await asyncio.sleep(5)
             # this is tested every five seconds
             if self.connected and self.txque.empty():
                  # only need to test if the queue is empty
                 if self.timer.elapsed():
                     # no transmission in timeout seconds so send defVectors
                     for device in self.devices.values():
+                        if not device.enable:
+                            continue
                         for vector in device.values():
                             xmldata =  vector._make_defVector()
-                            await self.txque.put(xmldata)
+                            if xmldata:
+                                await self.txque.put(xmldata)
 
 
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
         self.connected = True
         blobstatus = BLOBSstatus(self.devices)
-        rx = Port_RX(blobstatus, reader)
+        addr = writer.get_extra_info('peername')
+        rx = Port_RX(blobstatus, reader, addr)
         tx = Port_TX(blobstatus, writer, self.timer)
+        logger.info(f"Connection received from {addr}")
         try:
             txtask = asyncio.create_task(tx.run_tx(self.txque))
             rxtask = asyncio.create_task(rx.run_rx(self.serverreaderque))
             montask = asyncio.create_task(self._monitor_connection())
             await asyncio.gather(txtask, rxtask, montask)
-        except ConnectionResetError:
+        except ConnectionError:
             self.connected = False
             txtask.cancel()
             rxtask.cancel()
             montask.cancel()
             cleanque(self.txque)
+        logger.info(f"Connection from {addr} closed")
```

### Comparing `indipydriver-1.2.0/indipydriver/propertymembers.py` & `indipydriver-1.2.1/indipydriver/propertymembers.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         xmldata.set("size", str(self.blobsize))
         # the value set in the xmldata object should be a bytes object
         if isinstance(self._membervalue, bytes):
             xmldata.text = self._membervalue
         elif isinstance(self._membervalue, pathlib.Path):
             try:
                 xmldata.text = self._membervalue.read_bytes()
-            except:
+            except Exception:
                 raise ValueError(f"Unable to read BLOBMember {self.name}")
         elif hasattr(self._membervalue, "seek") and hasattr(self._membervalue, "read") and callable(self._membervalue.read):
             # a file-like object
             # set seek(0) so is read from start of file
             self._membervalue.seek(0)
             bytescontent = self._membervalue.read()
             self._membervalue.close()
@@ -334,13 +334,13 @@
                 raise ValueError(f"The BLOBMember {self.name} value is empty")
             xmldata.text = bytescontent
         else:
             # could be a path to a file
             try:
                 with open(self._membervalue, "rb") as fp:
                     bytescontent = fp.read()
-            except:
+            except Exception:
                 raise ValueError(f"The BLOBMember {self.name} value cannot be openned")
             if bytescontent == b"":
                 raise ValueError(f"The BLOBMember {self.name} value is empty")
             xmldata.text = bytescontent
         return xmldata
```

### Comparing `indipydriver-1.2.0/indipydriver/propertyvectors.py` & `indipydriver-1.2.1/indipydriver/propertyvectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 from datetime import datetime, timezone
 
 import asyncio
 
 import xml.etree.ElementTree as ET
 
+import logging
+logger = logging.getLogger(__name__)
+
 from .events import EventException, getProperties, newSwitchVector, newTextVector, newBLOBVector, enableBLOB, newNumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, NumberMember, BLOBMember
 
 
 def timestamp_string(timestamp = None):
     "Return a string timestamp or None if invalid"
     if timestamp is None:
@@ -47,17 +50,14 @@
 
         # this will be set when the device is initialised
         self.devicename = None
 
         # this will be set when the driver asyncrun is run
         self.driver = None
 
-    def _reporterror(self, message):
-        "Prints message to stderr"
-        print(message, file=sys.stderr)
 
     @property
     def device(self):
         return self.driver.devices[self.devicename]
 
     async def send_delProperty(self, message="", timestamp=None):
         """Informs the client this vector is not available, it also sets an 'enable' attribute to
@@ -67,15 +67,15 @@
 
            The message argument is any appropriate string which the client could display to the user.
 
            The timestamp should be either None or a datetime.datetime object. If the timestamp is None
            a UTC value will be inserted."""
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending delProperty: The given send_delProperty timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending delProperty: The given send_delProperty timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('delProperty')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("timestamp", tstring)
         if message:
             xmldata.set("message", message)
@@ -103,21 +103,21 @@
            The state should be either None - in which case no change to the state attribute
            will be made, or one of Idle, Ok, Busy or Alert.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending defVector: The given send_defVector timeout value must be either None or a string object")
+                logger.error("Aborting sending defVector: The given send_defVector timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending defVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending defVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         xmldata = self._make_defVector(message, timestamp)
         if not xmldata is None:
             await self.driver.send(xmldata)
 
 
     def checkvalue(self, value, allowed):
@@ -131,21 +131,21 @@
         return self._state
 
     @state.setter
     def state(self, value):
         try:
             self._state = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     def __setitem__(self, membername, value):
         try:
             self.data[membername].membervalue = value
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     def __getitem__(self, membername):
         return self.data[membername].membervalue
 
 
 class SwitchVector(PropertyVector):
 
@@ -175,26 +175,26 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     @property
     def rule(self):
         return self._rule
 
     @rule.setter
     def rule(self, value):
         try:
             self._rule = self.checkvalue(value, ['OneOfMany','AtMostOne','AnyOfMany'])
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -202,29 +202,29 @@
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
                 elif root.tag == "newSwitchVector":
                     # create event
                     event = newSwitchVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
-            except EventException:
+            except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                pass
+                logger.error(str(ex))
             self.dataque.task_done()
 
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending defSwitchVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending defSwitchVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('defSwitchVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
@@ -266,29 +266,29 @@
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setSwitchVector: The given send_setVector timeout value must be either None or a string object")
+                logger.error("Aborting sending setSwitchVector: The given send_setVector timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setSwitchVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setSwitchVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setSwitchVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setSwitchVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setSwitchVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -327,29 +327,29 @@
            then a vector will still be sent, empty of members, which may be required if
            just a state or message is to be sent.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setSwitchVector: The given send_setVectorMembers timeout value must be either None or a string object")
+                logger.error("Aborting sending setSwitchVector: The given send_setVectorMembers timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setSwitchVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setSwitchVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setSwitchVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setSwitchVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setSwitchVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -390,32 +390,32 @@
             # test if any xml data has been received
             try:
                 root = await self.dataque.get()
                 if root.tag == "getProperties":
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
-            except EventException:
+            except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                pass
+                logger.error(str(ex))
             self.dataque.task_done()
 
     @property
     def perm(self):
         return "ro"
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending defLightVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending defLightVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('defLightVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
@@ -449,23 +449,23 @@
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setLightVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setLightVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setLightVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setLightVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setLightVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if message:
@@ -492,23 +492,23 @@
            just a state or message is to be sent.
         """
         # Note timeout is not used
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setLightVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setLightVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setLightVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setLightVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setLightVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if message:
@@ -539,15 +539,15 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -555,28 +555,28 @@
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
                 elif root.tag == "newTextVector":
                     # create event
                     event = newTextVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
-            except EventException:
+            except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                pass
+                logger.error(str(ex))
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending defTextVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending defTextVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('defTextVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
@@ -615,29 +615,29 @@
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setTextVector: The given send_setVector timeout value must be either None or a string object")
+                logger.error("Aborting sending setTextVector: The given send_setVector timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setTextVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setTextVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setTextVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setTextVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setTextVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -665,29 +665,29 @@
            then a vector will still be sent, empty of members, which may be required if
            just a state or message is to be sent.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setTextVector: The given send_setVectorMembers timeout value must be either None or a string object")
+                logger.error("Aborting sending setTextVector: The given send_setVectorMembers timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setTextVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setTextVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setTextVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setTextVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setTextVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -717,15 +717,15 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -733,28 +733,28 @@
                     # create event
                     event = getProperties(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
                 elif root.tag == "newNumberVector":
                     # create event
                     event = newNumberVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
-            except EventException:
+            except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                pass
+                logger.error(str(ex))
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending defNumberVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending defNumberVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('defNumberVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
@@ -793,29 +793,29 @@
            vector message, state or time values are sent to the client, then use the more
            explicit send_setVectorMembers method instead.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setNumberVector: The given send_setVector timeout value must be either None or a string object")
+                logger.error("Aborting sending setNumberVector: The given send_setVector timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setNumberVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setNumberVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setNumberVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setNumberVector: The given send_setVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setNumberVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -843,29 +843,29 @@
            then a vector will still be sent, empty of members, which may be required if
            just a state or message is to be sent.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setNumberVector: The given send_setVectorMembers timeout value must be either None or a string object")
+                logger.error("Aborting sending setNumberVector: The given send_setVectorMembers timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setNumberVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setNumberVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setNumberVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setNumberVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setNumberVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -883,26 +883,26 @@
 
     def __init__(self, name, label, group, perm, state, blobmembers):
         super().__init__(name, label, group, state)
         self.perm = perm
         # self.data is a dictionary of blob name : blobmember
         for blob in blobmembers:
             if not isinstance(blob, BLOBMember):
-                self._reporterror("Members of a BLOBVector must all be BLOBMembers")
+                logger.error("Members of a BLOBVector must all be BLOBMembers")
                 raise TypeError("Members of a BLOBVector must all be BLOBMembers")
             self.data[blob.name] = blob
 
     def set_blobsize(self, membername, blobsize):
         """Sets the size attribute in the blob member. If the default of zero is used,
            the size will be set to the number of bytes in the BLOB. The INDI standard
            specifies the size should be that of the BLOB before any compression,
            therefore if you are sending a compressed file, you should set the blobsize
            prior to compression with this method."""
         if not isinstance(blobsize, int):
-            self._reporterror("blobsize rejected, must be an integer object")
+            logger.error("blobsize rejected, must be an integer object")
             return
         member = self.data.get[membername]
         if not member:
             return
         member.blobsize = blobsize
 
     @property
@@ -910,15 +910,15 @@
         return self._perm
 
     @perm.setter
     def perm(self, value):
         try:
             self._perm = self.checkvalue(value, ['ro','wo','rw'])
         except ValueError as ex:
-            self._reporterror(ex)
+            logger.error(str(ex))
 
     async def _handler(self):
         """Check received data and take action"""
         while True:
             await asyncio.sleep(0)
             try:
                 root = await self.dataque.get()
@@ -930,28 +930,28 @@
                     # create event
                     event = enableBLOB(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
                 elif root.tag == "newBLOBVector":
                     # create event
                     event = newBLOBVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
-            except EventException:
+            except EventException as ex:
                 # if an error is raised parsing the incoming data, just continue
-                pass
+                logger.error(str(ex))
             self.dataque.task_done()
 
     def _make_defVector(self, message='', timestamp=None):
         "Creates xml data object for vector definition"
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending defBLOBVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending defBLOBVector: The given send_defVector timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('defBLOBVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("label", self.label)
         xmldata.set("group", self.group)
         xmldata.set("state", self.state)
@@ -979,29 +979,29 @@
            a file-like object is given, its contents will be read and its close() method
            will be called, so you do not have to close it.
         """
         if not timeout is None:
             if isinstance(timeout, str):
                 self.timeout = timeout
             else:
-                self._reporterror("Aborting sending setBLOBVector: The given send_setVectorMembers timeout value must be either None or a string object")
+                logger.error("Aborting sending setBLOBVector: The given send_setVectorMembers timeout value must be either None or a string object")
                 return
         if state:
             if state in ('Idle','Ok','Busy','Alert'):
                 self._state = state
             else:
-                self._reporterror("Aborting sending setBLOBVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
+                logger.error("Aborting sending setBLOBVector: The given state must be either None or one of Idle, Ok, Busy or Alert")
                 return
         if not self.device.enable:
             return
         if not self.enable:
             return
         tstring = timestamp_string(timestamp)
         if not tstring:
-            self._reporterror("Aborting sending setBLOBVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
+            logger.error("Aborting sending setBLOBVector: The given send_setVectorMembers timestamp must be a UTC datetime.datetime object")
             return
         xmldata = ET.Element('setBLOBVector')
         xmldata.set("device", self.devicename)
         xmldata.set("name", self.name)
         xmldata.set("state", self.state)
         xmldata.set("timestamp", tstring)
         if self._perm != 'ro':
@@ -1009,9 +1009,9 @@
         if message:
             xmldata.set("message", message)
         for blob in self.data.values():
             if (blob.name in members) and (blob.membervalue is not None):
                 try:
                     xmldata.append(blob.oneblob())
                 except ValueError as ex:
-                    self._reporterror(ex)
+                    logger.error(str(ex))
         await self.driver.send(xmldata)
```

### Comparing `indipydriver-1.2.0/pyproject.toml` & `indipydriver-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.2.0"
+version = "1.2.1"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.2.0/PKG-INFO` & `indipydriver-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.2.0
+Version: 1.2.1
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

