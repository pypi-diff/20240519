# Comparing `tmp/vr180_convert-0.2.2.tar.gz` & `tmp/vr180_convert-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vr180_convert-0.2.2.tar", max compression
+gzip compressed data, was "vr180_convert-0.3.0.tar", max compression
```

## Comparing `vr180_convert-0.2.2.tar` & `vr180_convert-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-05-15 03:22:30.419482 vr180_convert-0.2.2/LICENSE
--rw-r--r--   0        0        0    10741 2024-05-15 03:22:30.419482 vr180_convert-0.2.2/README.md
--rw-r--r--   0        0        0     3837 2024-05-15 03:22:31.855484 vr180_convert-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      707 2024-05-15 03:22:31.855484 vr180_convert-0.2.2/src/vr180_convert/__init__.py
--rw-r--r--   0        0        0      113 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/__main__.py
--rw-r--r--   0        0        0    12817 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/cli.py
--rw-r--r--   0        0        0        0 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/py.typed
--rw-r--r--   0        0        0    12090 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/remapper.py
--rw-r--r--   0        0        0     1889 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/testing.py
--rw-r--r--   0        0        0    18069 2024-05-15 03:22:30.435482 vr180_convert-0.2.2/src/vr180_convert/transformer.py
--rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-19 06:19:09.880628 vr180_convert-0.3.0/LICENSE
+-rw-r--r--   0        0        0    10741 2024-05-19 06:19:09.880628 vr180_convert-0.3.0/README.md
+-rw-r--r--   0        0        0     3837 2024-05-19 06:19:11.120636 vr180_convert-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-05-19 06:19:11.120636 vr180_convert-0.3.0/src/vr180_convert/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/__main__.py
+-rw-r--r--   0        0        0    12817 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/cli.py
+-rw-r--r--   0        0        0        0 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/py.typed
+-rw-r--r--   0        0        0    12090 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/remapper.py
+-rw-r--r--   0        0        0     1889 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/testing.py
+-rw-r--r--   0        0        0    20213 2024-05-19 06:19:09.896628 vr180_convert-0.3.0/src/vr180_convert/transformer.py
+-rw-r--r--   0        0        0    12140 1970-01-01 00:00:00.000000 vr180_convert-0.3.0/PKG-INFO
```

### Comparing `vr180_convert-0.2.2/LICENSE` & `vr180_convert-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.2/README.md` & `vr180_convert-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.2/pyproject.toml` & `vr180_convert-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vr180-convert"
-version = "0.2.2"
+version = "0.3.0"
 description = "Simple VR180 image converter"
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/vr180-convert"
 documentation = "https://vr180-convert.readthedocs.io"
 classifiers = [
```

### Comparing `vr180_convert-0.2.2/src/vr180_convert/__init__.py` & `vr180_convert-0.3.0/src/vr180_convert/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 from .remapper import apply, apply_lr, get_map
 from .transformer import (
     DenormalizeTransformer,
     EquirectangularEncoder,
     Euclidean3DRotator,
     Euclidean3DTransformer,
     FisheyeDecoder,
```

### Comparing `vr180_convert-0.2.2/src/vr180_convert/cli.py` & `vr180_convert-0.3.0/src/vr180_convert/cli.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.2/src/vr180_convert/remapper.py` & `vr180_convert-0.3.0/src/vr180_convert/remapper.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.2/src/vr180_convert/testing.py` & `vr180_convert-0.3.0/src/vr180_convert/testing.py`

 * *Files identical despite different names*

### Comparing `vr180_convert-0.2.2/src/vr180_convert/transformer.py` & `vr180_convert-0.3.0/src/vr180_convert/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import warnings
 from abc import ABCMeta, abstractmethod
 from typing import Any, Generic, Literal, Sequence, TypeVar
 
 import attrs
 import numpy as np
 from numpy.typing import NDArray
 from quaternion import quaternion, rotate_vectors
@@ -282,14 +283,75 @@
         theta, roll = self.inverse_transform_polar(theta, roll, **kwargs)
         x = theta * np.cos(roll)
         y = theta * np.sin(roll)
         return x, y
 
 
 @attrs.define()
+class RectilinearDecoder(PolarRollTransformer):
+    """Encodes rectilinear image."""
+
+    # https://en.wikipedia.org/wiki/Image_sensor_format
+    focal_length: float
+    """The focal length of the lens in mm."""
+    sensor_width: (
+        Literal["35mm", "APS-H", "APS-C", "APS-C-Canon", "Foveon", "MFT"] | str | float
+    ) = "35mm"
+    """The sensor width of the camera in mm if float,
+    or in inches if str, or a standard sensor width if str."""
+
+    @property
+    def sensor_width_mm(self) -> float:
+        """Sensor width in mm."""
+        if self.sensor_width in ["35mm", "APS-C", "1/2.3"]:
+            warnings.warn(
+                "Sensor size may vary by about 0.2 mm depending on the camera model. "
+                "To get very accurate results, consider setting the sensor width in mm manually.",
+                UserWarning,
+                stacklevel=2,
+            )
+        # https://en.wikipedia.org/wiki/Image_sensor_format#Table_of_sensor_formats_and_sizes
+        known_widths = {
+            "35mm": 36.0,  # ~ 35.8mm
+            "APS-H": 27.90,
+            "APS-C": 23.6,  # ~ 23.7mm
+            "APS-C-Canon": 22.30,
+            "MFT": 17.30,
+            "1": 13.20,
+            "1/1.12": 11.43,
+            "1/1.2": 10.67,
+            "1/1.33": 9.6,
+            "1/1.6": 8.08,
+            "1/1.7": 7.60,
+            "1/1.8": 7.18,
+            "1/2": 6.40,
+            "1/2.3": 6.17,
+        }
+        if isinstance(self.sensor_width, str):
+            return known_widths[self.sensor_width]
+        return self.sensor_width
+
+    @property
+    def factor(self) -> float:
+        """Zoom factor applied after tan."""
+        return 2 * self.focal_length / self.sensor_width_mm
+
+    def transform_polar(
+        self, theta: NDArray, roll: NDArray, **kwargs: Any
+    ) -> tuple[NDArray, NDArray]:
+        return np.tan(theta) * self.factor, roll
+
+    def inverse_transform_polar(
+        self, theta: NDArray, roll: NDArray, **kwargs: Any
+    ) -> tuple[NDArray, NDArray]:
+        # fov = 2 arctan sensor_width / (2 * focal_length)
+        return np.arctan(theta / self.factor), roll
+
+
+@attrs.define()
 class FisheyeEncoder(PolarRollTransformer):
     """Encodes fisheye image."""
 
     mapping_type: Literal[
         "rectilinear", "stereographic", "equidistant", "equisolid", "orthographic"
     ]
     """The mapping type of the fisheye image."""
```

### Comparing `vr180_convert-0.2.2/PKG-INFO` & `vr180_convert-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vr180-convert
-Version: 0.2.2
+Version: 0.3.0
 Summary: Simple VR180 image converter
 Home-page: https://github.com/34j/vr180-convert
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vr180-convert Version: 0.2.2 Summary: Simple VR180
+Metadata-Version: 2.1 Name: vr180-convert Version: 0.3.0 Summary: Simple VR180
 image converter Home-page: https://github.com/34j/vr180-convert License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

