# Comparing `tmp/dongraphio-0.3.3.tar.gz` & `tmp/dongraphio-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dongraphio-0.3.3.tar", max compression
+gzip compressed data, was "dongraphio-0.3.4.tar", max compression
```

## Comparing `dongraphio-0.3.3.tar` & `dongraphio-0.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1469 2024-05-17 11:52:05.679820 dongraphio-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1384 2024-05-07 09:01:32.594501 dongraphio-0.3.3/README.md
--rw-r--r--   0        0        0      262 2024-05-17 11:52:24.405407 dongraphio-0.3.3/src/dongraphio/__init__.py
--rw-r--r--   0        0        0      133 2024-05-07 09:01:37.910553 dongraphio-0.3.3/src/dongraphio/base_models/__init__.py
--rw-r--r--   0        0        0    14979 2024-05-07 09:01:37.926179 dongraphio-0.3.3/src/dongraphio/base_models/grapher_logic.py
--rw-r--r--   0        0        0     5383 2024-05-07 09:01:37.941805 dongraphio-0.3.3/src/dongraphio/base_models/isochrones_logic.py
--rw-r--r--   0        0        0     2719 2024-05-07 09:01:37.941805 dongraphio-0.3.3/src/dongraphio/base_models/matrix_logic.py
--rw-r--r--   0        0        0     6330 2024-05-17 11:50:10.665504 dongraphio-0.3.3/src/dongraphio/dongraphio.py
--rw-r--r--   0        0        0     1056 2024-05-07 09:01:37.848049 dongraphio-0.3.3/src/dongraphio/enums.py
--rw-r--r--   0        0        0      559 2024-05-07 09:01:38.004309 dongraphio-0.3.3/src/dongraphio/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-07 09:01:38.019935 dongraphio-0.3.3/src/dongraphio/utils/geometry_utils.py
--rw-r--r--   0        0        0    19283 2024-05-07 09:01:38.035562 dongraphio-0.3.3/src/dongraphio/utils/graph_utils.py
--rw-r--r--   0        0        0     2602 2024-05-07 09:01:38.051187 dongraphio-0.3.3/src/dongraphio/utils/matrix_utils.py
--rw-r--r--   0        0        0     1713 2024-05-07 09:01:38.066813 dongraphio-0.3.3/src/dongraphio/utils/osm_worker.py
--rw-r--r--   0        0        0     1647 2024-05-07 09:01:38.066813 dongraphio-0.3.3/src/dongraphio/utils/tsp_solver.py
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 dongraphio-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1400 2024-05-19 12:55:20.541236 dongraphio-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1384 2024-05-19 12:41:43.471387 dongraphio-0.3.4/README.md
+-rw-r--r--   0        0        0      245 2024-05-19 12:55:20.539237 dongraphio-0.3.4/src/dongraphio/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-19 12:41:43.473390 dongraphio-0.3.4/src/dongraphio/base_models/__init__.py
+-rw-r--r--   0        0        0    14979 2024-05-19 12:41:43.473390 dongraphio-0.3.4/src/dongraphio/base_models/grapher_logic.py
+-rw-r--r--   0        0        0     5383 2024-03-31 13:07:05.513564 dongraphio-0.3.4/src/dongraphio/base_models/isochrones_logic.py
+-rw-r--r--   0        0        0     2719 2024-05-19 12:41:43.474388 dongraphio-0.3.4/src/dongraphio/base_models/matrix_logic.py
+-rw-r--r--   0        0        0     6194 2024-05-19 12:42:22.439889 dongraphio-0.3.4/src/dongraphio/dongraphio.py
+-rw-r--r--   0        0        0     1056 2024-05-19 12:41:43.431091 dongraphio-0.3.4/src/dongraphio/enums.py
+-rw-r--r--   0        0        0      523 2024-05-19 12:43:26.743296 dongraphio-0.3.4/src/dongraphio/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-19 12:41:43.475388 dongraphio-0.3.4/src/dongraphio/utils/geometry_utils.py
+-rw-r--r--   0        0        0    19283 2024-05-19 12:41:43.476388 dongraphio-0.3.4/src/dongraphio/utils/graph_utils.py
+-rw-r--r--   0        0        0     2602 2024-05-19 12:41:43.477391 dongraphio-0.3.4/src/dongraphio/utils/matrix_utils.py
+-rw-r--r--   0        0        0     1713 2024-05-19 12:41:43.477391 dongraphio-0.3.4/src/dongraphio/utils/osm_worker.py
+-rw-r--r--   0        0        0     1647 2024-03-31 14:31:51.764945 dongraphio-0.3.4/src/dongraphio/utils/tsp_solver.py
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 dongraphio-0.3.4/PKG-INFO
```

### Comparing `dongraphio-0.3.3/pyproject.toml` & `dongraphio-0.3.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-[tool.poetry]
-name = "dongraphio"
-version = "0.3.3"
-description = "Small utility library containing graph algorighms used in other projects"
-authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
-readme = "README.md"
-
-packages = [{ include = "dongraphio", from = "src" }]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-geopandas = "^0.14.3"
-osmnx = "^1.9.1"
-tqdm = "^4.66.2"
-osm2geojson = "^0.2.4"
-pydantic = "^2.6.1"
-momepy = "^0.6.0"
-networkit = "^11.0"
-numpy = "^1.23.5"
-pandas = "^2.2.0"
-networkx = "^3.2.1"
-loguru = "^0.7.2"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^24.2.0"
-pylint = "^3.0.3"
-isort = "^5.13.2"
-jupyter = "^1.0.0"
-ortools = "^9.9.3963"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.black]
-line-length = 120
-target-version = ['py310']
-
-[tool.pylint.format]
-max-line-length = 120
-expected-line-ending-format = "LF"
-max-locals = 20
-extension-pkg-allow-list = ["networkit"]
-disable = [
-    "duplicate-code",
-    "missing-module-docstring",
-    "missing-function-docstring",
-]
-good-names = [
-    "G",
-    "G_ox",
-    "G_nx",
-    "G_nk",
-    "G_walk",
-    "G_drive",
-    "G_base",
-    "G_to_project",
-    "G_public_transport",
-]
-
-[tool.isort]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-line_length = 120
-split_on_trailing_comma = true
+[tool.poetry]
+name = "dongraphio"
+version = "0.3.4"
+description = "Small utility library containing graph algorighms used in other projects"
+authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
+readme = "README.md"
+
+packages = [{ include = "dongraphio", from = "src" }]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+geopandas = "^0.14.3"
+osmnx = "^1.9.1"
+tqdm = "^4.66.2"
+osm2geojson = "^0.2.4"
+pydantic = "^2.6.1"
+momepy = "^0.6.0"
+networkit = "^11.0"
+numpy = "^1.23.5"
+pandas = "^2.2.0"
+networkx = "^3.2.1"
+loguru = "^0.7.2"
+
+
+[tool.poetry.group.dev.dependencies]
+black = "^24.2.0"
+pylint = "^3.0.3"
+isort = "^5.13.2"
+jupyter = "^1.0.0"
+ortools = "^9.9.3963"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
+target-version = ['py310']
+
+[tool.pylint.format]
+max-line-length = 120
+expected-line-ending-format = "LF"
+max-locals = 20
+extension-pkg-allow-list = ["networkit"]
+disable = [
+    "duplicate-code",
+    "missing-module-docstring",
+    "missing-function-docstring",
+]
+good-names = [
+    "G",
+    "G_ox",
+    "G_nx",
+    "G_nk",
+    "G_walk",
+    "G_drive",
+    "G_base",
+    "G_to_project",
+    "G_public_transport",
+]
+
+[tool.isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+line_length = 120
+split_on_trailing_comma = true
```

### Comparing `dongraphio-0.3.3/README.md` & `dongraphio-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/base_models/grapher_logic.py` & `dongraphio-0.3.4/src/dongraphio/base_models/grapher_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/base_models/isochrones_logic.py` & `dongraphio-0.3.4/src/dongraphio/base_models/isochrones_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/base_models/matrix_logic.py` & `dongraphio-0.3.4/src/dongraphio/base_models/matrix_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/dongraphio.py` & `dongraphio-0.3.4/src/dongraphio/dongraphio.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from typing import Optional, Tuple
-
-import geopandas as gpd
-import networkx as nx
-import pandas as pd
-from loguru import logger
-
-from .base_models import BuildsAvailabilitier, BuildsGrapher, BuildsMatrixer
-from .enums import GraphType
-
-
-class DonGraphio:
-    def __init__(self, city_crs: int, intermodal_graph: nx.MultiDiGraph | None = None):
-        self.city_crs = city_crs
-        # self.graphs: dict[GraphType, nx.Graph] = {} # TODO: add graphs to Invoker
-
-        self._intermodal_graph = intermodal_graph
-
-    # TODO: replace non-alternative OSM integration with optional graphs build from OSM
-    # def try_build_graph_from_osm(self, graph_type: GraphType, osm_id: int) -> nx.Graph:
-    #     """Build a graph from OSM data and save it as the given graph type"""
-    #     raise NotImplementedError()
-
-    def get_graph(self) -> Optional[nx.DiGraph]:
-        """
-        Return the intermodal graph.
-
-        Returns:
-            Optional[nx.DiGraph]: The intermodal graph if it exists, else None.
-        Raises:
-            RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
-        """
-        if self._intermodal_graph is None:
-            raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
-        return self._intermodal_graph
-
-    def set_graph(self, graph: nx.DiGraph) -> None:
-        """
-        Set the intermodal graph for the object.
-
-        Args:
-            graph (nx.DiGraph): The graph to be set.
-        Returns:
-            None
-        """
-        self._intermodal_graph = graph
-
-    # TODO: update BuildsGrapher logic to construct from the graphs, fail if not all graphs are available
-
-    def get_intermodal_graph_from_osm(self, city_osm_id: int, keep_city_boundary: bool = True) -> nx.MultiDiGraph:
-        """
-        Retrieves the intermodal graph for a given city from OpenStreetMap.
-        Args:
-            city_osm_id (int): The OpenStreetMap ID of the city.
-            keep_city_boundary (bool, optional): Whether to keep the city boundary in the graph. Defaults to True.
-        Returns:
-            nx.MultiDiGraph: The intermodal graph representing the city.
-        """
-        # if not all(graph_type in self.graphs for graph_type in GraphType):
-        #     raise ValueError("Some graph types are missing")
-        logger.info("Creating intermodal graph from OSM...")
-        self._intermodal_graph = BuildsGrapher(
-            city_osm_id=city_osm_id, city_crs=self.city_crs, keep_city_boundary=keep_city_boundary
-        ).get_intermodal_graph()
-        return self._intermodal_graph
-
-    def get_adjacency_matrix(
-        self,
-        gdf_from: gpd.GeoDataFrame,
-        gdf_to: gpd.GeoDataFrame,
-        weight: str,
-        graph_type: list[GraphType] | None = None,
-    ) -> Optional[pd.DataFrame]:
-        """
-        Calculate the adjacency matrix between the given GeoDataFrames based on
-        the specified weight and intermodal graph.
-
-        Args:
-            gdf_from (gpd.GeoDataFrame): The GeoDataFrame containing the buildings.
-            gdf_to (gpd.GeoDataFrame): The GeoDataFrame containing the services.
-            weight (str): The weight attribute, could be only "time_min" or"length_meter".
-            graph_type (list[GraphType]): The List of Enum types of the graph to search shortest way.
-        Returns:
-            Optional[pd.DataFrame]: The adjacency matrix as a DataFrame, or None if the intermodal graph is not set.
-        Raises:
-            RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
-        """
-        if self._intermodal_graph is None:
-            raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
-        logger.info("Creating adjacency matrix based on provided graph...")
-        to_return = BuildsMatrixer(
-            gdf_from=gdf_from,
-            gdf_to=gdf_to,
-            weight=weight,
-            city_crs=self.city_crs,
-            nx_intermodal_graph=self._intermodal_graph,
-            graph_type=graph_type,
-        ).get_adjacency_matrix()
-        logger.info("Adjacency matrix done!")
-        return to_return
-
-    def get_accessibility_isochrones(
-        self, graph_type: list[GraphType], x_from: float, y_from: float, weight_value: int, weight_type: str
-    ) -> Tuple[gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]]:
-        """
-        Get accessibility isochrones and return three GeoDataFrame objects with isochrones, and
-        if graph_type contains GraphType.PUBLIC_TRANSPORT enum - routes and public transport stops.
-
-        Args:
-            graph_type (list[GraphType]): The List of Enum types of the graph to build isochrones.
-            x_from (float): The x-coordinate of the starting point in the corresponding coordinate system.
-            y_from (float): The y-coordinate of the starting point in the corresponding coordinate system.
-            weight_value (int): The value of the weight.
-            weight_type (str): The type of the weight, could be only "time_min" or "length_meter" .
-
-        Returns:
-            (gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]): Isochrones,routes,stops.
-        Raises:
-            RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
-        """
-        # Check if intermodal graph is set
-        if self._intermodal_graph is None:
-            raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
-        # Build accessibility isochrones
-        logger.info("Creating accessibility isochrones based on provided graph and point...")
-        to_return = BuildsAvailabilitier(
-            graph_type=graph_type,
-            city_crs=self.city_crs,
-            x_from=x_from,
-            y_from=y_from,
-            weight_value=weight_value,
-            weight_type=weight_type,
-            nx_intermodal_graph=self._intermodal_graph,
-        ).get_accessibility_isochrone()
-        logger.info("Accessibility isochrones done!\n")
-        return to_return
+from typing import Optional, Tuple
+
+import geopandas as gpd
+import networkx as nx
+import pandas as pd
+from loguru import logger
+
+from .base_models import BuildsAvailabilitier, BuildsGrapher, BuildsMatrixer
+from .enums import GraphType
+
+
+class DonGraphio:
+    def __init__(self, city_crs: int, intermodal_graph: nx.MultiDiGraph | None = None):
+        self.city_crs = city_crs
+        # self.graphs: dict[GraphType, nx.Graph] = {} # TODO: add graphs to Invoker
+
+        self._intermodal_graph = intermodal_graph
+
+    # TODO: replace non-alternative OSM integration with optional graphs build from OSM
+    # def try_build_graph_from_osm(self, graph_type: GraphType, osm_id: int) -> nx.Graph:
+    #     """Build a graph from OSM data and save it as the given graph type"""
+    #     raise NotImplementedError()
+
+    def get_graph(self) -> Optional[nx.DiGraph]:
+        """
+        Return the intermodal graph.
+
+        Returns:
+            Optional[nx.DiGraph]: The intermodal graph if it exists, else None.
+        Raises:
+            RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
+        """
+        if self._intermodal_graph is None:
+            raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
+        return self._intermodal_graph
+
+    def set_graph(self, graph: nx.DiGraph) -> None:
+        """
+        Set the intermodal graph for the object.
+
+        Args:
+            graph (nx.DiGraph): The graph to be set.
+        Returns:
+            None
+        """
+        self._intermodal_graph = graph
+
+    # TODO: update BuildsGrapher logic to construct from the graphs, fail if not all graphs are available
+
+    def get_intermodal_graph_from_osm(self, city_osm_id: int, keep_city_boundary: bool = True) -> nx.MultiDiGraph:
+        """
+        Retrieves the intermodal graph for a given city from OpenStreetMap.
+        Args:
+            city_osm_id (int): The OpenStreetMap ID of the city.
+            keep_city_boundary (bool, optional): Whether to keep the city boundary in the graph. Defaults to True.
+        Returns:
+            nx.MultiDiGraph: The intermodal graph representing the city.
+        """
+        # if not all(graph_type in self.graphs for graph_type in GraphType):
+        #     raise ValueError("Some graph types are missing")
+        logger.info("Creating intermodal graph from OSM...")
+        self._intermodal_graph = BuildsGrapher(
+            city_osm_id=city_osm_id, city_crs=self.city_crs, keep_city_boundary=keep_city_boundary
+        ).get_intermodal_graph()
+        return self._intermodal_graph
+
+    def get_adjacency_matrix(
+        self,
+        gdf_from: gpd.GeoDataFrame,
+        gdf_to: gpd.GeoDataFrame,
+        weight: str,
+        graph_type: list[GraphType] | None = None,
+    ) -> Optional[pd.DataFrame]:
+        """
+        Calculate the adjacency matrix between the given GeoDataFrames based on
+        the specified weight and intermodal graph.
+
+        Args:
+            gdf_from (gpd.GeoDataFrame): The GeoDataFrame containing the buildings.
+            gdf_to (gpd.GeoDataFrame): The GeoDataFrame containing the services.
+            weight (str): The weight attribute, could be only "time_min" or"length_meter".
+            graph_type (list[GraphType]): The List of Enum types of the graph to search shortest way.
+        Returns:
+            Optional[pd.DataFrame]: The adjacency matrix as a DataFrame, or None if the intermodal graph is not set.
+        Raises:
+            RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
+        """
+        if self._intermodal_graph is None:
+            raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
+        logger.info("Creating adjacency matrix based on provided graph...")
+        to_return = BuildsMatrixer(
+            gdf_from=gdf_from,
+            gdf_to=gdf_to,
+            weight=weight,
+            city_crs=self.city_crs,
+            nx_intermodal_graph=self._intermodal_graph,
+            graph_type=graph_type,
+        ).get_adjacency_matrix()
+        logger.info("Adjacency matrix done!")
+        return to_return
+
+    def get_accessibility_isochrones(
+        self, graph_type: list[GraphType], x_from: float, y_from: float, weight_value: int, weight_type: str
+    ) -> Tuple[gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]]:
+        """
+        Get accessibility isochrones and return three GeoDataFrame objects with isochrones, and
+        if graph_type contains GraphType.PUBLIC_TRANSPORT enum - routes and public transport stops.
+
+        Args:
+            graph_type (list[GraphType]): The List of Enum types of the graph to build isochrones.
+            x_from (float): The x-coordinate of the starting point in the corresponding coordinate system.
+            y_from (float): The y-coordinate of the starting point in the corresponding coordinate system.
+            weight_value (int): The value of the weight.
+            weight_type (str): The type of the weight, could be only "time_min" or "length_meter" .
+
+        Returns:
+            (gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]): Isochrones,routes,stops.
+        Raises:
+            RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
+        """
+        # Check if intermodal graph is set
+        if self._intermodal_graph is None:
+            raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
+        # Build accessibility isochrones
+        logger.info("Creating accessibility isochrones based on provided graph and point...")
+        to_return = BuildsAvailabilitier(
+            graph_type=graph_type,
+            city_crs=self.city_crs,
+            x_from=x_from,
+            y_from=y_from,
+            weight_value=weight_value,
+            weight_type=weight_type,
+            nx_intermodal_graph=self._intermodal_graph,
+        ).get_accessibility_isochrone()
+        logger.info("Accessibility isochrones done!\n")
+        return to_return
```

### Comparing `dongraphio-0.3.3/src/dongraphio/enums.py` & `dongraphio-0.3.4/src/dongraphio/enums.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/utils/__init__.py` & `dongraphio-0.3.4/src/dongraphio/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,7 @@
     project_point_on_edge,
     project_points_on_graph,
     subgraph_by_path,
     update_edges,
 )
 from .matrix_utils import get_dist_matrix, get_dist_matrix_for_tsp, get_nx2nk_idmap, get_subgraph
 from .osm_worker import get_boundary, get_routes, overpass_request
-from .tsp_solver import resolve_tsp
```

### Comparing `dongraphio-0.3.3/src/dongraphio/utils/geometry_utils.py` & `dongraphio-0.3.4/src/dongraphio/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/utils/graph_utils.py` & `dongraphio-0.3.4/src/dongraphio/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/utils/matrix_utils.py` & `dongraphio-0.3.4/src/dongraphio/utils/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/utils/osm_worker.py` & `dongraphio-0.3.4/src/dongraphio/utils/osm_worker.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/src/dongraphio/utils/tsp_solver.py` & `dongraphio-0.3.4/src/dongraphio/utils/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.3/PKG-INFO` & `dongraphio-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dongraphio
-Version: 0.3.3
+Version: 0.3.4
 Summary: Small utility library containing graph algorighms used in other projects
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

