# Comparing `tmp/audiconnectpy-2.1.7.tar.gz` & `tmp/audiconnectpy-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-2.1.7.tar", last modified: Sun May 19 11:26:52 2024, max compression
+gzip compressed data, was "audiconnectpy-2.1.8.tar", last modified: Sun May 19 13:58:19 2024, max compression
```

## Comparing `audiconnectpy-2.1.7.tar` & `audiconnectpy-2.1.8.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/pythonpackage.yml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.202625 audiconnectpy-2.1.7/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 11:26:51.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 11:26:52.000000 audiconnectpy-2.1.7/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 11:26:52.206625 audiconnectpy-2.1.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/fixtures/audi0.json
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/fixtures/info_vehicles.json
--rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/fixtures/location.json
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-19 11:26:41.000000 audiconnectpy-2.1.7/tests/test_home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.623786 audiconnectpy-2.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.623786 audiconnectpy-2.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.623786 audiconnectpy-2.1.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11853 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26001 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 13:58:19.000000 audiconnectpy-2.1.8/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:58:19.627786 audiconnectpy-2.1.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/audi0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/audi1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/audi2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/info_vehicles.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62872 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/fixtures/location.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-19 13:58:08.000000 audiconnectpy-2.1.8/tests/test_home.py
```

### Comparing `audiconnectpy-2.1.7/.github/dependabot.yml` & `audiconnectpy-2.1.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/.github/workflows/auto-approve.yml` & `audiconnectpy-2.1.8/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/.github/workflows/pythonpackage.yml` & `audiconnectpy-2.1.8/.github/workflows/pythonpackage.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/.github/workflows/pythonpublish.yml` & `audiconnectpy-2.1.8/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/.github/workflows/release.yml` & `audiconnectpy-2.1.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/.gitignore` & `audiconnectpy-2.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/.pre-commit-config.yaml` & `audiconnectpy-2.1.8/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -47,8 +47,8 @@
           - --keep-updates
         files: ^(/.+)?[^/]+\.py$
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.10.0
     hooks:
       - id: mypy
         args: [--strict, --ignore-missing-imports]
-        files: ^(/.+)?[^/]+\.py$
+        exclude: (tests)
```

### Comparing `audiconnectpy-2.1.7/LICENSE` & `audiconnectpy-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/PKG-INFO` & `audiconnectpy-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.7/README.md` & `audiconnectpy-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/audiconnectpy/api.py` & `audiconnectpy-2.1.8/audiconnectpy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 await self.auth.async_connect(self._username, self._password, self.uris)
             except AudiException as error:
                 raise AuthorizationError(error) from error
             else:
                 self.is_connected = True
 
         # Update the state of all vehicles.
-        if self.is_connected:
+        if self.is_connected and len(self.vehicles) == 0:
             try:
                 vehicles_response = await self.async_get_information_vehicles()
             except AudiException as error:
                 raise AudiException(
                     "Error to get information vehicles ({error})"
                 ) from error
             else:
@@ -90,16 +90,14 @@
                         try:
                             # Fetch data for a vehicle
                             await vehicle.async_update()
                         except AudiException as error:
                             _LOGGER.error(
                                 "Error while updating - %s - (%s)", vehicle.vin, error
                             )
-        else:
-            raise AuthorizationError("API not connected")
 
     async def async_get_information_vehicles(self) -> Any:
         """Get information vehicles."""
         headers = await self.auth.async_get_headers(
             token_type="audi",
             headers={
                 "Accept-Language": f"{self.uris['language']}-{self.country}",
```

### Comparing `audiconnectpy-2.1.7/audiconnectpy/auth.py` & `audiconnectpy-2.1.8/audiconnectpy/auth.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/audiconnectpy/const.py` & `audiconnectpy-2.1.8/audiconnectpy/const.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/audiconnectpy/helpers.py` & `audiconnectpy-2.1.8/audiconnectpy/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         windows_open.append(open_sun_roof)
 
     metadatas.update({"any_windows_status": any(windows_open)})
 
     return metadatas
 
 
-def doors_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
+def doors_status(attrs: list[dict[str, Any]]) -> dict[str, dict[str, bool]]:
     """Doors lock status."""
     status = map_name_status(attrs)
     left_unlock = "locked" not in status.get("frontLeft", [])
     left_rear_unlock = "locked" not in status.get("rearLeft", [])
     right_unlock = "locked" not in status.get("frontRight", [])
     right_rear_unlock = "locked" not in status.get("rearRight", [])
     trunk_unlock = "locked" not in status.get("trunk", [])
@@ -200,19 +200,19 @@
         }
     )
 
     return metadatas
 
 
 def lights_status(attrs: list[dict[str, Any]]) -> dict[str, bool]:
+    """Light status."""
     status = map_name_status(attrs)
-    metadatas = {
-        "left": status.get("left") != "off",
-        "right": status.get("right") != "off",
-    }
+    left = status.get("left") != "off"
+    right = status.get("right") != "off"
+    metadatas = {"left": left, "right": right, "status": any([left, right])}
 
     return metadatas
 
 
 def camel2snake(name: str) -> str:
     """Camel case to Snake case."""
     return re.sub(r"(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])", "_", name).lower()
```

### Comparing `audiconnectpy-2.1.7/audiconnectpy/model.py` & `audiconnectpy-2.1.8/audiconnectpy/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,34 +28,48 @@
         return value != "off"
 
 
 class WindowsStrategy(SerializationStrategy):  # type: ignore
     def serialize(self, value: str) -> str:
         return value
 
-    def deserialize(self, value: str) -> bool:
+    def deserialize(self, value: list[dict[str, Any]]) -> Any:
         return Window.from_dict(windows_status(value))
 
 
 class DoorsStrategy(SerializationStrategy):  # type: ignore
     def serialize(self, value: str) -> str:
         return value
 
-    def deserialize(self, value: str) -> bool:
+    def deserialize(self, value: list[dict[str, Any]]) -> Any:
         return Doors.from_dict(doors_status(value))
 
 
 class LightsStrategy(SerializationStrategy):  # type: ignore
     def serialize(self, value: str) -> str:
         return value
 
-    def deserialize(self, value: str) -> bool:
+    def deserialize(self, value: list[dict[str, Any]]) -> Any:
         return Lights.from_dict(lights_status(value))
 
 
+class WindowHeatingStrategy(SerializationStrategy):  # type: ignore
+    def serialize(self, value: str) -> str:
+        return value
+
+    def deserialize(self, values: list[dict[str, Any]]) -> Any:
+        status = {
+            value["windowLocation"]: (value["windowHeatingState"] != "off")
+            for value in values
+            if "windowLocation" in value.keys() and "windowHeatingState" in value.keys()
+        }
+
+        return WindowHeating.from_dict(status)
+
+
 @dataclass
 class Base(DataClassDictMixin):  # type: ignore
     @classmethod
     def __pre_deserialize__(cls, d: dict[Any, Any]) -> dict[Any, Any]:
         return {camel2snake(k): v for k, v in d.items()}
 
 
@@ -97,47 +111,47 @@
     )
     windows: Window | None = field(
         metadata=field_options(serialization_strategy=WindowsStrategy()), default=None
     )
 
 
 @dataclass
-class Doors(DataClassDictMixin):
+class Doors(Base):
     locked: DoorLocked | None = None
     opened: DoorOpened | None = None
 
 
 @dataclass
-class DoorLocked(DataClassDictMixin):
+class DoorLocked(Base):
     """Windows status."""
 
     left_front: bool | None = None
     right_front: bool | None = None
     left_rear: bool | None = None
     right_rear: bool | None = None
     trunk: bool | None = None
     doors_trunk: bool | None = None
     any_doors_status: bool | None = None
 
 
 @dataclass
-class DoorOpened(DataClassDictMixin):
+class DoorOpened(Base):
     """Windows status."""
 
     left_front: bool | None = None
     right_front: bool | None = None
     left_rear: bool | None = None
     right_rear: bool | None = None
     trunk: bool | None = None
     bonnet: bool | None = None
     any_doors_status: bool | None = None
 
 
 @dataclass
-class Window(DataClassDictMixin):
+class Window(Base):
     """Windows status."""
 
     left_front: bool | None = None
     right_front: bool | None = None
     left_rear: bool | None = None
     right_rear: bool | None = None
     roof_cover: bool | None = None
@@ -193,15 +207,17 @@
 class PlugStatus(Base):
     plug_connection_state: bool | None = field(
         metadata=field_options(deserialize=lambda x: x == "connected"), default=None
     )
     plug_lock_state: bool | None = field(
         metadata=field_options(serialization_strategy=Locked()), default=None
     )
-    external_power: str | None = None
+    external_power: bool | None = field(
+        metadata=field_options(deserialize=lambda x: x == "active"), default=None
+    )
     led_color: str | None = None
 
 
 @dataclass
 class ChargeMode(Base):
     preferred_charge_mode: str | None = None
     available_charge_modes: list[str] | None = None
@@ -213,15 +229,27 @@
     window_heating_status: WindowHeatingStatus | None = None
     climatisation_status: ClimatisationStatus | None = None
     climatisation_settings: ClimatisationSettings | None = None
 
 
 @dataclass
 class WindowHeatingStatus(Base):
-    window_heating_status: list[dict[str, str]] | None = None
+    state: WindowHeating | None = field(
+        metadata=field_options(
+            alias="window_heating_status",
+            serialization_strategy=WindowHeatingStrategy(),
+        ),
+        default=None,
+    )
+
+
+@dataclass
+class WindowHeating(Base):
+    front: bool | None = None
+    rear: bool | None = None
 
 
 @dataclass
 class ClimatisationStatus(Base):
     remaining_climatisation_time_min: int | None = None
     climatisation_state: bool | None = field(
         metadata=field_options(serialization_strategy=OnOff()), default=None
@@ -325,14 +353,15 @@
     )
 
 
 @dataclass
 class Lights(Base):
     left: bool | None = None
     right: bool | None = None
+    status: bool | None = None
 
 
 # SECTION
 @dataclass
 class VehicleHealthInspection(Base):
     maintenance_status: MaintenanceStatus | None = None
```

### Comparing `audiconnectpy-2.1.7/audiconnectpy/vehicle.py` & `audiconnectpy-2.1.8/audiconnectpy/vehicle.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-2.1.8/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 2.1.7
+Version: 2.1.8
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-2.1.7/audiconnectpy.egg-info/SOURCES.txt` & `audiconnectpy-2.1.8/audiconnectpy.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -27,9 +27,11 @@
 audiconnectpy.egg-info/not-zip-safe
 audiconnectpy.egg-info/requires.txt
 audiconnectpy.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_home.py
 tests/fixtures/audi0.json
+tests/fixtures/audi1.json
+tests/fixtures/audi2.json
 tests/fixtures/info_vehicles.json
 tests/fixtures/location.json
```

### Comparing `audiconnectpy-2.1.7/example.py` & `audiconnectpy-2.1.8/example.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/pyproject.toml` & `audiconnectpy-2.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/tests/conftest.py` & `audiconnectpy-2.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/tests/fixtures/audi0.json` & `audiconnectpy-2.1.8/tests/fixtures/audi0.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/tests/fixtures/info_vehicles.json` & `audiconnectpy-2.1.8/tests/fixtures/info_vehicles.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/tests/fixtures/location.json` & `audiconnectpy-2.1.8/tests/fixtures/location.json`

 * *Files identical despite different names*

### Comparing `audiconnectpy-2.1.7/tests/test_home.py` & `audiconnectpy-2.1.8/tests/test_home.py`

 * *Files 20% similar despite different names*

```diff
@@ -150,10 +150,35 @@
         ),
         patch(
             "audiconnectpy.vehicle.Vehicle.async_get_capabilities",
             return_value=capabilities,
         ),
     ):
         await api.async_login()
+        my_vehicle = api.vehicles[0]
 
         assert api.vehicles is not None
-        assert api.vehicles[0].infos is not None
+        assert my_vehicle.infos is not None
+        assert my_vehicle.climatisation.window_heating_status.state.front is False
+        assert my_vehicle.vehicle_lights.lights_status.lights.status is False
+        assert my_vehicle.measurements.range_status.electric_range == 212
+        assert my_vehicle.measurements.odometer_status.odometer == 10329
+        assert (
+            my_vehicle.vehicle_health_inspection.maintenance_status.mileage_km == 10329
+        )
+        assert my_vehicle.fuel_status.range_status.total_range_km == 212
+        assert my_vehicle.climatisation.window_heating_status.state.front is False
+        assert (
+            my_vehicle.climatisation.climatisation_status.climatisation_state is False
+        )
+        assert (
+            my_vehicle.climatisation.climatisation_status.climatisation_state is False
+        )
+        assert (
+            my_vehicle.climatisation.climatisation_settings.climatization_at_unlock
+            is True
+        )
+        assert my_vehicle.charging.battery_status.cruising_range_electric_km == 212
+        assert my_vehicle.charging.charge_mode.preferred_charge_mode == "manual"
+        assert my_vehicle.charging.charging_settings.max_charge_current_ac == "maximum"
+        assert my_vehicle.charging.charging_status.remaining == 400
+        assert my_vehicle.charging.plug_status.led_color == "green"
```

