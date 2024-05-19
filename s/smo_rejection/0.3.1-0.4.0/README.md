# Comparing `tmp/smo_rejection-0.3.1.tar.gz` & `tmp/smo_rejection-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.3.1.tar", max compression
+gzip compressed data, was "smo_rejection-0.4.0.tar", max compression
```

## Comparing `smo_rejection-0.3.1.tar` & `smo_rejection-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      283 2024-05-18 09:43:19.823377 smo_rejection-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2061 2024-05-18 09:16:32.069301 smo_rejection-0.3.1/README.md
--rw-r--r--   0        0        0      152 2024-05-18 09:42:02.234382 smo_rejection-0.3.1/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-18 09:16:32.075303 smo_rejection-0.3.1/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-18 09:16:32.076302 smo_rejection-0.3.1/smo_rejection/models.py
--rw-r--r--   0        0        0     4417 2024-05-18 09:17:38.463921 smo_rejection-0.3.1/smo_rejection/processing.py
--rw-r--r--   0        0        0     4304 2024-05-18 09:16:32.077303 smo_rejection-0.3.1/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-18 09:16:32.077303 smo_rejection-0.3.1/smo_rejection/utils.py
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-05-19 12:01:10.683744 smo_rejection-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2061 2024-05-18 10:29:03.252234 smo_rejection-0.4.0/README.md
+-rw-r--r--   0        0        0      188 2024-05-19 12:00:20.787948 smo_rejection-0.4.0/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.0/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.0/smo_rejection/models.py
+-rw-r--r--   0        0        0     2193 2024-05-19 11:59:54.473573 smo_rejection-0.4.0/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.0/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.0/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.0/smo_rejection/utils.py
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 smo_rejection-0.4.0/PKG-INFO
```

### Comparing `smo_rejection-0.3.1/README.md` & `smo_rejection-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.3.1/smo_rejection/exception.py` & `smo_rejection-0.4.0/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.3.1/smo_rejection/models.py` & `smo_rejection-0.4.0/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.3.1/smo_rejection/processing.py` & `smo_rejection-0.4.0/smo_rejection/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from models import SimulationParameters, SimulationResult
-from utils import generate_random_number, calculate_time
+from .models import SimulationParameters, SimulationResult
+from .utils import generate_random_number, calculate_time
 
 def process_iteration(params: SimulationParameters, iteration: int) -> SimulationResult:
     """
     Выполняет одну итерацию симуляции обслуживания заявок.
 
     Параметры:
     params (SimulationParameters): Параметры симуляции.
```

### Comparing `smo_rejection-0.3.1/smo_rejection/simulation.py` & `smo_rejection-0.4.0/smo_rejection/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from exception import InvalidInputError, NumIterationsNegative, NumIterationsIsZero, NumChannelsNegative, NumChannelsIsZero, AlphaIsZero, AlphaNegative, ServiceTimeNegative, MaxTimeNegative
-from models import SimulationParameters
-from processing import process_iteration
+from .exception import InvalidInputError, NumIterationsNegative, NumIterationsIsZero, NumChannelsNegative, NumChannelsIsZero, AlphaIsZero, AlphaNegative, ServiceTimeNegative, MaxTimeNegative
+from .models import SimulationParameters
+from .processing import process_iteration
 
 def run_simulation(T: float, num_channels: int, service_time: float, num_iterations: int, alfa: int):
     """
     Запускает симуляцию обслуживания заявок с заданными параметрами.
 
     Параметры:
     T (float): Общее время симуляции.
```

### Comparing `smo_rejection-0.3.1/smo_rejection/utils.py` & `smo_rejection-0.4.0/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.3.1/PKG-INFO` & `smo_rejection-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

