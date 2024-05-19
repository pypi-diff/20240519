# Comparing `tmp/oresat_cfc-0.1.0.tar.gz` & `tmp/oresat_cfc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_cfc-0.1.0.tar", last modified: Sun Apr 28 05:12:48 2024, max compression
+gzip compressed data, was "oresat_cfc-0.1.1.tar", last modified: Sun May 19 18:27:59 2024, max compression
```

## Comparing `oresat_cfc-0.1.0.tar` & `oresat_cfc-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.552154 oresat_cfc-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.556154 oresat_cfc-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.556154 oresat_cfc-0.1.0/oresat_cfc/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.556154 oresat_cfc-0.1.0/oresat_cfc/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/drivers/pirt1280.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/drivers/rc625.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/oresat_cfc/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/services/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/services/tec_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/oresat_cfc/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/templates/cfc.html
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/oresat_cfc/templates/pid.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/oresat_cfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 05:12:48.000000 oresat_cfc-0.1.0/oresat_cfc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/tests/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/tests/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/tests/drivers/test_pirt1280.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:48.560154 oresat_cfc-0.1.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:12:44.000000 oresat_cfc-0.1.0/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.251846 oresat_cfc-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.243846 oresat_cfc-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-19 18:27:59.251846 oresat_cfc-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/oresat_cfc/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/oresat_cfc/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/drivers/pirt1280.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/drivers/rc625.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/oresat_cfc/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/services/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/services/tec_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/oresat_cfc/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/templates/cfc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/oresat_cfc/templates/pid.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/oresat_cfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 18:27:59.000000 oresat_cfc-0.1.1/oresat_cfc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 18:27:59.251846 oresat_cfc-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/tests/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/tests/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/tests/drivers/test_pirt1280.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:59.247846 oresat_cfc-0.1.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 18:27:54.000000 oresat_cfc-0.1.1/tests/services/__init__.py
```

### Comparing `oresat_cfc-0.1.0/.github/workflows/pypi.yaml` & `oresat_cfc-0.1.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/.github/workflows/tests.yaml` & `oresat_cfc-0.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/.gitignore` & `oresat_cfc-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/LICENSE` & `oresat_cfc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/PKG-INFO` & `oresat_cfc-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: oresat-cfc
-Version: 0.1.0
+Version: 0.1.1
 Summary: OreSat CFC OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: imagecodecs
 Requires-Dist: numpy
 Requires-Dist: opencv-python-headless==4.6.0.66
 Requires-Dist: oresat-configs
 Requires-Dist: oresat-olaf>=3.4.0
 Requires-Dist: simple-pid
 Requires-Dist: spidev
 Requires-Dist: tifffile
```

### Comparing `oresat_cfc-0.1.0/README.md` & `oresat_cfc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/oresat_cfc/__main__.py` & `oresat_cfc-0.1.1/oresat_cfc/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/oresat_cfc/drivers/pirt1280.py` & `oresat_cfc-0.1.1/oresat_cfc/drivers/pirt1280.py`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/oresat_cfc/drivers/rc625.py` & `oresat_cfc-0.1.1/oresat_cfc/drivers/rc625.py`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/oresat_cfc/services/camera.py` & `oresat_cfc-0.1.1/oresat_cfc/services/camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Main camera service.
 
 Seperate from the TEC controller service as the camera can be used regaurdless if the TEC is
 enabled or not.
 """
 
 from enum import IntEnum
-from time import time
+from time import monotonic, time
 
 import canopen
 import cv2
 import numpy as np
 import tifffile
 from olaf import Service, logger, new_oresat_file
 
@@ -23,39 +23,44 @@
 
     OFF = 0x1
     """Camera is off"""
     STANDBY = 0x2
     """Camera is on, but no doing anything"""
     CAPTURE = 0x3
     """Camera is capturing image and saving them to freac cache"""
+    BOOT_LOCKOUT = 0x4
+    """Camera is locked out until system is done booting and PRUs are available."""
     ERROR = 0xFF
     """Error with camera hardware"""
 
 
 STATE_TRANSMISSIONS = {
     CameraState.OFF: [CameraState.OFF, CameraState.STANDBY],
     CameraState.STANDBY: [CameraState.OFF, CameraState.STANDBY, CameraState.CAPTURE],
     CameraState.CAPTURE: [
         CameraState.OFF,
         CameraState.STANDBY,
         CameraState.CAPTURE,
         CameraState.ERROR,
     ],
+    CameraState.BOOT_LOCKOUT: [CameraState.OFF],
     CameraState.ERROR: [CameraState.OFF, CameraState.ERROR],
 }
 """Valid state transistions."""
 
 
 class CameraService(Service):
     """Service for camera and capture state machine"""
 
+    _BOOT_LOCKOUT_S = 70
+
     def __init__(self, pirt1280: Pirt1280):
         super().__init__()
 
-        self._state = CameraState.OFF
+        self._state = CameraState.BOOT_LOCKOUT
         self._next_state_internal = -1
         self._next_state_user = -1
 
         self._pirt1280 = pirt1280
 
         self._capture_delay_obj: canopen.objectdictionary.Variable = None
         self._capture_count_obj: canopen.objectdictionary.Variable = None
@@ -117,22 +122,31 @@
             new_state = CameraState.ERROR
 
         logger.info(f"state transistion {self._state.name} -> {new_state.name}")
 
         self._state = new_state
 
     def on_loop(self):
+
+        if self._state == CameraState.BOOT_LOCKOUT and monotonic() > self._BOOT_LOCKOUT_S:
+            self._next_state_internal = CameraState.OFF.value
+
         if self._next_state_internal != -1:
             self._state_machine_transition(self._next_state_internal)
             self._next_state_internal = -1
         elif self._next_state_user != -1:
             self._state_machine_transition(self._next_state_user)
             self._next_state_user = -1
 
-        if self._state in [CameraState.OFF, CameraState.STANDBY, CameraState.ERROR]:
+        if self._state in [
+            CameraState.OFF,
+            CameraState.STANDBY,
+            CameraState.ERROR,
+            CameraState.BOOT_LOCKOUT,
+        ]:
             self.sleep(0.1)
         elif self._state == CameraState.CAPTURE:
             self._count += 1
 
             try:
                 self._capture()
             except Pirt1280Error:
```

### Comparing `oresat_cfc-0.1.0/oresat_cfc/services/tec_controller.py` & `oresat_cfc-0.1.1/oresat_cfc/services/tec_controller.py`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/oresat_cfc/templates/cfc.html` & `oresat_cfc-0.1.1/oresat_cfc/templates/cfc.html`

 * *Files 5% similar despite different names*

```diff
@@ -30,23 +30,23 @@
     <div id="gridColumn">
       <!--only here for spacing-->
     </div>
     <div id="gridColumn">
       <!--the "//:0" is a basically the way to make any empty img-->
       <img id="image" src="//:0" alt="camera"/>
       <br/>
-      <button onclick="downloadRawImage()">Download Raw Image</button>
-      <button onclick="downloadDisplayImage()">Download Display Image</button>
+      <button id="downloadRawImageButton" onclick="downloadRawImage()" disabled>Download Raw Image</button>
+      <button id="downloadDisplayImageButton" onclick="downloadDisplayImage()" disabled>Download Display Image</button>
     </div>
     <div id="gridColumn">
       <h4>State Machine</h4>
       <table>
         <tr>
           <td>Status</td>
-          <td><span id="cfcState">OFF</span></td>
+          <td><span id="cfcState">BOOT_LOCKOUT</span></td>
         </tr>
         <tr>
           <td>Capture Delay</td>
           <td><span id="captureDelay">1000</span> ms</td>
         </tr>
         <tr>
           <td>Capture Amount</td>
@@ -87,15 +87,15 @@
         <tr>
           <td>Target Temperature</td>
           <td><span id="tecSetpoint">0</span> °C</td>
         </tr>
       </table>
       <br />
       <div>
-        <button id="changeSettings">Change Settings</button>
+        <button id="changeSettingsButton" disabled>Change Settings</button>
       </div>
     </div>
   </div>
   <dialog id="favDialog">
     <form method="dialog">
       <p>
         <b>Change Settings</b>
@@ -145,15 +145,15 @@
         <button id="cancel" type="reset">Cancel</button>
         <button id="submit" type="submit">Set</button>
       </div>
     </form>
   </dialog>
   <script>
     let lastDisplayImage;
-    const settingsButton = document.getElementById("changeSettings");
+    const settingsButton = document.getElementById("changeSettingsButton");
     const cancelButton = document.getElementById("cancel");
     const submitButton = document.getElementById("submit");
     const dialog = document.getElementById("favDialog");
     dialog.returnValue = "cancel";
 
     async function openCheck(dialog) {
       if (dialog.open) {
@@ -261,14 +261,15 @@
       a.click();
     }
 
     const STATES = {
       0x01: "OFF",
       0x02: "STANDBY",
       0x03: "CAPTURE",
+      0x04: "BOOT_LOCKOUT",
       0xFF: "ERROR",
     };
     let lastCapture = 0;
 
     /** Update all info / data being displayed */
     async function update() {
       let obj;
@@ -284,14 +285,24 @@
       obj = await readValue("camera", "save_captures");
       if (obj.value === true) {
         document.getElementById("saveCaptures").innerHTML = "TRUE";
       } else {
         document.getElementById("saveCaptures").innerHTML = "FALSE";
       }
 
+      if (state === "BOOT_LOCKOUT") {
+        document.getElementById("changeSettingsButton").disabled = true;
+        document.getElementById("downloadRawImageButton").disabled = true;
+        document.getElementById("downloadDisplayImageButton").disabled = true;
+      } else {
+        document.getElementById("changeSettingsButton").disabled = false;
+        document.getElementById("downloadRawImageButton").disabled = false;
+        document.getElementById("downloadDisplayImageButton").disabled = false;
+      }
+
       // get last image capture for display
       obj = await readValue("camera", "last_capture_time");
       if (state != "OFF" && obj.value != lastCapture) {
         lastCapture = obj.value;
         obj = await readValue("camera", "last_display_image");
         lastDisplayImage = obj.value;
         document.getElementById("image").src = "data:image/jpg;base64, " + obj.value;
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends "base.html" %} {% block content %}
 [camera]
 Download Raw Image Download Display Image
 ****** SSttaattee MMaacchhiinnee ******
-Status         OFF
+Status         BOOT_LOCKOUT
 Capture Delay  1000 ms
 Capture Amount 1
 Save Captures  TRUE
 
 ****** CCaammeerraa ******
 Enable Status       DISABLED
 Integration Time    0 us
```

### Comparing `oresat_cfc-0.1.0/oresat_cfc/templates/pid.html` & `oresat_cfc-0.1.1/oresat_cfc/templates/pid.html`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/oresat_cfc.egg-info/PKG-INFO` & `oresat_cfc-0.1.1/oresat_cfc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: oresat-cfc
-Version: 0.1.0
+Version: 0.1.1
 Summary: OreSat CFC OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: imagecodecs
 Requires-Dist: numpy
 Requires-Dist: opencv-python-headless==4.6.0.66
 Requires-Dist: oresat-configs
 Requires-Dist: oresat-olaf>=3.4.0
 Requires-Dist: simple-pid
 Requires-Dist: spidev
 Requires-Dist: tifffile
```

### Comparing `oresat_cfc-0.1.0/oresat_cfc.egg-info/SOURCES.txt` & `oresat_cfc-0.1.1/oresat_cfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_cfc-0.1.0/pyproject.toml` & `oresat_cfc-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Embedded Systems",
 ]
 dependencies = [
-    "imagecodecs",
     "numpy",
     "opencv-python-headless==4.6.0.66",
     "oresat-configs",
     "oresat-olaf>=3.4.0",
     "simple-pid",
     "spidev",
     "tifffile",
```

### Comparing `oresat_cfc-0.1.0/tests/drivers/test_pirt1280.py` & `oresat_cfc-0.1.1/tests/drivers/test_pirt1280.py`

 * *Files identical despite different names*

