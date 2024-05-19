# Comparing `tmp/openplantbook-sdk-0.4.5.tar.gz` & `tmp/openplantbook_sdk-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplantbook-sdk-0.4.5.tar", last modified: Mon Dec 11 10:38:23 2023, max compression
+gzip compressed data, was "openplantbook_sdk-0.4.6.tar", last modified: Sun May 19 11:58:57 2024, max compression
```

## Comparing `openplantbook-sdk-0.4.5.tar` & `openplantbook_sdk-0.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.940710 openplantbook-sdk-0.4.5/
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       79 2023-10-15 11:57:13.000000 openplantbook-sdk-0.4.5/.gitignore
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      592 2023-05-14 11:48:03.000000 openplantbook-sdk-0.4.5/.readthedocs.yml
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1074 2023-03-28 00:27:02.000000 openplantbook-sdk-0.4.5/LICENSE
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1853 2023-12-11 12:01:25.933537 openplantbook-sdk-0.4.5/PKG-INFO
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1020 2023-10-17 11:51:05.000000 openplantbook-sdk-0.4.5/README.md
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       87 2023-12-11 06:00:28.000000 openplantbook-sdk-0.4.5/TODO.txt
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      130 2023-11-09 11:31:25.000000 openplantbook-sdk-0.4.5/build.sh
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       29 2023-08-19 05:13:15.000000 openplantbook-sdk-0.4.5/config.yaml.dist
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     2726 2023-12-11 05:05:08.000000 openplantbook-sdk-0.4.5/demo.py
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.619073 openplantbook-sdk-0.4.5/docs/
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      634 2023-05-07 04:38:02.000000 openplantbook-sdk-0.4.5/docs/Makefile
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1170 2023-10-11 11:32:25.000000 openplantbook-sdk-0.4.5/docs/conf.py
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      505 2023-10-15 11:34:29.000000 openplantbook-sdk-0.4.5/docs/index.rst
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      800 2023-05-07 04:38:02.000000 openplantbook-sdk-0.4.5/docs/make.bat
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       54 2023-10-15 11:36:54.000000 openplantbook-sdk-0.4.5/docs/requirements.txt
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.648207 openplantbook-sdk-0.4.5/docs/source/
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.683489 openplantbook-sdk-0.4.5/docs/source/api/
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      208 2023-10-16 12:00:13.000000 openplantbook-sdk-0.4.5/docs/source/api/opb_sdk.rst
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       31 2023-05-14 10:41:37.000000 openplantbook-sdk-0.4.5/docs/source/readme.rst
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.731882 openplantbook-sdk-0.4.5/openplantbook_sdk/
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      158 2023-10-20 10:50:19.000000 openplantbook-sdk-0.4.5/openplantbook_sdk/__init__.py
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)    16964 2023-12-11 11:40:03.000000 openplantbook-sdk-0.4.5/openplantbook_sdk/sdk.py
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.921534 openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1853 2023-12-11 12:01:24.000000 openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/PKG-INFO
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      568 2023-12-11 12:01:25.000000 openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/SOURCES.txt
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        1 2023-12-11 12:01:24.000000 openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/dependency_links.txt
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       24 2023-12-11 12:01:24.000000 openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/requires.txt
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       24 2023-12-11 12:01:24.000000 openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/top_level.txt
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       99 2023-05-08 12:17:32.000000 openplantbook-sdk-0.4.5/pyproject.toml
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       52 2023-10-16 11:21:50.000000 openplantbook-sdk-0.4.5/requirements.txt
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      968 2023-12-11 12:01:25.949940 openplantbook-sdk-0.4.5/setup.cfg
-drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-12-11 12:01:25.888580 openplantbook-sdk-0.4.5/tests/
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-03-30 00:31:15.000000 openplantbook-sdk-0.4.5/tests/__init__.py
--rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     5562 2023-12-11 12:01:01.000000 openplantbook-sdk-0.4.5/tests/test_openplantbook_sdk.py
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.569523 openplantbook_sdk-0.4.6/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       79 2023-10-15 11:57:13.000000 openplantbook_sdk-0.4.6/.gitignore
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      592 2023-05-14 11:48:03.000000 openplantbook_sdk-0.4.6/.readthedocs.yml
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1074 2023-03-28 00:27:02.000000 openplantbook_sdk-0.4.6/LICENSE
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1853 2024-05-19 11:58:57.566523 openplantbook_sdk-0.4.6/PKG-INFO
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1020 2023-10-17 11:51:05.000000 openplantbook_sdk-0.4.6/README.md
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      139 2023-12-14 06:14:18.000000 openplantbook_sdk-0.4.6/TODO.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      130 2023-11-09 11:31:25.000000 openplantbook_sdk-0.4.6/build.sh
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       29 2023-08-19 05:13:15.000000 openplantbook_sdk-0.4.6/config.yaml.dist
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     2726 2023-12-11 05:05:08.000000 openplantbook_sdk-0.4.6/demo.py
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.392481 openplantbook_sdk-0.4.6/docs/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      634 2023-05-07 04:38:02.000000 openplantbook_sdk-0.4.6/docs/Makefile
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1170 2023-10-11 11:32:25.000000 openplantbook_sdk-0.4.6/docs/conf.py
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      505 2023-10-15 11:34:29.000000 openplantbook_sdk-0.4.6/docs/index.rst
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      800 2023-05-07 04:38:02.000000 openplantbook_sdk-0.4.6/docs/make.bat
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       54 2023-10-15 11:36:54.000000 openplantbook_sdk-0.4.6/docs/requirements.txt
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.409667 openplantbook_sdk-0.4.6/docs/source/
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.430348 openplantbook_sdk-0.4.6/docs/source/api/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      208 2023-10-16 12:00:13.000000 openplantbook_sdk-0.4.6/docs/source/api/opb_sdk.rst
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       31 2023-05-14 10:41:37.000000 openplantbook_sdk-0.4.6/docs/source/readme.rst
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.459183 openplantbook_sdk-0.4.6/openplantbook_sdk/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      158 2023-10-20 10:50:19.000000 openplantbook_sdk-0.4.6/openplantbook_sdk/__init__.py
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)    17866 2024-05-19 11:55:26.000000 openplantbook_sdk-0.4.6/openplantbook_sdk/sdk.py
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.558258 openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     1853 2024-05-19 11:58:56.000000 openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/PKG-INFO
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      568 2024-05-19 11:58:57.000000 openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        1 2024-05-19 11:58:56.000000 openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       24 2024-05-19 11:58:56.000000 openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/requires.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       24 2024-05-19 11:58:56.000000 openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/top_level.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       99 2023-05-08 12:17:32.000000 openplantbook_sdk-0.4.6/pyproject.toml
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)       52 2023-10-16 11:21:50.000000 openplantbook_sdk-0.4.6/requirements.txt
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)      968 2024-05-19 11:58:57.573521 openplantbook_sdk-0.4.6/setup.cfg
+drwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2024-05-19 11:58:57.543862 openplantbook_sdk-0.4.6/tests/
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)        0 2023-03-30 00:31:15.000000 openplantbook_sdk-0.4.6/tests/__init__.py
+-rwxrwxrwx   0 slaxor    (1000) slaxor    (1000)     7274 2024-05-17 12:35:58.000000 openplantbook_sdk-0.4.6/tests/test_openplantbook_sdk.py
```

### Comparing `openplantbook-sdk-0.4.5/.readthedocs.yml` & `openplantbook_sdk-0.4.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/LICENSE` & `openplantbook_sdk-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/PKG-INFO` & `openplantbook_sdk-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplantbook-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Open Plantbook SDK for Python
 Home-page: https://github.com/slaxor505/openplantbook-sdk-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://openplantbook-sdk-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/openplantbook-sdk-py
```

### Comparing `openplantbook-sdk-0.4.5/README.md` & `openplantbook_sdk-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/demo.py` & `openplantbook_sdk-0.4.6/demo.py`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/docs/Makefile` & `openplantbook_sdk-0.4.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/docs/conf.py` & `openplantbook_sdk-0.4.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/docs/make.bat` & `openplantbook_sdk-0.4.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/openplantbook_sdk/sdk.py` & `openplantbook_sdk-0.4.6/openplantbook_sdk/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 import aiohttp
 from json_timeseries import JtsDocument
 
 _LOGGER = logging.getLogger(__name__)
 
 PLANTBOOK_BASEURL = "https://open.plantbook.io/api/v1"
+
+
 # PLANTBOOK_BASEURL = "http://localhost:8000/api/v1"
 
 
 class OpenPlantBookApi:
     """
     Open Plantbook SDK class
     """
@@ -161,30 +163,32 @@
     # async def async_post(self,session, url, api_payload):
     #
     #     async with session.post(url, json=api_payload, raise_for_status=False) as result:
     #         _LOGGER.debug("Registered sensor %s", api_payload)
     #         res = await result.json(content_type=None)
 
     async def async_plant_instance_register(self, sensor_pid_map: dict, location_by_ip: bool = None,
-                                            location_country: str = None, location_lon: float = None, location_lat: float = None):
+                                            location_country: str = None, location_lon: float = None,
+                                            location_lat: float = None):
         """
         Register a plant sensor
 
-        :param sensor_pid_map: Plant Instance to PlantID map. Dictionary id-pid
+        :param sensor_pid_map: Plant Instance to PlantID map. Dictionary id-pid. ONLY 1 item is currently supported.
         :param location_by_ip: Allow to take location from IP address
         :param location_country: Country location of the plant
         :param location_lon: Location longitude of the plant
         :param location_lat: Location latitude of the plant
         :return: JSON dict with API response
         :rtype: dict
-        :raise [ValidationError]: [Value of 'series' must be types of TimeSeries or List[TimeSeries]]
+        :raise [ValidationError]: API could not validate JSON payload due to some errors which are returned within the exception's attribute 'errors'
         :raise [aiohttp.ClientError]: [aiohttp client error exception]
         :raise [aiohttp.ServerTimeoutError]: [aiohttp exception]
         :raise [aiohttp.aiohttp.TooManyRedirects]: [aiohttp exception]
         """
+        # TODO O: Docs for new exception ValidationError
         try:
             await self._async_get_token()
         except Exception:  # pylint: disable=broad-except
             _LOGGER.error("No plantbook token")
             raise
 
         url = f"{self._PLANTBOOK_BASEURL}/sensor-data/instance"
@@ -197,46 +201,52 @@
             "location_lon": location_lon,
             "location_lat": location_lat,
             # "location_name": "Sydney",
             # "location_region": "New South Wales"
         }
         # TODO TEST: Location values
         clean_items = api_payload.copy()
-        for k,v in clean_items.items():
+        for k, v in clean_items.items():
             if v is None:
                 api_payload.pop(k)
 
         try:
             async with aiohttp.ClientSession(raise_for_status=True, headers=headers) as session:
 
                 results = []
                 for custom_id_value, pid_value in sensor_pid_map.items():
 
+                    # TODO N: Multiple items is not working properly because if failure occurs with one of the items
+                    #  the entire transaction stops and partial result is observed. I need to continue to create
+                    #  until the end and report back only faulty ones or rollback (not possible) entire transaction
                     api_payload['custom_id'] = custom_id_value
                     api_payload['pid'] = pid_value
 
                     async with session.post(url, json=api_payload, raise_for_status=False) as result:
-                        _LOGGER.debug("Registered sensor %s", api_payload)
-
                         res = await result.json()
                         # TODO TEST: Handling not OK responses
-                        if str(result.status)[0] != "2":
-                            _LOGGER.error(str(result.status) + ' ' + result.reason + ": " + str(res))
-                            raise aiohttp.ClientError
+                        # if str(result.status)[0] != "2":
+                        #     _LOGGER.error(str(result.status) + ' ' + result.reason + ": " + str(res))
+                        if result.status == 400 and res['type'] == "validation_error":
+                            raise ValidationError(res['errors'])
+
+                            # else:
+                            #     raise aiohttp.ClientError
+                        result.raise_for_status()
 
                         results.append(res)
-
+                        _LOGGER.debug("Registered sensor: %s", api_payload)
 
                 return results
                 # TODO 2: Optimize as in https://www.twilio.com/blog/asynchronous-http-requests-in-python-with-aiohttp
                 #   tasks.append(asyncio.ensure_future(get_pokemon(session, url)))
                 # original_pokemon = await asyncio.gather(*tasks)
 
-        except ValidationError as err:
-            _LOGGER.error("Validation error {}".format(err))
+        except ValidationError as e:
+            # _LOGGER.error("Validation errors: {}".format(e))
             raise
 
         except aiohttp.ServerTimeoutError:
             # Maybe set up for a retry, or continue in a retry loop
             _LOGGER.error("Timeout connecting to {}".format(url))
             return None
         except aiohttp.TooManyRedirects:
@@ -391,9 +401,13 @@
 
 class MissingClientIdOrSecret(Exception):
     """Exception for missing client_id or token."""
     pass
 
 
 class ValidationError(Exception):
-    """Exception for validation error"""
-    pass
+    def __init__(self, errors, *args):
+        super().__init__(args)
+        self.errors = errors
+
+    def __str__(self):
+        return f'{self.errors}'
```

### Comparing `openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/PKG-INFO` & `openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplantbook-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Open Plantbook SDK for Python
 Home-page: https://github.com/slaxor505/openplantbook-sdk-py
 Author: Slava Pisarevskiy
 Author-email: slava@plantbook.io
 License: MIT
 Project-URL: Documentation, https://openplantbook-sdk-py.readthedocs.io
 Project-URL: Source, https://github.com/slaxor505/openplantbook-sdk-py
```

### Comparing `openplantbook-sdk-0.4.5/openplantbook_sdk.egg-info/SOURCES.txt` & `openplantbook_sdk-0.4.6/openplantbook_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openplantbook-sdk-0.4.5/setup.cfg` & `openplantbook_sdk-0.4.6/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openplantbook-sdk
-version = 0.4.5
+version = 0.4.6
 author = Slava Pisarevskiy
 author_email = slava@plantbook.io
 description = Open Plantbook SDK for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/slaxor505/openplantbook-sdk-py
 keywords = json, timeseries, iot, jts
```

### Comparing `openplantbook-sdk-0.4.5/tests/test_openplantbook_sdk.py` & `openplantbook_sdk-0.4.6/tests/test_openplantbook_sdk.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import numpy as np
 import pandas as pd
 import yaml
 from json_timeseries import TimeSeries, TsRecord, JtsDocument
 
 import openplantbook_sdk
+from openplantbook_sdk import ValidationError
 
 
 class TestSdk(unittest.TestCase):
     maxDiff = None
 
     def setUp(self):
         path = Path(__file__).parent / "../config.yaml"
@@ -45,30 +46,69 @@
         api = openplantbook_sdk.OpenPlantBookApi(self.client_id, self.client_secret, base_url=self.base_url)
 
         response = asyncio.run(api.async_plant_detail_get(self.test_pid))
 
         test_json = '''{"pid": "abelia chinensis", "display_pid": "Abelia chinensis", "alias": "chinese abelia", "category": "Caprifoliaceae, Abelia", "max_light_mmol": 4500, "min_light_mmol": 2500, "max_light_lux": 30000, "min_light_lux": 3500, "max_temp": 35, "min_temp": 8, "max_env_humid": 85, "min_env_humid": 30, "max_soil_moist": 60, "min_soil_moist": 15, "max_soil_ec": 2000, "min_soil_ec": 350, "image_url": "https://opb-img.plantbook.io/abelia%20chinensis.jpg"}'''
         self.assertEqual(json.dumps(response), test_json)
 
-    def test_plant_instance_register_multiple(self):
+    def test_plant_instance_register(self):
         api = openplantbook_sdk.OpenPlantBookApi(self.client_id, self.client_secret, base_url=self.base_url)
-        found_plants = asyncio.run(api.async_plant_search("acer"))['results'][:5]
+        # ONLY 1 plant registration is currently supported by SDK
+        found_plants = asyncio.run(api.async_plant_search("acer"))['results'][:1]
         pid_instance_map = {}
-        location_country = "Australia"
+        location_country = "AU"
         for i in range(len(found_plants)):
             the_pid = found_plants[i]['pid']
             pid_instance_map["Sensor-" + str(i)] = the_pid
         res = asyncio.run(
-            api.async_plant_instance_register(sensor_pid_map=pid_instance_map, location_country=location_country))
+            api.async_plant_instance_register(sensor_pid_map=pid_instance_map))
 
         for k, v in pid_instance_map.items():
             self.assertIn(k, json.dumps(res))
             self.assertIn(v, json.dumps(res))
             self.assertIn(location_country, json.dumps(res))
 
+    def test_plant_instance_register_invalid_pid(self):
+        api = openplantbook_sdk.OpenPlantBookApi(self.client_id, self.client_secret, base_url=self.base_url)
+
+        # Only 1 item creation is currently supported
+        found_plants = [({"pid": "non_existent_pid_1"})]
+
+        pid_instance_map = {}
+        for i in range(len(found_plants)):
+            the_pid = found_plants[i]['pid']
+            pid_instance_map["Sensor-" + str(i)] = the_pid
+
+        with self.assertRaises(ValidationError) as cm:
+            asyncio.run(api.async_plant_instance_register(sensor_pid_map=pid_instance_map))
+        errors = cm.exception.errors
+
+        self.assertEqual(len(errors), 1)
+        self.assertIn("non_existent_pid_1", errors[0]['detail'])
+        self.assertEqual("invalid_pid", errors[0]['code'])
+
+    def test_plant_instance_register_invalid_country(self):
+        api = openplantbook_sdk.OpenPlantBookApi(self.client_id, self.client_secret, base_url=self.base_url)
+
+        # Only 1 item creation is currently supported
+        found_plants = asyncio.run(api.async_plant_search("acer"))['results'][:1]
+
+        pid_instance_map = {}
+        location_country = "ZZ"
+        for i in range(len(found_plants)):
+            the_pid = found_plants[i]['pid']
+            pid_instance_map["Sensor-" + str(i)] = the_pid
+
+        with self.assertRaises(ValidationError) as cm:
+            asyncio.run(api.async_plant_instance_register(sensor_pid_map=pid_instance_map, location_country=location_country))
+        errors = cm.exception.errors
+
+        self.assertEqual(len(errors), 1)
+        self.assertEqual(errors[0]['code'], "invalid_location_country")
+
     def test_plant_data_upload(self):
         api = openplantbook_sdk.OpenPlantBookApi(self.client_id, self.client_secret, base_url=self.base_url)
 
         found_plants = asyncio.run(api.async_plant_search("acer"))['results'][:5]
         pid_instance_map = {}
         jts_doc = JtsDocument()
         for i in range(len(found_plants)):
@@ -78,15 +118,15 @@
             # Corresponding PID/Plant ID
             the_pid = found_plants[i]['pid']
 
             # pid_instance_map["Sensor-"+str(i)]=the_pid
 
             # Register Plant Instance
             res = asyncio.run(
-                api.async_plant_instance_register(sensor_pid_map={sensor_id: the_pid}, location_country="Australia",
+                api.async_plant_instance_register(sensor_pid_map={sensor_id: the_pid}, location_country="AU",
                 location_lat=-33.8678500, location_lon=151.2073200))
 
             custom_id = res[0].get('id')
             # the same "plant_id" but different sensors identified by "name"
             temp = TimeSeries(identifier=custom_id, name="temp")
             soil_moist = TimeSeries(identifier=custom_id, name="soil_moist")
             soil_ec = TimeSeries(identifier=custom_id, name="soil_ec")
```

