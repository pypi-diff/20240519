# Comparing `tmp/threed_optix-5.0.7.tar.gz` & `tmp/threed_optix-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-5.0.7.tar", last modified: Tue May  7 09:43:00 2024, max compression
+gzip compressed data, was "threed_optix-5.0.9.tar", last modified: Thu May  9 10:39:49 2024, max compression
```

## Comparing `threed_optix-5.0.7.tar` & `threed_optix-5.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:43:00.153022 threed_optix-5.0.7/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.7/.gitignore
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.7/LICENSE.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 09:43:00.153022 threed_optix-5.0.7/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.7/README.md
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:43:00.153022 threed_optix-5.0.7/help/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.7/help/SDK help text.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.7/help/SDK help.md
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 09:43:00.153022 threed_optix-5.0.7/setup.cfg
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1222 2024-05-06 11:41:26.000000 threed_optix-5.0.7/setup.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:43:00.153022 threed_optix-5.0.7/src/
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:43:00.153022 threed_optix-5.0.7/src/threed_optix/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      844 2024-05-06 11:41:26.000000 threed_optix-5.0.7/src/threed_optix/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23949 2024-05-07 07:32:41.000000 threed_optix-5.0.7/src/threed_optix/analyses.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.7/src/threed_optix/beams.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43648 2024-05-07 07:32:41.000000 threed_optix-5.0.7/src/threed_optix/client.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.7/src/threed_optix/optimize.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:43:00.153022 threed_optix-5.0.7/src/threed_optix/package_utils/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.7/src/threed_optix/package_utils/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15738 2024-05-07 09:42:39.000000 threed_optix-5.0.7/src/threed_optix/package_utils/api.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3248 2024-05-07 07:32:41.000000 threed_optix-5.0.7/src/threed_optix/package_utils/general.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.7/src/threed_optix/package_utils/math.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.7/src/threed_optix/package_utils/matlab.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19177 2024-05-07 09:42:57.000000 threed_optix-5.0.7/src/threed_optix/package_utils/vars.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-07 07:32:32.000000 threed_optix-5.0.7/src/threed_optix/parts.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15046 2024-05-06 11:41:26.000000 threed_optix-5.0.7/src/threed_optix/simulations.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4719 2024-05-07 07:32:41.000000 threed_optix-5.0.7/src/threed_optix/utils.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-07 09:43:00.153022 threed_optix-5.0.7/src/threed_optix.egg-info/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-07 09:43:00.000000 threed_optix-5.0.7/src/threed_optix.egg-info/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-07 09:43:00.000000 threed_optix-5.0.7/src/threed_optix.egg-info/SOURCES.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-07 09:43:00.000000 threed_optix-5.0.7/src/threed_optix.egg-info/dependency_links.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-07 09:43:00.000000 threed_optix-5.0.7/src/threed_optix.egg-info/requires.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-07 09:43:00.000000 threed_optix-5.0.7/src/threed_optix.egg-info/top_level.txt
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-09 10:39:49.788513 threed_optix-5.0.9/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.9/.gitignore
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.9/LICENSE.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-09 10:39:49.788513 threed_optix-5.0.9/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.9/README.md
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-09 10:39:49.788513 threed_optix-5.0.9/help/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.9/help/SDK help text.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43940 2024-05-06 11:41:26.000000 threed_optix-5.0.9/help/SDK help.md
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-09 10:39:49.788513 threed_optix-5.0.9/setup.cfg
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1242 2024-05-09 10:38:32.000000 threed_optix-5.0.9/setup.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-09 10:39:49.788513 threed_optix-5.0.9/src/
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-09 10:39:49.788513 threed_optix-5.0.9/src/threed_optix/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      885 2024-05-09 10:38:32.000000 threed_optix-5.0.9/src/threed_optix/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23944 2024-05-09 10:38:32.000000 threed_optix-5.0.9/src/threed_optix/analyses.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.9/src/threed_optix/beams.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43810 2024-05-09 10:38:32.000000 threed_optix-5.0.9/src/threed_optix/client.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.9/src/threed_optix/optimize.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-09 10:39:49.788513 threed_optix-5.0.9/src/threed_optix/package_utils/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.9/src/threed_optix/package_utils/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15738 2024-05-09 10:38:32.000000 threed_optix-5.0.9/src/threed_optix/package_utils/api.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3248 2024-05-07 07:32:41.000000 threed_optix-5.0.9/src/threed_optix/package_utils/general.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.9/src/threed_optix/package_utils/math.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.9/src/threed_optix/package_utils/matlab.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19122 2024-05-09 10:38:32.000000 threed_optix-5.0.9/src/threed_optix/package_utils/vars.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    61029 2024-05-09 10:37:13.000000 threed_optix-5.0.9/src/threed_optix/parts.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15382 2024-05-09 10:38:32.000000 threed_optix-5.0.9/src/threed_optix/simulations.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4719 2024-05-07 07:32:41.000000 threed_optix-5.0.9/src/threed_optix/utils.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-09 10:39:49.788513 threed_optix-5.0.9/src/threed_optix.egg-info/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-09 10:39:49.000000 threed_optix-5.0.9/src/threed_optix.egg-info/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-09 10:39:49.000000 threed_optix-5.0.9/src/threed_optix.egg-info/SOURCES.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-09 10:39:49.000000 threed_optix-5.0.9/src/threed_optix.egg-info/dependency_links.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      116 2024-05-09 10:39:49.000000 threed_optix-5.0.9/src/threed_optix.egg-info/requires.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-09 10:39:49.000000 threed_optix-5.0.9/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-5.0.7/LICENSE.txt` & `threed_optix-5.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/PKG-INFO` & `threed_optix-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed_optix
-Version: 5.0.7
+Version: 5.0.9
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.7/README.md` & `threed_optix-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/help/SDK help text.txt` & `threed_optix-5.0.9/help/SDK help text.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/help/SDK help.md` & `threed_optix-5.0.9/help/SDK help.md`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/setup.py` & `threed_optix-5.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     keywords=["Optics", "Optical Design", "Optical Simulation", "Optical Design Software", "3DOptix"],
     install_requires=[
         'requests',
         'pandas',
         'matplotlib',
         'plotly',
         'colorama',
+        'nbformat',
         'numpy',
         'scikit-image',
         'scipy',
         'opencv-python',
         'dill',
         "ply",
         "networkx",
```

### Comparing `threed_optix-5.0.7/src/threed_optix/__init__.py` & `threed_optix-5.0.9/src/threed_optix/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .utils import *
 from . import package_utils
 from . import optimize
 
 # Allow users to easily access the enums
 from .package_utils.vars import eOpticsSubtypes, ANALYSIS_NAMES, Setups, Coating, SETUP_LABELS
 
+__version__ = package_utils.vars.VERSION
 GRATING_SUBTYPES = eOpticsSubtypes.GRATING_SUBTYPES
 SETUP_LABELS = Setups.SETUP_LABELS
 
 # Enter debug mode, which will print out pretty much every step of the way.
 def debug(boolean = None):
 
     # If the user has specified a boolean, set the debug mode to that value.
```

### Comparing `threed_optix-5.0.7/src/threed_optix/analyses.py` & `threed_optix-5.0.9/src/threed_optix/analyses.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         os.system(f'rm -rf {directory}')
         self.reset()
         return self.results
 
     def reset(self):
         self._urls = []
         self._raw_results = {}
-        return None
+        return
 
     def _check_file_version(self, file_path):
         version_bytes  =v.AnalysisFile2.VERSION_BYTES
         with open(file_path, 'rb') as f:
             # versin bytes is the range of the 4 bytes indicating the int32 version number. The first int is the beginning, the second is the end
             f.seek(version_bytes[0])
             version = struct.unpack('i', f.read(version_bytes[1] - version_bytes[0]))[0]
```

### Comparing `threed_optix-5.0.7/src/threed_optix/beams.py` & `threed_optix-5.0.9/src/threed_optix/beams.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/src/threed_optix/client.py` & `threed_optix-5.0.9/src/threed_optix/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1004,36 +1004,38 @@
                      auto_add: bool = False,
                      force: bool = False
                      ) -> bool:
         if auto_add:
             self._add_analysis(analysis, force = force)
 
         data, _ =  au._run_analysis(setup_id=analysis.surface._part._setup.id, api_key=self.api_key, analysis_id=analysis.id)
+        if v.ORIGIN == '0':
+            if data['results']['error']['code'] != 0:
+                raise Exception(data['results']['error']['message'])
 
-        if data['results']['error']['code'] != 0:
-            raise Exception(data['results']['error']['message'])
+            maps_url = data['maps_url']
+            analysis._maps_json = requests.get(maps_url).json()
 
-        maps_url = data['maps_url']
-        analysis._maps_json = requests.get(maps_url).json()
+            if v.DEBUG:
+                print(f'Maps json is {analysis._maps_json}')
 
-        if v.DEBUG:
-            print(f'Maps json is {analysis._maps_json}')
 
+            analysis_datos = data['results']['data']['analysis']
+            analysis._urls = [data['url'] for data in analysis_datos]
 
-        analysis_datos = data['results']['data']['analysis']
-        for data in analysis_datos:
-            url = data['url']
-            analysis._urls.append(url)
+            if v.DEBUG:
+                print(f'Analysis urls is {analysis._urls}')
 
-        if v.DEBUG:
-            print(f'Analysis urls is {analysis._urls}')
+            analysis.results = analysis._process_results()
 
-        analysis.results = analysis._process_results()
+            return copy.deepcopy(analysis.results)
+
+        if v.ORIGIN == '1':
+            return {'status': 'success', 'message': f'Analysis {analysis.id} ran successfully'}
 
-        return copy.deepcopy(analysis.results)
 
     def _run_analyses(self,
                      analyses: list,
                      auto_add: bool = False,
                      force:bool = False
                      ):
         '''
```

### Comparing `threed_optix-5.0.7/src/threed_optix/package_utils/api.py` & `threed_optix-5.0.9/src/threed_optix/package_utils/api.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/src/threed_optix/package_utils/general.py` & `threed_optix-5.0.9/src/threed_optix/package_utils/general.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/src/threed_optix/package_utils/math.py` & `threed_optix-5.0.9/src/threed_optix/package_utils/math.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/src/threed_optix/package_utils/vars.py` & `threed_optix-5.0.9/src/threed_optix/package_utils/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import re
 
 DEBUG = False
 BASE_BACKUP = 'DEFAULT'
 VALID_RESPONSE_CODES = [200, 201, 202, 204]
 # Take the version of the package
-VERSION = "5.0.7"
+VERSION = "5.0.9"
 
 
 #Base API URL
 API_URL = "https://api.3doptix.com/v1"
 ORIGIN = '0' #0 for origin that is a human user
 
 class Surfaces:
@@ -33,15 +33,14 @@
     VALID_LIGHT_SOURCE_ARGUMENTS = ['wavelengths', 'add_wavelengths', 'power', 'vis_count', 'vis_count_type', 'rays_direction', 'opacity', 'color', 'gaussian_beam', 'point_source', 'plane_wave'] + VALID_PART_ARGUMENTS
 
 
 #GET endpoints
 GET_SETUPS_ENDPOINT = 'setups'
 GET_SETUP_ENDPOINT = 'setups/{setup_id}'
 GET_PART_ENDPOINT = 'setups/{setup_id}/parts/{part_id}'
-GET_ANSWER_ENDPOINT = 'http://chatbot.5doptix.com/ask'
 MAX_HISTORY_LEN = 5
 
 # DELETE endpoints
 DELETE_PART_ENDPOINT = 'setups/{setup_id}/parts/{part_id}'
 
 #PUT endpoints
 PUT_BATCH_CHANGES_ENDPOINT = "setups/{setup_id}/batch_changes"
```

### Comparing `threed_optix-5.0.7/src/threed_optix/parts.py` & `threed_optix-5.0.9/src/threed_optix/parts.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/src/threed_optix/simulations.py` & `threed_optix-5.0.9/src/threed_optix/simulations.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,23 @@
         '''
         part = self._api._get_part(part_id, self.id)
         return part
 
     def _get_surface(self, part_id, surface_id):
         return self._api._get_surface(setup_id = self.id, part_id=part_id, surface_id=surface_id)
 
+    def add_analysis(self, analysis, force = False):
+        analysis.surface.add_analysis(analysis, force = force)
+        return
+
+    def delete_analysis(self, analysis: Union[str, tdo_analyses.Analysis]):
+        analysis.surface.delete_analysis(analysis)
+        return
+
+
     def get(self,
             part_label: str,
             all: bool = False):
         """
         Returns the part object with the specified label.
 
         Args:
@@ -216,15 +225,15 @@
                     parts.append(part)
             return parts
 
         for part in self:
             if part.label == part_label:
                 return part
 
-        return None
+        raise KeyError(f"Part with label {part_label} not found in the setup.")
 
     def at(self, location: tuple):
         """
         Private.
         Returns the closest part object to the specified location in the global coordinate system.
 
         Args:
```

### Comparing `threed_optix-5.0.7/src/threed_optix/utils.py` & `threed_optix-5.0.9/src/threed_optix/utils.py`

 * *Files identical despite different names*

### Comparing `threed_optix-5.0.7/src/threed_optix.egg-info/PKG-INFO` & `threed_optix-5.0.9/src/threed_optix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed-optix
-Version: 5.0.7
+Version: 5.0.9
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-5.0.7/src/threed_optix.egg-info/SOURCES.txt` & `threed_optix-5.0.9/src/threed_optix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

