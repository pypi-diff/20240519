# Comparing `tmp/indipyclient-0.1.4.tar.gz` & `tmp/indipyclient-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.1.4.tar` & `indipyclient-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.4/LICENSE
--rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.4/README.md
--rw-r--r--   0        0        0      416 2024-05-16 10:35:07.000000 indipyclient-0.1.4/indipyclient/__init__.py
--rw-r--r--   0        0        0     3663 2024-05-16 10:28:14.000000 indipyclient-0.1.4/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.4/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    21226 2024-05-15 17:27:54.000000 indipyclient-0.1.4/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.4/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.4/indipyclient/console/windows.py
--rw-r--r--   0        0        0    26848 2024-05-15 10:33:05.000000 indipyclient-0.1.4/indipyclient/events.py
--rw-r--r--   0        0        0    32735 2024-05-15 11:40:24.000000 indipyclient-0.1.4/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.1.4/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.4/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-05-16 10:34:35.000000 indipyclient-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2677 2024-05-03 10:25:21.000000 indipyclient-0.1.5/README.md
+-rw-r--r--   0        0        0      416 2024-05-19 14:24:30.000000 indipyclient-0.1.5/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-16 10:28:14.000000 indipyclient-0.1.5/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.5/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    21226 2024-05-15 17:27:54.000000 indipyclient-0.1.5/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.5/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144019 2024-05-05 09:43:32.000000 indipyclient-0.1.5/indipyclient/console/windows.py
+-rw-r--r--   0        0        0    26848 2024-05-15 10:33:05.000000 indipyclient-0.1.5/indipyclient/events.py
+-rw-r--r--   0        0        0    32802 2024-05-19 14:22:05.000000 indipyclient-0.1.5/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16339 2024-05-15 11:03:42.000000 indipyclient-0.1.5/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27626 2024-05-03 10:01:46.000000 indipyclient-0.1.5/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-19 14:24:11.000000 indipyclient-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3448 1970-01-01 00:00:00.000000 indipyclient-0.1.5/PKG-INFO
```

### Comparing `indipyclient-0.1.4/LICENSE` & `indipyclient-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/README.md` & `indipyclient-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/__main__.py` & `indipyclient-0.1.5/indipyclient/__main__.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/console/consoleclient.py` & `indipyclient-0.1.5/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/console/widgets.py` & `indipyclient-0.1.5/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/console/windows.py` & `indipyclient-0.1.5/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/events.py` & `indipyclient-0.1.5/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/ipyclient.py` & `indipyclient-0.1.5/indipyclient/ipyclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,29 +299,30 @@
         "log tx data with level debug, and detail depends on self._verbose"
 
         startlog = "TX:: "
         if self._verbose == 3:
             binarydata = ET.tostring(txdata)
             logger.debug(startlog + binarydata.decode())
         elif self._verbose == 2:
-            tag = txdata.tag
-            for element in txdata:
+            data = copy.deepcopy(txdata)
+            tag = data.tag
+            for element in data:
                 if tag == "newBLOBVector":
                     element.text = "NOT LOGGED"
-            binarydata = ET.tostring(txdata)
+            binarydata = ET.tostring(data)
             logger.debug(startlog + binarydata.decode())
         elif self._verbose == 1:
-            for element in txdata:
-                txdata.remove(element)
-            txdata.text = ""
-            binarydata = ET.tostring(txdata, short_empty_elements=False).split(b">")
+            data = copy.deepcopy(txdata)
+            for element in data:
+                data.remove(element)
+            data.text = ""
+            binarydata = ET.tostring(data, short_empty_elements=False).split(b">")
             logger.debug(startlog + binarydata[0].decode()+">")
 
 
-
     async def _run_tx(self, writer):
         "Monitors self.writerque and if it has data, uses writer to send it"
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
                 try:
                     txdata = self.writerque.popleft()
```

### Comparing `indipyclient-0.1.4/indipyclient/propertymembers.py` & `indipyclient-0.1.5/indipyclient/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/indipyclient/propertyvectors.py` & `indipyclient-0.1.5/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.1.4/pyproject.toml` & `indipyclient-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.1.4"
+version = "0.1.5"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.1.4/PKG-INFO` & `indipyclient-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

