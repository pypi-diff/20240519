# Comparing `tmp/pycitysim-1.12.2.tar.gz` & `tmp/pycitysim-1.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycitysim-1.12.2.tar", last modified: Mon Apr  8 03:53:56 2024, max compression
+gzip compressed data, was "pycitysim-1.13.0.tar", last modified: Sun May 19 17:29:20 2024, max compression
```

## Comparing `pycitysim-1.12.2.tar` & `pycitysim-1.13.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 03:53:49.000000 pycitysim-1.12.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-08 03:53:56.763809 pycitysim-1.12.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-08 03:53:49.000000 pycitysim-1.12.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.755808 pycitysim-1.12.2/pycitysim/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/apphub/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/apphub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/apphub/apphub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/map/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/map/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/routing/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.759809 pycitysim-1.12.2/pycitysim/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sidecar/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/aoi_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/clock_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/economy_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/lane_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/light_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/person_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/road_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/sim/social_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim/urbankg/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/urbankg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/urbankg/kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pycitysim/utils/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 03:53:56.763809 pycitysim-1.12.2/pycitysim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 03:53:56.000000 pycitysim-1.12.2/pycitysim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-08 03:53:49.000000 pycitysim-1.12.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 03:53:56.763809 pycitysim-1.12.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.603683 pycitysim-1.13.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 17:29:14.000000 pycitysim-1.13.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-19 17:29:20.603683 pycitysim-1.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-19 17:29:14.000000 pycitysim-1.13.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.595683 pycitysim-1.13.0/pycitysim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.595683 pycitysim-1.13.0/pycitysim/apphub/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/apphub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/apphub/apphub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.595683 pycitysim-1.13.0/pycitysim/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37630 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/map/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/routing/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sidecar/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/aoi_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/clock_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/economy_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/lane_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/light_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/person_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/road_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/sim/social_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/urbankg/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/urbankg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/urbankg/kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.599683 pycitysim-1.13.0/pycitysim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pycitysim/utils/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:29:20.603683 pycitysim-1.13.0/pycitysim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 17:29:20.000000 pycitysim-1.13.0/pycitysim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-19 17:29:14.000000 pycitysim-1.13.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:29:20.603683 pycitysim-1.13.0/setup.cfg
```

### Comparing `pycitysim-1.12.2/LICENSE` & `pycitysim-1.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/PKG-INFO` & `pycitysim-1.13.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.12.2
+Version: 1.13.0
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: grpcio<2.0.0,>=1.42.0
 Requires-Dist: lru-dict>=1.3.0
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: Pillow>=10.0.0
-Requires-Dist: pycityproto==1.12.0
+Requires-Dist: pycityproto==1.13.1
 Requires-Dist: pymongo>=3.12.1
 Requires-Dist: pyproj>=3.0.0
 Requires-Dist: shapely>=2.0.0
 
 # pycitysim
 
 City Simulator and OpenCity databases Python SDK
```

### Comparing `pycitysim-1.12.2/README.md` & `pycitysim-1.13.0/README.md`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/__init__.py` & `pycitysim-1.13.0/pycitysim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/apphub/apphub.py` & `pycitysim-1.13.0/pycitysim/apphub/apphub.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,24 +168,23 @@
         - agent_id: 绑定后的agent ID。the bound agent ID.
 
         Raises:
         - Exception: 绑定失败。Binding failed.
         """
         return self._bind(org_id, "org", name, avatar)
     
-    def bind_func(self, func_id:int, name:str, avatar:Image):
+    def bind_func(self, name:str, avatar:Image):
         """
         插入非模拟器相关的智能体——func类型智能体
 
         Args:
-        - func_id (str): 该智能体的编号——唯一
         - name (str): 该智能体的名字
         - avatar (Image): 该智能体的头像
         """
-        return self._bind(func_id+10000000, "func", name, avatar)
+        return self._bind(-1, "func", name, avatar)
 
     def release_agent(self, agent_id: int) -> bool:
         """
         释放agent(person/org), 释放后agent将不再被访问并允许其他app绑定
         Release the agent (person/org). After the release, the agent will no longer be accessed and allows other apps to bind.
 
         Args:
```

### Comparing `pycitysim-1.12.2/pycitysim/map/map.py` & `pycitysim-1.13.0/pycitysim/map/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         - positions (list[XYPosition]): 多边形空间范围。Shape of polygon.
         - area (float): 面积(单位: m2)。Area.
         - external["population"] (int): worldpop人口。population from WorldPop.
         - driving_positions (list[LanePosition]): 和道路网中行车道的连接点。Connection points to driving lanes.
         - walking_positions (list[LanePosition]): 和道路网中人行道的连接点。Connection points to pedestrian lanes.
         - driving_gates (list[XYPosition]): 和道路网中行车道的连接点对应的AOI边界上的位置。Position on the AOI boundary corresponding to the connection point to driving lanes.
         - walking_gates (list[XYPosition]): 和道路网中人行道的连接点对应的AOI边界上的位置。Position on the AOI boundary corresponding to the connection point to pedestrian lanes.
-        - land_use (Optional[int]): 用地类型(5:商服用地|6:工矿仓储用地|7:住宅用地|8:公共管理与公共服务用地|10:交通运输用地|12:其他)。Landuse type (5: Commercial land | 6: Industrial, mining and warehousing land | 7: Residential land | 8: Public management and public service land | 10: Transportation land | 12: Others).
+        - urban_land_use (Optional[str]): 城市建设用地分类，参照执行标准GB 50137-2011（https://www.planning.org.cn/law/uploads/2013/1383993139.pdf） Urban Land use type, refer to the national standard GB 50137-2011.
         - poi_ids (list[int]): 包含的POI列表。Contained POI IDs.
         - shapely_xy (shapely.geometry.Polygon): AOI的形状（xy坐标系）。Shape of polygon (in xy coordinates).
         - shapely_lnglat (shapely.geometry.Polygon): AOI的形状（经纬度坐标系）。Shape of polygon (in latitude and longitude).
         """
 
         self.pois: Dict[int, dict] = map_data["pois"]
         """
@@ -133,14 +133,16 @@
 
         self.projector: pyproj.Proj = map_data["projector"]
         """
         采用PROJ.4投影字符串创建的转换器，用以支持xy坐标到WGS84坐标系的转换
         Converter created using PROJ.4 projection string to support conversion of xy coordinates to WGS84 coordinate system
         """
         (
+            self._aoi_tree,
+            self._aoi_list,
             self._poi_tree,
             self._poi_list,
             self._driving_lane_tree,
             self._driving_lane_list,
             self._walking_lane_tree,
             self._walking_lane_list,
         ) = self._build_geo_index()
@@ -254,14 +256,16 @@
         #     "category": "131300",
         #     "position": {
         #       "x": 448802.148620172,
         #       "y": 4412128.118718166
         #     },
         #     "aoi_id": 500018954,
         # }
+        aoi_list = list(self.aois.values())
+        aoi_tree = shapely.STRtree([aoi["shapely_xy"] for aoi in aoi_list])
         poi_list = list(self.pois.values())
         poi_tree = shapely.STRtree([poi["shapely_xy"] for poi in poi_list])
         driving_lane_list = [
             lane for lane in self.lanes.values() if lane["type"] == 1  # driving
         ]
         driving_lane_tree = shapely.STRtree(
             [lane["shapely_xy"] for lane in driving_lane_list]
@@ -269,14 +273,16 @@
         walking_lane_list = [
             lane for lane in self.lanes.values() if lane["type"] == 2  # walking
         ]
         walking_lane_tree = shapely.STRtree(
             [lane["shapely_xy"] for lane in walking_lane_list]
         )
         return (
+            aoi_tree,
+            aoi_list,
             poi_tree,
             poi_list,
             driving_lane_tree,
             driving_lane_list,
             walking_lane_tree,
             walking_lane_list,
         )
@@ -736,15 +742,15 @@
 
         Args:
         - center (x, y): 中心点（xy坐标系）。Center point (xy coordinate system).
         - radius (float): 半径（单位：m）。Radius (unit: m).
         - category_prefix (str): 类别前缀，如实际类别为100000，那么匹配的前缀可以为10、1000等。Category prefix, if the actual category is 100000, then the matching prefix can be 10, 1000, etc.
         - limit (int, optional): 最多返回的poi数量，按距离排序，近的优先（默认None）. The maximum number of POIs returned, sorted by distance, closest ones first (default to None).
 
-        Returns
+        Returns:
         - List[Tuple[Any, float]]: poi列表，每个元素为（poi, 距离）。poi list, each element is (poi, distance).
         """
         if not isinstance(center, Point):
             center = Point(center)
         # 获取半径内的poi
         indices = self._poi_tree.query(center.buffer(radius))
         # 过滤掉不满足类别前缀的poi
@@ -756,14 +762,55 @@
                 pois.append((poi, distance))
         # 按照距离排序
         pois = sorted(pois, key=lambda x: x[1])
         if limit is not None:
             pois = pois[:limit]
         return pois
 
+    def query_aois(
+        self,
+        center: Union[Tuple[float, float], Point],
+        radius: float,
+        urban_land_uses: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+    ) -> List[Tuple[Any, float]]:
+        """
+        查询center点指定半径内城市用地满足条件的aoi（按距离排序）。Query the AOIs whose urban land use within the specified radius of the center point meets the conditions (sorted by distance).
+
+        Args:
+        - center (x, y): 中心点（xy坐标系）。Center point (xy coordinate system).
+        - radius (float): 半径（单位：m）。Radius (unit: m).
+        - urban_land_uses (List[str], optional): 城市用地分类列表，参照执行标准GB 50137-2011（https://www.planning.org.cn/law/uploads/2013/1383993139.pdf）. Urban land use classification list, refer to the national standard GB 50137-2011.
+        - limit (int, optional): 最多返回的aoi数量，按距离排序，近的优先（默认None）. The maximum number of AOIs returned, sorted by distance, closest ones first (default to None).
+
+        Returns:
+        - List[Tuple[Any, float]]: aoi列表，每个元素为（aoi, 距离）。aoi list, each element is (aoi, distance).
+        """
+
+        if not isinstance(center, Point):
+            center = Point(center)
+        # 获取半径内的aoi
+        indices = self._aoi_tree.query(center.buffer(radius))
+        # 过滤掉不满足城市用地条件的aoi
+        aois = []
+        for index in indices:
+            aoi = self._aoi_list[index]
+            if (
+                urban_land_uses is not None
+                and aoi["urban_land_use"] not in urban_land_uses
+            ):
+                continue
+            distance = center.distance(aoi["shapely_xy"])
+            aois.append((aoi, distance))
+        # 按照距离排序
+        aois = sorted(aois, key=lambda x: x[1])
+        if limit is not None:
+            aois = aois[:limit]
+        return aois
+
     def query_lane(
         self,
         xy: Union[Tuple[float, float], Point],
         radius: float,
         lane_type: int = 1,
     ):
         """
```

### Comparing `pycitysim-1.12.2/pycitysim/routing/client.py` & `pycitysim-1.13.0/pycitysim/routing/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sidecar/sidecar.py` & `pycitysim-1.13.0/pycitysim/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/__init__.py` & `pycitysim-1.13.0/pycitysim/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/aoi_service.py` & `pycitysim-1.13.0/pycitysim/sim/aoi_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/client.py` & `pycitysim-1.13.0/pycitysim/sim/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/clock_service.py` & `pycitysim-1.13.0/pycitysim/sim/clock_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/economy_services.py` & `pycitysim-1.13.0/pycitysim/sim/economy_services.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/event_service.py` & `pycitysim-1.13.0/pycitysim/sim/event_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/lane_service.py` & `pycitysim-1.13.0/pycitysim/sim/lane_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/light_service.py` & `pycitysim-1.13.0/pycitysim/sim/light_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/person_service.py` & `pycitysim-1.13.0/pycitysim/sim/person_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/road_service.py` & `pycitysim-1.13.0/pycitysim/sim/road_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/sim/social_service.py` & `pycitysim-1.13.0/pycitysim/sim/social_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/urbankg/kg.py` & `pycitysim-1.13.0/pycitysim/urbankg/kg.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/utils/geojson.py` & `pycitysim-1.13.0/pycitysim/utils/geojson.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/utils/grpc.py` & `pycitysim-1.13.0/pycitysim/utils/grpc.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim/utils/protobuf.py` & `pycitysim-1.13.0/pycitysim/utils/protobuf.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pycitysim.egg-info/PKG-INFO` & `pycitysim-1.13.0/pycitysim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.12.2
+Version: 1.13.0
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,15 +37,15 @@
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: geojson>=3.1.0
 Requires-Dist: grpcio<2.0.0,>=1.42.0
 Requires-Dist: lru-dict>=1.3.0
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: Pillow>=10.0.0
-Requires-Dist: pycityproto==1.12.0
+Requires-Dist: pycityproto==1.13.1
 Requires-Dist: pymongo>=3.12.1
 Requires-Dist: pyproj>=3.0.0
 Requires-Dist: shapely>=2.0.0
 
 # pycitysim
 
 City Simulator and OpenCity databases Python SDK
```

### Comparing `pycitysim-1.12.2/pycitysim.egg-info/SOURCES.txt` & `pycitysim-1.13.0/pycitysim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.2/pyproject.toml` & `pycitysim-1.13.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dependencies = [
     'importlib-metadata; python_version<"3.8"',
     "geojson >= 3.1.0",
     "grpcio >= 1.42.0, < 2.0.0",
     "lru-dict >= 1.3.0",
     "numpy >= 1.24.0",
     "Pillow >= 10.0.0",
-    "pycityproto == 1.12.0",
+    "pycityproto == 1.13.1",
     "pymongo >= 3.12.1",
     "pyproj >= 3.0.0",
     "shapely >= 2.0.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

