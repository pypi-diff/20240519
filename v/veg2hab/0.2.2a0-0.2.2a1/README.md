# Comparing `tmp/veg2hab-0.2.2a0.tar.gz` & `tmp/veg2hab-0.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veg2hab-0.2.2a0.tar", max compression
+gzip compressed data, was "veg2hab-0.2.2a1.tar", max compression
```

## Comparing `veg2hab-0.2.2a0.tar` & `veg2hab-0.2.2a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7626 2024-05-17 01:04:43.905056 veg2hab-0.2.2a0/LICENSE.md
--rw-r--r--   0        0        0    12995 2024-05-17 01:04:43.905056 veg2hab-0.2.2a0/README.md
--rw-r--r--   0        0        0     1328 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/__init__.py
--rw-r--r--   0        0        0     1086 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/__main__.py
--rw-r--r--   0        0        0     6540 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/access_db.py
--rw-r--r--   0        0        0      411 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/constants.py
--rw-r--r--   0        0        0     6408 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/criteria.py
--rw-r--r--   0        0        0     8640 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/definitietabel.py
--rw-r--r--   0        0        0     5151 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/enums.py
--rw-r--r--   0        0        0      576 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/fgr.py
--rw-r--r--   0        0        0    15989 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/habitat.py
--rw-r--r--   0        0        0     6946 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/io/arcgis.py
--rw-r--r--   0        0        0     2673 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/io/cli.py
--rw-r--r--   0        0        0     5305 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/io/common.py
--rw-r--r--   0        0        0     3051 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/main.py
--rw-r--r--   0        0        0    10867 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/mozaiek.py
--rw-r--r--   0        0        0 13900219 2024-05-17 01:04:44.345060 veg2hab-0.2.2a0/veg2hab/package_data/FGR.json
--rw-r--r--   0        0        0      130 2024-05-17 01:04:45.073068 veg2hab-0.2.2a0/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
--rw-r--r--   0        0        0      130 2024-05-17 01:04:45.073068 veg2hab-0.2.2a0/veg2hab/package_data/opgeschoonde_waswordt.xlsx
--rw-r--r--   0        0        0     2653 2024-05-17 01:04:45.073068 veg2hab-0.2.2a0/veg2hab/package_data/veg2hab.pyt
--rw-r--r--   0        0        0    13084 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/validation.py
--rw-r--r--   0        0        0    15272 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/vegetatietypen.py
--rw-r--r--   0        0        0    47885 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/vegkartering.py
--rw-r--r--   0        0        0     4585 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/waswordtlijst.py
--rw-r--r--   0        0        0    14101 1970-01-01 00:00:00.000000 veg2hab-0.2.2a0/PKG-INFO
+-rw-r--r--   0        0        0     7626 2024-05-17 17:11:00.254874 veg2hab-0.2.2a1/LICENSE.md
+-rw-r--r--   0        0        0    12995 2024-05-17 17:11:00.254874 veg2hab-0.2.2a1/README.md
+-rw-r--r--   0        0        0     1328 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/__init__.py
+-rw-r--r--   0        0        0     1086 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/__main__.py
+-rw-r--r--   0        0        0     6540 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/access_db.py
+-rw-r--r--   0        0        0      411 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/constants.py
+-rw-r--r--   0        0        0     6408 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/criteria.py
+-rw-r--r--   0        0        0     8640 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/definitietabel.py
+-rw-r--r--   0        0        0     5151 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/enums.py
+-rw-r--r--   0        0        0      576 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/fgr.py
+-rw-r--r--   0        0        0    15989 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/habitat.py
+-rw-r--r--   0        0        0     6946 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/io/arcgis.py
+-rw-r--r--   0        0        0     2673 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/io/cli.py
+-rw-r--r--   0        0        0     5305 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/io/common.py
+-rw-r--r--   0        0        0     3051 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/main.py
+-rw-r--r--   0        0        0    10867 2024-05-17 17:11:00.654874 veg2hab-0.2.2a1/veg2hab/mozaiek.py
+-rw-r--r--   0        0        0 13900219 2024-05-17 17:11:00.706874 veg2hab-0.2.2a1/veg2hab/package_data/FGR.json
+-rw-r--r--   0        0        0    39321 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
+-rw-r--r--   0        0        0    19151 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/package_data/opgeschoonde_waswordt.xlsx
+-rw-r--r--   0        0        0     2626 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/package_data/veg2hab.pyt
+-rw-r--r--   0        0        0    13084 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/validation.py
+-rw-r--r--   0        0        0    15272 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/vegetatietypen.py
+-rw-r--r--   0        0        0    47885 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/vegkartering.py
+-rw-r--r--   0        0        0     4585 2024-05-17 17:11:00.730874 veg2hab-0.2.2a1/veg2hab/waswordtlijst.py
+-rw-r--r--   0        0        0    14101 1970-01-01 00:00:00.000000 veg2hab-0.2.2a1/PKG-INFO
```

### Comparing `veg2hab-0.2.2a0/LICENSE.md` & `veg2hab-0.2.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/README.md` & `veg2hab-0.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/pyproject.toml` & `veg2hab-0.2.2a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "veg2hab"
-version = "0.2.2a0"
+version = "0.2.2a1"
 description = "Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten"
 authors = ["Spheer.ai <info@spheer.ai>"]
 readme = "README.md"
 license = "LGPLv3"
 classifiers = [
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
```

### Comparing `veg2hab-0.2.2a0/veg2hab/__main__.py` & `veg2hab-0.2.2a1/veg2hab/__main__.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/access_db.py` & `veg2hab-0.2.2a1/veg2hab/access_db.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/criteria.py` & `veg2hab-0.2.2a1/veg2hab/criteria.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/definitietabel.py` & `veg2hab-0.2.2a1/veg2hab/definitietabel.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/enums.py` & `veg2hab-0.2.2a1/veg2hab/enums.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/fgr.py` & `veg2hab-0.2.2a1/veg2hab/fgr.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/habitat.py` & `veg2hab-0.2.2a1/veg2hab/habitat.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/io/arcgis.py` & `veg2hab-0.2.2a1/veg2hab/io/arcgis.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/io/cli.py` & `veg2hab-0.2.2a1/veg2hab/io/cli.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/io/common.py` & `veg2hab-0.2.2a1/veg2hab/io/common.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/main.py` & `veg2hab-0.2.2a1/veg2hab/main.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/mozaiek.py` & `veg2hab-0.2.2a1/veg2hab/mozaiek.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/package_data/FGR.json` & `veg2hab-0.2.2a1/veg2hab/package_data/FGR.json`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/package_data/veg2hab.pyt` & `veg2hab-0.2.2a1/veg2hab/package_data/veg2hab.pyt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Type, Union
 
 import veg2hab.io.arcgis
 import veg2hab.main
 import veg2hab.constants
 import logging
 
-SUPPORTED_VERSIONS = ["0.1.0", "0.1.1", "0.2.1", "0.2.2a0"]
+SUPPORTED_VERSIONS = ["0.2.2a1"]
 
 # this instantiates the arcgis interface and configures the logging
 veg2hab.io.arcgis.ArcGISInterface.get_instance().instantiate_loggers()
 
 class Toolbox:
     def __init__(self):
         """Define the toolbox (the name of the toolbox is the name of the
```

### Comparing `veg2hab-0.2.2a0/veg2hab/validation.py` & `veg2hab-0.2.2a1/veg2hab/validation.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/vegetatietypen.py` & `veg2hab-0.2.2a1/veg2hab/vegetatietypen.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/vegkartering.py` & `veg2hab-0.2.2a1/veg2hab/vegkartering.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/veg2hab/waswordtlijst.py` & `veg2hab-0.2.2a1/veg2hab/waswordtlijst.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.2a0/PKG-INFO` & `veg2hab-0.2.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veg2hab
-Version: 0.2.2a0
+Version: 0.2.2a1
 Summary: Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten
 License: LGPLv3
 Author: Spheer.ai
 Author-email: info@spheer.ai
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: Other/Proprietary License
```

