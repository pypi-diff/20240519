# Comparing `tmp/abses-0.6.5.tar.gz` & `tmp/abses-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.6.5.tar", max compression
+gzip compressed data, was "abses-0.6.6.tar", max compression
```

## Comparing `abses-0.6.5.tar` & `abses-0.6.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.5/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.5/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.5/README.md
--rw-r--r--   0        0        0     1125 2024-05-17 02:47:42.709224 abses-0.6.5/abses/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-16 08:41:24.081841 abses-0.6.5/abses/_bases/bases.py
--rw-r--r--   0        0        0     3124 2024-05-16 03:43:18.344259 abses-0.6.5/abses/_bases/components.py
--rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.5/abses/_bases/dynamic.py
--rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.5/abses/_bases/errors.py
--rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.5/abses/_bases/logging.py
--rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.5/abses/_bases/modules.py
--rw-r--r--   0        0        0     3157 2024-05-16 09:29:06.415637 abses-0.6.5/abses/_bases/objects.py
--rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.5/abses/_bases/states.py
--rw-r--r--   0        0        0     9755 2024-05-16 07:58:52.452219 abses-0.6.5/abses/actor.py
--rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.5/abses/cells.py
--rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.5/abses/conf/__init__.py
--rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.5/abses/conf/default.yaml
--rw-r--r--   0        0        0    17578 2024-05-16 08:31:28.732690 abses-0.6.5/abses/container.py
--rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.5/abses/data.py
--rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.5/abses/decision.py
--rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.5/abses/experiment.py
--rw-r--r--   0        0        0     3872 2024-05-16 06:59:47.771801 abses-0.6.5/abses/human.py
--rw-r--r--   0        0        0    19386 2024-05-15 07:23:23.061845 abses-0.6.5/abses/links.py
--rw-r--r--   0        0        0    15588 2024-05-16 11:13:35.757091 abses-0.6.5/abses/main.py
--rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.5/abses/move.py
--rw-r--r--   0        0        0    12661 2024-05-16 09:25:11.727552 abses-0.6.5/abses/nature.py
--rw-r--r--   0        0        0    28792 2024-05-17 02:13:20.828886 abses-0.6.5/abses/patch.py
--rw-r--r--   0        0        0     8193 2024-05-17 02:47:03.678593 abses-0.6.5/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.5/abses/selection.py
--rw-r--r--   0        0        0    11767 2024-05-17 02:37:06.722538 abses-0.6.5/abses/sequences.py
--rw-r--r--   0        0        0    15523 2024-05-16 08:29:09.798671 abses-0.6.5/abses/time.py
--rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.5/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.5/abses/tools/regex.py
--rw-r--r--   0        0        0     1134 2024-05-12 12:57:47.944073 abses-0.6.5/abses/viz/viz_actors.py
--rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.5/abses/viz/viz_model.py
--rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.5/abses/viz/viz_nature.py
--rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.5/data/.DS_Store
--rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.5/data/YR_cities.zip
--rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.5/data/farmland.tif
--rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.5/data/irr_lands.csv
--rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.5/data/precipitation.nc
--rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.5/icons/fa-regular-400.otf
--rw-r--r--   0        0        0     2764 2024-05-17 02:47:42.703517 abses-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     7271 1970-01-01 00:00:00.000000 abses-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.6/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.6/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.6/README.md
+-rw-r--r--   0        0        0     1131 2024-05-19 13:14:11.539321 abses-0.6.6/abses/__init__.py
+-rw-r--r--   0        0        0    11469 2024-05-19 09:46:33.897240 abses-0.6.6/abses/_bases/base_container.py
+-rw-r--r--   0        0        0     2598 2024-05-18 08:54:14.557507 abses-0.6.6/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3124 2024-05-16 03:43:18.344259 abses-0.6.6/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.6/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.6/abses/_bases/errors.py
+-rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.6/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.6/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3157 2024-05-18 14:49:08.436242 abses-0.6.6/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.6/abses/_bases/states.py
+-rw-r--r--   0        0        0    10588 2024-05-19 10:17:00.008167 abses-0.6.6/abses/actor.py
+-rw-r--r--   0        0        0     5534 2024-05-19 09:46:33.898054 abses-0.6.6/abses/cells.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.6/abses/conf/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.6/abses/conf/default.yaml
+-rw-r--r--   0        0        0    11590 2024-05-19 13:10:29.734790 abses-0.6.6/abses/container.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.6/abses/decision.py
+-rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.6/abses/experiment.py
+-rw-r--r--   0        0        0     3845 2024-05-19 13:10:29.735156 abses-0.6.6/abses/human.py
+-rw-r--r--   0        0        0    22297 2024-05-19 13:10:29.735424 abses-0.6.6/abses/links.py
+-rw-r--r--   0        0        0    15614 2024-05-19 09:46:33.899490 abses-0.6.6/abses/main.py
+-rw-r--r--   0        0        0     8295 2024-05-19 09:46:33.899859 abses-0.6.6/abses/move.py
+-rw-r--r--   0        0        0    12661 2024-05-19 05:49:39.650125 abses-0.6.6/abses/nature.py
+-rw-r--r--   0        0        0    30977 2024-05-19 09:46:33.900107 abses-0.6.6/abses/patch.py
+-rw-r--r--   0        0        0     8193 2024-05-17 02:47:03.678593 abses-0.6.6/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.6/abses/selection.py
+-rw-r--r--   0        0        0    13800 2024-05-19 09:46:33.900478 abses-0.6.6/abses/sequences.py
+-rw-r--r--   0        0        0    15523 2024-05-16 08:29:09.798671 abses-0.6.6/abses/time.py
+-rw-r--r--   0        0        0      969 2024-05-19 09:46:33.900596 abses-0.6.6/abses/tools/data.py
+-rw-r--r--   0        0        0     6780 2024-05-19 09:46:33.901051 abses-0.6.6/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.6/abses/tools/regex.py
+-rw-r--r--   0        0        0     1205 2024-05-19 09:46:33.901287 abses-0.6.6/abses/tools/viz.py
+-rw-r--r--   0        0        0     4046 2024-05-19 13:10:29.735954 abses-0.6.6/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.6/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     1709 2024-05-19 09:46:33.901856 abses-0.6.6/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.6/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.6/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.6/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.6/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.6/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.6/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2784 2024-05-19 13:14:11.538040 abses-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     7262 1970-01-01 00:00:00.000000 abses-0.6.6/PKG-INFO
```

### Comparing `abses-0.6.5/LICENSE` & `abses-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/README.md` & `abses-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/__init__.py` & `abses-0.6.6/abses/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,19 +27,19 @@
     "perception",
     "alive_required",
     "time_condition",
     "Experiment",
     "load_data",
     "logger",
 ]
-__version__ = "v0.6.5"
+__version__ = "v0.6.6"
 
 from ._bases.logging import logger
 from .actor import Actor, alive_required, perception
-from .container import ActorsList
-from .data import load_data
 from .decision import Decision
 from .experiment import Experiment
 from .human import BaseHuman
 from .main import MainModel
 from .nature import BaseNature, PatchCell, PatchModule
+from .sequences import ActorsList
 from .time import time_condition
+from .tools.data import load_data
```

### Comparing `abses-0.6.5/abses/_bases/bases.py` & `abses-0.6.6/abses/_bases/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/_bases/components.py` & `abses-0.6.6/abses/_bases/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/_bases/dynamic.py` & `abses-0.6.6/abses/_bases/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/_bases/logging.py` & `abses-0.6.6/abses/_bases/logging.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/_bases/modules.py` & `abses-0.6.6/abses/_bases/modules.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/_bases/objects.py` & `abses-0.6.6/abses/_bases/objects.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/_bases/states.py` & `abses-0.6.6/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/actor.py` & `abses-0.6.6/abses/actor.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,42 +15,47 @@
 
 from functools import cached_property, wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
+    Literal,
     Optional,
     Union,
     cast,
 )
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 import mesa_geo as mg
+from shapely import Point
+from shapely.geometry.base import BaseGeometry
 
 from abses._bases.errors import ABSESpyError
 from abses._bases.objects import _BaseObj
 from abses.decision import _DecisionFactory
 from abses.links import TargetName, _LinkNodeActor, _LinkNodeCell
 from abses.move import _Movements
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
+    from abses._bases.base_container import UniqueID
     from abses.cells import Pos
     from abses.main import MainModel
     from abses.nature import PatchCell, PatchModule
 
 
 Selection: TypeAlias = Union[str, Iterable[bool]]
 Trigger: TypeAlias = Union[Callable, str]
 Breeds: TypeAlias = Optional[Union[str, Iterable[str]]]
+GeoType: TypeAlias = Literal["Point", "Shape"]
 
 
 def alive_required(method):
     """
     A decorator that only executes the method when the object's alive attribute is True.
     """
 
@@ -146,20 +151,18 @@
     # when checking the rules
     __decisions__ = None
 
     def __init__(
         self,
         model: MainModel[Any, Any],
         observer: bool = True,
-        unique_id: Optional[int] = None,
+        unique_id: Optional[UniqueID] = None,
         **kwargs,
     ) -> None:
         _BaseObj.__init__(self, model, observer=observer)
-        if not unique_id:
-            unique_id = self.model.next_id()
         crs = kwargs.pop("crs", model.nature.crs)
         geometry = kwargs.pop("geometry", None)
         mg.GeoAgent.__init__(
             self, unique_id, model=model, geometry=geometry, crs=crs
         )
         _LinkNodeActor.__init__(self)
         self._cell: Optional[PatchCell] = None
@@ -173,14 +176,34 @@
 
     def _setup_decisions(self) -> _DecisionFactory:
         """Decisions that this actor makes."""
         decisions = make_list(getattr(self, "__decisions__", None))
         return _DecisionFactory(self, decisions)
 
     @property
+    def geo_type(self) -> Optional[GeoType]:
+        """The type of the geo info."""
+        if self.geometry is None:
+            return None
+        if isinstance(self.geometry, Point):
+            return "Point"
+        return "Shape"
+
+    @property
+    def geometry(self) -> Optional[BaseGeometry]:
+        """The geometry of the actor."""
+        return Point(self.at.coordinate) if self.at else self._geometry
+
+    @geometry.setter
+    def geometry(self, value: Optional[BaseGeometry]) -> None:
+        if not isinstance(value, BaseGeometry) and value is not None:
+            raise TypeError(f"{value} is not a valid geometry.")
+        self._geometry = value
+
+    @property
     def alive(self) -> bool:
         """Whether the actor is alive."""
         return self._alive
 
     @property
     def decisions(self) -> _DecisionFactory:
         """The decisions that this actor makes."""
@@ -193,15 +216,15 @@
     def layer(self) -> Optional[PatchModule]:
         """Get the layer where the actor is located."""
         return None if self._cell is None else self._cell.layer
 
     @property
     def on_earth(self) -> bool:
         """Whether agent stands on a cell."""
-        return bool(self._cell)
+        return bool(self.geometry)
 
     @property
     def at(self) -> PatchCell | None:
         """Get the cell where the agent is located."""
         return self._cell if self._cell is not None else None
 
     @at.setter
@@ -210,14 +233,15 @@
         if not isinstance(cell, _LinkNodeCell):
             raise TypeError(f"{cell} is not a cell.")
         if self not in cell.agents:
             raise ABSESpyError(
                 "Cannot set location directly because the actor is not added to the cell."
             )
         self._cell = cell
+        self.crs = cell.crs
 
     @at.deleter
     def at(self) -> None:
         """Remove the agent from the located cell."""
         cell = cast("PatchCell", self.at)
         if self.on_earth and cell.agents is not None and self in cell.agents:
             raise ABSESpyError(
```

### Comparing `abses-0.6.5/abses/cells.py` & `abses-0.6.6/abses/cells.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, Union
 
 from mesa_geo.raster_layers import RasterBase
+from pyproj import CRS
 
-from abses import ActorsList
 from abses._bases.errors import ABSESpyError
+from abses._bases.objects import _BaseObj
 from abses.container import _CellAgentsContainer
 from abses.links import TargetName, _LinkNodeCell
 
 if TYPE_CHECKING:
-    from abses.main import H, MainModel, N
+    from abses.main import MainModel
     from abses.nature import PatchModule
+    from abses.sequences import ActorsList
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 Pos: TypeAlias = Tuple[int, int]
@@ -63,30 +65,31 @@
         ])
         ```
     """
     setattr(func, "is_decorated", True)
     return property(func)
 
 
-class PatchCell(_LinkNodeCell):
+class PatchCell(_LinkNodeCell, _BaseObj):
     """A patch cell of a `RasterLayer`.
     Subclassing this class to create a custom cell.
     When class attribute `max_agents` is assigned,
     the `agents` property will be limited to the number of agents.
 
     Attributes:
         agents:
             The agents located at here.
         layer:
             The `RasterLayer` where this `PatchCell` belongs.
     """
 
     max_agents: Optional[int] = None
 
-    def __init__(self, layer, indices: Optional[Pos] = None):
+    def __init__(self, layer, indices: Pos):
+        _BaseObj.__init__(self, model=layer.model, observer=True)
         _LinkNodeCell.__init__(self)
         self.indices = indices
         self._set_layer(layer=layer)
 
     def __repr__(self) -> str:
         return f"<Cell at {self.layer}[{self.indices}]>"
 
@@ -110,31 +113,47 @@
             raise ABSESpyError(
                 "PatchCell must belong to a layer."
                 f"However, {self} has no layer."
                 "Did you create this cell in the correct way?"
             )
         return self._layer
 
+    @property
+    def agents(self) -> _CellAgentsContainer:
+        """The agents located at here."""
+        return self._agents
+
+    @property
+    def coordinate(self) -> Tuple[float, float]:
+        """The position of this cell."""
+        row, col = self.indices
+        return self.layer.transform_coord(row=row, col=col)
+
+    @property
+    def geo_type(self) -> str:
+        """Return the geo_type"""
+        return "Cell"
+
+    @property
+    def crs(self) -> Optional[CRS]:
+        """Return the crs of this cell."""
+        return self.layer.crs
+
     def _set_layer(self, layer: PatchModule) -> None:
         if not isinstance(layer, RasterBase):
             raise TypeError(f"{type(layer)} is not valid layer.")
         # set layer property
         self._layer = layer
         # set layer's model as the model
         self.model: MainModel[Any, Any] = layer.model
         # set agents container
         self._agents = _CellAgentsContainer(
             layer.model, cell=self, max_len=getattr(self, "max_agents", None)
         )
 
-    @property
-    def agents(self) -> _CellAgentsContainer:
-        """The agents located at here."""
-        return self._agents
-
     def get(self, attr: str, target: Optional[TargetName] = None) -> Any:
         """Gets the value of an attribute or registered property.
         Automatically update the value if it is the dynamic variable of the layer.
 
         Parameters:
             attr:
                 The name of attribute to get.
```

### Comparing `abses-0.6.5/abses/container.py` & `abses-0.6.6/abses/_bases/base_container.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 #!/usr/bin/env python 3.11.0
 # -*-coding:utf-8 -*-
 # @Author  : Shuang (Twist) Song
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
-"""
-行动者容器，集中保存行动者。
-Container for actors.
+"""Base container, common methods for both the main model and the cells.
 """
 
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     Optional,
     Type,
     Union,
-    cast,
 )
 
 import numpy as np
+import pyproj
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
-import geopandas as gpd
-import mesa_geo as mg
-from loguru import logger
-
 from abses._bases.errors import ABSESpyError
 from abses.actor import Actor, Breeds
 from abses.sequences import HOW, ActorsList, Selection
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
-    from abses.cells import PatchCell
     from abses.main import MainModel
 
 ActorTypes: TypeAlias = Union[Type[Actor], Iterable[Type[Actor]]]
 Actors: TypeAlias = Union[Actor, ActorsList, Iterable[Actor]]
+UniqueID: TypeAlias = Union[str, int]
 
 
 class _AgentsContainer(dict):
     """AgentsContainer for the main model."""
 
     def __init__(
         self,
@@ -75,14 +69,19 @@
             raise TypeError(f"{type(actor)} is not a Actor.")
         return actor in self.get()
 
     def __call__(self, *args: Breeds, **kwargs: Breeds) -> ActorsList[Actor]:
         return self.get(*args, **kwargs)
 
     @property
+    def crs(self) -> pyproj.CRS:
+        """Returns the current CRS."""
+        return self._model.nature.crs
+
+    @property
     def model(self) -> MainModel[Any, Any]:
         """The ABSESpy model where the container belongs to."""
         return self._model
 
     @property
     def is_full(self) -> bool:
         """Whether the container is full."""
@@ -93,29 +92,34 @@
         )
 
     @property
     def is_empty(self) -> bool:
         """Check whether the container is empty."""
         return len(self.get()) == 0
 
-    def check_registration(self, actor_cls: Type[Actor]) -> bool:
+    def check_registration(
+        self, actor_cls: Type[Actor], register: bool = False
+    ) -> bool:
         """Whether the breed of the actor is registered.
 
         Parameters:
             actor_cls:
                 The class of the actor.
                 If the actor is registered,
                 it will be accessible from all containers
                 (despite count is zero).
 
         Returns:
             True if the breed of the actor is registered.
             False otherwise.
         """
-        return actor_cls.breed in self.keys()
+        flag = actor_cls.breed in self.keys()
+        if not flag and register:
+            self._model.agents.register(actor_cls)
+        return flag
 
     def _check_adding_for_length(self, when_adding: int = 1) -> None:
         """Check if the container is invalid for adding the agent.
 
         Parameters:
             when_adding:
                 The number of agents to add.
@@ -127,116 +131,14 @@
         if self._max_length is None:
             return
         if self.has() + when_adding > self._max_length:
             e1 = f"{self} is full (maximum {self._max_length}: "
             e2 = f"Now has {self.has()}), trying to add {when_adding} more."
             raise ABSESpyError(e1 + e2)
 
-    def register(self, actor_cls: ActorTypes) -> None:
-        """Registers a new breed of actors.
-
-        Parameters:
-            actor_cls:
-                The class of the actor to register.
-                It can be a single class, or an iterable of classes.
-                Once a breed is registered,
-                it will be added to all the containers of the model globally.
-                It means, it's not necessary to register the same breed again.
-
-        Raises:
-            ValueError:
-                If the breed is already registered.
-        """
-        for a_cls in make_list(actor_cls):
-            breed = a_cls.breed
-            if breed in self._model.breeds:
-                raise ValueError(f"{breed} is already registered.")
-            self._model.breeds = a_cls
-
-    def new_from_gdf(
-        self,
-        gdf: gpd.GeoDataFrame,
-        unique_id: str = "Index",
-        agent_cls: type[Actor] = Actor,
-    ) -> ActorsList[Actor]:
-        """Create actors from a `geopandas.GeoDataFrame` object.
-
-        Parameters:
-            gdf:
-                The `geopandas.GeoDataFrame` object to convert.
-            unique_id:
-                A column name, to be converted to unique index
-                of created geo-agents (Social-ecological system Actors).
-            agent_cls:
-                Agent class to create.
-
-        Returns:
-            An `ActorsList` with all new created actors stored.
-        """
-        creator = mg.AgentCreator(
-            model=self.model, agent_class=agent_cls, crs=self.model.nature.crs
-        )
-        agents = creator.from_GeoDataFrame(gdf=gdf, unique_id=unique_id)
-        self.register(agent_cls)
-        self.add(agents)
-        return ActorsList(model=self.model, objs=agents)
-
-    def new(
-        self,
-        breed_cls: Optional[Type[Actor]] = None,
-        num: int = 1,
-        singleton: bool = False,
-        **kwargs: Any,
-    ) -> Union[Actor, ActorsList[Actor]]:
-        """Create one or more actors of the given breed class.
-
-        Parameters:
-            breed_cls:
-                The breed class of the actor(s) to create.
-            num:
-                The number of actors to create. Defaults to 1.
-            singleton (bool, optional):
-                Whether to create a singleton actor. Defaults to False.
-            **kwargs:
-                Additional keyword arguments to pass to the actor constructor.
-
-        Returns:
-            The created actor(s).
-
-        Example:
-            ```python
-            from abses import Actor, MainModel
-            model = MainModel()
-            actor = model.agents.new(singleton=True)
-            >>> type(actor)
-            >>> Actor
-
-            actors = model.agents.new(singleton=False)
-            >>> type(actors)
-            >>> ActorsList
-            ```
-        """
-        if breed_cls is None:
-            breed_cls = Actor
-        # check if the breed class is registered, if not, register it.
-        if not self.check_registration(breed_cls):
-            self.register(breed_cls)
-        # create actors.
-        objs = [breed_cls(self._model, **kwargs) for _ in range(num)]
-        logger.debug(f"{self} created {num} {breed_cls.__name__}.")
-        # add actors to the container and the schedule.
-        for agent in objs:
-            self.add(agent)
-            self.model.schedule.add(agent)
-        # return the created actor(s).
-        actors_list: ActorsList[Actor] = ActorsList(
-            model=self.model, objs=objs
-        )
-        return cast(Actor, actors_list.item()) if singleton else actors_list
-
     def get(self, breeds: Breeds = None) -> ActorsList[Actor]:
         """Get all entities of specified breeds to a list.
 
         Parameters:
             breeds:
                 The breed(s) of entities to convert to a list.
                 If None, all breeds are used.
@@ -290,29 +192,26 @@
                 Keyword arguments to be passed to the `trigger` method of each agent.
 
         Returns:
             In row, what the triggered function returned.
         """
         return self.get().trigger(*args, **kwargs)
 
-    def _add_one(self, agent: Actor, register: bool = False) -> None:
+    def _add_one(self, agent: Actor) -> None:
         """Add one agent to the container."""
-        if agent.breed not in self.keys():
-            if register:
-                self.register(agent.__class__)
-            else:
-                raise TypeError(
-                    f"'{agent.breed}' not registered. Is it created by `.create()` method?"
-                )
+        if not self.check_registration(agent.__class__):
+            raise TypeError(
+                f"Breed '{agent.breed}' not registered."
+                "Is it created by `agents.new()` method?"
+            )
         self[agent.breed].add(agent)
 
     def add(
         self,
         agents: Actors,
-        register: bool = False,
     ) -> None:
         """Add one or more actors to the container.
 
         Parameters:
             agents:
                 The actor(s) to add to the container.
                 It can be a single actor, a list of actors, or an iterable of actors.
@@ -328,15 +227,15 @@
                 If a breed of the actor(s) is not registered and `register` is False.
             ABSESpyError:
                 If the container is full after adding these agents.
         """
         to_add = make_list(agents)
         self._check_adding_for_length(len(to_add))
         for item in to_add:
-            self._add_one(item, register)
+            self._add_one(item)
 
     def remove(self, agent: Actor) -> None:
         """Remove the given agent from the container and the schedule.
         Generally, it stores all the agents in the model.
         Therefore, it is not recommended to use this method directly.
         Consider to use `actor.die()` instead.
 
@@ -457,83 +356,7 @@
             index:
                 The index of the agent to retrieve.
 
         Returns:
             The agent if found, otherwise None.
         """
         return self.get().item(how=how, index=index)
-
-
-class _CellAgentsContainer(_AgentsContainer):
-    """Container for agents located at cells."""
-
-    def __init__(
-        self,
-        model: MainModel[Any, Any],
-        cell: PatchCell,
-        max_len: int | None = None,
-    ):
-        super().__init__(model, max_len)
-        self._cell = cell
-
-    def __str__(self) -> str:
-        return "CellAgents"
-
-    def _add_one(self, agent: Actor, register: bool = False) -> None:
-        if agent.on_earth and agent not in self:
-            e1 = f"{agent} is on another cell thus cannot be added."
-            e2 = "You may use 'actor.move.to()' to change its location."
-            e3 = "Or you may use 'actor.move.off()' before adding it."
-            raise ABSESpyError(e1 + e2 + e3)
-        super()._add_one(agent, register)
-        agent.at = self._cell
-
-    def remove(self, agent: Actor) -> None:
-        """Remove the given agent from the cell.
-        Generally, it stores all the agents on this cell.
-        Therefore, it is not recommended to use this method directly.
-        Consider to use `actor.move.off()` to let the actor leave this cell instead.
-
-        Parameters:
-            agent:
-                The agent (actor) to remove.
-
-        Raises:
-            ABSESpyError:
-                If the agent is not on this cell.
-        """
-        if agent.at is not self._cell:
-            raise ABSESpyError(f"{agent} is not on this cell.")
-        self[agent.breed].remove(agent)
-        del agent.at
-
-    def new(
-        self,
-        breed_cls: Type[Actor],
-        num: int = 1,
-        singleton: bool = False,
-        **kwargs: Any,
-    ) -> Actor | ActorsList:
-        """Creates a new actor or a list of actors of the given breed class.
-        The created actors are added to both the cell and the model's global container.
-
-        Parameters:
-            breed_cls:
-                The breed class of the actor(s) to create.
-            num:
-                The number of actors to create. Defaults to 1.
-            singleton:
-                Whether to create a singleton actor. Defaults to False.
-            **kwargs:
-                Additional keyword arguments to pass to the actor constructor.
-
-        Returns:
-            The created actor(s).
-        """
-        # create a list of actors
-        new_actors = super().new(breed_cls, num, singleton, **kwargs)
-        # also add the actors to the model's global agents container
-        self.model.agents.add(new_actors)
-        # move the actors to the cell
-        for a in make_list(new_actors):
-            a.move.to(self._cell)
-        return new_actors
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `abses-0.6.5/abses/data.py` & `abses-0.6.6/abses/tools/data.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/decision.py` & `abses-0.6.6/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/experiment.py` & `abses-0.6.6/abses/experiment.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/human.py` & `abses-0.6.6/abses/human.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Set, Union
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
-from loguru import logger
-
 from abses.actor import Actor
 from abses.links import _LinkContainer
 
 from ._bases.modules import CompositeModule, Module
 from .cells import PatchCell
 from .container import _AgentsContainer
 from .sequences import ActorsList, Selection
```

### Comparing `abses-0.6.5/abses/links.py` & `abses-0.6.6/abses/links.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,40 +24,57 @@
     List,
     Literal,
     Optional,
     Set,
     Tuple,
     Union,
     cast,
+    overload,
 )
 
+import numpy as np
+import pandas as pd
+from loguru import logger
+
 with contextlib.suppress(ImportError):
     import networkx as nx
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from abses._bases.errors import ABSESpyError
 from abses.sequences import ActorsList
+from abses.tools.func import make_list
+from abses.tools.viz import get_marker
 
 if TYPE_CHECKING:
     from abses import MainModel
     from abses.actor import Actor
     from abses.cells import PatchCell
-    from abses.container import _CellAgentsContainer
+    from abses.container import UniqueID, _CellAgentsContainer
     from abses.sequences import Link
 
 LinkingNode: TypeAlias = "Actor | PatchCell"
 Direction: TypeAlias = Optional[Literal["in", "out"]]
 DEFAULT_TARGETS: Tuple[str, str] = ("cell", "actor")
 TargetName: TypeAlias = Union[Literal["cell", "actor", "self"], str]
 AttrGetter: TypeAlias = Union["Link", ActorsList["Link"]]
 
 
+def get_node_unique_id(node: Any) -> UniqueID:
+    """When import actors from graph, decide the unique ID."""
+    if not isinstance(node, (str, int)):
+        logger.warning(
+            f"Using repr for '{type(node)}' unique ID to create actor."
+        )
+        return repr(node)
+    return node
+
+
 class _LinkContainer:
     """Container for links."""
 
     def __init__(self) -> None:
         self._back_links: Dict[str, Dict[LinkingNode, Set]] = {}
         self._links: Dict[str, Dict[LinkingNode, Set]] = {}
         self._cached_networks: Dict[str, object] = {}
@@ -85,30 +102,45 @@
             links_out = self.owns_links(node, direction="out")
             return tuple(set(links_in) | set(links_out))
         else:
             raise ValueError(f"Invalid direction '{direction}'.")
         links = {link for link, agents in data.items() if node in agents}
         return tuple(links)
 
-    def get_graph(self, link_name: str) -> "nx.Graph":  # type: ignore
+    @overload
+    def get_graph(
+        self, link_name: str, directions: bool = False
+    ) -> "nx.Graph":
+        ...
+
+    @overload
+    def get_graph(
+        self, link_name: str, directions: bool = True
+    ) -> "nx.DiGraph":
+        ...
+
+    def get_graph(
+        self, link_name: str, directions: bool = False
+    ) -> "nx.Graph | nx.DiGraph":
         """Get the networkx graph.
 
         Parameters:
             link_name:
                 The link name for converting into a graph.
 
         Raises:
             ImportError:
                 If networkx is not installed.
         """
         if "nx" not in globals():
             raise ImportError(
                 "You need to install networkx to use this function."
             )
-        graph = nx.from_dict_of_lists(self._links[link_name])
+        creating_using = nx.DiGraph if directions else nx.Graph
+        graph = nx.from_dict_of_lists(self._links[link_name], creating_using)
         self._cached_networks[link_name] = graph
         return graph
 
     def _register_link(
         self, link_name: str, source: LinkingNode, target: LinkingNode
     ) -> None:
         """Register a link."""
@@ -300,14 +332,49 @@
         agents: Set[LinkingNode] = set()
         for name in link_names:
             if name not in data and default:
                 continue
             agents = agents.union(data[name].get(node, set()))
         return agents
 
+    def _check_is_node(
+        self,
+        node: UniqueID | LinkingNode,
+        mapping_dict: Optional[Dict[UniqueID, Actor]] = None,
+    ) -> LinkingNode:
+        if mapping_dict:
+            unique_id = get_node_unique_id(node)
+            node = mapping_dict[unique_id]
+        if not isinstance(node, _LinkNode):
+            raise TypeError(
+                f"Invalid node type {type(node)}, mapping: {mapping_dict}."
+            )
+        return node
+
+    def add_links_from_graph(
+        self,
+        graph: "nx.Graph",
+        link_name: str,
+        mapping_dict: Optional[Dict[UniqueID, Actor]] = None,
+        mutual: Optional[bool] = None,
+    ) -> None:
+        """Add links from graph."""
+        if mutual is None:
+            mutual = False if isinstance(graph, nx.DiGraph) else True
+        if mapping_dict is None:
+            mapping_dict = {}
+        edges = 0
+        for source, targets in nx.to_dict_of_lists(graph).items():
+            source = self._check_is_node(source, mapping_dict)
+            for target in targets:
+                target = self._check_is_node(target, mapping_dict)
+                self.add_a_link(link_name, source, target, mutual=mutual)
+                edges += 1
+        logger.info(f"Imported links {edges} links from graph {graph}.")
+
 
 class _LinkProxy:
     """Proxy for linking."""
 
     def __init__(self, node: LinkingNode, model: MainModel) -> None:
         self.node: LinkingNode = node
         self.model: MainModel = model
@@ -464,18 +531,21 @@
     breed = _BreedDescriptor()
 
     @abstractmethod
     def _default_redirection(self, target: Optional[TargetName]) -> AttrGetter:
         """默认重定向"""
 
     @classmethod
-    def viz_attrs(cls, **kwargs) -> Dict[str, Any]:
+    def viz_attrs(
+        cls, render_marker: bool = False, **kwargs
+    ) -> Dict[str, Any]:
         """Return the attributes for viz."""
+        maker = getattr(cls, "marker", "o")
         return {
-            "marker": getattr(cls, "marker", "o"),
+            "marker": get_marker(maker) if render_marker else maker,
             "color": getattr(cls, "color", "black"),
             "alpha": getattr(cls, "alpha", 1.0),
         } | kwargs
 
     @cached_property
     def link(self) -> _LinkProxy:
         """A proxy which can be used to manipulate the links:
@@ -569,14 +639,34 @@
                 target is None
             ), f"The target '{target}' is set when '{self}' already has attr '{attr}'."
             setattr(self, attr, value)
         else:
             new_target = self._redirect_getting(target=target)
             new_target.set(attr, value, "self")
 
+    def summary(
+        self,
+        coords: bool = False,
+        attrs: Optional[Iterable[str] | str] = None,
+    ) -> pd.Series:
+        """Returns a summary of the object."""
+        geo_type = self.get("geo_type")
+        if geo_type in ("Point", "Cell"):
+            a, b = self.get("coordinate" if coords else "pos")
+        else:
+            a, b = np.nan, np.nan
+        result = {
+            "breed": self.breed,
+            "geo_type": geo_type,
+            "x" if coords else "row": a,
+            "y" if coords else "col": b,
+        }
+        result.update({attr: self.get(attr) for attr in make_list(attrs)})
+        return pd.Series(result, name=self.unique_id)
+
 
 class _LinkNodeCell(_LinkNode):
     def _default_redirection(
         self, target: Optional[TargetName]
     ) -> _CellAgentsContainer | _LinkNodeCell:
         if target == "cell":
             return self
```

### Comparing `abses-0.6.5/abses/main.py` & `abses-0.6.6/abses/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     logger,
     setup_logger_info,
 )
 from abses.actor import Actor
 
 from ._bases.bases import _Notice
 from ._bases.states import _States
-from .container import _AgentsContainer
+from .container import _AgentsContainer, _ModelAgentsContainer
 from .human import BaseHuman
 from .nature import BaseNature
 from .sequences import ActorsList
 from .time import TimeDriver
 from .viz.viz_model import _VizModel
 
 if TYPE_CHECKING:
@@ -125,15 +125,15 @@
         self.running: bool = True
         self._breeds: Dict[str, Type[Actor]] = {}
         self._containers: List[_AgentsContainer] = []
         self._settings = DictConfig(parameters)
         self._version: str = __version__
         self._logging_begin()  # logging
         self._check_subsystems(h_cls=human_class, n_cls=nature_class)
-        self._agents = _AgentsContainer(
+        self._agents = _ModelAgentsContainer(
             model=self, max_len=kwargs.get("max_agents")
         )
         self._time = TimeDriver(model=self)
         self.schedule: BaseScheduler = BaseScheduler(model=self)
         self.initialize_data_collector()
         self._do_each("initialize", order=("nature", "human"))
         self._do_each("set_state", code=1)  # initial state
@@ -255,15 +255,15 @@
         users can access the parameter 'test' by both ways:
             1. `model.nature.params.test`.
             2. `model.nature.p.test`.
         """
         return self._settings
 
     @property
-    def agents(self) -> _AgentsContainer:
+    def agents(self) -> _ModelAgentsContainer:
         """The container of all agents.
         One model only has one specific container where all alive agents are stored.
         Users can access, manipulate, and create agents by this container:
 
         For instances:
         1. `model.agents.get()` to access all agents.
         2. `model.agents.new(Actor, num=3)` to create 3 agents of Actor.
@@ -299,17 +299,17 @@
         """The global parameters of this model."""
         return self.settings.get("model", DictConfig({}))
 
     # alias for model's parameters
     p = params
 
     @property
-    def breeds(self) -> Tuple[str, ...]:
+    def breeds(self) -> Dict[str, Type[Actor]]:
         """All breeds in the model."""
-        return tuple(self._breeds.keys())
+        return self._breeds
 
     @breeds.setter
     def breeds(self, breed: Type[Actor]) -> None:
         """Register a new breed of agents in the model."""
         if not issubclass(breed, Actor):
             raise TypeError(f"{breed} is not a subclass of Actor.")
         self._breeds[breed.breed] = breed
```

### Comparing `abses-0.6.5/abses/move.py` & `abses-0.6.6/abses/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,17 +67,16 @@
     if agent.on_earth:
         agent.move.off()
     # before moving to the new cell, agent may do something
     keep_moving = agent.moving(cell=cell)
     if keep_moving is False:
         return
     # put the agent on the new cell after check.
-    cell.agents.add(agent, register=True)
+    cell.agents.add(agent)
     agent.at = cell
-    # self.geometry = Point(cell.layer.transform * cell.indices)
 
 
 def move_agent_to(
     agent: Actor,
     layer: PatchModule,
     pos: Coordinate | _LinkNodeCell,
 ) -> None:
```

### Comparing `abses-0.6.5/abses/nature.py` & `abses-0.6.6/abses/nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/patch.py` & `abses-0.6.6/abses/patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,33 @@
     Callable,
     Dict,
     Iterator,
     Literal,
     Optional,
     Sequence,
     Set,
+    Tuple,
     Type,
     Union,
     cast,
     overload,
 )
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
+import geopandas as gpd
 import numpy as np
 import pyproj
 import rasterio
 import rioxarray
 import xarray as xr
+from geocube.api.core import make_geocube
 from loguru import logger
 from mesa.space import Coordinate
 from mesa_geo.raster_layers import RasterBase
 from rasterio import mask
 from rasterio.enums import Resampling
 from rasterio.warp import calculate_default_transform, transform_bounds
 from shapely import Geometry
@@ -160,25 +163,95 @@
             width=layer.width,
             height=layer.height,
             crs=layer.crs,
             total_bounds=layer.total_bounds,
             cell_cls=cell_cls,
         )
 
+    def from_xarray(
+        self,
+        xda: xr.DataArray,
+        model: MainModel[Any, Any],
+        module_cls: Optional[Type[PatchModule]] = None,
+        name: str | None = None,
+        attr_name: str | None = None,
+        apply_raster: bool = False,
+        masked: bool = True,
+        cell_cls: type[PatchCell] = PatchCell,
+        **kwargs,
+    ) -> PatchModule:
+        """Create a new module instance from `xarray.DataArray` data."""
+        # 如果 y 轴是从小到大的，反转它
+        if xda.y[0].item() < xda.y[-1].item():
+            xda.data = np.flipud(xda.data)
+        # 创建模块
+        to_create = cast(PatchModule, self._check_cls(module_cls=module_cls))
+        module: PatchModule = to_create(
+            model=model,
+            name=name,
+            width=xda.rio.width,
+            height=xda.rio.height,
+            crs=xda.rio.crs,
+            total_bounds=xda.rio.bounds(),
+            cell_cls=cell_cls,
+        )
+        if masked:
+            module.mask = xda.notnull().to_numpy()
+        if apply_raster:
+            module.apply_raster(xda.to_numpy(), attr_name=attr_name, **kwargs)
+        return module
+
+    def from_vector(
+        self,
+        vector_file: str | gpd.GeoDataFrame,
+        resolution: Tuple[float, float] | float,
+        model: MainModel[Any, Any],
+        module_cls: Optional[Type[PatchModule]] = None,
+        name: str | None = None,
+        attr_name: Optional[str] = None,
+        apply_raster: bool = False,
+        masked: bool = True,
+        cell_cls: type[PatchCell] = PatchCell,
+    ) -> PatchModule:
+        """Create a layer module from a shape file."""
+        if isinstance(vector_file, str):
+            gdf = gpd.read_file(vector_file)
+        elif isinstance(vector_file, gpd.GeoDataFrame):
+            gdf = vector_file
+        else:
+            raise TypeError(f"Unsupported vector {type(vector_file)}.")
+        if attr_name is None:
+            gdf, attr_name = gdf.reset_index(), "index"
+        if isinstance(resolution, float):
+            resolution = (resolution, resolution)
+        xda = make_geocube(
+            gdf, measurements=[attr_name], resolution=resolution
+        )[attr_name]
+        return self.from_xarray(
+            xda=xda,
+            model=model,
+            module_cls=module_cls,
+            name=name,
+            attr_name=attr_name,
+            apply_raster=apply_raster,
+            masked=masked,
+            cell_cls=cell_cls,
+        )
+
     def from_file(
         self,
         raster_file: str,
         model: MainModel[Any, Any],
         cell_cls: type[PatchCell] = PatchCell,
         module_cls: Optional[Type[PatchModule]] = None,
         name: str | None = None,
         attr_name: str | None = None,
         apply_raster: bool = False,
         band: int = 1,
-        apply_nodata: bool = True,
+        masked: bool = True,
         **kwargs: Any,
     ) -> PatchModule:
         """Create a raster layer module from a file.
 
         Parameters:
             raster_file:
                 File path of a geo-tiff dataset.
@@ -190,41 +263,26 @@
                 Name of the new module.
                 If None (by default), using lowercase of the '__class__.__name__'.
                 E.g., class Module -> module.
             cell_cls:
                 Class type of `PatchCell` to create.
 
         """
-        to_create = cast(PatchModule, self._check_cls(module_cls=module_cls))
-        with rasterio.open(raster_file, "r") as dataset:
-            values = dataset.read(band).astype(float)
-            nodata_mask = values == dataset.nodata
-            set_null_values(values, nodata_mask)
-            height, width = values.shape
-            total_bounds = [
-                dataset.bounds.left,
-                dataset.bounds.bottom,
-                dataset.bounds.right,
-                dataset.bounds.top,
-            ]
-        obj: PatchModule = to_create(
+        xda = rioxarray.open_rasterio(raster_file, masked=masked, **kwargs)
+        xda = xda.sel(band=band)
+        return self.from_xarray(
+            xda=xda,
             model=model,
+            module_cls=module_cls,
             name=name,
-            width=width,
-            height=height,
-            crs=dataset.crs,
-            total_bounds=total_bounds,
+            attr_name=attr_name,
+            apply_raster=apply_raster,
+            masked=masked,
             cell_cls=cell_cls,
         )
-        if apply_nodata:
-            obj.mask = np.squeeze(~nodata_mask)
-        # obj._transform = dataset.transform
-        if apply_raster:
-            obj.apply_raster(values, attr_name=attr_name, **kwargs)
-        return obj
 
 
 class PatchModule(Module, RasterBase):
     """
     The spatial sub-module base class.
     Inherit from this class to create a submodule.
     [This tutorial](../tutorial/beginner/organize_model_structure.ipynb) shows the model structure.
@@ -357,27 +415,34 @@
         return 1, self.height, self.width
 
     @functools.cached_property
     def array_cells(self) -> np.ndarray:
         """Array type of the `PatchCell` stored in this module."""
         return self._cells
 
-    @functools.cached_property
+    @property
     def coords(self) -> Coordinate:
         """Coordinate system of the raster data.
+
         This is useful when working with `xarray.DataArray`.
         """
-        min_x, min_y, max_x, max_y = self.total_bounds
-        coords_x = np.linspace(min_x, max_x, self.width, endpoint=False)
-        coords_y = np.linspace(max_y, min_y, self.height, endpoint=False)
+        nrows, ncols = self.shape2d
+        coords_x = np.arange(ncols) * self.transform[0] + self.transform[2]
+        coords_y = np.arange(nrows) * self.transform[4] + self.transform[5]
         return {
             "y": coords_y,
             "x": coords_x,
         }
 
+    def transform_coord(self, row: int, col: int) -> Coordinate:
+        """Transforming the row, col to the real-world coordinate."""
+        if self.out_of_bounds(pos=(row, col)):
+            raise IndexError(f"Out of bounds: {row, col}")
+        return self.transform * (col, row)
+
     def to_crs(self, crs, inplace=False) -> Optional[PatchModule]:
         """Converting the raster data to a another CRS."""
         super()._to_crs_check(crs)
         layer = self if inplace else copy.copy(self)
 
         src_crs = rasterio.crs.CRS.from_user_input(layer.crs)
         dst_crs = rasterio.crs.CRS.from_user_input(crs)
```

### Comparing `abses-0.6.5/abses/random.py` & `abses-0.6.6/abses/random.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/selection.py` & `abses-0.6.6/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/sequences.py` & `abses-0.6.6/abses/sequences.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,31 +26,36 @@
     Sized,
     TypeVar,
     Union,
     cast,
     overload,
 )
 
+import pandas as pd
+from loguru import logger
+from pyproj import CRS
+
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
+import geopandas as gpd
 import mesa_geo as mg
 import numpy as np
 from numpy.typing import NDArray
 
 from abses._bases.errors import ABSESpyError
 from abses.random import ListRandom
 from abses.selection import selecting
 from abses.tools.func import make_list
 from abses.viz.viz_actors import _VizNodeList
 
 if TYPE_CHECKING:
-    from abses.actor import Actor, TargetName
+    from abses.actor import Actor, GeoType, TargetName
     from abses.links import _LinkNode
     from abses.main import MainModel
 
 Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, Any]]
 HOW: TypeAlias = Literal["only", "random", "item"]
 Link = TypeVar("Link", bound="_LinkNode")
 
@@ -116,15 +121,15 @@
     def random(self) -> ListRandom:
         """Random module"""
         return ListRandom(actors=self, model=self._model)
 
     @cached_property
     def plot(self) -> _VizNodeList:
         """Plotting module"""
-        return _VizNodeList(self)
+        return _VizNodeList(self._model, self)
 
     def to_dict(self) -> Dict[str, ActorsList[Link]]:
         """Convert all actors in this list to a dictionary like {breed: ActorList}.
 
         Returns:
             key is the breed of actors, and values are corresponding actors.
         """
@@ -133,30 +138,54 @@
             breed = actor.breed
             if breed not in dic:
                 dic[breed] = ActorsList(self._model, [actor])
             else:
                 dic[breed].append(actor)
         return dic
 
-    def select(self, selection: Selection) -> ActorsList[Link]:
+    def _subset(
+        self, geo_type: Optional[GeoType | bool] = None
+    ) -> ActorsList[Link]:
+        """Returns dataset for plotting."""
+        if geo_type is None:
+            return self
+        if isinstance(geo_type, bool):
+            selection: Dict[str, Any] = {"on_earth": geo_type}
+        elif geo_type in ("Point", "Shape"):
+            selection = {"geo_type": geo_type}
+        return self.select(selection)
+
+    def select(
+        self,
+        selection: Optional[Selection] = None,
+        geo_type: Optional[GeoType] = None,
+    ) -> ActorsList[Link]:
         """
         Returns a new :class:`ActorList` based on `selection`.
 
         Parameters:
             selection:
                 List with same length as the agent list.
                 Positions that return True will be selected.
+            geo_type:
+                Type of Actors' Geometry.
+
+        Returns:
+            A subset containing.
         """
+        actors = self._subset(geo_type=geo_type)
+        if selection is None:
+            return actors
         if isinstance(selection, (str, dict)):
-            bool_ = [selecting(actor, selection) for actor in self]
+            bool_ = [selecting(actor, selection) for actor in actors]
         elif isinstance(selection, (list, tuple, np.ndarray)):
             bool_ = make_list(selection)
         else:
             raise TypeError(f"Invalid selection type {type(selection)}")
-        selected = [a for a, s in zip(self, bool_) if s]
+        selected = [a for a, s in zip(actors, bool_) if s]
         return ActorsList(self._model, selected)
 
     def ids(self, ids: Iterable[int]) -> ActorsList[Link]:
         """Subsets ActorsList by a `ids`.
 
         Parameters:
             ids:
@@ -344,7 +373,39 @@
             return get_only_agent(self)
         if how == "random":
             actor = self.random.choice(when_empty="return None")
             return cast(Optional["Actor"], actor)
         if how == "item":
             return self[index] if len(self) > index else None
         raise ValueError(f"Invalid how method '{how}'.")
+
+    def _check_crs_consistent(self) -> CRS:
+        crs_set = set(self.array("crs"))
+        if None in crs_set:
+            logger.warning("Some agents don't have a crs.")
+            crs_set.remove(None)
+        if len(crs_set) > 1:
+            raise ValueError(f"More than one crs: {crs_set}.")
+        if len(crs_set) == 0:
+            logger.warning("No crs when init a GeoDataFrame.")
+        return crs_set.pop()
+
+    @overload
+    def summary(self, geometry: bool = True, **kwargs) -> gpd.GeoDataFrame:
+        ...
+
+    @overload
+    def summary(self, geometry: bool = False, **kwargs) -> pd.DataFrame:
+        ...
+
+    def summary(
+        self, geometry: bool = False, **kwargs
+    ) -> pd.DataFrame | gpd.GeoDataFrame:
+        """Returns a summarized dataframe of the actors."""
+        if len(self) == 0:
+            raise ValueError("No actors to retrieve summary information.")
+        df = pd.concat([actor.summary(**kwargs) for actor in self], axis=1).T
+        if geometry:
+            crs = self._check_crs_consistent()
+            df["geometry"] = self.array("geometry")
+            return gpd.GeoDataFrame(df, geometry="geometry", crs=crs)
+        return df
```

### Comparing `abses-0.6.5/abses/time.py` & `abses-0.6.6/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/tools/func.py` & `abses-0.6.6/abses/tools/func.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,29 +5,44 @@
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
 """
 这个模块储存一些
 """
 
-import logging
 from functools import wraps
-from typing import Any, Callable, List, Optional, Tuple, TypeVar, cast
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    TypeVar,
+    cast,
+    overload,
+)
 
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from scipy import ndimage
 
 from abses.tools.regex import CAMEL_NAME
 
-logger = logging.getLogger(__name__)
+try:
+    from typing import TypeAlias
+except ImportError:
+    from typing_extensions import TypeAlias
 
 F = TypeVar("F", bound=Callable[..., Any])
 
+IncludeFlag: TypeAlias = str | bool | Iterable[str] | Dict[str, str]
+
 
 def get_buffer(
     array: np.ndarray,
     radius: int = 1,
     moor: bool = False,
     annular: bool = False,
 ) -> np.ndarray:
@@ -178,7 +193,55 @@
     # # Byte string
     elif arr.dtype.kind == "S":
         null_value = b""
     else:
         raise ValueError(f"Unsupported data type {arr.dtype}")
     arr[mask] = null_value
     return arr
+
+
+@overload
+def clean_attrs(
+    all_attrs: Iterable[str],
+    include: Optional[IncludeFlag],
+    exclude: Optional[Iterable[str]] = None,
+) -> Dict[str, str]:
+    ...
+
+
+@overload
+def clean_attrs(
+    all_attrs: Iterable[str],
+    include: Dict[str, str],
+    exclude: Optional[Iterable[str]] = None,
+) -> Dict[str, str]:
+    ...
+
+
+def clean_attrs(
+    all_attrs: Iterable[str],
+    include: Optional[IncludeFlag | Dict[str, str]] = True,
+    exclude: Optional[Iterable[str]] = None,
+) -> List[str] | Dict[str, str]:
+    """
+    Clean attributes based on include and exclude lists.
+
+    Parameters:
+        all_attrs:
+            All attributes to clean.
+        include:
+            Attributes to include.
+        exclude:
+            Attributes to exclude.
+
+    Returns:
+        The cleaned attributes.
+    """
+    if isinstance(include, dict):
+        attrs = clean_attrs(all_attrs, list(include.keys()), exclude)
+        return {attr: include[attr] for attr in attrs}
+    if isinstance(include, bool):
+        include = all_attrs if include else None
+    selected = set(all_attrs) & set(make_list(include))
+    if exclude:
+        selected -= set(make_list(exclude))
+    return list(selected)
```

### Comparing `abses-0.6.5/abses/tools/regex.py` & `abses-0.6.6/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/viz/viz_model.py` & `abses-0.6.6/abses/viz/viz_model.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/abses/viz/viz_nature.py` & `abses-0.6.6/abses/viz/viz_actors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,145 +1,135 @@
 #!/usr/bin/env python 3.11.0
 # -*-coding:utf-8 -*-
 # @Author  : Shuang (Twist) Song
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
-"""Viz natural module.
+"""Visualize ActorsList
 """
 from __future__ import annotations
 
-import importlib.resources as pkg_resources
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Type, cast
+import contextlib
+from pathlib import Path
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
-import fontawesome as fa
-import matplotlib.markers as markers
-import numpy as np
-import pandas as pd
+import geopandas as gpd
 import seaborn as sns
+from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
-from matplotlib.font_manager import FontProperties
-from matplotlib.path import Path
-from matplotlib.textpath import TextToPath
 
 from abses.tools.func import with_axes
 
+with contextlib.suppress(ImportError):
+    import networkx as nx
+try:
+    from typing import TypeAlias
+except ImportError:
+    from typing_extensions import TypeAlias
+
 if TYPE_CHECKING:
-    from abses.actor import Actor
-    from abses.nature import PatchModule
+    from abses.actor import Actor, GeoType
+    from abses.main import MainModel
+    from abses.sequences import ActorsList
+
+StyleDict: TypeAlias = Dict[str, Dict[str, Any]]
 
-COLOR_BAR = {"fraction": 0.03, "pad": 0.04}
 
-FONT = pkg_resources.files("icons") / "fa-regular-400.otf"
-FONT_AWESOME = FontProperties(fname=str(FONT))
+class _VizNodeList:
+    def __init__(self, model: MainModel, actors: ActorsList) -> None:
+        self.actors = actors
+        self.model = model
 
+    @with_axes(figsize=(6, 4))
+    def hist(
+        self,
+        attr: str,
+        ax: Optional[Axes] = None,
+        savefig: Optional[str | Path] = None,
+        palette: Optional[str | Dict] = None,
+    ):
+        """Plot hist."""
+        df = self.actors.summary(attrs=attr)
+        if palette is None:
+            palette = self._style_dict("color", "blue")
+        sns.histplot(df, x=attr, ax=ax, hue="breed", palette=palette)
+        if savefig:
+            plt.savefig(savefig)
+            plt.close()
+        return ax
 
-# https://stackoverflow.com/questions/52902086/how-to-use-font-awesome-symbol-as-marker-in-matplotlib
-def get_marker(symbol: str) -> Path:
-    """Returns Font Awesome marker."""
-    if symbol in markers.MarkerStyle.markers:
-        return symbol
-    symbol = fa.icons.get(symbol)
-    if not symbol:
-        raise KeyError(f"Could not find {symbol} in marker style.")
-    v, codes = TextToPath().get_text_path(FONT_AWESOME, symbol)
-    v = np.array(v)
-    mean = np.mean([np.max(v, axis=0), np.min(v, axis=0)], axis=0)
-    return Path(v - mean, codes, closed=False)
-
-
-class _VizNature:
-    """Visualize the nature module"""
-
-    def __init__(self, module: PatchModule):
-        self.module = module
-        self.model = module.model
-
-    def _retrieve_marker(self, breed, **kwargs) -> Dict[str, str]:
-        breed_cls: Type[Actor] = getattr(self.model, "_breeds")[breed]
-        marker_kwargs = breed_cls.viz_attrs(**kwargs)
-        marker_kwargs["marker"] = get_marker(marker_kwargs["marker"])
-        return marker_kwargs
-
-    def _stat_actors(self, breed: str) -> pd.DataFrame:
-        matrix = self.module.apply(lambda c: c.agents.has(breed))
-        rows, cols = np.where(matrix)
-        rows_coords = self.module.coords["y"][rows]
-        cols_coords = self.module.coords["x"][cols]
-        numbers = matrix[rows, cols]
-        return pd.DataFrame(
-            {
-                "x": cols_coords,
-                "y": rows_coords,
-                "Number": numbers.flatten(),
-                "Breed": breed,
-            }
+    def _style_dict(self, request: str, default: Any, **kwargs) -> StyleDict:
+        styles = {}
+        for breed in self.actors.to_dict().keys():
+            breed_cls = self.model.breeds[breed]
+            style_dict = breed_cls.viz_attrs(render_marker=True, **kwargs)
+            styles[breed] = style_dict.get(request, default)
+        return styles
+
+    @with_axes
+    def show(self, ax: Optional[Axes] = None) -> Axes:
+        """Show all the actors with geometry attributes."""
+        self.display(ax=ax)
+        self.positions(ax=ax)
+        return ax
+
+    @with_axes
+    def display(
+        self, boundary: bool = False, ax: Optional[Axes] = None, **kwargs
+    ) -> Axes:
+        """Show the shapefile."""
+        alpha = kwargs.pop("alpha", 0.8)
+        subset = self.actors.select(geo_type="Shape")
+        if not subset:
+            return ax
+        data = gpd.GeoSeries(
+            subset.array("geometry"), crs=self.model.nature.crs
         )
+        obj = data.boundary if boundary else data
+        obj.plot(ax=ax, alpha=alpha, **kwargs)
+        return ax
 
     @with_axes
-    def scatter(
+    def positions(
         self,
-        breeds: Optional[Iterable[str]] = None,
-        size: Optional[str] = None,
-        hue: Optional[str] = None,
+        coords: bool = True,
         ax: Optional[Axes] = None,
-        # sizes: Tuple[int, int] = (20, 200),
+        hue: Optional[str] = "breed",
+        size: Optional[str] = None,
         palette: Optional[str | Dict] = None,
         **kwargs,
     ) -> Axes:
-        """Adding"""
-        data = []
-        if breeds is None:
-            breeds = self.model.breeds
-        markers_used = {}
-        colors = {}
-        for breed in breeds:
-            data.append(self._stat_actors(breed=breed))
-            style_dict = self._retrieve_marker(breed, **kwargs)
-            markers_used[breed] = style_dict["marker"]
-            colors[breed] = style_dict["color"]
-        df = pd.concat(data, axis=0)
-        if palette is None and hue == "Breed":
-            palette = colors
+        """Plotting spatial distribution of the actors."""
+        points = self.actors.select(geo_type="Point")
+        if not points:
+            return ax
+        data = points.summary(coords=coords)
+        y_axis = "y" if coords else "row"
+        x_axis = "x" if coords else "col"
+        count_data = (
+            data.groupby([y_axis, x_axis, "breed"])
+            .size()
+            .reset_index(name="count")
+        )
+        if hue == "breed":
+            palette = self._style_dict("color", "blue")
         sns.scatterplot(
-            df,
-            x="x",
-            y="y",
-            ax=ax,
+            x=x_axis,
+            y=y_axis,
             size=size,
-            style="Breed",
+            data=count_data,
             hue=hue,
-            markers=markers_used,
-            # sizes=sizes,
+            ax=ax,
+            style="breed",
+            markers=self._style_dict("marker", "o"),
             palette=palette,
+            **kwargs,
         )
         return ax
 
     @with_axes
-    def show(
-        self,
-        attr: Optional[str] = None,
-        ax: Optional[Axes] = None,
-        with_actors: bool = True,
-        scatter_kwargs: Optional[Dict[str, Any]] = None,
-        legend_kwargs: Optional[Dict[str, Any]] = None,
-    ) -> Axes:
-        """Show the nature module"""
-        if scatter_kwargs is None:
-            scatter_kwargs = {}
-        if legend_kwargs is None:
-            legend_kwargs = {}
-        # because of `with_axes`, it must be a valid Axes object
-        ax = cast(Axes, ax)
-        if attr is None:
-            xda = self.module.xda
-            xda.plot(ax=ax, add_colorbar=False, alpha=0.8)
-        else:
-            xda = self.module.get_xarray(attr)
-            xda.plot(ax=ax, cbar_kwargs=COLOR_BAR, alpha=0.8)
-        if self.model.breeds and with_actors:
-            self.scatter(ax=ax, **scatter_kwargs)
-        ax.axes.set_aspect("equal")
-        if self.model.breeds:
-            ax.legend(**legend_kwargs)
+    def graph(self, link_name: str, ax: Optional[Axes] = None) -> Axes:
+        """Plotting the Graph of selected actors by `networkx`."""
+        graph = self.model.human.get_graph(link_name).subgraph(self.actors)
+        nx.draw(graph, arrows=True, with_labels=True, ax=ax)
         return ax
```

### Comparing `abses-0.6.5/data/.DS_Store` & `abses-0.6.6/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/data/YR_cities.zip` & `abses-0.6.6/data/YR_cities.zip`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/data/farmland.tif` & `abses-0.6.6/data/farmland.tif`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/data/irr_lands.csv` & `abses-0.6.6/data/irr_lands.csv`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/data/precipitation.nc` & `abses-0.6.6/data/precipitation.nc`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/icons/fa-regular-400.otf` & `abses-0.6.6/icons/fa-regular-400.otf`

 * *Files identical despite different names*

### Comparing `abses-0.6.5/pyproject.toml` & `abses-0.6.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.6.5"
+version = "0.6.6"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 include = [
   "icons/fa-regular-400.otf",
   "abses/conf/**/*.yaml",
@@ -44,27 +44,28 @@
   "hydra_plugins.abses_searchpath_plugin"
 ]
 
 [tool.poetry.plugins."hydra.searchpath"]
 abses = "hydra_plugins.abses_searchpath_plugin:ABSESpySearchPathPlugin"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.10,<3.12"
 netcdf4 = ">=1.6"
 hydra-core = "~1.3"
 mesa-geo = ">=0.6"
 xarray = ">=2023"
 fiona = ">1.8"
 loguru = ">=0.7"
 rioxarray = ">=0.13"
 pendulum = "~2"
 geopandas = "~0"
 typing-extensions = "~4"
 fontawesome = ">=5"
 seaborn = ">=0.13"
+geocube = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest-clarity = "^1.0.1"
 pre-commit = "^3.0.1"
 scriv = "^1.2.0"
 pytest = "^7.2.1"
 sourcery = "^1.0.6"
```

### Comparing `abses-0.6.5/PKG-INFO` & `abses-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.6.5
+Version: 0.6.6
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fiona (>1.8)
 Requires-Dist: fontawesome (>=5)
+Requires-Dist: geocube (>=0.5.2,<0.6.0)
 Requires-Dist: geopandas (>=0,<1)
 Requires-Dist: hydra-core (>=1.3,<1.4)
 Requires-Dist: loguru (>=0.7)
 Requires-Dist: mesa-geo (>=0.6)
 Requires-Dist: netcdf4 (>=1.6)
 Requires-Dist: pendulum (>=2,<3)
 Requires-Dist: rioxarray (>=0.13)
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: abses Version: 0.6.5 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.6.6 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
->=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
+>=3.10,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
-Dist: fontawesome (>=5) Requires-Dist: geopandas (>=0,<1) Requires-Dist: hydra-
-core (>=1.3,<1.4) Requires-Dist: loguru (>=0.7) Requires-Dist: mesa-geo (>=0.6)
-Requires-Dist: netcdf4 (>=1.6) Requires-Dist: pendulum (>=2,<3) Requires-Dist:
-rioxarray (>=0.13) Requires-Dist: seaborn (>=0.13) Requires-Dist: typing-
-extensions (>=4,<5) Requires-Dist: xarray (>=2023) Description-Content-Type:
-text/markdown # ABSESpy: Agent-Based Modeling Framework for Social-Ecological
-Systems ![ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-
-beijing.myqcloud.com/uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fiona
+(>1.8) Requires-Dist: fontawesome (>=5) Requires-Dist: geocube (>=0.5.2,<0.6.0)
+Requires-Dist: geopandas (>=0,<1) Requires-Dist: hydra-core (>=1.3,<1.4)
+Requires-Dist: loguru (>=0.7) Requires-Dist: mesa-geo (>=0.6) Requires-Dist:
+netcdf4 (>=1.6) Requires-Dist: pendulum (>=2,<3) Requires-Dist: rioxarray
+(>=0.13) Requires-Dist: seaborn (>=0.13) Requires-Dist: typing-extensions
+(>=4,<5) Requires-Dist: xarray (>=2023) Description-Content-Type: text/markdown
+# ABSESpy: Agent-Based Modeling Framework for Social-Ecological Systems !
+[ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-beijing.myqcloud.com/
+uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_R_e_p_o
 _S_i_z_e_]_[_f_o_l_l_o_w_ _o_n_ _T_w_i_t_t_e_r_]_[_g_i_t_h_u_b_]--- Language: [English Readme] | [ç®ä½ä¸­æ]
                                     **[â
                                  âInstallâ
                             â][Install]** **[â
                              âGetting startedâ
                         â][Getting Started]** **[â
```

