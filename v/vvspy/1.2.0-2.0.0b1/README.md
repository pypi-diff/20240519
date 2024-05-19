# Comparing `tmp/vvspy-1.2.0.tar.gz` & `tmp/vvspy-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvspy-1.2.0.tar", last modified: Sun Sep 18 07:36:03 2022, max compression
+gzip compressed data, was "vvspy-2.0.0b1.tar", last modified: Sun May 19 13:50:33 2024, max compression
```

## Comparing `vvspy-1.2.0.tar` & `vvspy-2.0.0b1.tar`

### file list

```diff
@@ -1,46 +1,33 @@
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2022-09-18 07:36:03.626421 vvspy-1.2.0/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1071 2022-05-27 15:56:32.000000 vvspy-1.2.0/LICENSE
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      116 2022-05-27 15:27:32.000000 vvspy-1.2.0/MANIFEST.in
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4687 2022-09-18 07:36:03.626421 vvspy-1.2.0/PKG-INFO
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3925 2022-05-27 15:38:06.000000 vvspy-1.2.0/readme.md
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       52 2022-05-27 15:27:32.000000 vvspy-1.2.0/requirements.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       79 2022-09-18 07:36:03.626421 vvspy-1.2.0/setup.cfg
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1108 2022-09-18 07:35:51.000000 vvspy-1.2.0/setup.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2022-09-18 07:36:03.622421 vvspy-1.2.0/vvspy/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5389 2022-09-18 07:35:51.000000 vvspy-1.2.0/vvspy/__init__.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2022-09-18 07:36:03.626421 vvspy-1.2.0/vvspy/__pycache__/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3388 2022-09-18 07:10:40.000000 vvspy-1.2.0/vvspy/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4004 2022-09-18 07:10:40.000000 vvspy-1.2.0/vvspy/__pycache__/arrivals.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3953 2022-09-18 07:10:40.000000 vvspy-1.2.0/vvspy/__pycache__/departures.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4720 2022-09-18 07:10:40.000000 vvspy-1.2.0/vvspy/__pycache__/trip.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4992 2022-09-18 07:35:51.000000 vvspy-1.2.0/vvspy/arrivals.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4941 2022-09-18 07:35:51.000000 vvspy-1.2.0/vvspy/departures.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2022-09-18 07:36:03.626421 vvspy-1.2.0/vvspy/obj/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      334 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/__init__.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2022-09-18 07:36:03.626421 vvspy-1.2.0/vvspy/obj/__pycache__/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      547 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3525 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/arrival.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2694 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/connection.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3395 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/departure.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2256 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/destination.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1071 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/line_operator.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2229 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/origin.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2545 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/serving_line.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1761 2022-05-27 15:28:00.000000 vvspy-1.2.0/vvspy/obj/__pycache__/transportation.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1922 2022-05-27 15:36:46.000000 vvspy-1.2.0/vvspy/obj/__pycache__/trip.cpython-38.pyc
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4071 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/arrival.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2832 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/connection.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3931 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/departure.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2205 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/destination.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      663 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/line_operator.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2246 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/origin.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2340 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/serving_line.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1561 2022-05-27 15:27:32.000000 vvspy-1.2.0/vvspy/obj/transportation.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1384 2022-05-27 15:36:34.000000 vvspy-1.2.0/vvspy/obj/trip.py
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     6040 2022-09-18 07:35:51.000000 vvspy-1.2.0/vvspy/trip.py
-drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2022-09-18 07:36:03.626421 vvspy-1.2.0/vvspy.egg-info/
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4687 2022-09-18 07:36:03.000000 vvspy-1.2.0/vvspy.egg-info/PKG-INFO
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1153 2022-09-18 07:36:03.000000 vvspy-1.2.0/vvspy.egg-info/SOURCES.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        1 2022-09-18 07:36:03.000000 vvspy-1.2.0/vvspy.egg-info/dependency_links.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       16 2022-09-18 07:36:03.000000 vvspy-1.2.0/vvspy.egg-info/requires.txt
--rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        6 2022-09-18 07:36:03.000000 vvspy-1.2.0/vvspy.egg-info/top_level.txt
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.830130 vvspy-2.0.0b1/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1071 2024-05-19 11:23:13.000000 vvspy-2.0.0b1/LICENSE
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      207 2024-05-19 11:25:25.000000 vvspy-2.0.0b1/MANIFEST.in
+-rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5250 2024-05-19 13:50:33.830130 vvspy-2.0.0b1/PKG-INFO
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      313 2024-05-19 13:47:44.000000 vvspy-2.0.0b1/pyproject.toml
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4186 2024-05-19 13:41:30.000000 vvspy-2.0.0b1/readme.md
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       33 2024-05-19 11:23:47.000000 vvspy-2.0.0b1/requirements.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       38 2024-05-19 13:50:33.830130 vvspy-2.0.0b1/setup.cfg
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1395 2024-05-19 13:50:26.000000 vvspy-2.0.0b1/setup.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.825130 vvspy-2.0.0b1/vvspy/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5499 2024-05-19 13:11:28.000000 vvspy-2.0.0b1/vvspy/__init__.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4906 2024-05-19 13:20:17.000000 vvspy-2.0.0b1/vvspy/arrivals.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4794 2024-05-19 13:20:15.000000 vvspy-2.0.0b1/vvspy/departures.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.826130 vvspy-2.0.0b1/vvspy/enums/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)  1576406 2024-05-19 12:37:53.000000 vvspy-2.0.0b1/vvspy/enums/stations.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.829130 vvspy-2.0.0b1/vvspy/models/
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      334 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/__init__.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     4071 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/arrival.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2832 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/connection.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     3931 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/departure.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2205 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/destination.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      663 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/line_operator.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2246 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/origin.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     2340 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/serving_line.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1561 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/transportation.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     1384 2024-05-19 10:57:56.000000 vvspy-2.0.0b1/vvspy/models/trip.py
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)     5964 2024-05-19 13:19:51.000000 vvspy-2.0.0b1/vvspy/trip.py
+drwxrwxr-x   0 zaanposni  (1000) zaanposni  (1000)        0 2024-05-19 13:50:33.829130 vvspy-2.0.0b1/vvspy.egg-info/
+-rw-r--r--   0 zaanposni  (1000) zaanposni  (1000)     5250 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/PKG-INFO
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)      572 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        1 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)       16 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/requires.txt
+-rw-rw-r--   0 zaanposni  (1000) zaanposni  (1000)        6 2024-05-19 13:50:33.000000 vvspy-2.0.0b1/vvspy.egg-info/top_level.txt
```

### Comparing `vvspy-1.2.0/LICENSE` & `vvspy-2.0.0b1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2022 zaanposni
+Copyright (c) 2019-2024 zaanposni
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `vvspy-1.2.0/setup.py` & `vvspy-2.0.0b1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-  name='vvspy',
-  py_modules=["vvspy"],
-  version='1.2.0',
-  license='MIT',
-  description='API Wrapper for VVS (Verkehrsverbund Stuttgart)',
-  author='zaanposni',
-  author_email='zaanposni@users.noreply.github.com',
-  url='https://github.com/FI18-Trainees/vvspy',
-  keywords=['VVS', 'API', 'STUTTGART', 'WRAPPER', 'JSON', 'REST', 'EFA', 'PYTHON'],
-  packages=find_packages(exclude=["*tests"]),
-  package_data={
-    "vvspy": ["vvspy/*"]
-  },
-  install_requires=[
-          'requests',
-          'typing',
-      ],
-  classifiers=[
-    'Development Status :: 5 - Production/Stable',
-    'Intended Audience :: Developers',
-    'Topic :: Software Development :: Build Tools',
-    'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
-    'Programming Language :: Python :: 3.8',
-  ],
-  long_description=long_description,
-  long_description_content_type="text/markdown"
+    name="vvspy",
+    version="2.0.0-beta.1",
+    license="MIT",
+    description="API Wrapper for VVS (Verkehrsverbund Stuttgart)",
+    author="zaanposni",
+    author_email="vvspy@zaanposni.com",
+    url="https://github.com/zaanposni/vvspy",
+    keywords=["vvs", "api", "stuttgart", "wrapper", "json", "rest", "efa", "python"],
+    packages=find_packages(exclude=["*tests"]),
+    package_data={"vvspy": ["vvspy/*"]},
+    python_requires=">=3.6",
+    install_requires=[
+        "requests",
+        "typing",
+    ],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Operating System :: OS Independent",
+    ],
+    long_description=long_description,
+    long_description_content_type="text/markdown",
 )
```

### Comparing `vvspy-1.2.0/vvspy/__init__.py` & `vvspy-2.0.0b1/vvspy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,189 +1,187 @@
 from datetime import datetime as __datetime
 from typing import List as __List
 from typing import Union as __Union
 from requests.models import Response as __Response
 from requests import Session
+import logging as __logging
 
-from .obj import Arrival as __Arrival
-from .obj import Departure as __Departure
-from .obj import Trip as __Trip
+from .enums.stations import Station
+from .models import Arrival as __Arrival
+from .models import Departure as __Departure
+from .models import Trip as __Trip
 from .trip import get_trips
 from .departures import get_departures
 from .arrivals import get_arrivals
 
 
+__logger = __logging.getLogger("vvspy")
+
 def departures_now(
-    station_id: __Union[str, int],
+    station_id: __Union[str, int, Station],
     limit: int = 100,
     return_resp: bool = False,
     session: Session = None,
-    **kwargs
+    **kwargs,
 ) -> __Union[__List[__Departure], __Response, None]:
     """
     Same as `get_departures`
     But `datetime.datetime.now()` is already used as parameter.
 
-    Returns: List[:class:`vvspy.obj.Departure`]
+    Returns: List[:class:`vvspy.models.Departure`]
     Returns none on webrequest errors or no results found.
 
     """
     return get_departures(
         station_id=station_id,
         check_time=__datetime.now(),
         limit=limit,
         return_resp=return_resp,
         session=session,
-        **kwargs
+        **kwargs,
     )
 
 
 def get_departure(
-    station_id: __Union[str, int],
+    station_id: __Union[str, int, Station],
     check_time: __datetime = None,
     debug: bool = False,
     request_params: dict = None,
     return_resp: bool = False,
     session: Session = None,
-    **kwargs
+    **kwargs,
 ) -> __Union[__Departure, __Response, None]:
     """
     Same as `get_departures`
     But limited to one obj as result.
 
-    Returns: :class:`vvspy.obj.Departure`
+    Returns: :class:`vvspy.models.Departure`
     Returns none on webrequest errors or no results found.
 
     """
     try:
         if return_resp:
             return get_departures(
                 station_id=station_id,
                 check_time=check_time,
                 limit=1,
                 debug=debug,
                 request_params=request_params,
                 return_resp=return_resp,
                 session=session,
-                **kwargs
+                **kwargs,
             )
         else:
             return get_departures(
                 station_id=station_id,
                 check_time=check_time,
                 limit=1,
                 debug=debug,
                 request_params=request_params,
                 return_resp=return_resp,
                 session=session,
-                **kwargs
+                **kwargs,
             )[0]
-    except IndexError:  # no results returned
-        if debug:
-            print("No departures found.")
-        return
-    except TypeError:  # none returned | most likely an error
-        if debug:
-            print("Error on webrequest")
-        return
+    except IndexError as e:  # no results returned
+        __logger.error(f"No departures found. {e}")
+        raise e
+    except TypeError as e:  # none returned | most likely an error
+        __logger.error(f"Error on webrequest. {e}")
+        raise e
 
 
 def get_arrival(
-    station_id: __Union[str, int],
+    station_id: __Union[str, int, Station],
     check_time: __datetime = None,
     debug: bool = False,
     request_params: dict = None,
     return_resp: bool = False,
     session: Session = None,
-    **kwargs
+    **kwargs,
 ) -> __Union[__Arrival, __Response, None]:
     """
     Same as `get_arrivals`
     But limited to one obj as result.
 
-    Returns: :class:`vvspy.obj.Arrival`
+    Returns: :class:`vvspy.models.Arrival`
     Returns none on webrequest errors or no results found.
 
     """
     try:
         if return_resp:
             return get_arrivals(
                 station_id=station_id,
                 check_time=check_time,
                 limit=1,
                 debug=debug,
                 request_params=request_params,
                 return_resp=return_resp,
                 session=session,
-                **kwargs
+                **kwargs,
             )
         else:
             return get_arrivals(
                 station_id=station_id,
                 check_time=check_time,
                 limit=1,
                 debug=debug,
                 request_params=request_params,
                 return_resp=return_resp,
                 session=session,
-                **kwargs
+                **kwargs,
             )[0]
-    except IndexError:  # no results returned
-        if debug:
-            print("No arrivals found.")
-        return
-    except TypeError:  # none returned | most likely an error
-        if debug:
-            print("Error on webrequest")
-        return
+    except IndexError as e:  # no results returned
+        __logger.error(f"No arrivals found. {e}")
+        raise e
+    except TypeError as e:  # none returned | most likely an error
+        __logger.error(f"Error on webrequest. {e}")
+        raise e
 
 
 def get_trip(
-    origin_station_id: __Union[str, int],
-    destination_station_id: __Union[str, int],
+    origin_station_id: __Union[str, int, Station],
+    destination_station_id: __Union[str, int, Station],
     check_time: __datetime = None,
     debug: bool = False,
     request_params: dict = None,
     return_resp: bool = False,
     session: Session = None,
-    **kwargs
+    **kwargs,
 ) -> __Union[__Trip, __Response, None]:
     """
     Same as `get_trips`
     But limited to one obj as result.
 
-    Returns: :class:`vvspy.obj.Trip`
+    Returns: :class:`vvspy.models.Trip`
     Returns none on webrequest errors or no results found.
 
     """
     try:
         if return_resp:
             return get_trips(
                 origin_station_id=origin_station_id,
                 destination_station_id=destination_station_id,
                 check_time=check_time,
                 limit=1,
                 debug=debug,
                 request_params=request_params,
                 return_resp=return_resp,
                 session=session,
-                **kwargs
+                **kwargs,
             )
         else:
             return get_trips(
                 origin_station_id=origin_station_id,
                 destination_station_id=destination_station_id,
                 check_time=check_time,
                 limit=1,
                 debug=debug,
                 request_params=request_params,
                 session=session,
-                **kwargs
+                **kwargs,
             )[0]
-    except IndexError:  # no results returned
-        if debug:
-            print("No trips found.")
-        return
-    except TypeError:  # none returned | most likely an error
-        if debug:
-            print("Error on webrequest")
-        return
+    except IndexError as e:
+        __logger.error(f"No trips found. {e}")
+        raise e
+    except TypeError as e:
+        __logger.error(f"Error on webrequest. {e}")
+        raise e
```

### Comparing `vvspy-1.2.0/vvspy/arrivals.py` & `vvspy-2.0.0b1/vvspy/departures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,136 @@
 from typing import List, Union
 from datetime import datetime
 import requests
 from requests.models import Response
 import json
-import traceback
+import logging as __logging
 
-from .obj import Arrival
+from .enums.stations import Station
+from vvspy.models import Departure
 
-_API_URL = "http://www3.vvs.de/vvs/widget/XML_DM_REQUEST?"
+__API_URL = "http://www3.vvs.de/vvs/widget/XML_DM_REQUEST?"
+__logger = __logging.getLogger("vvspy")
 
-
-def get_arrivals(
-    station_id: Union[str, int],
+def get_departures(
+    station_id: Union[str, int, Station],
     check_time: datetime = None,
     limit: int = 100,
-    debug: bool = False,
     request_params: dict = None,
-    return_resp: bool = False,
+    return_response: bool = False,
     session: requests.Session = None,
     **kwargs,
-) -> Union[List[Arrival], Response, None]:
+) -> Union[List[Departure], Response, None]:
     r"""
 
-    Returns: List[:class:`vvspy.obj.Arrival`]
+    Returns: List[:class:`vvspy.models.Departure`]
     Returns none on webrequest errors.
 
     Examples
     --------
     Basic usage:
 
     .. code-block:: python
 
-        results = vvspy.get_arrivals("5006115", limit=3)  # Stuttgart main station
+        results = vvspy.get_departures("5006115", limit=3)  # Stuttgart main station
 
     Set proxy for request:
 
     .. code-block:: python
 
         proxies = {}  # see https://stackoverflow.com/a/8287752/9850709
-        results = vvspy.get_arrivals("5006115", request_params={"proxies": proxies})
+        results = vvspy.get_departures("5006115", request_params={"proxies": proxies})
 
     Parameters
     ----------
-        station_id Union[:class:`int`, :class:`str`]
-            Station you want to get arrivals from.
-            See csv on root of repository to get your id.
+        station_id Union[:class:`int`, :class:`str`, :class:`vvspy.enums.Station`]
+            Station you want to get departures from.
         check_time Optional[:class:`datetime.datetime`]
             Time you want to check.
             default datetime.now()
         limit Optional[:class:`int`]
             Limit request/result on this integer.
             default 100
-        debug Optional[:class:`bool`]
-            Get advanced debug prints on failed web requests
-            default False
         request_params Optional[:class:`dict`]
             params parsed to the api request (e.g. proxies)
             default {}
-        return_resp Optional[:class:`bool`]
+        return_response Optional[:class:`bool`]
             if set, the function returns the response object of the API request.
         session Optional[:class:`requests.Session`]
             if set, uses a given requests.session object for requests
         kwargs Optional[:class:`dict`]
-            Check arrivals.py to see all available kwargs.
+            Check departures.py to see all available kwargs.
+
     """
 
     if not check_time:
         check_time = datetime.now()
     if request_params is None:
         request_params = dict()
+
     params = {
-        "locationServerActive": kwargs.get(
-            "locationServerActive", 1
-        ),  # typo from zocationServerActive ?!
+        "locationServerActive": kwargs.get("locationServerActive", 1),
         "lsShowTrainsExplicit": kwargs.get("lsShowTrainsExplicit", 1),
         "stateless": kwargs.get("stateless", 1),
         "language": kwargs.get("language", "de"),
         "SpEncId": kwargs.get("SpEncId", 0),
         "anySigWhenPerfectNoOtherMatches": kwargs.get(
             "anySigWhenPerfectNoOtherMatches", 1
         ),
         "limit": limit,
-        "depArr": "arrival",
+        "depArr": "departure",
         "type_dm": kwargs.get("type_dm", "any"),
         "anyObjFilter_dm": kwargs.get("anyObjFilter_dm", 2),
         "deleteAssignedStops": kwargs.get("deleteAssignedStops", 1),
-        "name_dm": station_id,
+        "name_dm": station_id.value,
         "mode": kwargs.get("mode", "direct"),
         "dmLineSelectionAll": kwargs.get("dmLineSelectionAll", 1),
         "useRealtime": kwargs.get("useRealtime", 1),  # live delay
-        "outputFormat": kwargs.get("outputFormat", "json"),
+        "outputFormat": "json",
         "coordOutputFormat": kwargs.get("coordOutputFormat", "WGS84[DD.ddddd]"),
-        "itdDateTimeDepArr": "arr",
         "itdDateYear": check_time.strftime("%Y"),
         "itdDateMonth": check_time.strftime("%m"),
         "itdDateDay": check_time.strftime("%d"),
         "itdTimeHour": check_time.strftime("%H"),
         "itdTimeMinute": check_time.strftime("%M"),
-        "itdTripDateTimeDepArr": "arr",
     }
 
-    try:
-        if session:
-            session.get(_API_URL, **{**request_params, **{"params": params}})
-        else:
-            r = requests.get(_API_URL, **{**request_params, **{"params": params}})
-    except ConnectionError as e:
-        print("ConnectionError")
-        traceback.print_exc()
-        return
+    if session:
+        r = session.get(__API_URL, **{**request_params, **{"params": params}})
+    else:
+        r = requests.get(__API_URL, **{**request_params, **{"params": params}})
+
+    __logger.debug(f"Request took {r.elapsed.total_seconds()}s and returned {r.status_code}")
 
     if r.status_code != 200:
-        if debug:
-            print("Error in API request")
-            print(f"Request: {r.status_code}")
-            print(f"{r.text}")
-        return
+        __logger.error("Error in API request")
+        __logger.error(f"Request: {r.status_code}")
+        __logger.error(f"{r.text}")
+        raise Exception(f"Error in API request: {r.status_code}")
 
-    if return_resp:
+    if return_response:
         return r
 
+    __logger.debug("Initializing parsing of response...")
+
     try:
         r.encoding = "UTF-8"
-        return _parse_response(r.json())  # TODO: error handling
-    except json.decoder.JSONDecodeError:
-        if debug:
-            print("Error in API request")
-            print("Received invalid json")
-            print(f"Request: {r.status_code}")
-            print(f"{r.text}")
-        return
+        return _parse_response(r.json())
+    except json.decoder.JSONDecodeError as e:
+        __logger.error("Error in API request. Received invalid JSON. Status code: %s", r.status_code)
+        raise e
 
 
-def _parse_response(result: dict) -> List[Arrival]:
+def _parse_response(result: dict) -> List[Departure]:
     parsed_response = []
-
     if (
-        not result or "arrivalList" not in result or not result["arrivalList"]
+        not result or "departureList" not in result or not result["departureList"]
     ):  # error in response/request
         return []  # no results
 
-    if isinstance(result["arrivalList"], dict):  # one result
-        parsed_response.append(Arrival(**result["arrivalList"]["arrival"]))
-    elif isinstance(result["arrivalList"], list):  # multiple result
-        for arrival in result["arrivalList"]:
-            parsed_response.append(Arrival(**arrival))
+    if isinstance(result["departureList"], dict):  # one result
+        parsed_response.append(Departure(**result["departureList"]["departure"]))
+    elif isinstance(result["departureList"], list):  # multiple result
+        for departure in result["departureList"]:
+            parsed_response.append(Departure(**departure))
 
     return parsed_response
```

### Comparing `vvspy-1.2.0/vvspy/departures.py` & `vvspy-2.0.0b1/vvspy/arrivals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,139 @@
 from typing import List, Union
 from datetime import datetime
 import requests
 from requests.models import Response
 import json
-import traceback
+import logging as __logging
 
-from vvspy.obj import Departure
+from .enums.stations import Station
+from .models import Arrival
 
-__API_URL = "http://www3.vvs.de/vvs/widget/XML_DM_REQUEST?"
-# TODO: new station id format de:08111:2599 (lapp kabel)
+_API_URL = "http://www3.vvs.de/vvs/widget/XML_DM_REQUEST?"
+__logger = __logging.getLogger("vvspy")
 
-
-def get_departures(
-    station_id: Union[str, int],
+def get_arrivals(
+    station_id: Union[str, int, Station],
     check_time: datetime = None,
     limit: int = 100,
-    debug: bool = False,
     request_params: dict = None,
-    return_resp: bool = False,
+    return_response: bool = False,
     session: requests.Session = None,
     **kwargs,
-) -> Union[List[Departure], Response, None]:
+) -> Union[List[Arrival], Response, None]:
     r"""
 
-    Returns: List[:class:`vvspy.obj.Departure`]
+    Returns: List[:class:`vvspy.models.Arrival`]
     Returns none on webrequest errors.
 
     Examples
     --------
     Basic usage:
 
     .. code-block:: python
 
-        results = vvspy.get_departures("5006115", limit=3)  # Stuttgart main station
+        results = vvspy.get_arrivals("5006115", limit=3)  # Stuttgart main station
 
     Set proxy for request:
 
     .. code-block:: python
 
         proxies = {}  # see https://stackoverflow.com/a/8287752/9850709
-        results = vvspy.get_departures("5006115", request_params={"proxies": proxies})
+        results = vvspy.get_arrivals("5006115", request_params={"proxies": proxies})
 
     Parameters
     ----------
-        station_id Union[:class:`int`, :class:`str`]
-            Station you want to get departures from.
-            See csv on root of repository to get your id.
+        station_id Union[:class:`int`, :class:`str`, :class:`vvspy.enums.Station`]
+            Station you want to get arrivals from.
         check_time Optional[:class:`datetime.datetime`]
             Time you want to check.
             default datetime.now()
         limit Optional[:class:`int`]
             Limit request/result on this integer.
             default 100
-        debug Optional[:class:`bool`]
-            Get advanced debug prints on failed web requests
-            default False
         request_params Optional[:class:`dict`]
             params parsed to the api request (e.g. proxies)
             default {}
-        return_resp Optional[:class:`bool`]
+        return_response Optional[:class:`bool`]
             if set, the function returns the response object of the API request.
         session Optional[:class:`requests.Session`]
             if set, uses a given requests.session object for requests
         kwargs Optional[:class:`dict`]
-            Check departures.py to see all available kwargs.
-
+            Check arrivals.py to see all available kwargs.
     """
 
     if not check_time:
         check_time = datetime.now()
     if request_params is None:
         request_params = dict()
-
     params = {
-        "locationServerActive": kwargs.get("locationServerActive", 1),
+        "locationServerActive": kwargs.get(
+            "locationServerActive", 1
+        ),  # typo from zocationServerActive ?!
         "lsShowTrainsExplicit": kwargs.get("lsShowTrainsExplicit", 1),
         "stateless": kwargs.get("stateless", 1),
         "language": kwargs.get("language", "de"),
         "SpEncId": kwargs.get("SpEncId", 0),
         "anySigWhenPerfectNoOtherMatches": kwargs.get(
             "anySigWhenPerfectNoOtherMatches", 1
         ),
         "limit": limit,
-        "depArr": "departure",
+        "depArr": "arrival",
         "type_dm": kwargs.get("type_dm", "any"),
         "anyObjFilter_dm": kwargs.get("anyObjFilter_dm", 2),
         "deleteAssignedStops": kwargs.get("deleteAssignedStops", 1),
-        "name_dm": station_id,
+        "name_dm": station_id.value,
         "mode": kwargs.get("mode", "direct"),
         "dmLineSelectionAll": kwargs.get("dmLineSelectionAll", 1),
         "useRealtime": kwargs.get("useRealtime", 1),  # live delay
-        "outputFormat": "json",
+        "outputFormat": kwargs.get("outputFormat", "json"),
         "coordOutputFormat": kwargs.get("coordOutputFormat", "WGS84[DD.ddddd]"),
+        "itdDateTimeDepArr": "arr",
         "itdDateYear": check_time.strftime("%Y"),
         "itdDateMonth": check_time.strftime("%m"),
         "itdDateDay": check_time.strftime("%d"),
         "itdTimeHour": check_time.strftime("%H"),
         "itdTimeMinute": check_time.strftime("%M"),
+        "itdTripDateTimeDepArr": "arr",
     }
 
-    try:
-        if session:
-            r = session.get(__API_URL, **{**request_params, **{"params": params}})
-        else:
-            r = requests.get(__API_URL, **{**request_params, **{"params": params}})
-    except ConnectionError as e:
-        print("ConnectionError")
-        traceback.print_exc()
-        return
+    if session:
+        r = session.get(_API_URL, **{**request_params, **{"params": params}})
+    else:
+        r = requests.get(_API_URL, **{**request_params, **{"params": params}})
+
+    __logger.debug(f"Request took {r.elapsed.total_seconds()}s and returned {r.status_code}")
 
     if r.status_code != 200:
-        if debug:
-            print("Error in API request")
-            print(f"Request: {r.status_code}")
-            print(f"{r.text}")
-        return
+        __logger.error("Error in API request")
+        __logger.error(f"Request: {r.status_code}")
+        __logger.error(f"{r.text}")
+        raise Exception(f"Error in API request: {r.status_code}")
 
-    if return_resp:
+    if return_response:
         return r
 
+    __logger.debug("Initializing parsing of response...")
+
     try:
         r.encoding = "UTF-8"
-        return _parse_response(r.json())  # TODO: error handling
-    except json.decoder.JSONDecodeError:
-        if debug:
-            print("Error in API request")
-            print("Received invalid json")
-            print(f"Request: {r.status_code}")
-            print(f"{r.text}")
-        return
+        return _parse_response(r.json())
+    except json.decoder.JSONDecodeError as e:
+        __logger.error("Error in API request. Received invalid JSON. Status code: %s", r.status_code)
+        raise e
 
 
-def _parse_response(result: dict) -> List[Departure]:
+def _parse_response(result: dict) -> List[Arrival]:
     parsed_response = []
+
     if (
-        not result or "departureList" not in result or not result["departureList"]
+        not result or "arrivalList" not in result or not result["arrivalList"]
     ):  # error in response/request
         return []  # no results
 
-    if isinstance(result["departureList"], dict):  # one result
-        parsed_response.append(Departure(**result["departureList"]["departure"]))
-    elif isinstance(result["departureList"], list):  # multiple result
-        for departure in result["departureList"]:
-            parsed_response.append(Departure(**departure))
+    if isinstance(result["arrivalList"], dict):  # one result
+        parsed_response.append(Arrival(**result["arrivalList"]["arrival"]))
+    elif isinstance(result["arrivalList"], list):  # multiple result
+        for arrival in result["arrivalList"]:
+            parsed_response.append(Arrival(**arrival))
 
     return parsed_response
```

### Comparing `vvspy-1.2.0/vvspy/obj/arrival.py` & `vvspy-2.0.0b1/vvspy/models/arrival.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/connection.py` & `vvspy-2.0.0b1/vvspy/models/connection.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/departure.py` & `vvspy-2.0.0b1/vvspy/models/departure.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/destination.py` & `vvspy-2.0.0b1/vvspy/models/destination.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/line_operator.py` & `vvspy-2.0.0b1/vvspy/models/line_operator.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/origin.py` & `vvspy-2.0.0b1/vvspy/models/origin.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/serving_line.py` & `vvspy-2.0.0b1/vvspy/models/serving_line.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/transportation.py` & `vvspy-2.0.0b1/vvspy/models/transportation.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/obj/trip.py` & `vvspy-2.0.0b1/vvspy/models/trip.py`

 * *Files identical despite different names*

### Comparing `vvspy-1.2.0/vvspy/trip.py` & `vvspy-2.0.0b1/vvspy/trip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from datetime import datetime, timezone
 import requests
 from requests.models import Response
 import json
 from typing import Union, List
-import traceback
+import logging as __logging
 
-from .obj import Trip
+from .enums.stations import Station
+from .models import Trip
 
 __API_URL = "https://www3.vvs.de/mngvvs/XML_TRIP_REQUEST2"
-
+__logger = __logging.getLogger("vvspy")
 
 def get_trips(
-    origin_station_id: Union[str, int],
-    destination_station_id: Union[str, int],
+    origin_station_id: Union[str, int, Station],
+    destination_station_id: Union[str, int, Station],
     check_time: datetime = None,
     limit: int = 100,
-    debug: bool = False,
     request_params: dict = None,
-    return_resp: bool = False,
+    return_response: bool = False,
     session: requests.Session = None,
     **kwargs,
 ) -> Union[List[Trip], Response, None]:
     r"""
 
-    Returns: List[:class:`vvspy.obj.Trip`]
+    Returns: List[:class:`vvspy.models.Trip`]
     Returns none on webrequest errors.
 
     Examples
     --------
     Basic usage:
 
     .. code-block:: python
@@ -39,30 +39,26 @@
     .. code-block:: python
 
         proxies = {}  # see https://stackoverflow.com/a/8287752/9850709
         results = vvspy.get_arrivals("5006115", "5006465", request_params={"proxies": proxies})
 
     Parameters
     ----------
-        station_id Union[:class:`int`, :class:`str`]
+        station_id Union[:class:`int`, :class:`str`, :class:`vvspy.enums.Station`]
             Station you want to get trips from.
-            See csv on root of repository to get your id.
         check_time Optional[:class:`datetime.datetime`]
             Time you want to check.
             default datetime.now()
         limit Optional[:class:`int`]
             Limit request/result on this integer.
             default 100
-        debug Optional[:class:`bool`]
-            Get advanced debug prints on failed web requests
-            default False
         request_params Optional[:class:`dict`]
             params parsed to the api request (e.g. proxies)
             default {}
-        return_resp Optional[:class:`bool`]
+        return_response Optional[:class:`bool`]
             if set, the function returns the response object of the API request.
         session Optional[:class:`requests.Session`]
             if set, uses a given requests.session object for requests
         kwargs Optional[:class:`dict`]
             Check trips.py to see all available kwargs.
     """
 
@@ -85,16 +81,16 @@
         "imparedOptionsActive": kwargs.get("imparedOptionsActive", "1"),
         "itOptionsActive": kwargs.get("itOptionsActive", "1"),
         "itdDate": check_time.strftime("%Y%m%d"),
         "itdTime": check_time.strftime("%H%M"),
         "language": kwargs.get("language", "de"),
         "locationServerActive": kwargs.get("locationServerActive", "1"),
         "macroWebTrip": kwargs.get("macroWebTrip", "true"),
-        "name_destination": destination_station_id,
-        "name_origin": origin_station_id,
+        "name_destination": destination_station_id.value,
+        "name_origin": origin_station_id.value,
         "noElevationProfile": kwargs.get("noElevationProfile", "1"),
         "noElevationSummary": kwargs.get("noElevationSummary", "1"),
         "outputFormat": "rapidJSON",
         "outputOptionsActive": "1",
         "ptOptionsActive": kwargs.get("ptOptionsActive", "1"),
         "routeType": kwargs.get("routeType", "leasttime"),
         "searchLimitMinutes": kwargs.get("searchLimitMinutes", "360"),
@@ -113,44 +109,38 @@
         "useRealtime": kwargs.get("useRealtime", "1"),
         "useUT": kwargs.get("useUT", "1"),
         "version": kwargs.get("version", "10.2.10.139"),
         "w_objPrefAl": kwargs.get("w_objPrefAl", "12"),
         "w_regPrefAm": kwargs.get("w_regPrefAm", "1"),
     }
 
-    try:
-        if session:
-            r = session.get(__API_URL, **{**request_params, **{"params": params}})
-        else:
-            r = requests.get(__API_URL, **{**request_params, **{"params": params}})
-    except ConnectionError:
-        print("ConnectionError")
-        traceback.print_exc()
-        return
+    if session:
+        r = session.get(__API_URL, **{**request_params, **{"params": params}})
+    else:
+        r = requests.get(__API_URL, **{**request_params, **{"params": params}})
+
+    __logger.debug(f"Request took {r.elapsed.total_seconds()}s and returned {r.status_code}")
 
     if r.status_code != 200:
-        if debug:
-            print("Error in API request")
-            print(f"Request: {r.status_code}")
-            print(f"{r.text}")
-        return
+        __logger.error("Error in API request")
+        __logger.error(f"Request: {r.status_code}")
+        __logger.error(f"{r.text}")
+        raise Exception(f"Error in API request: {r.status_code}")
 
-    if return_resp:
+    if return_response:
         return r
 
+    __logger.debug("Initializing parsing of response...")
+
     try:
         r.encoding = "UTF-8"
-        return _parse_response(r.json(), limit=limit)  # TODO: error handling
-    except json.decoder.JSONDecodeError:
-        if debug:
-            print("Error in API request")
-            print("Received invalid json")
-            print(f"Request: {r.status_code}")
-            print(f"{r.text}")
-        return
+        return _parse_response(r.json(), limit)
+    except json.decoder.JSONDecodeError as e:
+        __logger.error("Error in API request. Received invalid JSON. Status code: %s", r.status_code)
+        raise e
 
 
 def _parse_response(result: dict, limit: int = 100) -> Union[List[Trip], None]:
     parsed_trips = []
     if not result or "journeys" not in result or not result["journeys"]:
         return []  # no trips found
     for trip in result["journeys"][: int(limit)]:
```

