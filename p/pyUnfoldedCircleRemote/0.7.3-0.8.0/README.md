# Comparing `tmp/pyunfoldedcircleremote-0.7.3.tar.gz` & `tmp/pyunfoldedcircleremote-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyunfoldedcircleremote-0.7.3.tar", max compression
+gzip compressed data, was "pyunfoldedcircleremote-0.8.0.tar", max compression
```

## Comparing `pyunfoldedcircleremote-0.7.3.tar` & `pyunfoldedcircleremote-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.7.3/LICENSE
--rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.7.3/README.md
--rw-r--r--   0        0        0      604 2024-05-17 18:18:22.940867 pyunfoldedcircleremote-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/__init__.py
--rw-r--r--   0        0        0      783 2024-04-21 21:46:12.575871 pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/const.py
--rw-r--r--   0        0        0    68866 2024-05-17 18:18:17.583284 pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/remote.py
--rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/remote_websocket.py
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-11-11 18:51:29.176913 pyunfoldedcircleremote-0.8.0/LICENSE
+-rw-r--r--   0        0        0      119 2023-11-11 18:52:24.241472 pyunfoldedcircleremote-0.8.0/README.md
+-rw-r--r--   0        0        0      604 2024-05-19 21:56:54.597096 pyunfoldedcircleremote-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-03 21:50:52.813920 pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/__init__.py
+-rw-r--r--   0        0        0      783 2024-04-21 21:46:12.575871 pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/const.py
+-rw-r--r--   0        0        0    69514 2024-05-19 21:54:32.065057 pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/remote.py
+-rw-r--r--   0        0        0     7345 2024-03-17 01:49:19.890767 pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/remote_websocket.py
+-rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 pyunfoldedcircleremote-0.8.0/PKG-INFO
```

### Comparing `pyunfoldedcircleremote-0.7.3/LICENSE` & `pyunfoldedcircleremote-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.3/pyproject.toml` & `pyunfoldedcircleremote-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyUnfoldedCircleRemote"
-version = "0.7.3"
+version = "0.8.0"
 description = "A python library to interact with the Unfolded Circle Remote"
 authors = ["Jack Powell <jackjpowell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jackjpowell/py-unfolded-circle"
 packages = [{include = "pyUnfoldedCircleRemote", from = "src"}]
```

### Comparing `pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/const.py` & `pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/const.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/remote.py` & `pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/remote.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,15 @@
         self._sound_effects_volume = 0
         self._haptic_feedback = False
         self._display_timeout = 0
         self._wakeup_sensitivity = 0
         self._sleep_timeout = 0
         self._update_in_progress = False
         self._update_percent = 0
+        self._download_percent = 0
         self._next_update_check_date = ""
         self._sw_version = ""
         self._check_for_updates = False
         self._automatic_updates = False
         self._available_update = []
         self._latest_sw_version = ""
         self._release_notes_url = ""
@@ -295,14 +296,19 @@
 
     @property
     def update_percent(self):
         """Remote Update percentage."""
         return self._update_percent
 
     @property
+    def download_percent(self):
+        """Remote download percentage."""
+        return self._download_percent
+
+    @property
     def next_update_check_date(self):
         """Remote Next Update Check Date."""
         return self._next_update_check_date
 
     @property
     def automatic_updates(self):
         """Does remote have automatic updates turned on."""
@@ -847,18 +853,18 @@
             else:
                 self._latest_sw_version = self._sw_version
 
             if download_status in ("PENDING", "ERROR"):
                 try:
                     # When download status is pending, the first request to system/update
                     # will request the download of the latest firmware but will not install
-                    response = await self.update_remote()
+                    response = await self.update_remote(download_only=True)
                 except HTTPError:
                     pass
-            return information
+                return information
 
     async def get_remote_force_update_information(self) -> bool:
         """Force a remote firmware update check."""
         async with (
             self.client() as session,
             session.put(self.url("system/update")) as response,
         ):
@@ -884,22 +890,29 @@
             else:
                 self._latest_sw_version = self._sw_version
 
             if download_status in ("PENDING", "ERROR"):
                 try:
                     # When download status is pending, the first request to system/update
                     # will request the download of the latest firmware but will not install
-                    response = await self.update_remote()
+                    response = await self.update_remote(download_only=True)
                 except HTTPError:
                     pass
             return information
 
-    async def update_remote(self) -> str:
+    async def update_remote(self, download_only: bool = False) -> str:
         """Update Remote."""
-        # WIP: Starts the latest firmware update."
+        # If we only want to download the firmware, check the status.
+        # If it's not pending or error, bail so we don't accidentally
+        # invoke an install
+        if download_only is True:
+            download_status = await self.get_update_status()
+            if download_status.get("state") not in ("PENDING", "ERROR"):
+                return
+
         async with (
             self.client() as session,
             session.post(self.url("system/update/latest")) as response,
         ):
             await self.raise_on_error(response)
             information = await response.json()
             if information.get("state") == "DOWNLOAD":
@@ -908,20 +921,22 @@
             if information.get("state") == "START":
                 self._update_in_progress = True
             return information
 
     async def get_update_status(self) -> str:
         """Update remote status."""
         # WIP: Gets Update Status -- Only supports latest."
+        self._download_percent = 0
         async with (
             self.client() as session,
             session.get(self.url("system/update/latest")) as response,
         ):
             await self.raise_on_error(response)
             information = await response.json()
+            self._download_percent = information.get("download_percent")
             return information
 
     async def get_activity_state(self, entity_id) -> str:
         """Get activity state for a remote entity."""
         async with (
             self.client() as session,
             session.get(self.url("activities")) as response,
```

### Comparing `pyunfoldedcircleremote-0.7.3/src/pyUnfoldedCircleRemote/remote_websocket.py` & `pyunfoldedcircleremote-0.8.0/src/pyUnfoldedCircleRemote/remote_websocket.py`

 * *Files identical despite different names*

### Comparing `pyunfoldedcircleremote-0.7.3/PKG-INFO` & `pyunfoldedcircleremote-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUnfoldedCircleRemote
-Version: 0.7.3
+Version: 0.8.0
 Summary: A python library to interact with the Unfolded Circle Remote
 Home-page: https://github.com/jackjpowell/py-unfolded-circle
 License: MIT
 Author: Jack Powell
 Author-email: jackjpowell@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

