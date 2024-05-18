# Comparing `tmp/pyluba-0.0.5.tar.gz` & `tmp/pyluba-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluba-0.0.5.tar", max compression
+gzip compressed data, was "pyluba-0.0.6.tar", max compression
```

## Comparing `pyluba-0.0.5.tar` & `pyluba-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,74 @@
--rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.5/LICENSE
--rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.5/README.md
--rw-r--r--   0        0        0      903 2024-05-14 22:41:07.300874 pyluba-0.0.5/pyluba/__init__.py
--rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.5/pyluba/aliyun/cloud_gateway.py
--rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.5/pyluba/aliyun/cloud_service.py
--rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.5/pyluba/aliyun/test_alicloud_api_gateway.py
--rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/aliyun/tmp_constant.py
--rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.5/pyluba/bluetooth/__init__.py
--rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.5/pyluba/bluetooth/ble.py
--rw-r--r--   0        0        0    40462 2024-05-14 22:33:38.213581 pyluba-0.0.5/pyluba/bluetooth/ble_message.py
--rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/bluetooth/const.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/bluetooth/data/__init__.py
--rw-r--r--   0        0        0     4455 2024-05-14 09:19:33.644102 pyluba-0.0.5/pyluba/bluetooth/data/convert.py
--rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/bluetooth/data/framectrldata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/bluetooth/data/model/__init__.py
--rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/bluetooth/data/notifydata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/__init__.py
--rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/__init__.py
--rw-r--r--   0        0        0     1359 2024-05-14 22:34:13.652444 pyluba-0.0.5/pyluba/data/model/excute_boarder_params.py
--rw-r--r--   0        0        0     1099 2024-05-14 22:35:28.648628 pyluba-0.0.5/pyluba/data/model/execute_boarder.py
--rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/generate_route_information.py
--rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/hash_list.py
--rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/mowing_modes.py
--rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/plan.py
--rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/rapid_state.py
--rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/model/region_data.py
--rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.5/pyluba/data/mqtt/__init__.py
--rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/data/mqtt/event.py
--rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/data/mqtt/properties.py
--rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/data/mqtt/status.py
--rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/event/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.5/pyluba/event/event.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/http/_init_.py
--rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.5/pyluba/http/http.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/luba/_init_.py
--rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/luba/base.py
--rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.5/pyluba/mammotion/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.5/pyluba/mammotion/commands/proto.py
--rw-r--r--   0        0        0       48 2024-05-14 22:27:59.597338 pyluba-0.0.5/pyluba/mammotion/devices/__init__.py
--rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.5/pyluba/mammotion/devices/luba.py
--rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.5/pyluba/mqtt/mqtt.py
--rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.5/pyluba/proto/common.proto
--rw-r--r--   0        0        0      428 2024-05-08 21:10:33.874300 pyluba-0.0.5/pyluba/proto/common_p2p.py
--rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.5/pyluba/proto/common_pb2.py
--rw-r--r--   0        0        0     3330 2024-05-13 07:27:07.774053 pyluba-0.0.5/pyluba/proto/dev_net.proto
--rw-r--r--   0        0        0     5090 2024-05-13 20:01:44.718647 pyluba-0.0.5/pyluba/proto/dev_net_p2p.py
--rw-r--r--   0        0        0     6968 2024-05-13 07:28:18.216030 pyluba-0.0.5/pyluba/proto/dev_net_pb2.py
--rw-r--r--   0        0        0     1271 2024-05-12 22:00:22.601976 pyluba-0.0.5/pyluba/proto/luba_msg.proto
--rw-r--r--   0        0        0     1984 2024-05-08 21:10:25.440293 pyluba-0.0.5/pyluba/proto/luba_msg_p2p.py
--rw-r--r--   0        0        0     3575 2024-05-12 22:27:40.502487 pyluba-0.0.5/pyluba/proto/luba_msg_pb2.py
--rw-r--r--   0        0        0      589 2024-05-08 21:08:24.231673 pyluba-0.0.5/pyluba/proto/mctrl_driver.proto
--rw-r--r--   0        0        0     1347 2024-05-08 21:10:04.558292 pyluba-0.0.5/pyluba/proto/mctrl_driver_p2p.py
--rw-r--r--   0        0        0     2024 2024-05-06 21:49:09.712665 pyluba-0.0.5/pyluba/proto/mctrl_driver_pb2.py
--rw-r--r--   0        0        0     9943 2024-05-12 21:44:30.955843 pyluba-0.0.5/pyluba/proto/mctrl_nav.proto
--rw-r--r--   0        0        0    15703 2024-05-13 20:02:00.650601 pyluba-0.0.5/pyluba/proto/mctrl_nav_p2p.py
--rw-r--r--   0        0        0    19003 2024-05-12 22:27:53.181170 pyluba-0.0.5/pyluba/proto/mctrl_nav_pb2.py
--rw-r--r--   0        0        0      682 2024-05-13 20:58:20.824741 pyluba-0.0.5/pyluba/proto/mctrl_ota.proto
--rw-r--r--   0        0        0     2370 2024-05-13 20:59:13.504552 pyluba-0.0.5/pyluba/proto/mctrl_ota_pb2.py
--rw-r--r--   0        0        0     8857 2024-05-13 21:29:49.796694 pyluba-0.0.5/pyluba/proto/mctrl_sys.proto
--rw-r--r--   0        0        0    13657 2024-05-08 21:10:56.506338 pyluba-0.0.5/pyluba/proto/mctrl_sys_p2p.py
--rw-r--r--   0        0        0    18942 2024-05-13 21:30:02.817702 pyluba-0.0.5/pyluba/proto/mctrl_sys_pb2.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.5/pyluba/py.typed
--rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.5/pyluba/utility/constant/device_constant.py
--rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.5/pyluba/utility/periodic.py
--rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.5/pyluba/utility/rocker_util.py
--rw-r--r--   0        0        0     1496 2024-05-14 22:40:23.305615 pyluba-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 pyluba-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.6/LICENSE
+-rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.6/README.md
+-rw-r--r--   0        0        0      903 2024-05-15 09:07:45.520662 pyluba-0.0.6/pyluba/__init__.py
+-rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.6/pyluba/aliyun/cloud_gateway.py
+-rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.6/pyluba/aliyun/cloud_service.py
+-rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.6/pyluba/aliyun/test_alicloud_api_gateway.py
+-rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/aliyun/tmp_constant.py
+-rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.6/pyluba/bluetooth/__init__.py
+-rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.6/pyluba/bluetooth/ble.py
+-rw-r--r--   0        0        0    40473 2024-05-15 09:07:42.251526 pyluba-0.0.6/pyluba/bluetooth/ble_message.py
+-rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/bluetooth/const.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/bluetooth/data/__init__.py
+-rw-r--r--   0        0        0     4405 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/bluetooth/data/convert.py
+-rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/bluetooth/data/framectrldata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/bluetooth/data/model/__init__.py
+-rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/bluetooth/data/notifydata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/__init__.py
+-rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/__init__.py
+-rw-r--r--   0        0        0     1359 2024-05-14 22:34:13.652444 pyluba-0.0.6/pyluba/data/model/excute_boarder_params.py
+-rw-r--r--   0        0        0     1099 2024-05-14 22:35:28.648628 pyluba-0.0.6/pyluba/data/model/execute_boarder.py
+-rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/generate_route_information.py
+-rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/hash_list.py
+-rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/mowing_modes.py
+-rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/plan.py
+-rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/rapid_state.py
+-rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/model/region_data.py
+-rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.6/pyluba/data/mqtt/__init__.py
+-rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/data/mqtt/event.py
+-rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/data/mqtt/properties.py
+-rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/data/mqtt/status.py
+-rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/event/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.6/pyluba/event/event.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/http/_init_.py
+-rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.6/pyluba/http/http.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/luba/_init_.py
+-rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/luba/base.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.6/pyluba/mammotion/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.6/pyluba/mammotion/commands/proto.py
+-rw-r--r--   0        0        0       48 2024-05-14 22:27:59.597338 pyluba-0.0.6/pyluba/mammotion/devices/__init__.py
+-rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.6/pyluba/mammotion/devices/luba.py
+-rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.6/pyluba/mqtt/mqtt.py
+-rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.6/pyluba/proto/common.proto
+-rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.6/pyluba/proto/common_pb2.py
+-rw-r--r--   0        0        0      460 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/common_pb2.pyi
+-rw-r--r--   0        0        0     5502 2024-05-15 09:07:42.251526 pyluba-0.0.6/pyluba/proto/dev_net.proto
+-rw-r--r--   0        0        0    12853 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/dev_net_pb2.py
+-rw-r--r--   0        0        0    21825 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/dev_net_pb2.pyi
+-rw-r--r--   0        0        0     1553 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/luba_msg.proto
+-rw-r--r--   0        0        0     4215 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/luba_msg_pb2.py
+-rw-r--r--   0        0        0     4031 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/luba_msg_pb2.pyi
+-rw-r--r--   0        0        0     1114 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/luba_mul.proto
+-rw-r--r--   0        0        0     3387 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/luba_mul_pb2.py
+-rw-r--r--   0        0        0     3913 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/luba_mul_pb2.pyi
+-rw-r--r--   0        0        0     1383 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/mctrl_driver.proto
+-rw-r--r--   0        0        0     3770 2024-05-15 09:07:42.252526 pyluba-0.0.6/pyluba/proto/mctrl_driver_pb2.py
+-rw-r--r--   0        0        0     5852 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/mctrl_driver_pb2.pyi
+-rw-r--r--   0        0        0    10530 2024-05-15 09:07:42.253526 pyluba-0.0.6/pyluba/proto/mctrl_nav.proto
+-rw-r--r--   0        0        0    21725 2024-05-15 09:07:42.253526 pyluba-0.0.6/pyluba/proto/mctrl_nav_pb2.py
+-rw-r--r--   0        0        0    45951 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/mctrl_nav_pb2.pyi
+-rw-r--r--   0        0        0      629 2024-05-15 09:07:42.253526 pyluba-0.0.6/pyluba/proto/mctrl_ota.proto
+-rw-r--r--   0        0        0     2259 2024-05-15 09:07:42.254526 pyluba-0.0.6/pyluba/proto/mctrl_ota_pb2.py
+-rw-r--r--   0        0        0     2821 2024-05-18 08:45:36.775444 pyluba-0.0.6/pyluba/proto/mctrl_ota_pb2.pyi
+-rw-r--r--   0        0        0      664 2024-05-15 09:07:42.254526 pyluba-0.0.6/pyluba/proto/mctrl_pept.proto
+-rw-r--r--   0        0        0     2121 2024-05-15 09:07:42.254526 pyluba-0.0.6/pyluba/proto/mctrl_pept_pb2.py
+-rw-r--r--   0        0        0     2840 2024-05-18 08:45:36.776446 pyluba-0.0.6/pyluba/proto/mctrl_pept_pb2.pyi
+-rw-r--r--   0        0        0    10186 2024-05-15 09:07:42.254526 pyluba-0.0.6/pyluba/proto/mctrl_sys.proto
+-rw-r--r--   0        0        0    21469 2024-05-15 09:07:42.254526 pyluba-0.0.6/pyluba/proto/mctrl_sys_pb2.py
+-rw-r--r--   0        0        0    38893 2024-05-18 08:45:36.776446 pyluba-0.0.6/pyluba/proto/mctrl_sys_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.6/pyluba/py.typed
+-rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.6/pyluba/utility/constant/device_constant.py
+-rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.6/pyluba/utility/periodic.py
+-rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.6/pyluba/utility/rocker_util.py
+-rw-r--r--   0        0        0     1497 2024-05-18 08:46:00.155390 pyluba-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 pyluba-0.0.6/PKG-INFO
```

### Comparing `pyluba-0.0.5/LICENSE` & `pyluba-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/README.md` & `pyluba-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/__init__.py` & `pyluba-0.0.6/pyluba/__init__.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/aliyun/cloud_gateway.py` & `pyluba-0.0.6/pyluba/aliyun/cloud_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/aliyun/cloud_service.py` & `pyluba-0.0.6/pyluba/aliyun/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/aliyun/test_alicloud_api_gateway.py` & `pyluba-0.0.6/pyluba/aliyun/test_alicloud_api_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/aliyun/tmp_constant.py` & `pyluba-0.0.6/pyluba/aliyun/tmp_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/bluetooth/ble.py` & `pyluba-0.0.6/pyluba/bluetooth/ble.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/bluetooth/ble_message.py` & `pyluba-0.0.6/pyluba/bluetooth/ble_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
         lubaMsg.subtype = 1
         lubaMsg.sys.CopyFrom(mctrl_sys)
         byte_arr = lubaMsg.SerializeToString()
         await self.postCustomDataBytes(byte_arr)
 
 
     async def send_order_msg_ota(self, type: int):
-        mctrl_ota = mctrl_ota_pb2.MctrlOta(
-            to_dev_get_info_req=mctrl_ota_pb2.ToDevGetInfoReq(
+        mctrl_ota = mctrl_ota_pb2.MctlOta(
+            todev_get_info_req=mctrl_ota_pb2.getInfoReq(
                 type=type
             )
         )
 
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_OTA
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
@@ -91,45 +91,45 @@
         await self.postCustomDataBytes(byte_arr)
 
 
     async def get_report_cfg(self, timeout: int, period: int, no_change_period: int):
 
 
         mctlsys = mctrl_sys_pb2.MctlSys(
-            todev_report_cfg=mctrl_sys_pb2.ReportInfoCfg(
+            todev_report_cfg=mctrl_sys_pb2.report_info_cfg(
                 timeout=timeout,
                 period=period,
                 no_change_period=no_change_period,
                 count=1
             )
         )
 
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_CONNECT
+            mctrl_sys_pb2.rpt_info_type.RIT_CONNECT
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_RTK
+            mctrl_sys_pb2.rpt_info_type.RIT_RTK
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_DEV_LOCAL
+            mctrl_sys_pb2.rpt_info_type.RIT_DEV_LOCAL
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_WORK
+            mctrl_sys_pb2.rpt_info_type.RIT_WORK
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_DEV_STA
+            mctrl_sys_pb2.rpt_info_type.RIT_DEV_STA
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_VISION_POINT
+            mctrl_sys_pb2.rpt_info_type.RIT_VISION_POINT
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_VIO
+            mctrl_sys_pb2.rpt_info_type.RIT_VIO
         )
         mctlsys.todev_report_cfg.sub.append(
-            mctrl_sys_pb2.RptInfoType.RIT_VISION_STATISTIC
+            mctrl_sys_pb2.rpt_info_type.RIT_VISION_STATISTIC
         )
 
         lubaMsg = luba_msg_pb2.LubaMsg()
         lubaMsg.msgtype = luba_msg_pb2.MSG_CMD_TYPE_EMBED_SYS
         lubaMsg.sender = luba_msg_pb2.DEV_MOBILEAPP
         lubaMsg.rcver = luba_msg_pb2.DEV_MAINCTL
         lubaMsg.msgattr = luba_msg_pb2.MSG_ATTR_REQ
```

### Comparing `pyluba-0.0.5/pyluba/bluetooth/const.py` & `pyluba-0.0.6/pyluba/bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/bluetooth/data/convert.py` & `pyluba-0.0.6/pyluba/bluetooth/data/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 from typing import Dict
 
 from google.protobuf.message import DecodeError
 
 from pyluba.proto import mctrl_driver_pb2, luba_msg_pb2, dev_net_pb2, mctrl_nav_pb2, mctrl_sys_pb2
-from pyluba.proto import luba_msg_p2p
 from pyluba.data.model import HashList, RegionData
 
 # until we have a proper store or send messages somewhere
 device_charge_map: Dict[str, int] = {}
 deviceRtkStatusMap: Dict[str, int] = {}
 deviceSelfCheckFlagMap: Dict[str, bool] = {}
 devicePileMap: Dict[str, int] = {}
@@ -55,26 +54,26 @@
         return luba_msg
         
     except DecodeError as err:
         print(err)
         
         
 def store_sys_data(sys):
-    if(sys.HasField("system_tard_state_tunnel")):
-        tard_state_data_list = sys.system_tard_state_tunnel.tard_state_data
+    if(sys.HasField("systemTardStateTunnel")):
+        tard_state_data_list = sys.systemTardStateTunnel.tard_state_data
         longValue8 = tard_state_data_list[0]
         longValue9 = tard_state_data_list[1]
         print("Device status report,deviceState:", longValue8, ",deviceName:", "Luba...")
         chargeStateTemp = longValue9
         longValue10 = tard_state_data_list[6]
         longValue11 = tard_state_data_list[7]
 
         #device_state_map        
-    if sys.HasField("system_rapid_state_tunnel"):
-        rapid_state_data_list = sys.system_rapid_state_tunnel.rapid_state_data
+    if sys.HasField("systemRapidStateTunnel"):
+        rapid_state_data_list = sys.systemRapidStateTunnel.rapid_state_data
         print(rapid_state_data_list)
 
     if sys.HasField("toapp_batinfo"):
         battery_info = sys.toapp_batinfo
         print(battery_info)
```

### Comparing `pyluba-0.0.5/pyluba/bluetooth/data/framectrldata.py` & `pyluba-0.0.6/pyluba/bluetooth/data/framectrldata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/bluetooth/data/notifydata.py` & `pyluba-0.0.6/pyluba/bluetooth/data/notifydata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/model/excute_boarder_params.py` & `pyluba-0.0.6/pyluba/data/model/excute_boarder_params.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/model/execute_boarder.py` & `pyluba-0.0.6/pyluba/data/model/execute_boarder.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/model/generate_route_information.py` & `pyluba-0.0.6/pyluba/data/model/generate_route_information.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/model/plan.py` & `pyluba-0.0.6/pyluba/data/model/plan.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/model/rapid_state.py` & `pyluba-0.0.6/pyluba/data/model/rapid_state.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/model/region_data.py` & `pyluba-0.0.6/pyluba/data/model/region_data.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/mqtt/event.py` & `pyluba-0.0.6/pyluba/data/mqtt/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/mqtt/properties.py` & `pyluba-0.0.6/pyluba/data/mqtt/properties.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/data/mqtt/status.py` & `pyluba-0.0.6/pyluba/data/mqtt/status.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/event/event.py` & `pyluba-0.0.6/pyluba/event/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/http/http.py` & `pyluba-0.0.6/pyluba/http/http.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/luba/base.py` & `pyluba-0.0.6/pyluba/luba/base.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/mammotion/devices/luba.py` & `pyluba-0.0.6/pyluba/mammotion/devices/luba.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/mqtt/mqtt.py` & `pyluba-0.0.6/pyluba/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/proto/common_pb2.py` & `pyluba-0.0.6/pyluba/proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/proto/luba_msg.proto` & `pyluba-0.0.6/pyluba/proto/luba_msg.proto`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 syntax = "proto3";
 
-
 import "pyluba/proto/mctrl_driver.proto";
 import "pyluba/proto/mctrl_nav.proto";
 import "pyluba/proto/mctrl_sys.proto";
 import "pyluba/proto/dev_net.proto";
 import "pyluba/proto/mctrl_ota.proto";
-
+import "pyluba/proto/luba_mul.proto";
+import "pyluba/proto/mctrl_pept.proto";
 
 message MsgNull {
-} 
+}
 
 message LubaMsg {
-
   MsgCmdType msgtype = 1;
   MsgDevice sender = 2;
   MsgDevice rcver = 3;
   MsgAttr msgattr = 4;
   int32 seqs = 5;
   int32 version = 6;
   int32 subtype = 7;
-  int64 timestamp = 15;
-  
-  
   oneof LubaSubMsg {
     DevNet net = 8;
     MctlSys sys = 10;
     MctlNav nav = 11;
-    MctrlDriver driver = 12;
-    MctrlOta ota = 13;
-    MsgNull null = 14;
+    MctlDriver driver = 12;
+    MctlOta ota = 13;
+    SocMul mul = 14;
+    MsgNull null = 16;
+    MctlPept pept = 17;
   }
-
+  uint64 timestamp = 15;
 }
 
 enum MsgCmdType {
   MSG_CMD_TYPE_START = 0;
   MSG_CMD_TYPE_NAV = 240;
   MSG_CMD_TYPE_LOCALIZATION = 241;
   MSG_CMD_TYPE_PLANNING = 242;
   MSG_CMD_TYPE_EMBED_DRIVER = 243;
   MSG_CMD_TYPE_EMBED_SYS = 244;
   MSG_CMD_TYPE_EMBED_MIDWARE = 245;
   MSG_CMD_TYPE_EMBED_OTA = 246;
   MSG_CMD_TYPE_APPLICATION = 247;
   MSG_CMD_TYPE_ESP = 248;
+  MSG_CMD_TYPE_MUL = 249;
+  MSG_CMD_TYPE_PEPT = 250;
 }
 
 enum MsgAttr {
-
   MSG_ATTR_NONE = 0;
-  MSG_ATTR_REPORT = 3;
   MSG_ATTR_REQ = 1;
   MSG_ATTR_RESP = 2;
-
+  MSG_ATTR_REPORT = 3;
 }
 
 enum MsgDevice {
   DEV_COMM_ESP = 0;
-  DEV_BASESTATION = 4;
-  DEV_BMS = 9;
-  DEV_IOTSERVER = 8;
-  DEV_LEFTMOTOR = 2;
   DEV_MAINCTL = 1;
-  DEV_MOBILEAPP = 7;
+  DEV_LEFTMOTOR = 2;
   DEV_RIGHTMOTOR = 3;
+  DEV_BASESTATION = 4;
   DEV_RTKCLI = 5;
   DEV_USBHOST = 6;
-}
+  DEV_MOBILEAPP = 7;
+  DEV_IOTSERVER = 8;
+  DEV_BMS = 9;
+  DEV_NAVIGATION = 17;
+  DEV_LOCALIZATION = 18;
+  DEV_PERCEPTION = 19;
+  SOC_MODULE_MULTIMEDIA = 21;
+  DEV_IOTCTRL = 25;
+}
```

### Comparing `pyluba-0.0.5/pyluba/proto/luba_msg_pb2.py` & `pyluba-0.0.6/pyluba/proto/luba_msg_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 
 
 from pyluba.proto import mctrl_driver_pb2 as pyluba_dot_proto_dot_mctrl__driver__pb2
 from pyluba.proto import mctrl_nav_pb2 as pyluba_dot_proto_dot_mctrl__nav__pb2
 from pyluba.proto import mctrl_sys_pb2 as pyluba_dot_proto_dot_mctrl__sys__pb2
 from pyluba.proto import dev_net_pb2 as pyluba_dot_proto_dot_dev__net__pb2
 from pyluba.proto import mctrl_ota_pb2 as pyluba_dot_proto_dot_mctrl__ota__pb2
+from pyluba.proto import luba_mul_pb2 as pyluba_dot_proto_dot_luba__mul__pb2
+from pyluba.proto import mctrl_pept_pb2 as pyluba_dot_proto_dot_mctrl__pept__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bpyluba/proto/luba_msg.proto\x1a\x1fpyluba/proto/mctrl_driver.proto\x1a\x1cpyluba/proto/mctrl_nav.proto\x1a\x1cpyluba/proto/mctrl_sys.proto\x1a\x1apyluba/proto/dev_net.proto\x1a\x1cpyluba/proto/mctrl_ota.proto\"\t\n\x07MsgNull\"\xe8\x02\n\x07LubaMsg\x12\x1c\n\x07msgtype\x18\x01 \x01(\x0e\x32\x0b.MsgCmdType\x12\x1a\n\x06sender\x18\x02 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x05rcver\x18\x03 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x07msgattr\x18\x04 \x01(\x0e\x32\x08.MsgAttr\x12\x0c\n\x04seqs\x18\x05 \x01(\x05\x12\x0f\n\x07version\x18\x06 \x01(\x05\x12\x0f\n\x07subtype\x18\x07 \x01(\x05\x12\x11\n\ttimestamp\x18\x0f \x01(\x03\x12\x16\n\x03net\x18\x08 \x01(\x0b\x32\x07.DevNetH\x00\x12\x17\n\x03sys\x18\n \x01(\x0b\x32\x08.MctlSysH\x00\x12\x17\n\x03nav\x18\x0b \x01(\x0b\x32\x08.MctlNavH\x00\x12\x1e\n\x06\x64river\x18\x0c \x01(\x0b\x32\x0c.MctrlDriverH\x00\x12\x18\n\x03ota\x18\r \x01(\x0b\x32\t.MctrlOtaH\x00\x12\x18\n\x04null\x18\x0e \x01(\x0b\x32\x08.MsgNullH\x00\x42\x0c\n\nLubaSubMsg*\xa8\x02\n\nMsgCmdType\x12\x16\n\x12MSG_CMD_TYPE_START\x10\x00\x12\x15\n\x10MSG_CMD_TYPE_NAV\x10\xf0\x01\x12\x1e\n\x19MSG_CMD_TYPE_LOCALIZATION\x10\xf1\x01\x12\x1a\n\x15MSG_CMD_TYPE_PLANNING\x10\xf2\x01\x12\x1e\n\x19MSG_CMD_TYPE_EMBED_DRIVER\x10\xf3\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_SYS\x10\xf4\x01\x12\x1f\n\x1aMSG_CMD_TYPE_EMBED_MIDWARE\x10\xf5\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_OTA\x10\xf6\x01\x12\x1d\n\x18MSG_CMD_TYPE_APPLICATION\x10\xf7\x01\x12\x15\n\x10MSG_CMD_TYPE_ESP\x10\xf8\x01*V\n\x07MsgAttr\x12\x11\n\rMSG_ATTR_NONE\x10\x00\x12\x13\n\x0fMSG_ATTR_REPORT\x10\x03\x12\x10\n\x0cMSG_ATTR_REQ\x10\x01\x12\x11\n\rMSG_ATTR_RESP\x10\x02*\xbe\x01\n\tMsgDevice\x12\x10\n\x0c\x44\x45V_COMM_ESP\x10\x00\x12\x13\n\x0f\x44\x45V_BASESTATION\x10\x04\x12\x0b\n\x07\x44\x45V_BMS\x10\t\x12\x11\n\rDEV_IOTSERVER\x10\x08\x12\x11\n\rDEV_LEFTMOTOR\x10\x02\x12\x0f\n\x0b\x44\x45V_MAINCTL\x10\x01\x12\x11\n\rDEV_MOBILEAPP\x10\x07\x12\x12\n\x0e\x44\x45V_RIGHTMOTOR\x10\x03\x12\x0e\n\nDEV_RTKCLI\x10\x05\x12\x0f\n\x0b\x44\x45V_USBHOST\x10\x06\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1bpyluba/proto/luba_msg.proto\x1a\x1fpyluba/proto/mctrl_driver.proto\x1a\x1cpyluba/proto/mctrl_nav.proto\x1a\x1cpyluba/proto/mctrl_sys.proto\x1a\x1apyluba/proto/dev_net.proto\x1a\x1cpyluba/proto/mctrl_ota.proto\x1a\x1bpyluba/proto/luba_mul.proto\x1a\x1dpyluba/proto/mctrl_pept.proto\"\t\n\x07MsgNull\"\x99\x03\n\x07LubaMsg\x12\x1c\n\x07msgtype\x18\x01 \x01(\x0e\x32\x0b.MsgCmdType\x12\x1a\n\x06sender\x18\x02 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x05rcver\x18\x03 \x01(\x0e\x32\n.MsgDevice\x12\x19\n\x07msgattr\x18\x04 \x01(\x0e\x32\x08.MsgAttr\x12\x0c\n\x04seqs\x18\x05 \x01(\x05\x12\x0f\n\x07version\x18\x06 \x01(\x05\x12\x0f\n\x07subtype\x18\x07 \x01(\x05\x12\x16\n\x03net\x18\x08 \x01(\x0b\x32\x07.DevNetH\x00\x12\x17\n\x03sys\x18\n \x01(\x0b\x32\x08.MctlSysH\x00\x12\x17\n\x03nav\x18\x0b \x01(\x0b\x32\x08.MctlNavH\x00\x12\x1d\n\x06\x64river\x18\x0c \x01(\x0b\x32\x0b.MctlDriverH\x00\x12\x17\n\x03ota\x18\r \x01(\x0b\x32\x08.MctlOtaH\x00\x12\x16\n\x03mul\x18\x0e \x01(\x0b\x32\x07.SocMulH\x00\x12\x18\n\x04null\x18\x10 \x01(\x0b\x32\x08.MsgNullH\x00\x12\x19\n\x04pept\x18\x11 \x01(\x0b\x32\t.MctlPeptH\x00\x12\x11\n\ttimestamp\x18\x0f \x01(\x04\x42\x0c\n\nLubaSubMsg*\xd7\x02\n\nMsgCmdType\x12\x16\n\x12MSG_CMD_TYPE_START\x10\x00\x12\x15\n\x10MSG_CMD_TYPE_NAV\x10\xf0\x01\x12\x1e\n\x19MSG_CMD_TYPE_LOCALIZATION\x10\xf1\x01\x12\x1a\n\x15MSG_CMD_TYPE_PLANNING\x10\xf2\x01\x12\x1e\n\x19MSG_CMD_TYPE_EMBED_DRIVER\x10\xf3\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_SYS\x10\xf4\x01\x12\x1f\n\x1aMSG_CMD_TYPE_EMBED_MIDWARE\x10\xf5\x01\x12\x1b\n\x16MSG_CMD_TYPE_EMBED_OTA\x10\xf6\x01\x12\x1d\n\x18MSG_CMD_TYPE_APPLICATION\x10\xf7\x01\x12\x15\n\x10MSG_CMD_TYPE_ESP\x10\xf8\x01\x12\x15\n\x10MSG_CMD_TYPE_MUL\x10\xf9\x01\x12\x16\n\x11MSG_CMD_TYPE_PEPT\x10\xfa\x01*V\n\x07MsgAttr\x12\x11\n\rMSG_ATTR_NONE\x10\x00\x12\x10\n\x0cMSG_ATTR_REQ\x10\x01\x12\x11\n\rMSG_ATTR_RESP\x10\x02\x12\x13\n\x0fMSG_ATTR_REPORT\x10\x03*\xa8\x02\n\tMsgDevice\x12\x10\n\x0c\x44\x45V_COMM_ESP\x10\x00\x12\x0f\n\x0b\x44\x45V_MAINCTL\x10\x01\x12\x11\n\rDEV_LEFTMOTOR\x10\x02\x12\x12\n\x0e\x44\x45V_RIGHTMOTOR\x10\x03\x12\x13\n\x0f\x44\x45V_BASESTATION\x10\x04\x12\x0e\n\nDEV_RTKCLI\x10\x05\x12\x0f\n\x0b\x44\x45V_USBHOST\x10\x06\x12\x11\n\rDEV_MOBILEAPP\x10\x07\x12\x11\n\rDEV_IOTSERVER\x10\x08\x12\x0b\n\x07\x44\x45V_BMS\x10\t\x12\x12\n\x0e\x44\x45V_NAVIGATION\x10\x11\x12\x14\n\x10\x44\x45V_LOCALIZATION\x10\x12\x12\x12\n\x0e\x44\x45V_PERCEPTION\x10\x13\x12\x19\n\x15SOC_MODULE_MULTIMEDIA\x10\x15\x12\x0f\n\x0b\x44\x45V_IOTCTRL\x10\x19\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.luba_msg_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _MSGCMDTYPE._serialized_start=557
-  _MSGCMDTYPE._serialized_end=853
-  _MSGATTR._serialized_start=855
-  _MSGATTR._serialized_end=941
-  _MSGDEVICE._serialized_start=944
-  _MSGDEVICE._serialized_end=1134
-  _MSGNULL._serialized_start=182
-  _MSGNULL._serialized_end=191
-  _LUBAMSG._serialized_start=194
-  _LUBAMSG._serialized_end=554
+  _MSGCMDTYPE._serialized_start=666
+  _MSGCMDTYPE._serialized_end=1009
+  _MSGATTR._serialized_start=1011
+  _MSGATTR._serialized_end=1097
+  _MSGDEVICE._serialized_start=1100
+  _MSGDEVICE._serialized_end=1396
+  _MSGNULL._serialized_start=242
+  _MSGNULL._serialized_end=251
+  _LUBAMSG._serialized_start=254
+  _LUBAMSG._serialized_end=663
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.5/pyluba/proto/mctrl_driver_pb2.py` & `pyluba-0.0.6/pyluba/proto/mctrl_pept_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: pyluba/proto/mctrl_driver.proto
+# source: pyluba/proto/mctrl_pept.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fpyluba/proto/mctrl_driver.proto\"\x8f\x02\n\x0bMctrlDriver\x12.\n\x14todev_devmotion_ctrl\x18\x01 \x01(\x0b\x32\x0e.DrvMotionCtrlH\x00\x12\x30\n\x15todev_knife_hight_set\x18\x02 \x01(\x0b\x32\x0f.DrvKnifeHeightH\x00\x12,\n\x15\x62idire_speed_read_set\x18\x03 \x01(\x0b\x32\x0b.DrvSrSpeedH\x00\x12\x34\n\x19\x62idire_knife_hight_report\x18\x04 \x01(\x0b\x32\x0f.DrvKnifeHeightH\x00\x12-\n\x12toapp_knife_status\x18\x05 \x01(\x0b\x32\x0f.DrvKnifeStatusH\x00\x42\x0b\n\tSubDrvMsg\"@\n\rDrvMotionCtrl\x12\x17\n\x0fsetAngularSpeed\x18\x02 \x01(\x05\x12\x16\n\x0esetLinearSpeed\x18\x01 \x01(\x05\"%\n\x0e\x44rvKnifeHeight\x12\x13\n\x0bknifeHeight\x18\x01 \x01(\x05\"\'\n\nDrvSrSpeed\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\r\n\x05speed\x18\x02 \x01(\x02\"&\n\x0e\x44rvKnifeStatus\x12\x14\n\x0cknife_status\x18\x01 \x01(\x05\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dpyluba/proto/mctrl_pept.proto\"X\n\x16perception_obstacles_t\x12\r\n\x05label\x18\x01 \x01(\x05\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12\x10\n\x08points_x\x18\x03 \x03(\x05\x12\x10\n\x08points_y\x18\x04 \x03(\x05\"\x98\x01\n$perception_obstacles_visualization_t\x12\x15\n\ris_heart_beat\x18\x01 \x01(\x05\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12*\n\tobstacles\x18\x03 \x03(\x0b\x32\x17.perception_obstacles_t\x12\x11\n\ttimestamp\x18\x04 \x01(\x01\x12\r\n\x05scale\x18\x05 \x01(\x02\"f\n\x1bperception_universal_buff_t\x12\x17\n\x0fperception_type\x18\x01 \x01(\x05\x12\x16\n\x0eperception_len\x18\x02 \x01(\x05\x12\x16\n\x0euniversal_buff\x18\x03 \x03(\x03\"\xb0\x01\n\x08MctlPept\x12S\n\"perception_obstacles_visualization\x18\x01 \x01(\x0b\x32%.perception_obstacles_visualization_tH\x00\x12\x41\n\x19perception_universal_buff\x18\x02 \x01(\x0b\x32\x1c.perception_universal_buff_tH\x00\x42\x0c\n\nSubPeptMsgb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_driver_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_pept_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _MCTRLDRIVER._serialized_start=36
-  _MCTRLDRIVER._serialized_end=307
-  _DRVMOTIONCTRL._serialized_start=309
-  _DRVMOTIONCTRL._serialized_end=373
-  _DRVKNIFEHEIGHT._serialized_start=375
-  _DRVKNIFEHEIGHT._serialized_end=412
-  _DRVSRSPEED._serialized_start=414
-  _DRVSRSPEED._serialized_end=453
-  _DRVKNIFESTATUS._serialized_start=455
-  _DRVKNIFESTATUS._serialized_end=493
+  _PERCEPTION_OBSTACLES_T._serialized_start=33
+  _PERCEPTION_OBSTACLES_T._serialized_end=121
+  _PERCEPTION_OBSTACLES_VISUALIZATION_T._serialized_start=124
+  _PERCEPTION_OBSTACLES_VISUALIZATION_T._serialized_end=276
+  _PERCEPTION_UNIVERSAL_BUFF_T._serialized_start=278
+  _PERCEPTION_UNIVERSAL_BUFF_T._serialized_end=380
+  _MCTLPEPT._serialized_start=383
+  _MCTLPEPT._serialized_end=559
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.5/pyluba/proto/mctrl_nav.proto` & `pyluba-0.0.6/pyluba/proto/mctrl_nav.proto`

 * *Files 12% similar despite different names*

```diff
@@ -1,436 +1,485 @@
 syntax = "proto3";
 
 import "pyluba/proto/common.proto";
 
 message NavLatLonUp {
-    double lat = 1;
-    double lon = 2;
+  double lat = 1;
+  double lon = 2;
 }
 
 message NavBorderState {
-    int32 bdstate = 1;
+  int32 bdstate = 1;
 }
 
 message NavPosUp {
-    float x = 1;
-    float y = 2;
-    int32 status = 3;
-    int32 toward = 4;
-    int32 stars = 5;
-    float age = 6;
-    float latStddev = 7;
-    float lonStddev = 8;
-    int32 l2dfStars = 9;
-    int32 posType = 10;
-    int64 cHashId = 11;
-    int32 posLevel = 12;
-    
+  float x = 1;
+  float y = 2;
+  int32 status = 3;
+  int32 toward = 4;
+  int32 stars = 5;
+  float age = 6;
+  float latStddev = 7;
+  float lonStddev = 8;
+  int32 l2dfStars = 9;
+  int32 posType = 10;
+  int64 cHashId = 11;
+  int32 posLevel = 12;
 }
 
 message NavBorderDataGetAck {
-    int32 jobId = 1;
-    int32 currentFrame = 2;
+  int32 jobId = 1;
+  int32 currentFrame = 2;
 }
 
 message NavObstiBorderDataGet {
-    int32 obstacleIndex = 1;
-    int32 currentFrame = 2;
-    int32 obstaclesLen = 3;
+  int32 obstacleIndex = 1;
+  int32 currentFrame = 2;
+  int32 obstaclesLen = 3;
 }
 
 message NavObstiBorderDataGetAck {
-    int32 obstacleIndex = 1;
-    int32 currentFrame = 2;
+  int32 obstacleIndex = 1;
+  int32 currentFrame = 2;
 }
 
 message NavCHlLineData {
-    int32 channelLineLen = 4;
-    int32 currentFrame = 3;
-    int32 endJobRI = 2;
-    int32 startJobRI = 1;
+  int32 startJobRI = 1;
+  int32 endJobRI = 2;
+  int32 currentFrame = 3;
+  int32 channelLineLen = 4;
 }
 
 message NavCHlLineDataAck {
-    int32 currentFrame = 3;
-    int32 endJobRI = 2;
-    int32 startJobRI = 1;
+  int32 startJobRI = 1;
+  int32 endJobRI = 2;
+  int32 currentFrame = 3;
 }
 
-message NavBorderDataGet {
-    int32 currentFrame = 2;
-    int32 borderLen = 3;
-    int32 jobId = 1;
+message NavTaskInfo {
+  int32 area = 1;
+  int32 time = 2;
+  int32 allFrame = 3;
+  int32 currentFrame = 4;
+  int32 pathlen = 5;
+  repeated CommDataCouple dc = 6;
 }
 
-message NavTaskInfo {
-    int32 allFrame = 3;
-    int32 area = 1;
-    int32 time = 2;
-    int32 currentFrame = 4;
-    int32 pathlen = 5;
-    repeated CommDataCouple dc = 6;
+message NavBorderDataGet {
+  int32 jobId = 1;
+  int32 currentFrame = 2;
+  int32 borderLen = 3;
 }
 
 message NavOptLineUp {
-    int32 endJobRI = 2;
-    int32 startJobRI = 1;
-    int32 allFrame = 3;
-    int32 currentFrame = 4;
-    int32 channelDataLen = 5;
-    repeated CommDataCouple dc = 6;
+  int32 startJobRI = 1;
+  int32 endJobRI = 2;
+  int32 allFrame = 3;
+  int32 currentFrame = 4;
+  int32 channelDataLen = 5;
+  repeated CommDataCouple dc = 6;
 }
 
-
 message NavOptiBorderInfo {
-    int32 jobId = 1;
-    int32 allFrame = 2;
-    int32 currentFrame = 3;
-    int32 borderDataLen = 4;
-    repeated CommDataCouple dc = 5;
+  int32 jobId = 1;
+  int32 allFrame = 2;
+  int32 currentFrame = 3;
+  int32 borderDataLen = 4;
+  repeated CommDataCouple dc = 5;
 }
 
 message NavOptObsInfo {
-    int32 obstacleId = 1;
-    int32 allFrame = 2;
-    int32 currentFrame = 3;
-    int32 obstacleDataLen = 4;
-    repeated CommDataCouple dc = 5;
+  int32 obstacleId = 1;
+  int32 allFrame = 2;
+  int32 currentFrame = 3;
+  int32 obstacleDataLen = 4;
+  repeated CommDataCouple dc = 5;
 }
 
 message NavStartJob {
-    int64 jobId = 1;
-    int32 jobVer = 2;
-    int32 jobMode = 3;
-    int32 rainTactics = 4;
-    int32 knifeHeight = 5;
-    float speed = 6;
-    int32 channelWidth = 7;
-    int32 ultraWave = 8;
-    int32 channelMode = 9;
+  int64 jobId = 1;
+  int32 jobVer = 2;
+  int32 jobMode = 3;
+  int32 rainTactics = 4;
+  int32 knifeHeight = 5;
+  float speed = 6;
+  int32 channelWidth = 7;
+  int32 UltraWave = 8;
+  int32 channelMode = 9;
+}
+
+message NavTaskProgress {
+  int32 taskProgress = 1;
+}
+
+message NavResFrame {
+  int32 frameid = 1;
 }
 
 message NavGetHashList {
-    int32 pver = 1;
-    int32 subCmd = 2;
-    int32 totalFrame = 3;
-    int32 currentFrame = 4;
-    int64 dataHash = 5;
-    string reserved = 6;
+  int32 pver = 1;
+  int32 subCmd = 2;
+  int32 totalFrame = 3;
+  int32 currentFrame = 4;
+  fixed64 dataHash = 5;
+  string reserved = 6;
 }
 
 message NavGetHashListAck {
-    int32 pver = 1;
-    int32 subCmd = 2;
-    int32 totalFrame = 3;
-    int32 currentFrame = 4;
-    int64 dataHash = 5;
-    int32 hashLen = 6;
-    string reserved = 7;
-    repeated int64 dataCouple = 13;
+  int32 pver = 1;
+  int32 subCmd = 2;
+  int32 totalFrame = 3;
+  int32 currentFrame = 4;
+  fixed64 dataHash = 5;
+  int32 hashLen = 6;
+  string reserved = 7;
+  int32 result = 8;
+  repeated int64 dataCouple = 13;
 }
 
 message NavGetCommData {
-    int32 pver = 1;
-    int32 subCmd = 2;
-    int32 action = 3;
-    int32 type = 4;
-    int64 Hash = 5;
-    fixed64 paternalHashA = 6;
-    fixed64 paternalHashB = 7;
-    int32 totalFrame = 8;
-    int32 currentFrame = 9;
-    fixed64 dataHash = 10;
-    string reserved = 11;
+  int32 pver = 1;
+  int32 subCmd = 2;
+  int32 action = 3;
+  int32 type = 4;
+  int64 Hash = 5;
+  int64 paternalHashA = 6;
+  int64 paternalHashB = 7;
+  int32 totalFrame = 8;
+  int32 currentFrame = 9;
+  fixed64 dataHash = 10;
+  string reserved = 11;
 }
 
 message NavGetCommDataAck {
-    int32 pver = 1;
-    int32 subCmd = 2;
-    int32 result = 3;
-    int32 action = 4;
-    int32 type = 5;
-    fixed64 Hash = 6;
-    fixed64 paternalHashA = 7;
-    fixed64 paternalHashB = 8;
-    int32 totalFrame = 9;
-    int32 currentFrame = 10;
-    int64 dataHash = 11;
-    int32 dataLen = 12;
-    repeated CommDataCouple dataCouple = 13;
-    string reserved = 14;
+  int32 pver = 1;
+  int32 subCmd = 2;
+  int32 result = 3;
+  int32 action = 4;
+  int32 type = 5;
+  fixed64 Hash = 6;
+  fixed64 paternalHashA = 7;
+  fixed64 paternalHashB = 8;
+  int32 totalFrame = 9;
+  int32 currentFrame = 10;
+  fixed64 dataHash = 11;
+  int32 dataLen = 12;
+  repeated CommDataCouple dataCouple = 13;
+  string reserved = 14;
 }
 
 message NavReqCoverPath {
-    int32 pver = 1;
-    int64 jobId = 2;
-    int32 jobVer = 3;
-    int32 jobMode = 4;
-    int32 subCmd = 5;
-    int32 edgeMode = 6;
-    int32 knifeHeight = 7;
-    int32 channelWidth = 8;
-    int32 ultraWave = 9;
-    int32 channelMode = 10;
-    int32 toward = 11;
-    float speed = 12;
-    repeated int64 zoneHashs = 13;
-    int64 pathHash = 14;
-    string reserved = 15;
-    int32 result = 16;
-
+  int32 pver = 1;
+  int64 jobId = 2;
+  int32 jobVer = 3;
+  int32 jobMode = 4;
+  int32 subCmd = 5;
+  int32 edgeMode = 6;
+  int32 knifeHeight = 7;
+  int32 channelWidth = 8;
+  int32 UltraWave = 9;
+  int32 channelMode = 10;
+  int32 toward = 11;
+  float speed = 12;
+  repeated fixed64 zoneHashs = 13;
+  fixed64 pathHash = 14;
+  string reserved = 15;
+  int32 result = 16;
+  int32 toward_mode = 17;
+  int32 toward_included_angle = 18;
 }
 
 message NavUploadZigZagResult {
-    int32 pver = 1;
-    int64 jobId = 2;
-    int32 jobVer = 3;
-    int32 result = 4;
-    int32 area = 5;
-    int32 time = 6;
-    int32 totalZoneNum = 7;
-    int32 currentZonePathNum = 8;
-    int32 currentZonePathId = 9;
-    int32 currentZone = 10;
-    int64 currentHash = 11;
-    int32 totalFrame = 12;
-    int32 currentFrame = 13;
-    int32 channelMode = 14;
-    int32 channelModeId = 15;
-    int64 dataHash = 16;
-    int32 dataLen = 17;
-    string reserved = 18;
-    repeated CommDataCouple dataCouple = 19;
-    int32 subCmd = 20;
+  int32 pver = 1;
+  int64 jobId = 2;
+  int32 jobVer = 3;
+  int32 result = 4;
+  int32 area = 5;
+  int32 time = 6;
+  int32 totalZoneNum = 7;
+  int32 currentZonePathNum = 8;
+  int32 currentZonePathId = 9;
+  int32 currentZone = 10;
+  fixed64 currentHash = 11;
+  int32 totalFrame = 12;
+  int32 currentFrame = 13;
+  int32 channelMode = 14;
+  int32 channelModeId = 15;
+  fixed64 dataHash = 16;
+  int32 dataLen = 17;
+  string reserved = 18;
+  repeated CommDataCouple dataCouple = 19;
+  int32 subCmd = 20;
 }
 
 message NavUploadZigZagResultAck {
-    int32 pver = 1;
-    int32 currentZone = 2;
-    int64 currentHash = 3;
-    int32 totalFrame = 4;
-    int32 currentFrame = 5;
-    int64 dataHash = 6;
-    string reserved = 7;
-    int32 subCmd = 8;
+  int32 pver = 1;
+  int32 currentZone = 2;
+  fixed64 currentHash = 3;
+  int32 totalFrame = 4;
+  int32 currentFrame = 5;
+  fixed64 dataHash = 6;
+  string reserved = 7;
+  int32 subCmd = 8;
 }
 
 message NavTaskCtrl {
-    int32 type = 1;
-    int32 action = 2;
-    int32 result = 3;
-    int32 reserved = 4;
+  int32 type = 1;
+  int32 action = 2;
+  int32 result = 3;
+  string reserved = 4;
 }
 
 message NavTaskIdRw {
-    int32 pver = 1;
-    int32 subCmd = 2;
-    string taskName = 3;
-    string taskId = 4;
-    int32 result = 5;
-    string reserved = 6;
+  int32 pver = 1;
+  int32 subCmd = 2;
+  string taskName = 3;
+  string taskId = 4;
+  int32 result = 5;
+  string reserved = 6;
 }
 
 message NavSysHashOverview {
-    int64 commonhashOverview = 1;
-    int64 pathHashOverview = 2;
+  fixed64 commonhashOverview = 1;
+  fixed64 pathHashOverview = 2;
 }
 
 message NavTaskBreakPoint {
-    float x = 1;
-    float y = 2; 
-    int32 toward = 3;
-    int32 flag = 4;
-    int32 action = 5;
-    int64 zoneHash = 6;
+  float x = 1;
+  float y = 2;
+  int32 toward = 3;
+  int32 flag = 4;
+  int32 action = 5;
+  fixed64 zoneHash = 6;
 }
 
 message NavPlanJobSet {
-    int32 pver = 1;
-    int32 subCmd = 2;
-    int32 area = 3;
-    int32 workTime = 4;
-    string version = 5;
-    string id = 6;
-    string userId = 7;
-    string deviceId = 8;
-    string planId = 9;
-    string taskId = 10;
-    string jobId = 11;
-    string startTime = 12;
-    string endTime = 13;
-    int32 week = 14;
-    int32 knifeHeight = 15;
-    int32 model = 16;
-    int32 edgeMode = 17;
-    int32 requiredTime = 18;
-    int32 routeAngle = 19;
-    int32 routeModel = 20;
-    int32 routeSpacing = 21;
-    int32 ultrasonicBarrier = 22;
-    int32 totalPlanNum = 23;
-    int32 planIndex = 24;
-    int32 result = 25;
-    float speed = 26;
-    string taskName = 27;
-    string jobName = 28;
-    repeated int64 zoneHashs = 29;
-    string reserved = 30;
-
-}
-
-message NavResFrame {
-    int32 frameid = 1;
-}
-
-message NavTaskProgress {
-    int32 taskProgress = 1;
+  int32 pver = 1;
+  int32 subCmd = 2;
+  int32 area = 3;
+  int32 workTime = 4;
+  string version = 5;
+  string id = 6;
+  string userId = 7;
+  string deviceId = 8;
+  string planId = 9;
+  string taskId = 10;
+  string jobId = 11;
+  string startTime = 12;
+  string endTime = 13;
+  int32 week = 14;
+  int32 knifeHeight = 15;
+  int32 model = 16;
+  int32 edgeMode = 17;
+  int32 requiredTime = 18;
+  int32 routeAngle = 19;
+  int32 routeModel = 20;
+  int32 routeSpacing = 21;
+  int32 ultrasonicBarrier = 22;
+  int32 totalPlanNum = 23;
+  int32 PlanIndex = 24;
+  int32 result = 25;
+  float speed = 26;
+  string taskName = 27;
+  string jobName = 28;
+  repeated fixed64 zoneHashs = 29;
+  string reserved = 30;
+  string startDate = 31;
+  string endDate = 32;
+  int32 triggerType = 33;
+  int32 day = 34;
+  repeated fixed32 weeks = 35;
+  int64 remained_seconds = 36;
+  int32 towardMode = 37;
+  int32 towardIncludedAngle = 38;
 }
 
-
 message NavUnableTimeSet {
-    int32 subCmd = 1;
-    string deviceId = 2;
-    string unableStartTime = 3;
-    string unableEndTime = 4;
-    int32 result = 5;
-    string reserved = 6;
+  int32 subCmd = 1;
+  string deviceId = 2;
+  string unableStartTime = 3;
+  string unableEndTime = 4;
+  int32 result = 5;
+  string reserved = 6;
 }
 
-message SimulationCmdData {
-    int32 subCmd = 1;
-    int32 paramId = 2;
-    repeated int32 paramValue = 3;
+message chargePileType {
+  int32 toward = 1;
+  float x = 2;
+  float y = 3;
 }
 
-message WorkReportCmdData {
+message SimulationCmdData {
   int32 subCmd = 1;
-  int32 getInfoNum = 2;
+  int32 param_id = 2;
+  repeated int32 param_value = 3;
 }
 
-message WorkReportInfoAck {
-  int32 currentAckNum = 1;
-  int64 endWorkTime = 2;
-  int32 heightOfKnife = 3;
-  bool interruptFlag = 4;
-  int64 startWorkTime = 5;
-  int32 totalAckNum = 6;
-  double workAres = 7;
-  int32 workProgress = 8;
-  int32 workResult = 9;
-  int32 workTimeUsed = 10;
-  int32 workType = 11;
+message WorkReportUpdateCmd {
+  int32 subCmd = 1;
 }
 
 message WorkReportUpdateAck {
-  int32 infoNum = 2;
-  bool updateFlag = 1;
+  bool update_flag = 1;
+  int32 info_num = 2;
 }
 
-message WorkReportUpdateCmd {
-    int32 subCmd = 1;
+message WorkReportCmdData {
+  int32 subCmd = 1;
+  int32 getInfoNum = 2;
 }
 
-message chargePileType {
-  int32 toward = 1;
-  float x = 2;
-  float y = 3;
+message WorkReportInfoAck {
+  bool interrupt_flag = 1;
+  int64 start_work_time = 2;
+  int64 end_work_time = 3;
+  int32 work_time_used = 4;
+  double work_ares = 5;
+  int32 work_progress = 6;
+  int32 height_of_knife = 7;
+  int32 work_type = 8;
+  int32 work_result = 9;
+  int32 total_ack_num = 10;
+  int32 current_ack_num = 11;
 }
 
-message AppRequestCoverPaths {
+message app_request_cover_paths_t {
   int32 pver = 1;
   int32 subCmd = 2;
   int32 totalFrame = 3;
   int32 currentFrame = 4;
   fixed64 dataHash = 5;
-  int64 transactionId = 6;
+  int64 transaction_id = 6;
   repeated int64 reserved = 7;
-  repeated int64 hashList = 8;
+  repeated fixed64 hash_list = 8;
 }
 
-message CoverPathPacket {
-  fixed64 pathHash = 1;
-  int32 pathType = 2;
-  int32 pathTotal = 3;
-  int32 pathCur = 4;
-  fixed64 zoneHash = 5;
+message cover_path_packet_t {
+  fixed64 path_hash = 1;
+  int32 path_type = 2;
+  int32 path_total = 3;
+  int32 path_cur = 4;
+  fixed64 zone_hash = 5;
   repeated CommDataCouple dataCouple = 6;
 }
 
-message CoverPathUpload {
+message cover_path_upload_t {
   int32 pver = 1;
   int32 result = 2;
   int32 subCmd = 3;
   int32 area = 4;
   int32 time = 5;
   int32 totalFrame = 6;
   int32 currentFrame = 7;
-  int32 totalPathNum = 8;
-  int32 validPathNum = 9;
+  int32 total_path_num = 8;
+  int32 vaild_path_num = 9;
   fixed64 dataHash = 10;
-  int64 transactionId = 11;
+  int64 transaction_id = 11;
   repeated int64 reserved = 12;
   int32 dataLen = 13;
-  repeated CoverPathPacket pathPackets = 14;
+  repeated cover_path_packet_t path_packets = 14;
+}
+
+message zone_start_precent_t {
+  fixed64 dataHash = 1;
+  float x = 2;
+  float y = 3;
+  int32 index = 4;
+}
+
+message vision_ctrl_msg {
+  int32 type = 1;
+  int32 cmd = 2;
+}
+
+message nav_sys_param_msg {
+  int32 rw = 1;
+  int32 id = 2;
+  int32 context = 3;
+}
+
+message nav_plan_task_execute {
+  int32 subCmd = 1;
+  string id = 2;
+  string name = 3;
+  int32 result = 4;
 }
 
+message costmap_t {
+  int32 width = 1;
+  int32 height = 2;
+  float center_x = 3;
+  float center_y = 4;
+  float yaw = 5;
+  float res = 6;
+  repeated int32 costmap = 7;
+}
 
+message plan_task_name_id_t {
+  string id = 1;
+  string name = 2;
+}
 
+message nav_get_all_plan_task {
+  repeated plan_task_name_id_t tasks = 1;
+}
 
 message MctlNav {
-    oneof SubNavMsg {
-        NavLatLonUp toapp_lat_up = 1;
-        NavPosUp toapp_pos_up = 2;
-        NavCHlLineData todev_chl_line_data = 3;
-        NavTaskInfo toapp_task_info = 4;
-        NavOptLineUp toapp_opt_line_up = 5;
-        NavOptiBorderInfo toapp_opt_border_info = 6;
-        NavOptObsInfo toapp_opt_obs_info = 7;
-        NavResFrame todev_task_info_ack = 8;
-        NavResFrame todev_opt_border_info_ack = 9;
-        NavResFrame todev_opt_obs_info_ack = 10;
-        NavResFrame todev_opt_line_up_ack = 11;
-        chargePileType toapp_chgpileto = 12;
-        int32 todev_sustask = 13;
-        int32 todev_rechgcmd = 14;
-        int32 todev_edgecmd = 15;
-        int32 todev_draw_border = 16;
-        int32 todev_draw_border_end = 17;
-        int32 todev_draw_obs = 18;
-        int32 todev_draw_obs_end = 19;
-        int32 todev_chl_line = 20;
-        int32 todev_chl_line_end = 21;
-        int32 todev_save_task = 22;
-        int32 todev_cancel_suscmd = 23;
-        int32 todev_reset_chg_pile = 24;
-        int32 todev_cancel_draw_cmd = 25;
-        int32 todev_one_touch_leave_pile = 26;
-        NavStartJob todev_mow_task = 27;
-        NavBorderState toapp_bstate = 28;
-        int32 todev_lat_up_ack = 29;
-        NavGetHashList todev_gethash = 30;
-        NavGetHashListAck toapp_gethash_ack = 31;
-        NavGetCommData todev_get_commondata = 32;
-        NavGetCommDataAck toapp_get_commondata_ack = 33;
-        NavReqCoverPath bidire_reqconver_path = 34;
-        NavUploadZigZagResult toapp_zigzag = 35;
-        NavUploadZigZagResultAck todev_zigzag_ack = 36;
-        NavTaskCtrl todev_taskctrl = 37;
-        NavTaskIdRw bidire_taskid = 38;
-        NavTaskBreakPoint toapp_bp = 39;
-        NavPlanJobSet todev_planjob_set = 40;
-        NavUnableTimeSet todev_unable_time_set = 41;
-        SimulationCmdData simulation_cmd = 42;
-        WorkReportUpdateCmd todev_work_report_update_cmd = 43;
-        WorkReportUpdateAck toapp_work_report_update_ack = 44;
-        WorkReportCmdData todev_work_report_cmd = 45;
-        WorkReportInfoAck toapp_work_report_ack = 46;
-        WorkReportInfoAck toapp_work_report_upload = 47;
-        AppRequestCoverPaths app_request_cover_paths_t = 48;
-        CoverPathUpload cover_path_upload_t = 49;
-        // 50 zone_start_precent_t
-        // 51 vision_ctrl_msg
-        // 52 nav_sys_param_msg
-        // 53 nav_plan_task_execute
-        // 54 costmap_t
-    }
-}
+  oneof SubNavMsg {
+    NavLatLonUp toapp_lat_up = 1;
+    NavPosUp toapp_pos_up = 2;
+    NavCHlLineData todev_chl_line_data = 3;
+    NavTaskInfo toapp_task_info = 4;
+    NavOptLineUp toapp_opt_line_up = 5;
+    NavOptiBorderInfo toapp_opt_border_info = 6;
+    NavOptObsInfo toapp_opt_obs_info = 7;
+    NavResFrame todev_task_info_ack = 8;
+    NavResFrame todev_opt_border_info_ack = 9;
+    NavResFrame todev_opt_obs_info_ack = 10;
+    NavResFrame todev_opt_line_up_ack = 11;
+    chargePileType toapp_chgpileto = 12;
+    int32 todev_sustask = 13;
+    int32 todev_rechgcmd = 14;
+    int32 todev_edgecmd = 15;
+    int32 todev_draw_border = 16;
+    int32 todev_draw_border_end = 17;
+    int32 todev_draw_obs = 18;
+    int32 todev_draw_obs_end = 19;
+    int32 todev_chl_line = 20;
+    int32 todev_chl_line_end = 21;
+    int32 todev_save_task = 22;
+    int32 todev_cancel_suscmd = 23;
+    int32 todev_reset_chg_pile = 24;
+    int32 todev_cancel_draw_cmd = 25;
+    int32 todev_one_touch_leave_pile = 26;
+    NavStartJob todev_mow_task = 27;
+    NavBorderState toapp_bstate = 28;
+    int32 todev_lat_up_ack = 29;
+    NavGetHashList todev_gethash = 30;
+    NavGetHashListAck toapp_gethash_ack = 31;
+    NavGetCommData todev_get_commondata = 32;
+    NavGetCommDataAck toapp_get_commondata_ack = 33;
+    NavReqCoverPath bidire_reqconver_path = 34;
+    NavUploadZigZagResult toapp_zigzag = 35;
+    NavUploadZigZagResultAck todev_zigzag_ack = 36;
+    NavTaskCtrl todev_taskctrl = 37;
+    NavTaskIdRw bidire_taskid = 38;
+    NavTaskBreakPoint toapp_bp = 39;
+    NavPlanJobSet todev_planjob_set = 40;
+    NavUnableTimeSet todev_unable_time_set = 41;
+    SimulationCmdData simulation_cmd = 42;
+    WorkReportUpdateCmd todev_work_report_update_cmd = 43;
+    WorkReportUpdateAck toapp_work_report_update_ack = 44;
+    WorkReportCmdData todev_work_report_cmd = 45;
+    WorkReportInfoAck toapp_work_report_ack = 46;
+    WorkReportInfoAck toapp_work_report_upload = 47;
+    app_request_cover_paths_t app_request_cover_paths = 48;
+    cover_path_upload_t cover_path_upload = 49;
+    zone_start_precent_t zone_start_precent = 50;
+    vision_ctrl_msg vision_ctrl = 51;
+    nav_sys_param_msg nav_sys_param_cmd = 52;
+    nav_plan_task_execute plan_task_execute = 53;
+    costmap_t toapp_costmap = 54;
+    plan_task_name_id_t plan_task_name_id = 55;
+    nav_get_all_plan_task all_plan_task = 56;
+  }
+}
```

### Comparing `pyluba-0.0.5/pyluba/proto/mctrl_nav_pb2.py` & `pyluba-0.0.6/pyluba/proto/mctrl_nav_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from pyluba.proto import common_pb2 as pyluba_dot_proto_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_nav.proto\x1a\x19pyluba/proto/common.proto\"\'\n\x0bNavLatLonUp\x12\x0b\n\x03lat\x18\x01 \x01(\x01\x12\x0b\n\x03lon\x18\x02 \x01(\x01\"!\n\x0eNavBorderState\x12\x0f\n\x07\x62\x64state\x18\x01 \x01(\x05\"\xc9\x01\n\x08NavPosUp\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\x0e\n\x06status\x18\x03 \x01(\x05\x12\x0e\n\x06toward\x18\x04 \x01(\x05\x12\r\n\x05stars\x18\x05 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x06 \x01(\x02\x12\x11\n\tlatStddev\x18\x07 \x01(\x02\x12\x11\n\tlonStddev\x18\x08 \x01(\x02\x12\x11\n\tl2dfStars\x18\t \x01(\x05\x12\x0f\n\x07posType\x18\n \x01(\x05\x12\x0f\n\x07\x63HashId\x18\x0b \x01(\x03\x12\x10\n\x08posLevel\x18\x0c \x01(\x05\":\n\x13NavBorderDataGetAck\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"Z\n\x15NavObstiBorderDataGet\x12\x15\n\robstacleIndex\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x14\n\x0cobstaclesLen\x18\x03 \x01(\x05\"G\n\x18NavObstiBorderDataGetAck\x12\x15\n\robstacleIndex\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"d\n\x0eNavCHlLineData\x12\x16\n\x0e\x63hannelLineLen\x18\x04 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\"O\n\x11NavCHlLineDataAck\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\"J\n\x10NavBorderDataGet\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x11\n\tborderLen\x18\x03 \x01(\x05\x12\r\n\x05jobId\x18\x01 \x01(\x05\"\x7f\n\x0bNavTaskInfo\x12\x10\n\x08\x61llFrame\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x01 \x01(\x05\x12\x0c\n\x04time\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x0f\n\x07pathlen\x18\x05 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"\x91\x01\n\x0cNavOptLineUp\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x16\n\x0e\x63hannelDataLen\x18\x05 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"~\n\x11NavOptiBorderInfo\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x15\n\rborderDataLen\x18\x04 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x05 \x03(\x0b\x32\x0f.CommDataCouple\"\x81\x01\n\rNavOptObsInfo\x12\x12\n\nobstacleId\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x17\n\x0fobstacleDataLen\x18\x04 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x05 \x03(\x0b\x32\x0f.CommDataCouple\"\xb4\x01\n\x0bNavStartJob\x12\r\n\x05jobId\x18\x01 \x01(\x03\x12\x0e\n\x06jobVer\x18\x02 \x01(\x05\x12\x0f\n\x07jobMode\x18\x03 \x01(\x05\x12\x13\n\x0brainTactics\x18\x04 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x05 \x01(\x05\x12\r\n\x05speed\x18\x06 \x01(\x02\x12\x14\n\x0c\x63hannelWidth\x18\x07 \x01(\x05\x12\x11\n\tultraWave\x18\x08 \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\t \x01(\x05\"|\n\x0eNavGetHashList\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x03\x12\x10\n\x08reserved\x18\x06 \x01(\t\"\xa4\x01\n\x11NavGetHashListAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x03\x12\x0f\n\x07hashLen\x18\x06 \x01(\x05\x12\x10\n\x08reserved\x18\x07 \x01(\t\x12\x12\n\ndataCouple\x18\r \x03(\x03\"\xd6\x01\n\x0eNavGetCommData\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\x05\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\x0c\n\x04Hash\x18\x05 \x01(\x03\x12\x15\n\rpaternalHashA\x18\x06 \x01(\x06\x12\x15\n\rpaternalHashB\x18\x07 \x01(\x06\x12\x12\n\ntotalFrame\x18\x08 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\t \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\n \x01(\x06\x12\x10\n\x08reserved\x18\x0b \x01(\t\"\x9f\x02\n\x11NavGetCommDataAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\x05\x12\x0c\n\x04type\x18\x05 \x01(\x05\x12\x0c\n\x04Hash\x18\x06 \x01(\x06\x12\x15\n\rpaternalHashA\x18\x07 \x01(\x06\x12\x15\n\rpaternalHashB\x18\x08 \x01(\x06\x12\x12\n\ntotalFrame\x18\t \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\n \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x0b \x01(\x03\x12\x0f\n\x07\x64\x61taLen\x18\x0c \x01(\x05\x12#\n\ndataCouple\x18\r \x03(\x0b\x32\x0f.CommDataCouple\x12\x10\n\x08reserved\x18\x0e \x01(\t\"\xaa\x02\n\x0fNavReqCoverPath\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\r\n\x05jobId\x18\x02 \x01(\x03\x12\x0e\n\x06jobVer\x18\x03 \x01(\x05\x12\x0f\n\x07jobMode\x18\x04 \x01(\x05\x12\x0e\n\x06subCmd\x18\x05 \x01(\x05\x12\x10\n\x08\x65\x64geMode\x18\x06 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x07 \x01(\x05\x12\x14\n\x0c\x63hannelWidth\x18\x08 \x01(\x05\x12\x11\n\tultraWave\x18\t \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\n \x01(\x05\x12\x0e\n\x06toward\x18\x0b \x01(\x05\x12\r\n\x05speed\x18\x0c \x01(\x02\x12\x11\n\tzoneHashs\x18\r \x03(\x03\x12\x10\n\x08pathHash\x18\x0e \x01(\x03\x12\x10\n\x08reserved\x18\x0f \x01(\t\x12\x0e\n\x06result\x18\x10 \x01(\x05\"\xa7\x03\n\x15NavUploadZigZagResult\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\r\n\x05jobId\x18\x02 \x01(\x03\x12\x0e\n\x06jobVer\x18\x03 \x01(\x05\x12\x0e\n\x06result\x18\x04 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x05 \x01(\x05\x12\x0c\n\x04time\x18\x06 \x01(\x05\x12\x14\n\x0ctotalZoneNum\x18\x07 \x01(\x05\x12\x1a\n\x12\x63urrentZonePathNum\x18\x08 \x01(\x05\x12\x19\n\x11\x63urrentZonePathId\x18\t \x01(\x05\x12\x13\n\x0b\x63urrentZone\x18\n \x01(\x05\x12\x13\n\x0b\x63urrentHash\x18\x0b \x01(\x03\x12\x12\n\ntotalFrame\x18\x0c \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\r \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\x0e \x01(\x05\x12\x15\n\rchannelModeId\x18\x0f \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x10 \x01(\x03\x12\x0f\n\x07\x64\x61taLen\x18\x11 \x01(\x05\x12\x10\n\x08reserved\x18\x12 \x01(\t\x12#\n\ndataCouple\x18\x13 \x03(\x0b\x32\x0f.CommDataCouple\x12\x0e\n\x06subCmd\x18\x14 \x01(\x05\"\xb0\x01\n\x18NavUploadZigZagResultAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x13\n\x0b\x63urrentZone\x18\x02 \x01(\x05\x12\x13\n\x0b\x63urrentHash\x18\x03 \x01(\x03\x12\x12\n\ntotalFrame\x18\x04 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x05 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x06 \x01(\x03\x12\x10\n\x08reserved\x18\x07 \x01(\t\x12\x0e\n\x06subCmd\x18\x08 \x01(\x05\"M\n\x0bNavTaskCtrl\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x10\n\x08reserved\x18\x04 \x01(\x05\"o\n\x0bNavTaskIdRw\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x10\n\x08taskName\x18\x03 \x01(\t\x12\x0e\n\x06taskId\x18\x04 \x01(\t\x12\x0e\n\x06result\x18\x05 \x01(\x05\x12\x10\n\x08reserved\x18\x06 \x01(\t\"J\n\x12NavSysHashOverview\x12\x1a\n\x12\x63ommonhashOverview\x18\x01 \x01(\x03\x12\x18\n\x10pathHashOverview\x18\x02 \x01(\x03\"i\n\x11NavTaskBreakPoint\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\x0e\n\x06toward\x18\x03 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x04 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\x05\x12\x10\n\x08zoneHash\x18\x06 \x01(\x03\"\xa2\x04\n\rNavPlanJobSet\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x03 \x01(\x05\x12\x10\n\x08workTime\x18\x04 \x01(\x05\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\n\n\x02id\x18\x06 \x01(\t\x12\x0e\n\x06userId\x18\x07 \x01(\t\x12\x10\n\x08\x64\x65viceId\x18\x08 \x01(\t\x12\x0e\n\x06planId\x18\t \x01(\t\x12\x0e\n\x06taskId\x18\n \x01(\t\x12\r\n\x05jobId\x18\x0b \x01(\t\x12\x11\n\tstartTime\x18\x0c \x01(\t\x12\x0f\n\x07\x65ndTime\x18\r \x01(\t\x12\x0c\n\x04week\x18\x0e \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x0f \x01(\x05\x12\r\n\x05model\x18\x10 \x01(\x05\x12\x10\n\x08\x65\x64geMode\x18\x11 \x01(\x05\x12\x14\n\x0crequiredTime\x18\x12 \x01(\x05\x12\x12\n\nrouteAngle\x18\x13 \x01(\x05\x12\x12\n\nrouteModel\x18\x14 \x01(\x05\x12\x14\n\x0crouteSpacing\x18\x15 \x01(\x05\x12\x19\n\x11ultrasonicBarrier\x18\x16 \x01(\x05\x12\x14\n\x0ctotalPlanNum\x18\x17 \x01(\x05\x12\x11\n\tplanIndex\x18\x18 \x01(\x05\x12\x0e\n\x06result\x18\x19 \x01(\x05\x12\r\n\x05speed\x18\x1a \x01(\x02\x12\x10\n\x08taskName\x18\x1b \x01(\t\x12\x0f\n\x07jobName\x18\x1c \x01(\t\x12\x11\n\tzoneHashs\x18\x1d \x03(\x03\x12\x10\n\x08reserved\x18\x1e \x01(\t\"\x1e\n\x0bNavResFrame\x12\x0f\n\x07\x66rameid\x18\x01 \x01(\x05\"\'\n\x0fNavTaskProgress\x12\x14\n\x0ctaskProgress\x18\x01 \x01(\x05\"\x86\x01\n\x10NavUnableTimeSet\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x10\n\x08\x64\x65viceId\x18\x02 \x01(\t\x12\x17\n\x0funableStartTime\x18\x03 \x01(\t\x12\x15\n\runableEndTime\x18\x04 \x01(\t\x12\x0e\n\x06result\x18\x05 \x01(\x05\x12\x10\n\x08reserved\x18\x06 \x01(\t\"H\n\x11SimulationCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x0f\n\x07paramId\x18\x02 \x01(\x05\x12\x12\n\nparamValue\x18\x03 \x03(\x05\"7\n\x11WorkReportCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x12\n\ngetInfoNum\x18\x02 \x01(\x05\"\xfd\x01\n\x11WorkReportInfoAck\x12\x15\n\rcurrentAckNum\x18\x01 \x01(\x05\x12\x13\n\x0b\x65ndWorkTime\x18\x02 \x01(\x03\x12\x15\n\rheightOfKnife\x18\x03 \x01(\x05\x12\x15\n\rinterruptFlag\x18\x04 \x01(\x08\x12\x15\n\rstartWorkTime\x18\x05 \x01(\x03\x12\x13\n\x0btotalAckNum\x18\x06 \x01(\x05\x12\x10\n\x08workAres\x18\x07 \x01(\x01\x12\x14\n\x0cworkProgress\x18\x08 \x01(\x05\x12\x12\n\nworkResult\x18\t \x01(\x05\x12\x14\n\x0cworkTimeUsed\x18\n \x01(\x05\x12\x10\n\x08workType\x18\x0b \x01(\x05\":\n\x13WorkReportUpdateAck\x12\x0f\n\x07infoNum\x18\x02 \x01(\x05\x12\x12\n\nupdateFlag\x18\x01 \x01(\x08\"%\n\x13WorkReportUpdateCmd\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\"6\n\x0e\x63hargePileType\x12\x0e\n\x06toward\x18\x01 \x01(\x05\x12\t\n\x01x\x18\x02 \x01(\x02\x12\t\n\x01y\x18\x03 \x01(\x02\"\xab\x01\n\x14\x41ppRequestCoverPaths\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x06\x12\x15\n\rtransactionId\x18\x06 \x01(\x03\x12\x10\n\x08reserved\x18\x07 \x03(\x03\x12\x10\n\x08hashList\x18\x08 \x03(\x03\"\x90\x01\n\x0f\x43overPathPacket\x12\x10\n\x08pathHash\x18\x01 \x01(\x06\x12\x10\n\x08pathType\x18\x02 \x01(\x05\x12\x11\n\tpathTotal\x18\x03 \x01(\x05\x12\x0f\n\x07pathCur\x18\x04 \x01(\x05\x12\x10\n\x08zoneHash\x18\x05 \x01(\x06\x12#\n\ndataCouple\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"\xa4\x02\n\x0f\x43overPathUpload\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\x05\x12\x0e\n\x06subCmd\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x04 \x01(\x05\x12\x0c\n\x04time\x18\x05 \x01(\x05\x12\x12\n\ntotalFrame\x18\x06 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x07 \x01(\x05\x12\x14\n\x0ctotalPathNum\x18\x08 \x01(\x05\x12\x14\n\x0cvalidPathNum\x18\t \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\n \x01(\x06\x12\x15\n\rtransactionId\x18\x0b \x01(\x03\x12\x10\n\x08reserved\x18\x0c \x03(\x03\x12\x0f\n\x07\x64\x61taLen\x18\r \x01(\x05\x12%\n\x0bpathPackets\x18\x0e \x03(\x0b\x32\x10.CoverPathPacket\"\xa9\x10\n\x07MctlNav\x12$\n\x0ctoapp_lat_up\x18\x01 \x01(\x0b\x32\x0c.NavLatLonUpH\x00\x12!\n\x0ctoapp_pos_up\x18\x02 \x01(\x0b\x32\t.NavPosUpH\x00\x12.\n\x13todev_chl_line_data\x18\x03 \x01(\x0b\x32\x0f.NavCHlLineDataH\x00\x12\'\n\x0ftoapp_task_info\x18\x04 \x01(\x0b\x32\x0c.NavTaskInfoH\x00\x12*\n\x11toapp_opt_line_up\x18\x05 \x01(\x0b\x32\r.NavOptLineUpH\x00\x12\x33\n\x15toapp_opt_border_info\x18\x06 \x01(\x0b\x32\x12.NavOptiBorderInfoH\x00\x12,\n\x12toapp_opt_obs_info\x18\x07 \x01(\x0b\x32\x0e.NavOptObsInfoH\x00\x12+\n\x13todev_task_info_ack\x18\x08 \x01(\x0b\x32\x0c.NavResFrameH\x00\x12\x31\n\x19todev_opt_border_info_ack\x18\t \x01(\x0b\x32\x0c.NavResFrameH\x00\x12.\n\x16todev_opt_obs_info_ack\x18\n \x01(\x0b\x32\x0c.NavResFrameH\x00\x12-\n\x15todev_opt_line_up_ack\x18\x0b \x01(\x0b\x32\x0c.NavResFrameH\x00\x12*\n\x0ftoapp_chgpileto\x18\x0c \x01(\x0b\x32\x0f.chargePileTypeH\x00\x12\x17\n\rtodev_sustask\x18\r \x01(\x05H\x00\x12\x18\n\x0etodev_rechgcmd\x18\x0e \x01(\x05H\x00\x12\x17\n\rtodev_edgecmd\x18\x0f \x01(\x05H\x00\x12\x1b\n\x11todev_draw_border\x18\x10 \x01(\x05H\x00\x12\x1f\n\x15todev_draw_border_end\x18\x11 \x01(\x05H\x00\x12\x18\n\x0etodev_draw_obs\x18\x12 \x01(\x05H\x00\x12\x1c\n\x12todev_draw_obs_end\x18\x13 \x01(\x05H\x00\x12\x18\n\x0etodev_chl_line\x18\x14 \x01(\x05H\x00\x12\x1c\n\x12todev_chl_line_end\x18\x15 \x01(\x05H\x00\x12\x19\n\x0ftodev_save_task\x18\x16 \x01(\x05H\x00\x12\x1d\n\x13todev_cancel_suscmd\x18\x17 \x01(\x05H\x00\x12\x1e\n\x14todev_reset_chg_pile\x18\x18 \x01(\x05H\x00\x12\x1f\n\x15todev_cancel_draw_cmd\x18\x19 \x01(\x05H\x00\x12$\n\x1atodev_one_touch_leave_pile\x18\x1a \x01(\x05H\x00\x12&\n\x0etodev_mow_task\x18\x1b \x01(\x0b\x32\x0c.NavStartJobH\x00\x12\'\n\x0ctoapp_bstate\x18\x1c \x01(\x0b\x32\x0f.NavBorderStateH\x00\x12\x1a\n\x10todev_lat_up_ack\x18\x1d \x01(\x05H\x00\x12(\n\rtodev_gethash\x18\x1e \x01(\x0b\x32\x0f.NavGetHashListH\x00\x12/\n\x11toapp_gethash_ack\x18\x1f \x01(\x0b\x32\x12.NavGetHashListAckH\x00\x12/\n\x14todev_get_commondata\x18  \x01(\x0b\x32\x0f.NavGetCommDataH\x00\x12\x36\n\x18toapp_get_commondata_ack\x18! \x01(\x0b\x32\x12.NavGetCommDataAckH\x00\x12\x31\n\x15\x62idire_reqconver_path\x18\" \x01(\x0b\x32\x10.NavReqCoverPathH\x00\x12.\n\x0ctoapp_zigzag\x18# \x01(\x0b\x32\x16.NavUploadZigZagResultH\x00\x12\x35\n\x10todev_zigzag_ack\x18$ \x01(\x0b\x32\x19.NavUploadZigZagResultAckH\x00\x12&\n\x0etodev_taskctrl\x18% \x01(\x0b\x32\x0c.NavTaskCtrlH\x00\x12%\n\rbidire_taskid\x18& \x01(\x0b\x32\x0c.NavTaskIdRwH\x00\x12&\n\x08toapp_bp\x18\' \x01(\x0b\x32\x12.NavTaskBreakPointH\x00\x12+\n\x11todev_planjob_set\x18( \x01(\x0b\x32\x0e.NavPlanJobSetH\x00\x12\x32\n\x15todev_unable_time_set\x18) \x01(\x0b\x32\x11.NavUnableTimeSetH\x00\x12,\n\x0esimulation_cmd\x18* \x01(\x0b\x32\x12.SimulationCmdDataH\x00\x12<\n\x1ctodev_work_report_update_cmd\x18+ \x01(\x0b\x32\x14.WorkReportUpdateCmdH\x00\x12<\n\x1ctoapp_work_report_update_ack\x18, \x01(\x0b\x32\x14.WorkReportUpdateAckH\x00\x12\x33\n\x15todev_work_report_cmd\x18- \x01(\x0b\x32\x12.WorkReportCmdDataH\x00\x12\x33\n\x15toapp_work_report_ack\x18. \x01(\x0b\x32\x12.WorkReportInfoAckH\x00\x12\x36\n\x18toapp_work_report_upload\x18/ \x01(\x0b\x32\x12.WorkReportInfoAckH\x00\x12:\n\x19\x61pp_request_cover_paths_t\x18\x30 \x01(\x0b\x32\x15.AppRequestCoverPathsH\x00\x12/\n\x13\x63over_path_upload_t\x18\x31 \x01(\x0b\x32\x10.CoverPathUploadH\x00\x42\x0b\n\tSubNavMsgb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_nav.proto\x1a\x19pyluba/proto/common.proto\"\'\n\x0bNavLatLonUp\x12\x0b\n\x03lat\x18\x01 \x01(\x01\x12\x0b\n\x03lon\x18\x02 \x01(\x01\"!\n\x0eNavBorderState\x12\x0f\n\x07\x62\x64state\x18\x01 \x01(\x05\"\xc9\x01\n\x08NavPosUp\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\x0e\n\x06status\x18\x03 \x01(\x05\x12\x0e\n\x06toward\x18\x04 \x01(\x05\x12\r\n\x05stars\x18\x05 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x06 \x01(\x02\x12\x11\n\tlatStddev\x18\x07 \x01(\x02\x12\x11\n\tlonStddev\x18\x08 \x01(\x02\x12\x11\n\tl2dfStars\x18\t \x01(\x05\x12\x0f\n\x07posType\x18\n \x01(\x05\x12\x0f\n\x07\x63HashId\x18\x0b \x01(\x03\x12\x10\n\x08posLevel\x18\x0c \x01(\x05\":\n\x13NavBorderDataGetAck\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"Z\n\x15NavObstiBorderDataGet\x12\x15\n\robstacleIndex\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x14\n\x0cobstaclesLen\x18\x03 \x01(\x05\"G\n\x18NavObstiBorderDataGetAck\x12\x15\n\robstacleIndex\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"d\n\x0eNavCHlLineData\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x16\n\x0e\x63hannelLineLen\x18\x04 \x01(\x05\"O\n\x11NavCHlLineDataAck\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\"\x7f\n\x0bNavTaskInfo\x12\x0c\n\x04\x61rea\x18\x01 \x01(\x05\x12\x0c\n\x04time\x18\x02 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x0f\n\x07pathlen\x18\x05 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"J\n\x10NavBorderDataGet\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x11\n\tborderLen\x18\x03 \x01(\x05\"\x91\x01\n\x0cNavOptLineUp\x12\x12\n\nstartJobRI\x18\x01 \x01(\x05\x12\x10\n\x08\x65ndJobRI\x18\x02 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x16\n\x0e\x63hannelDataLen\x18\x05 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"~\n\x11NavOptiBorderInfo\x12\r\n\x05jobId\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x15\n\rborderDataLen\x18\x04 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x05 \x03(\x0b\x32\x0f.CommDataCouple\"\x81\x01\n\rNavOptObsInfo\x12\x12\n\nobstacleId\x18\x01 \x01(\x05\x12\x10\n\x08\x61llFrame\x18\x02 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x03 \x01(\x05\x12\x17\n\x0fobstacleDataLen\x18\x04 \x01(\x05\x12\x1b\n\x02\x64\x63\x18\x05 \x03(\x0b\x32\x0f.CommDataCouple\"\xb4\x01\n\x0bNavStartJob\x12\r\n\x05jobId\x18\x01 \x01(\x03\x12\x0e\n\x06jobVer\x18\x02 \x01(\x05\x12\x0f\n\x07jobMode\x18\x03 \x01(\x05\x12\x13\n\x0brainTactics\x18\x04 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x05 \x01(\x05\x12\r\n\x05speed\x18\x06 \x01(\x02\x12\x14\n\x0c\x63hannelWidth\x18\x07 \x01(\x05\x12\x11\n\tUltraWave\x18\x08 \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\t \x01(\x05\"\'\n\x0fNavTaskProgress\x12\x14\n\x0ctaskProgress\x18\x01 \x01(\x05\"\x1e\n\x0bNavResFrame\x12\x0f\n\x07\x66rameid\x18\x01 \x01(\x05\"|\n\x0eNavGetHashList\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x06\x12\x10\n\x08reserved\x18\x06 \x01(\t\"\xb4\x01\n\x11NavGetHashListAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x06\x12\x0f\n\x07hashLen\x18\x06 \x01(\x05\x12\x10\n\x08reserved\x18\x07 \x01(\t\x12\x0e\n\x06result\x18\x08 \x01(\x05\x12\x12\n\ndataCouple\x18\r \x03(\x03\"\xd6\x01\n\x0eNavGetCommData\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\x05\x12\x0c\n\x04type\x18\x04 \x01(\x05\x12\x0c\n\x04Hash\x18\x05 \x01(\x03\x12\x15\n\rpaternalHashA\x18\x06 \x01(\x03\x12\x15\n\rpaternalHashB\x18\x07 \x01(\x03\x12\x12\n\ntotalFrame\x18\x08 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\t \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\n \x01(\x06\x12\x10\n\x08reserved\x18\x0b \x01(\t\"\x9f\x02\n\x11NavGetCommDataAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x04 \x01(\x05\x12\x0c\n\x04type\x18\x05 \x01(\x05\x12\x0c\n\x04Hash\x18\x06 \x01(\x06\x12\x15\n\rpaternalHashA\x18\x07 \x01(\x06\x12\x15\n\rpaternalHashB\x18\x08 \x01(\x06\x12\x12\n\ntotalFrame\x18\t \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\n \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x0b \x01(\x06\x12\x0f\n\x07\x64\x61taLen\x18\x0c \x01(\x05\x12#\n\ndataCouple\x18\r \x03(\x0b\x32\x0f.CommDataCouple\x12\x10\n\x08reserved\x18\x0e \x01(\t\"\xde\x02\n\x0fNavReqCoverPath\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\r\n\x05jobId\x18\x02 \x01(\x03\x12\x0e\n\x06jobVer\x18\x03 \x01(\x05\x12\x0f\n\x07jobMode\x18\x04 \x01(\x05\x12\x0e\n\x06subCmd\x18\x05 \x01(\x05\x12\x10\n\x08\x65\x64geMode\x18\x06 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x07 \x01(\x05\x12\x14\n\x0c\x63hannelWidth\x18\x08 \x01(\x05\x12\x11\n\tUltraWave\x18\t \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\n \x01(\x05\x12\x0e\n\x06toward\x18\x0b \x01(\x05\x12\r\n\x05speed\x18\x0c \x01(\x02\x12\x11\n\tzoneHashs\x18\r \x03(\x06\x12\x10\n\x08pathHash\x18\x0e \x01(\x06\x12\x10\n\x08reserved\x18\x0f \x01(\t\x12\x0e\n\x06result\x18\x10 \x01(\x05\x12\x13\n\x0btoward_mode\x18\x11 \x01(\x05\x12\x1d\n\x15toward_included_angle\x18\x12 \x01(\x05\"\xa7\x03\n\x15NavUploadZigZagResult\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\r\n\x05jobId\x18\x02 \x01(\x03\x12\x0e\n\x06jobVer\x18\x03 \x01(\x05\x12\x0e\n\x06result\x18\x04 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x05 \x01(\x05\x12\x0c\n\x04time\x18\x06 \x01(\x05\x12\x14\n\x0ctotalZoneNum\x18\x07 \x01(\x05\x12\x1a\n\x12\x63urrentZonePathNum\x18\x08 \x01(\x05\x12\x19\n\x11\x63urrentZonePathId\x18\t \x01(\x05\x12\x13\n\x0b\x63urrentZone\x18\n \x01(\x05\x12\x13\n\x0b\x63urrentHash\x18\x0b \x01(\x06\x12\x12\n\ntotalFrame\x18\x0c \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\r \x01(\x05\x12\x13\n\x0b\x63hannelMode\x18\x0e \x01(\x05\x12\x15\n\rchannelModeId\x18\x0f \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x10 \x01(\x06\x12\x0f\n\x07\x64\x61taLen\x18\x11 \x01(\x05\x12\x10\n\x08reserved\x18\x12 \x01(\t\x12#\n\ndataCouple\x18\x13 \x03(\x0b\x32\x0f.CommDataCouple\x12\x0e\n\x06subCmd\x18\x14 \x01(\x05\"\xb0\x01\n\x18NavUploadZigZagResultAck\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x13\n\x0b\x63urrentZone\x18\x02 \x01(\x05\x12\x13\n\x0b\x63urrentHash\x18\x03 \x01(\x06\x12\x12\n\ntotalFrame\x18\x04 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x05 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x06 \x01(\x06\x12\x10\n\x08reserved\x18\x07 \x01(\t\x12\x0e\n\x06subCmd\x18\x08 \x01(\x05\"M\n\x0bNavTaskCtrl\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x10\n\x08reserved\x18\x04 \x01(\t\"o\n\x0bNavTaskIdRw\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x10\n\x08taskName\x18\x03 \x01(\t\x12\x0e\n\x06taskId\x18\x04 \x01(\t\x12\x0e\n\x06result\x18\x05 \x01(\x05\x12\x10\n\x08reserved\x18\x06 \x01(\t\"J\n\x12NavSysHashOverview\x12\x1a\n\x12\x63ommonhashOverview\x18\x01 \x01(\x06\x12\x18\n\x10pathHashOverview\x18\x02 \x01(\x06\"i\n\x11NavTaskBreakPoint\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\x0e\n\x06toward\x18\x03 \x01(\x05\x12\x0c\n\x04\x66lag\x18\x04 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\x05\x12\x10\n\x08zoneHash\x18\x06 \x01(\x06\"\xc2\x05\n\rNavPlanJobSet\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x03 \x01(\x05\x12\x10\n\x08workTime\x18\x04 \x01(\x05\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\n\n\x02id\x18\x06 \x01(\t\x12\x0e\n\x06userId\x18\x07 \x01(\t\x12\x10\n\x08\x64\x65viceId\x18\x08 \x01(\t\x12\x0e\n\x06planId\x18\t \x01(\t\x12\x0e\n\x06taskId\x18\n \x01(\t\x12\r\n\x05jobId\x18\x0b \x01(\t\x12\x11\n\tstartTime\x18\x0c \x01(\t\x12\x0f\n\x07\x65ndTime\x18\r \x01(\t\x12\x0c\n\x04week\x18\x0e \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x0f \x01(\x05\x12\r\n\x05model\x18\x10 \x01(\x05\x12\x10\n\x08\x65\x64geMode\x18\x11 \x01(\x05\x12\x14\n\x0crequiredTime\x18\x12 \x01(\x05\x12\x12\n\nrouteAngle\x18\x13 \x01(\x05\x12\x12\n\nrouteModel\x18\x14 \x01(\x05\x12\x14\n\x0crouteSpacing\x18\x15 \x01(\x05\x12\x19\n\x11ultrasonicBarrier\x18\x16 \x01(\x05\x12\x14\n\x0ctotalPlanNum\x18\x17 \x01(\x05\x12\x11\n\tPlanIndex\x18\x18 \x01(\x05\x12\x0e\n\x06result\x18\x19 \x01(\x05\x12\r\n\x05speed\x18\x1a \x01(\x02\x12\x10\n\x08taskName\x18\x1b \x01(\t\x12\x0f\n\x07jobName\x18\x1c \x01(\t\x12\x11\n\tzoneHashs\x18\x1d \x03(\x06\x12\x10\n\x08reserved\x18\x1e \x01(\t\x12\x11\n\tstartDate\x18\x1f \x01(\t\x12\x0f\n\x07\x65ndDate\x18  \x01(\t\x12\x13\n\x0btriggerType\x18! \x01(\x05\x12\x0b\n\x03\x64\x61y\x18\" \x01(\x05\x12\r\n\x05weeks\x18# \x03(\x07\x12\x18\n\x10remained_seconds\x18$ \x01(\x03\x12\x12\n\ntowardMode\x18% \x01(\x05\x12\x1b\n\x13towardIncludedAngle\x18& \x01(\x05\"\x86\x01\n\x10NavUnableTimeSet\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x10\n\x08\x64\x65viceId\x18\x02 \x01(\t\x12\x17\n\x0funableStartTime\x18\x03 \x01(\t\x12\x15\n\runableEndTime\x18\x04 \x01(\t\x12\x0e\n\x06result\x18\x05 \x01(\x05\x12\x10\n\x08reserved\x18\x06 \x01(\t\"6\n\x0e\x63hargePileType\x12\x0e\n\x06toward\x18\x01 \x01(\x05\x12\t\n\x01x\x18\x02 \x01(\x02\x12\t\n\x01y\x18\x03 \x01(\x02\"J\n\x11SimulationCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x10\n\x08param_id\x18\x02 \x01(\x05\x12\x13\n\x0bparam_value\x18\x03 \x03(\x05\"%\n\x13WorkReportUpdateCmd\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\"<\n\x13WorkReportUpdateAck\x12\x13\n\x0bupdate_flag\x18\x01 \x01(\x08\x12\x10\n\x08info_num\x18\x02 \x01(\x05\"7\n\x11WorkReportCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x12\n\ngetInfoNum\x18\x02 \x01(\x05\"\x8e\x02\n\x11WorkReportInfoAck\x12\x16\n\x0einterrupt_flag\x18\x01 \x01(\x08\x12\x17\n\x0fstart_work_time\x18\x02 \x01(\x03\x12\x15\n\rend_work_time\x18\x03 \x01(\x03\x12\x16\n\x0ework_time_used\x18\x04 \x01(\x05\x12\x11\n\twork_ares\x18\x05 \x01(\x01\x12\x15\n\rwork_progress\x18\x06 \x01(\x05\x12\x17\n\x0fheight_of_knife\x18\x07 \x01(\x05\x12\x11\n\twork_type\x18\x08 \x01(\x05\x12\x13\n\x0bwork_result\x18\t \x01(\x05\x12\x15\n\rtotal_ack_num\x18\n \x01(\x05\x12\x17\n\x0f\x63urrent_ack_num\x18\x0b \x01(\x05\"\xb2\x01\n\x19\x61pp_request_cover_paths_t\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06subCmd\x18\x02 \x01(\x05\x12\x12\n\ntotalFrame\x18\x03 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x04 \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\x05 \x01(\x06\x12\x16\n\x0etransaction_id\x18\x06 \x01(\x03\x12\x10\n\x08reserved\x18\x07 \x03(\x03\x12\x11\n\thash_list\x18\x08 \x03(\x06\"\x99\x01\n\x13\x63over_path_packet_t\x12\x11\n\tpath_hash\x18\x01 \x01(\x06\x12\x11\n\tpath_type\x18\x02 \x01(\x05\x12\x12\n\npath_total\x18\x03 \x01(\x05\x12\x10\n\x08path_cur\x18\x04 \x01(\x05\x12\x11\n\tzone_hash\x18\x05 \x01(\x06\x12#\n\ndataCouple\x18\x06 \x03(\x0b\x32\x0f.CommDataCouple\"\xb2\x02\n\x13\x63over_path_upload_t\x12\x0c\n\x04pver\x18\x01 \x01(\x05\x12\x0e\n\x06result\x18\x02 \x01(\x05\x12\x0e\n\x06subCmd\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x04 \x01(\x05\x12\x0c\n\x04time\x18\x05 \x01(\x05\x12\x12\n\ntotalFrame\x18\x06 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x07 \x01(\x05\x12\x16\n\x0etotal_path_num\x18\x08 \x01(\x05\x12\x16\n\x0evaild_path_num\x18\t \x01(\x05\x12\x10\n\x08\x64\x61taHash\x18\n \x01(\x06\x12\x16\n\x0etransaction_id\x18\x0b \x01(\x03\x12\x10\n\x08reserved\x18\x0c \x03(\x03\x12\x0f\n\x07\x64\x61taLen\x18\r \x01(\x05\x12*\n\x0cpath_packets\x18\x0e \x03(\x0b\x32\x14.cover_path_packet_t\"M\n\x14zone_start_precent_t\x12\x10\n\x08\x64\x61taHash\x18\x01 \x01(\x06\x12\t\n\x01x\x18\x02 \x01(\x02\x12\t\n\x01y\x18\x03 \x01(\x02\x12\r\n\x05index\x18\x04 \x01(\x05\",\n\x0fvision_ctrl_msg\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0b\n\x03\x63md\x18\x02 \x01(\x05\"<\n\x11nav_sys_param_msg\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\x05\"Q\n\x15nav_plan_task_execute\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06result\x18\x04 \x01(\x05\"y\n\tcostmap_t\x12\r\n\x05width\x18\x01 \x01(\x05\x12\x0e\n\x06height\x18\x02 \x01(\x05\x12\x10\n\x08\x63\x65nter_x\x18\x03 \x01(\x02\x12\x10\n\x08\x63\x65nter_y\x18\x04 \x01(\x02\x12\x0b\n\x03yaw\x18\x05 \x01(\x02\x12\x0b\n\x03res\x18\x06 \x01(\x02\x12\x0f\n\x07\x63ostmap\x18\x07 \x03(\x05\"/\n\x13plan_task_name_id_t\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"<\n\x15nav_get_all_plan_task\x12#\n\x05tasks\x18\x01 \x03(\x0b\x32\x14.plan_task_name_id_t\"\xfb\x12\n\x07MctlNav\x12$\n\x0ctoapp_lat_up\x18\x01 \x01(\x0b\x32\x0c.NavLatLonUpH\x00\x12!\n\x0ctoapp_pos_up\x18\x02 \x01(\x0b\x32\t.NavPosUpH\x00\x12.\n\x13todev_chl_line_data\x18\x03 \x01(\x0b\x32\x0f.NavCHlLineDataH\x00\x12\'\n\x0ftoapp_task_info\x18\x04 \x01(\x0b\x32\x0c.NavTaskInfoH\x00\x12*\n\x11toapp_opt_line_up\x18\x05 \x01(\x0b\x32\r.NavOptLineUpH\x00\x12\x33\n\x15toapp_opt_border_info\x18\x06 \x01(\x0b\x32\x12.NavOptiBorderInfoH\x00\x12,\n\x12toapp_opt_obs_info\x18\x07 \x01(\x0b\x32\x0e.NavOptObsInfoH\x00\x12+\n\x13todev_task_info_ack\x18\x08 \x01(\x0b\x32\x0c.NavResFrameH\x00\x12\x31\n\x19todev_opt_border_info_ack\x18\t \x01(\x0b\x32\x0c.NavResFrameH\x00\x12.\n\x16todev_opt_obs_info_ack\x18\n \x01(\x0b\x32\x0c.NavResFrameH\x00\x12-\n\x15todev_opt_line_up_ack\x18\x0b \x01(\x0b\x32\x0c.NavResFrameH\x00\x12*\n\x0ftoapp_chgpileto\x18\x0c \x01(\x0b\x32\x0f.chargePileTypeH\x00\x12\x17\n\rtodev_sustask\x18\r \x01(\x05H\x00\x12\x18\n\x0etodev_rechgcmd\x18\x0e \x01(\x05H\x00\x12\x17\n\rtodev_edgecmd\x18\x0f \x01(\x05H\x00\x12\x1b\n\x11todev_draw_border\x18\x10 \x01(\x05H\x00\x12\x1f\n\x15todev_draw_border_end\x18\x11 \x01(\x05H\x00\x12\x18\n\x0etodev_draw_obs\x18\x12 \x01(\x05H\x00\x12\x1c\n\x12todev_draw_obs_end\x18\x13 \x01(\x05H\x00\x12\x18\n\x0etodev_chl_line\x18\x14 \x01(\x05H\x00\x12\x1c\n\x12todev_chl_line_end\x18\x15 \x01(\x05H\x00\x12\x19\n\x0ftodev_save_task\x18\x16 \x01(\x05H\x00\x12\x1d\n\x13todev_cancel_suscmd\x18\x17 \x01(\x05H\x00\x12\x1e\n\x14todev_reset_chg_pile\x18\x18 \x01(\x05H\x00\x12\x1f\n\x15todev_cancel_draw_cmd\x18\x19 \x01(\x05H\x00\x12$\n\x1atodev_one_touch_leave_pile\x18\x1a \x01(\x05H\x00\x12&\n\x0etodev_mow_task\x18\x1b \x01(\x0b\x32\x0c.NavStartJobH\x00\x12\'\n\x0ctoapp_bstate\x18\x1c \x01(\x0b\x32\x0f.NavBorderStateH\x00\x12\x1a\n\x10todev_lat_up_ack\x18\x1d \x01(\x05H\x00\x12(\n\rtodev_gethash\x18\x1e \x01(\x0b\x32\x0f.NavGetHashListH\x00\x12/\n\x11toapp_gethash_ack\x18\x1f \x01(\x0b\x32\x12.NavGetHashListAckH\x00\x12/\n\x14todev_get_commondata\x18  \x01(\x0b\x32\x0f.NavGetCommDataH\x00\x12\x36\n\x18toapp_get_commondata_ack\x18! \x01(\x0b\x32\x12.NavGetCommDataAckH\x00\x12\x31\n\x15\x62idire_reqconver_path\x18\" \x01(\x0b\x32\x10.NavReqCoverPathH\x00\x12.\n\x0ctoapp_zigzag\x18# \x01(\x0b\x32\x16.NavUploadZigZagResultH\x00\x12\x35\n\x10todev_zigzag_ack\x18$ \x01(\x0b\x32\x19.NavUploadZigZagResultAckH\x00\x12&\n\x0etodev_taskctrl\x18% \x01(\x0b\x32\x0c.NavTaskCtrlH\x00\x12%\n\rbidire_taskid\x18& \x01(\x0b\x32\x0c.NavTaskIdRwH\x00\x12&\n\x08toapp_bp\x18\' \x01(\x0b\x32\x12.NavTaskBreakPointH\x00\x12+\n\x11todev_planjob_set\x18( \x01(\x0b\x32\x0e.NavPlanJobSetH\x00\x12\x32\n\x15todev_unable_time_set\x18) \x01(\x0b\x32\x11.NavUnableTimeSetH\x00\x12,\n\x0esimulation_cmd\x18* \x01(\x0b\x32\x12.SimulationCmdDataH\x00\x12<\n\x1ctodev_work_report_update_cmd\x18+ \x01(\x0b\x32\x14.WorkReportUpdateCmdH\x00\x12<\n\x1ctoapp_work_report_update_ack\x18, \x01(\x0b\x32\x14.WorkReportUpdateAckH\x00\x12\x33\n\x15todev_work_report_cmd\x18- \x01(\x0b\x32\x12.WorkReportCmdDataH\x00\x12\x33\n\x15toapp_work_report_ack\x18. \x01(\x0b\x32\x12.WorkReportInfoAckH\x00\x12\x36\n\x18toapp_work_report_upload\x18/ \x01(\x0b\x32\x12.WorkReportInfoAckH\x00\x12=\n\x17\x61pp_request_cover_paths\x18\x30 \x01(\x0b\x32\x1a.app_request_cover_paths_tH\x00\x12\x31\n\x11\x63over_path_upload\x18\x31 \x01(\x0b\x32\x14.cover_path_upload_tH\x00\x12\x33\n\x12zone_start_precent\x18\x32 \x01(\x0b\x32\x15.zone_start_precent_tH\x00\x12\'\n\x0bvision_ctrl\x18\x33 \x01(\x0b\x32\x10.vision_ctrl_msgH\x00\x12/\n\x11nav_sys_param_cmd\x18\x34 \x01(\x0b\x32\x12.nav_sys_param_msgH\x00\x12\x33\n\x11plan_task_execute\x18\x35 \x01(\x0b\x32\x16.nav_plan_task_executeH\x00\x12#\n\rtoapp_costmap\x18\x36 \x01(\x0b\x32\n.costmap_tH\x00\x12\x31\n\x11plan_task_name_id\x18\x37 \x01(\x0b\x32\x14.plan_task_name_id_tH\x00\x12/\n\rall_plan_task\x18\x38 \x01(\x0b\x32\x16.nav_get_all_plan_taskH\x00\x42\x0b\n\tSubNavMsgb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_nav_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _NAVLATLONUP._serialized_start=59
@@ -33,70 +33,84 @@
   _NAVOBSTIBORDERDATAGET._serialized_end=489
   _NAVOBSTIBORDERDATAGETACK._serialized_start=491
   _NAVOBSTIBORDERDATAGETACK._serialized_end=562
   _NAVCHLLINEDATA._serialized_start=564
   _NAVCHLLINEDATA._serialized_end=664
   _NAVCHLLINEDATAACK._serialized_start=666
   _NAVCHLLINEDATAACK._serialized_end=745
-  _NAVBORDERDATAGET._serialized_start=747
-  _NAVBORDERDATAGET._serialized_end=821
-  _NAVTASKINFO._serialized_start=823
-  _NAVTASKINFO._serialized_end=950
+  _NAVTASKINFO._serialized_start=747
+  _NAVTASKINFO._serialized_end=874
+  _NAVBORDERDATAGET._serialized_start=876
+  _NAVBORDERDATAGET._serialized_end=950
   _NAVOPTLINEUP._serialized_start=953
   _NAVOPTLINEUP._serialized_end=1098
   _NAVOPTIBORDERINFO._serialized_start=1100
   _NAVOPTIBORDERINFO._serialized_end=1226
   _NAVOPTOBSINFO._serialized_start=1229
   _NAVOPTOBSINFO._serialized_end=1358
   _NAVSTARTJOB._serialized_start=1361
   _NAVSTARTJOB._serialized_end=1541
-  _NAVGETHASHLIST._serialized_start=1543
-  _NAVGETHASHLIST._serialized_end=1667
-  _NAVGETHASHLISTACK._serialized_start=1670
-  _NAVGETHASHLISTACK._serialized_end=1834
-  _NAVGETCOMMDATA._serialized_start=1837
-  _NAVGETCOMMDATA._serialized_end=2051
-  _NAVGETCOMMDATAACK._serialized_start=2054
-  _NAVGETCOMMDATAACK._serialized_end=2341
-  _NAVREQCOVERPATH._serialized_start=2344
-  _NAVREQCOVERPATH._serialized_end=2642
-  _NAVUPLOADZIGZAGRESULT._serialized_start=2645
-  _NAVUPLOADZIGZAGRESULT._serialized_end=3068
-  _NAVUPLOADZIGZAGRESULTACK._serialized_start=3071
-  _NAVUPLOADZIGZAGRESULTACK._serialized_end=3247
-  _NAVTASKCTRL._serialized_start=3249
-  _NAVTASKCTRL._serialized_end=3326
-  _NAVTASKIDRW._serialized_start=3328
-  _NAVTASKIDRW._serialized_end=3439
-  _NAVSYSHASHOVERVIEW._serialized_start=3441
-  _NAVSYSHASHOVERVIEW._serialized_end=3515
-  _NAVTASKBREAKPOINT._serialized_start=3517
-  _NAVTASKBREAKPOINT._serialized_end=3622
-  _NAVPLANJOBSET._serialized_start=3625
-  _NAVPLANJOBSET._serialized_end=4171
-  _NAVRESFRAME._serialized_start=4173
-  _NAVRESFRAME._serialized_end=4203
-  _NAVTASKPROGRESS._serialized_start=4205
-  _NAVTASKPROGRESS._serialized_end=4244
-  _NAVUNABLETIMESET._serialized_start=4247
-  _NAVUNABLETIMESET._serialized_end=4381
-  _SIMULATIONCMDDATA._serialized_start=4383
-  _SIMULATIONCMDDATA._serialized_end=4455
-  _WORKREPORTCMDDATA._serialized_start=4457
-  _WORKREPORTCMDDATA._serialized_end=4512
-  _WORKREPORTINFOACK._serialized_start=4515
-  _WORKREPORTINFOACK._serialized_end=4768
-  _WORKREPORTUPDATEACK._serialized_start=4770
-  _WORKREPORTUPDATEACK._serialized_end=4828
-  _WORKREPORTUPDATECMD._serialized_start=4830
-  _WORKREPORTUPDATECMD._serialized_end=4867
-  _CHARGEPILETYPE._serialized_start=4869
-  _CHARGEPILETYPE._serialized_end=4923
-  _APPREQUESTCOVERPATHS._serialized_start=4926
-  _APPREQUESTCOVERPATHS._serialized_end=5097
-  _COVERPATHPACKET._serialized_start=5100
-  _COVERPATHPACKET._serialized_end=5244
-  _COVERPATHUPLOAD._serialized_start=5247
-  _COVERPATHUPLOAD._serialized_end=5539
-  _MCTLNAV._serialized_start=5542
-  _MCTLNAV._serialized_end=7631
+  _NAVTASKPROGRESS._serialized_start=1543
+  _NAVTASKPROGRESS._serialized_end=1582
+  _NAVRESFRAME._serialized_start=1584
+  _NAVRESFRAME._serialized_end=1614
+  _NAVGETHASHLIST._serialized_start=1616
+  _NAVGETHASHLIST._serialized_end=1740
+  _NAVGETHASHLISTACK._serialized_start=1743
+  _NAVGETHASHLISTACK._serialized_end=1923
+  _NAVGETCOMMDATA._serialized_start=1926
+  _NAVGETCOMMDATA._serialized_end=2140
+  _NAVGETCOMMDATAACK._serialized_start=2143
+  _NAVGETCOMMDATAACK._serialized_end=2430
+  _NAVREQCOVERPATH._serialized_start=2433
+  _NAVREQCOVERPATH._serialized_end=2783
+  _NAVUPLOADZIGZAGRESULT._serialized_start=2786
+  _NAVUPLOADZIGZAGRESULT._serialized_end=3209
+  _NAVUPLOADZIGZAGRESULTACK._serialized_start=3212
+  _NAVUPLOADZIGZAGRESULTACK._serialized_end=3388
+  _NAVTASKCTRL._serialized_start=3390
+  _NAVTASKCTRL._serialized_end=3467
+  _NAVTASKIDRW._serialized_start=3469
+  _NAVTASKIDRW._serialized_end=3580
+  _NAVSYSHASHOVERVIEW._serialized_start=3582
+  _NAVSYSHASHOVERVIEW._serialized_end=3656
+  _NAVTASKBREAKPOINT._serialized_start=3658
+  _NAVTASKBREAKPOINT._serialized_end=3763
+  _NAVPLANJOBSET._serialized_start=3766
+  _NAVPLANJOBSET._serialized_end=4472
+  _NAVUNABLETIMESET._serialized_start=4475
+  _NAVUNABLETIMESET._serialized_end=4609
+  _CHARGEPILETYPE._serialized_start=4611
+  _CHARGEPILETYPE._serialized_end=4665
+  _SIMULATIONCMDDATA._serialized_start=4667
+  _SIMULATIONCMDDATA._serialized_end=4741
+  _WORKREPORTUPDATECMD._serialized_start=4743
+  _WORKREPORTUPDATECMD._serialized_end=4780
+  _WORKREPORTUPDATEACK._serialized_start=4782
+  _WORKREPORTUPDATEACK._serialized_end=4842
+  _WORKREPORTCMDDATA._serialized_start=4844
+  _WORKREPORTCMDDATA._serialized_end=4899
+  _WORKREPORTINFOACK._serialized_start=4902
+  _WORKREPORTINFOACK._serialized_end=5172
+  _APP_REQUEST_COVER_PATHS_T._serialized_start=5175
+  _APP_REQUEST_COVER_PATHS_T._serialized_end=5353
+  _COVER_PATH_PACKET_T._serialized_start=5356
+  _COVER_PATH_PACKET_T._serialized_end=5509
+  _COVER_PATH_UPLOAD_T._serialized_start=5512
+  _COVER_PATH_UPLOAD_T._serialized_end=5818
+  _ZONE_START_PRECENT_T._serialized_start=5820
+  _ZONE_START_PRECENT_T._serialized_end=5897
+  _VISION_CTRL_MSG._serialized_start=5899
+  _VISION_CTRL_MSG._serialized_end=5943
+  _NAV_SYS_PARAM_MSG._serialized_start=5945
+  _NAV_SYS_PARAM_MSG._serialized_end=6005
+  _NAV_PLAN_TASK_EXECUTE._serialized_start=6007
+  _NAV_PLAN_TASK_EXECUTE._serialized_end=6088
+  _COSTMAP_T._serialized_start=6090
+  _COSTMAP_T._serialized_end=6211
+  _PLAN_TASK_NAME_ID_T._serialized_start=6213
+  _PLAN_TASK_NAME_ID_T._serialized_end=6260
+  _NAV_GET_ALL_PLAN_TASK._serialized_start=6262
+  _NAV_GET_ALL_PLAN_TASK._serialized_end=6322
+  _MCTLNAV._serialized_start=6325
+  _MCTLNAV._serialized_end=8752
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.5/pyluba/proto/mctrl_ota_pb2.py` & `pyluba-0.0.6/pyluba/proto/mctrl_ota_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_ota.proto\"f\n\x08\x42\x61seInfo\x12\x12\n\ndevVersion\x18\x01 \x01(\t\x12\x11\n\tdevStatus\x18\x02 \x01(\x05\x12\x0f\n\x07\x62\x61ttVal\x18\x03 \x01(\x05\x12\x12\n\ninitStatus\x18\x04 \x01(\x05\x12\x0e\n\x06isTilt\x18\x05 \x01(\x05\"\\\n\x07OtaInfo\x12\r\n\x05otaid\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08progress\x18\x03 \x01(\x05\x12\x0e\n\x06result\x18\x04 \x01(\x05\x12\x0f\n\x07message\x18\x05 \x01(\t\"\x1f\n\x0fToDevGetInfoReq\x12\x0c\n\x04type\x18\x01 \x01(\x05\"\xb7\x01\n\x0fToAppGetInfoRsp\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.ToAppGetInfoRsp.InfoCase\x12\x19\n\x04\x62\x61se\x18\x03 \x01(\x0b\x32\t.BaseInfoH\x00\x12\x17\n\x03ota\x18\x04 \x01(\x0b\x32\x08.OtaInfoH\x00\"/\n\x08InfoCase\x12\x08\n\x04\x42\x41SE\x10\x00\x12\x07\n\x03OTA\x10\x01\x12\x10\n\x0cINFO_NOT_SET\x10\x02\x42\x06\n\x04info\"y\n\x08MctrlOta\x12/\n\x13to_dev_get_info_req\x18\x01 \x01(\x0b\x32\x10.ToDevGetInfoReqH\x00\x12/\n\x13to_app_get_info_rsp\x18\x02 \x01(\x0b\x32\x10.ToAppGetInfoRspH\x00\x42\x0b\n\tSubOtaMsgb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_ota.proto\"k\n\x08\x62\x61seInfo\x12\x13\n\x0b\x64\x65v_version\x18\x01 \x01(\t\x12\x12\n\ndev_status\x18\x02 \x01(\x05\x12\x10\n\x08\x62\x61tt_val\x18\x03 \x01(\x05\x12\x13\n\x0binit_status\x18\x04 \x01(\x05\x12\x0f\n\x07is_tilt\x18\x05 \x01(\x05\"\\\n\x07otaInfo\x12\r\n\x05otaid\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08progress\x18\x03 \x01(\x05\x12\x0e\n\x06result\x18\x04 \x01(\x05\x12\x0f\n\x07message\x18\x05 \x01(\t\"%\n\ngetInfoReq\x12\x17\n\x04type\x18\x01 \x01(\x0e\x32\t.infoType\"q\n\ngetInfoRsp\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x17\n\x04type\x18\x02 \x01(\x0e\x32\t.infoType\x12\x19\n\x04\x62\x61se\x18\x03 \x01(\x0b\x32\t.baseInfoH\x00\x12\x17\n\x03ota\x18\x04 \x01(\x0b\x32\x08.otaInfoH\x00\x42\x06\n\x04info\"l\n\x07MctlOta\x12)\n\x12todev_get_info_req\x18\x01 \x01(\x0b\x32\x0b.getInfoReqH\x00\x12)\n\x12toapp_get_info_rsp\x18\x02 \x01(\x0b\x32\x0b.getInfoRspH\x00\x42\x0b\n\tSubOtaMsg*#\n\x08infoType\x12\x0b\n\x07IT_BASE\x10\x00\x12\n\n\x06IT_OTA\x10\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_ota_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  _INFOTYPE._serialized_start=499
+  _INFOTYPE._serialized_end=534
   _BASEINFO._serialized_start=32
-  _BASEINFO._serialized_end=134
-  _OTAINFO._serialized_start=136
-  _OTAINFO._serialized_end=228
-  _TODEVGETINFOREQ._serialized_start=230
-  _TODEVGETINFOREQ._serialized_end=261
-  _TOAPPGETINFORSP._serialized_start=264
-  _TOAPPGETINFORSP._serialized_end=447
-  _TOAPPGETINFORSP_INFOCASE._serialized_start=392
-  _TOAPPGETINFORSP_INFOCASE._serialized_end=439
-  _MCTRLOTA._serialized_start=449
-  _MCTRLOTA._serialized_end=570
+  _BASEINFO._serialized_end=139
+  _OTAINFO._serialized_start=141
+  _OTAINFO._serialized_end=233
+  _GETINFOREQ._serialized_start=235
+  _GETINFOREQ._serialized_end=272
+  _GETINFORSP._serialized_start=274
+  _GETINFORSP._serialized_end=387
+  _MCTLOTA._serialized_start=389
+  _MCTLOTA._serialized_end=497
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.5/pyluba/proto/mctrl_sys_pb2.py` & `pyluba-0.0.6/pyluba/proto/mctrl_sys_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,125 +10,133 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from pyluba.proto import dev_net_pb2 as pyluba_dot_proto_dot_dev__net__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_sys.proto\x1a\x1apyluba/proto/dev_net.proto\"\x98\x0c\n\x07MctlSys\x12\"\n\rtoapp_batinfo\x18\x01 \x01(\x0b\x32\t.SysBatUpH\x00\x12)\n\x10toapp_work_state\x18\x02 \x01(\x0b\x32\r.SysWorkStateH\x00\x12*\n\x0ftodev_time_zone\x18\x03 \x01(\x0b\x32\x0f.SysSetTimeZoneH\x00\x12*\n\x0ftodev_data_time\x18\x04 \x01(\x0b\x32\x0f.SysSetDateTimeH\x00\x12\x1f\n\x08job_plan\x18\x06 \x01(\x0b\x32\x0b.SysJobPlanH\x00\x12(\n\x0etoapp_err_code\x18\x07 \x01(\x0b\x32\x0e.SysDevErrCodeH\x00\x12.\n\x13todev_job_plan_time\x18\n \x01(\x0b\x32\x0f.SysJobPlanTimeH\x00\x12%\n\x0etoapp_mow_info\x18\x0b \x01(\x0b\x32\x0b.SysMowInfoH\x00\x12&\n\x0f\x62idire_comm_cmd\x18\x0c \x01(\x0b\x32\x0b.SysCommCmdH\x00\x12\x16\n\x0cplan_job_del\x18\x0e \x01(\x03H\x00\x12\x1c\n\x06\x62order\x18\x0f \x01(\x0b\x32\n.SysBorderH\x00\x12.\n\x11toapp_plan_status\x18\x12 \x01(\x0b\x32\x11.SysPlanJobStatusH\x00\x12\x34\n\x12toapp_ul_fprogress\x18\x13 \x01(\x0b\x32\x16.SysUploadFileProgressH\x00\x12*\n\x10todev_deljobplan\x18\x14 \x01(\x0b\x32\x0e.SysDelJobPlanH\x00\x12\x1b\n\x11todev_mow_info_up\x18\x15 \x01(\x05H\x00\x12,\n\x10todev_knife_ctrl\x18\x16 \x01(\x0b\x32\x10.SysKnifeControlH\x00\x12\x1c\n\x12todev_reset_system\x18\x17 \x01(\x05H\x00\x12:\n\x19todev_reset_system_status\x18\x18 \x01(\x0b\x32\x15.SysResetSystemStatusH\x00\x12@\n\x19system_rapid_state_tunnel\x18\x19 \x01(\x0b\x32\x1b.systemRapidStateTunnel_msgH\x00\x12>\n\x18system_tard_state_tunnel\x18\x1a \x01(\x0b\x32\x1a.systemTardStateTunnel_msgH\x00\x12\x31\n\x11system_update_buf\x18\x1b \x01(\x0b\x32\x14.systemUpdateBuf_msgH\x00\x12/\n\x15todev_time_ctrl_light\x18\x1c \x01(\x0b\x32\x0e.TimeCtrlLightH\x00\x12\x34\n\x13system_tmp_cycle_tx\x18\x1d \x01(\x0b\x32\x15.systemTmpCycleTx_msgH\x00\x12\x30\n\x14todev_off_chip_flash\x18\x1e \x01(\x0b\x32\x10.SysOffChipFlashH\x00\x12\x1f\n\x15todev_get_dev_fw_info\x18\x1f \x01(\x05H\x00\x12,\n\x11toapp_dev_fw_info\x18  \x01(\x0b\x32\x0f.device_fw_infoH\x00\x12)\n\x12todev_lora_cfg_req\x18! \x01(\x0b\x32\x0b.LoraCfgReqH\x00\x12)\n\x12toapp_lora_cfg_rsp\x18\" \x01(\x0b\x32\x0b.LoraCfgRspH\x00\x12-\n\x0fmow_to_app_info\x18# \x01(\x0b\x32\x12.mow_to_app_info_tH\x00\x12:\n\x18\x64\x65vice_product_type_info\x18$ \x01(\x0b\x32\x16.DeviceProductTypeInfoH\x00\x12\x37\n\x17mow_to_app_qctools_info\x18% \x01(\x0b\x32\x14.MowToAppQCToolsInfoH\x00\x12*\n\x10todev_report_cfg\x18& \x01(\x0b\x32\x0e.ReportInfoCfgH\x00\x12,\n\x11toapp_report_data\x18\' \x01(\x0b\x32\x0f.ReportInfoDataH\x00\x12\x31\n\x0esimulation_cmd\x18* \x01(\x0b\x32\x17.MCtrlSimulationCmdDataH\x00\x42\x0b\n\tsubSysMsg\"M\n\x16MCtrlSimulationCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x0f\n\x07paramId\x18\x02 \x01(\x05\x12\x12\n\nparamValue\x18\x03 \x03(\x05\";\n\x0fSysKnifeControl\x12\x13\n\x0bknifeStatus\x18\x01 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x02 \x01(\x05\"\x1a\n\x08SysBatUp\x12\x0e\n\x06\x62\x61tVal\x18\x01 \x01(\x05\"Z\n\x0cSysWorkState\x12\x13\n\x0b\x64\x65viceState\x18\x01 \x01(\x05\x12\x13\n\x0b\x63hargeState\x18\x02 \x01(\x05\x12\x0e\n\x06\x63mHash\x18\x03 \x01(\x03\x12\x10\n\x08pathHash\x18\x04 \x01(\x03\"5\n\x0eSysSetTimeZone\x12\x11\n\ttimeStamp\x18\x01 \x01(\x05\x12\x10\n\x08timeArea\x18\x02 \x01(\x05\"\x9e\x01\n\x0eSysSetDateTime\x12\x0c\n\x04year\x18\x01 \x01(\x05\x12\r\n\x05month\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61te\x18\x03 \x01(\x05\x12\x0c\n\x04week\x18\x04 \x01(\x05\x12\r\n\x05hours\x18\x05 \x01(\x05\x12\x0f\n\x07minutes\x18\x06 \x01(\x05\x12\x0f\n\x07seconds\x18\x07 \x01(\x05\x12\x10\n\x08timezone\x18\x08 \x01(\x05\x12\x10\n\x08\x64\x61ylight\x18\t \x01(\x05\"V\n\nSysJobPlan\x12\r\n\x05jobId\x18\x01 \x01(\x03\x12\x0f\n\x07jobMode\x18\x02 \x01(\x05\x12\x13\n\x0brainTactics\x18\x03 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x04 \x01(\x05\"\"\n\rSysDevErrCode\x12\x11\n\terrorCode\x18\x01 \x01(\x05\"!\n\x0cSysBoardType\x12\x11\n\tboardType\x18\x01 \x01(\x05\"5\n\x0cSysSwVersion\x12\x11\n\tboardType\x18\x01 \x01(\x05\x12\x12\n\nversionLen\x18\x02 \x01(\x05\"1\n\rSysDelJobPlan\x12\x10\n\x08\x64\x65viceId\x18\x01 \x01(\t\x12\x0e\n\x06planId\x18\x02 \x01(\t\"\xe1\x01\n\x0eSysJobPlanTime\x12\x0e\n\x06planId\x18\x01 \x01(\x03\x12\x14\n\x0cstartJobTime\x18\x02 \x01(\x05\x12\x12\n\nendJobTime\x18\x03 \x01(\x05\x12\x11\n\ttimeInDay\x18\x04 \x01(\x05\x12\x13\n\x0bjobPlanMode\x18\x05 \x01(\x05\x12\x15\n\rjobPlanEnable\x18\x06 \x01(\x05\x12\x1c\n\x07jobPlan\x18\n \x01(\x0b\x32\x0b.SysJobPlan\x12\x0f\n\x07weekDay\x18\x07 \x03(\x05\x12\x15\n\rtimeInWeekDay\x18\x08 \x01(\x05\x12\x10\n\x08\x65veryday\x18\t \x01(\x05\"k\n\nSysMowInfo\x12\x13\n\x0b\x64\x65viceState\x18\x01 \x01(\x05\x12\x0e\n\x06\x62\x61tVal\x18\x02 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x03 \x01(\x05\x12\x11\n\trTKstatus\x18\x04 \x01(\x05\x12\x10\n\x08rTKstars\x18\x05 \x01(\x05\";\n\x0eSysOptiLineAck\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\x12\x13\n\x0bresponesCmd\x18\x01 \x01(\x05\"5\n\nSysCommCmd\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\x05\"H\n\x15SysUploadFileProgress\x12\r\n\x05\x62izId\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\x05\x12\x10\n\x08progress\x18\x03 \x01(\x05\"\x1e\n\x0cSysErrorCode\x12\x0e\n\x06\x63odeNo\x18\x01 \x01(\x05\"\x1e\n\tSysBorder\x12\x11\n\tborderval\x18\x01 \x01(\x05\")\n\x10SysPlanJobStatus\x12\x15\n\rplanjobStatus\x18\x01 \x01(\x05\"*\n\x14SysResetSystemStatus\x12\x12\n\nresetStaus\x18\x01 \x01(\x05\"\x8a\x01\n\rTimeCtrlLight\x12\x0f\n\x07operate\x18\x01 \x01(\x05\x12\x0e\n\x06\x65nable\x18\x02 \x01(\x05\x12\x12\n\nstart_hour\x18\x03 \x01(\x05\x12\x10\n\x08\x65nd_hour\x18\x05 \x01(\x05\x12\x11\n\tstart_min\x18\x04 \x01(\x05\x12\x0f\n\x07\x65nd_min\x18\x06 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x07 \x01(\x05\"6\n\x1asystemRapidStateTunnel_msg\x12\x18\n\x10rapid_state_data\x18\x01 \x03(\x03\"4\n\x19systemTardStateTunnel_msg\x12\x17\n\x0ftard_state_data\x18\x01 \x03(\x03\".\n\x13systemUpdateBuf_msg\x12\x17\n\x0fupdate_buf_data\x18\x01 \x03(\x03\"\x86\x01\n\x0fSysOffChipFlash\x12\n\n\x02op\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x12\n\nstart_addr\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\x04 \x01(\x05\x12\x0e\n\x06length\x18\x05 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x0c\n\x04\x63ode\x18\x07 \x01(\x05\x12\x0b\n\x03msg\x18\x08 \x01(\t\"-\n\x14systemTmpCycleTx_msg\x12\x15\n\rcycle_tx_data\x18\x01 \x03(\x03\"&\n\nLoraCfgReq\x12\x0b\n\x03op_\x18\x01 \x01(\x05\x12\x0b\n\x03\x63\x66g\x18\x02 \x01(\t\"F\n\nLoraCfgRsp\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\n\n\x02op\x18\x02 \x01(\x05\x12\x0b\n\x03\x63\x66g\x18\x03 \x01(\t\x12\x0f\n\x07\x66\x61\x63_cfg\x18\x04 \x01(\t\">\n\x0bmod_fw_info\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x10\n\x08identify\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"L\n\x0e\x64\x65vice_fw_info\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x03mod\x18\x03 \x03(\x0b\x32\x0c.mod_fw_info\"@\n\x11mow_to_app_info_t\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0b\n\x03\x63md\x18\x02 \x01(\x05\x12\x10\n\x08mow_data\x18\x03 \x03(\x05\"\x98\x01\n\x10RptConnectStatus\x12\x14\n\x0c\x63onnect_type\x18\x01 \x01(\x05\x12\x10\n\x08\x62le_rssi\x18\x02 \x01(\x05\x12\x11\n\twifi_rssi\x18\x03 \x01(\x05\x12\x11\n\tlink_type\x18\x04 \x01(\x05\x12\x11\n\tmnet_rssi\x18\x05 \x01(\x05\x12\x11\n\tmnet_inet\x18\x06 \x01(\x05\x12\x10\n\x08used_net\x18\x07 \x01(\x05\"\x9f\x03\n\x07RptWork\x12\x0c\n\x04plan\x18\x01 \x01(\x05\x12\x11\n\tpath_hash\x18\x02 \x01(\x03\x12\x10\n\x08progress\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x04 \x01(\x05\x12\x0f\n\x07\x62p_info\x18\x05 \x01(\x05\x12\x0f\n\x07\x62p_hash\x18\x06 \x01(\x03\x12\x10\n\x08\x62p_pos_x\x18\x07 \x01(\x05\x12\x10\n\x08\x62p_pos_y\x18\x08 \x01(\x05\x12\x15\n\rreal_path_num\x18\t \x01(\x03\x12\x12\n\npath_pos_x\x18\n \x01(\x05\x12\x12\n\npath_pos_y\x18\x0b \x01(\x05\x12\x14\n\x0cub_zone_hash\x18\x0c \x01(\x03\x12\x14\n\x0cub_path_hash\x18\r \x01(\x03\x12\x15\n\rinit_cfg_hash\x18\x0e \x01(\x03\x12\x15\n\rub_ecode_hash\x18\x0f \x01(\x03\x12\x14\n\x0cnav_run_mode\x18\x10 \x01(\x05\x12\x18\n\x10test_mode_status\x18\x11 \x01(\x03\x12\x15\n\rman_run_speed\x18\x12 \x01(\x05\x12\x17\n\x0fnav_edit_status\x18\x13 \x01(\x05\x12\x14\n\x0cknife_height\x18\x14 \x01(\x05\"E\n\x0bRptMaintain\x12\x0f\n\x07mileage\x18\x01 \x01(\x03\x12\x11\n\twork_time\x18\x02 \x01(\x05\x12\x12\n\nbat_cycles\x18\x03 \x01(\x05\"\x84\x01\n\x0eRptDevLocation\x12\x12\n\nreal_pos_x\x18\x01 \x01(\x03\x12\x12\n\nreal_pos_y\x18\x02 \x01(\x03\x12\x13\n\x0breal_toward\x18\x03 \x01(\x05\x12\x10\n\x08pos_type\x18\x04 \x01(\x05\x12\x11\n\tzone_hash\x18\x05 \x01(\x03\x12\x10\n\x08\x62ol_hash\x18\x06 \x01(\x03\"8\n\x0f\x43ollectorStatus\x12%\n\x1d\x63ollector_installation_status\x18\x01 \x01(\x05\"0\n\x0fVioSurvivalInfo\x12\x1d\n\x15vio_survival_distance\x18\x01 \x01(\x02\"\x9e\x02\n\x0cRptDevStatus\x12\x12\n\nsys_status\x18\x01 \x01(\x05\x12\x14\n\x0c\x63harge_state\x18\x02 \x01(\x05\x12\x13\n\x0b\x62\x61ttery_val\x18\x03 \x01(\x05\x12\x15\n\rsensor_status\x18\x04 \x01(\x05\x12\x13\n\x0blast_status\x18\x05 \x01(\x05\x12\x16\n\x0esys_time_stamp\x18\x06 \x01(\x03\x12\x14\n\x0cvslam_status\x18\x07 \x01(\x05\x12\x1c\n\tmnet_info\x18\x08 \x01(\x0b\x32\t.MnetInfo\x12*\n\x10\x63ollector_status\x18\n \x01(\x0b\x32\x10.CollectorStatus\x12+\n\x11vio_survival_info\x18\t \x01(\x0b\x32\x10.VioSurvivalInfo\"\x8e\x01\n\x07RptLora\x12\x16\n\x0epair_code_scan\x18\x01 \x01(\x05\x12\x19\n\x11pair_code_channel\x18\x02 \x01(\x05\x12\x17\n\x0fpair_code_locid\x18\x03 \x01(\x05\x12\x17\n\x0fpair_code_netid\x18\x04 \x01(\x05\x12\x1e\n\x16lora_connection_status\x18\x05 \x01(\x05\"\xef\x01\n\x06RptRtk\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x11\n\tpos_level\x18\x02 \x01(\x05\x12\x11\n\tgps_stars\x18\x03 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x04 \x01(\x05\x12\x0f\n\x07lat_std\x18\x05 \x01(\x05\x12\x0f\n\x07lon_std\x18\x06 \x01(\x05\x12\x10\n\x08l2_stars\x18\x07 \x01(\x05\x12\x12\n\ndis_status\x18\x08 \x01(\x03\x12\x17\n\x0ftop4_total_mean\x18\t \x01(\x05\x12\x15\n\rco_view_stars\x18\n \x01(\x05\x12\r\n\x05reset\x18\x0b \x01(\x05\x12\x1b\n\tlora_info\x18\x0c \x01(\x0b\x32\x08.RptLora\"\x96\x01\n\x0fVioToAppInfoMsg\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x12\x0f\n\x07heading\x18\x03 \x01(\x01\x12\x11\n\tvio_state\x18\x04 \x01(\x05\x12\x12\n\nbrightness\x18\x05 \x01(\x05\x12\x1a\n\x12\x64\x65tect_feature_num\x18\x06 \x01(\x05\x12\x19\n\x11track_feature_num\x18\x07 \x01(\x05\"1\n\x0eVisionPointMsg\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"W\n\x12VisionPointInfoMsg\x12\r\n\x05label\x18\x01 \x01(\x05\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12%\n\x0cvision_point\x18\x03 \x03(\x0b\x32\x0f.VisionPointMsg\"/\n\x12VisionStatisticMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x02\x12\x0b\n\x03var\x18\x02 \x01(\x02\"h\n\x16VisionStatisticInfoMsg\x12\x11\n\ttimestamp\x18\x01 \x01(\x01\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12.\n\x11vision_statistics\x18\x03 \x03(\x0b\x32\x13.VisionStatisticMsg\"\xf7\x02\n\x0eReportInfoData\x12\"\n\x07\x63onnect\x18\x01 \x01(\x0b\x32\x11.RptConnectStatus\x12\x1a\n\x03\x64\x65v\x18\x02 \x01(\x0b\x32\r.RptDevStatus\x12 \n\x07\x66w_info\x18\x06 \x01(\x0b\x32\x0f.device_fw_info\x12\"\n\tlocations\x18\x04 \x03(\x0b\x32\x0f.RptDevLocation\x12\x1e\n\x08maintain\x18\x07 \x01(\x0b\x32\x0c.RptMaintain\x12\x14\n\x03rtk\x18\x03 \x01(\x0b\x32\x07.RptRtk\x12)\n\x0fvio_to_app_info\x18\t \x01(\x0b\x32\x10.VioToAppInfoMsg\x12.\n\x11vision_point_info\x18\x08 \x03(\x0b\x32\x13.VisionPointInfoMsg\x12\x36\n\x15vision_statistic_info\x18\n \x01(\x0b\x32\x17.VisionStatisticInfoMsg\x12\x16\n\x04work\x18\x05 \x01(\x0b\x32\x08.RptWork\"\\\n\x15\x44\x65viceProductTypeInfo\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x19\n\x11main_product_type\x18\x02 \x01(\t\x12\x18\n\x10sub_product_type\x18\x03 \x01(\t\"\x81\x01\n\rReportInfoCfg\x12\x0b\n\x03\x61\x63t\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x0e\n\x06period\x18\x03 \x01(\x05\x12\x18\n\x10no_change_period\x18\x04 \x01(\x05\x12\r\n\x05\x63ount\x18\x05 \x01(\x05\x12\x19\n\x03sub\x18\x06 \x03(\x0e\x32\x0c.RptInfoType\"\x87\x01\n\x13MowToAppQCToolsInfo\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x18\n\x10time_of_duration\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x16\n\x0eresult_details\x18\x04 \x01(\t\x12 \n\x06\x65xcept\x18\x05 \x03(\x0b\x32\x10.QCAppTestExcept\"P\n\x0fQCAppTestExcept\x12\x13\n\x0b\x65xcept_type\x18\x01 \x01(\t\x12(\n\nconditions\x18\x02 \x03(\x0b\x32\x14.QCAppTestConditions\"t\n\x13QCAppTestConditions\x12\x11\n\tcond_type\x18\x01 \x01(\t\x12\x0f\n\x07int_val\x18\x02 \x01(\x05\x12\x11\n\tfloat_val\x18\x03 \x01(\x02\x12\x12\n\ndouble_val\x18\x04 \x01(\x01\x12\x12\n\nstring_val\x18\x05 \x01(\t*+\n\tOperation\x12\t\n\x05WRITE\x10\x00\x12\x08\n\x04READ\x10\x01\x12\t\n\x05\x45RASE\x10\x02*\x8d\x02\n\tOffPartId\x12\x13\n\x0fOFF_PART_DL_IMG\x10\x00\x12\x19\n\x15OFF_PART_UPDINFO_BACK\x10\x01\x12\x14\n\x10OFF_PART_UPDINFO\x10\x02\x12\x13\n\x0fOFF_PART_NAKEDB\x10\x03\x12\x14\n\x10OFF_PART_FLASHDB\x10\x04\x12\x18\n\x14OFF_PART_UPD_APP_IMG\x10\x05\x12\x18\n\x14OFF_PART_UPD_BMS_IMG\x10\x06\x12\x18\n\x14OFF_PART_UPD_TMP_IMG\x10\x07\x12\x15\n\x11OFF_PART_DEV_INFO\x10\x08\x12\x18\n\x14OFF_PART_NAKEDB_BACK\x10\t\x12\x10\n\x0cOFF_PART_MAX\x10\n*\xbd\x01\n\x0bRptInfoType\x12\x0f\n\x0bRIT_CONNECT\x10\x00\x12\x0f\n\x0bRIT_DEV_STA\x10\x01\x12\x0b\n\x07RIT_RTK\x10\x02\x12\x11\n\rRIT_DEV_LOCAL\x10\x03\x12\x0c\n\x08RIT_WORK\x10\x04\x12\x0f\n\x0bRIT_FW_INFO\x10\x05\x12\x10\n\x0cRIT_MAINTAIN\x10\x06\x12\x14\n\x10RIT_VISION_POINT\x10\x07\x12\x0b\n\x07RIT_VIO\x10\x08\x12\x18\n\x14RIT_VISION_STATISTIC\x10\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cpyluba/proto/mctrl_sys.proto\x1a\x1apyluba/proto/dev_net.proto\"\x1a\n\x08SysBatUp\x12\x0e\n\x06\x62\x61tVal\x18\x01 \x01(\x05\"Z\n\x0cSysWorkState\x12\x13\n\x0b\x64\x65viceState\x18\x01 \x01(\x05\x12\x13\n\x0b\x63hargeState\x18\x02 \x01(\x05\x12\x0e\n\x06\x63mHash\x18\x03 \x01(\x03\x12\x10\n\x08pathHash\x18\x04 \x01(\x03\"5\n\x0eSysSetTimeZone\x12\x11\n\ttimeStamp\x18\x01 \x01(\x05\x12\x10\n\x08timeArea\x18\x02 \x01(\x05\"\x9e\x01\n\x0eSysSetDateTime\x12\x0c\n\x04Year\x18\x01 \x01(\x05\x12\r\n\x05Month\x18\x02 \x01(\x05\x12\x0c\n\x04\x44\x61te\x18\x03 \x01(\x05\x12\x0c\n\x04Week\x18\x04 \x01(\x05\x12\r\n\x05Hours\x18\x05 \x01(\x05\x12\x0f\n\x07Minutes\x18\x06 \x01(\x05\x12\x0f\n\x07Seconds\x18\x07 \x01(\x05\x12\x10\n\x08timeZone\x18\x08 \x01(\x05\x12\x10\n\x08\x64\x61ylight\x18\t \x01(\x05\"V\n\nSysJobPlan\x12\r\n\x05jobId\x18\x01 \x01(\x03\x12\x0f\n\x07jobMode\x18\x02 \x01(\x05\x12\x13\n\x0brainTactics\x18\x03 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x04 \x01(\x05\"\"\n\rSysDevErrCode\x12\x11\n\terrorCode\x18\x01 \x01(\x05\"!\n\x0cSysBoardType\x12\x11\n\tboardType\x18\x01 \x01(\x05\"5\n\x0cSysSwVersion\x12\x11\n\tboardType\x18\x01 \x01(\x05\x12\x12\n\nversionLen\x18\x02 \x01(\x05\"1\n\rSysDelJobPlan\x12\x10\n\x08\x64\x65viceId\x18\x01 \x01(\t\x12\x0e\n\x06planId\x18\x02 \x01(\t\"\xec\x01\n\x0eSysJobPlanTime\x12\x0e\n\x06planId\x18\x01 \x01(\x03\x12\x16\n\x0estart_job_time\x18\x02 \x01(\x05\x12\x14\n\x0c\x65nd_job_time\x18\x03 \x01(\x05\x12\x13\n\x0btime_in_day\x18\x04 \x01(\x05\x12\x15\n\rjob_plan_mode\x18\x05 \x01(\x05\x12\x17\n\x0fjob_plan_enable\x18\x06 \x01(\x05\x12\x0f\n\x07weekDay\x18\x07 \x03(\x05\x12\x15\n\rtimeInWeekDay\x18\x08 \x03(\x05\x12\x10\n\x08\x65veryDay\x18\t \x01(\x05\x12\x1d\n\x08job_plan\x18\n \x01(\x0b\x32\x0b.SysJobPlan\"k\n\nSysMowInfo\x12\x13\n\x0b\x64\x65viceState\x18\x01 \x01(\x05\x12\x0e\n\x06\x62\x61tVal\x18\x02 \x01(\x05\x12\x13\n\x0bknifeHeight\x18\x03 \x01(\x05\x12\x11\n\tRTKstatus\x18\x04 \x01(\x05\x12\x10\n\x08RTKstars\x18\x05 \x01(\x05\";\n\x0eSysOptiLineAck\x12\x13\n\x0bresponesCmd\x18\x01 \x01(\x05\x12\x14\n\x0c\x63urrentFrame\x18\x02 \x01(\x05\"5\n\nSysCommCmd\x12\n\n\x02rw\x18\x01 \x01(\x05\x12\n\n\x02id\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ontext\x18\x03 \x01(\x05\"H\n\x15SysUploadFileProgress\x12\r\n\x05\x62izId\x18\x01 \x01(\t\x12\x0e\n\x06result\x18\x02 \x01(\x05\x12\x10\n\x08progress\x18\x03 \x01(\x05\"\x1f\n\x0cSysErrorCode\x12\x0f\n\x07\x63ode_no\x18\x01 \x01(\x05\"\x1e\n\tSysBorder\x12\x11\n\tborderval\x18\x01 \x01(\x05\"*\n\x10SysPlanJobStatus\x12\x16\n\x0eplanjob_status\x18\x01 \x01(\x05\"=\n\x0fSysKnifeControl\x12\x14\n\x0cknife_status\x18\x01 \x01(\x05\x12\x14\n\x0cknife_height\x18\x02 \x01(\x05\"+\n\x14SysResetSystemStatus\x12\x13\n\x0breset_staus\x18\x01 \x01(\x05\"\x8a\x01\n\rTimeCtrlLight\x12\x0f\n\x07operate\x18\x01 \x01(\x05\x12\x0e\n\x06\x65nable\x18\x02 \x01(\x05\x12\x12\n\nstart_hour\x18\x03 \x01(\x05\x12\x11\n\tstart_min\x18\x04 \x01(\x05\x12\x10\n\x08\x65nd_hour\x18\x05 \x01(\x05\x12\x0f\n\x07\x65nd_min\x18\x06 \x01(\x05\x12\x0e\n\x06\x61\x63tion\x18\x07 \x01(\x05\"3\n\x10vision_point_msg\x12\t\n\x01x\x18\x01 \x01(\x02\x12\t\n\x01y\x18\x02 \x01(\x02\x12\t\n\x01z\x18\x03 \x01(\x02\"\\\n\x15vision_point_info_msg\x12\r\n\x05lable\x18\x01 \x01(\x05\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12\'\n\x0cvision_point\x18\x03 \x03(\x0b\x32\x11.vision_point_msg\"\x9a\x01\n\x13vio_to_app_info_msg\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x12\x0f\n\x07heading\x18\x03 \x01(\x01\x12\x11\n\tvio_state\x18\x04 \x01(\x05\x12\x12\n\nbrightness\x18\x05 \x01(\x05\x12\x1a\n\x12\x64\x65tect_feature_num\x18\x06 \x01(\x05\x12\x19\n\x11track_feature_num\x18\x07 \x01(\x05\"1\n\x14vision_statistic_msg\x12\x0c\n\x04mean\x18\x01 \x01(\x02\x12\x0b\n\x03var\x18\x02 \x01(\x02\"m\n\x19vision_statistic_info_msg\x12\x11\n\ttimestamp\x18\x01 \x01(\x01\x12\x0b\n\x03num\x18\x02 \x01(\x05\x12\x30\n\x11vision_statistics\x18\x03 \x03(\x0b\x32\x15.vision_statistic_msg\"\xd3\x01\n\x1asystemRapidStateTunnel_msg\x12\x18\n\x10rapid_state_data\x18\x01 \x03(\x03\x12\x31\n\x11vision_point_info\x18\x02 \x03(\x0b\x32\x16.vision_point_info_msg\x12-\n\x0fvio_to_app_info\x18\x03 \x01(\x0b\x32\x14.vio_to_app_info_msg\x12\x39\n\x15vision_statistic_info\x18\x04 \x01(\x0b\x32\x1a.vision_statistic_info_msg\"4\n\x19systemTardStateTunnel_msg\x12\x17\n\x0ftard_state_data\x18\x01 \x03(\x03\".\n\x13systemUpdateBuf_msg\x12\x17\n\x0fupdate_buf_data\x18\x01 \x03(\x03\"\x9e\x01\n\x0fSysOffChipFlash\x12\x16\n\x02op\x18\x01 \x01(\x0e\x32\n.Operation\x12\x16\n\x02id\x18\x02 \x01(\x0e\x32\n.OffPartId\x12\x12\n\nstart_addr\x18\x03 \x01(\r\x12\x0e\n\x06offset\x18\x04 \x01(\r\x12\x0e\n\x06length\x18\x05 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x0c\n\x04\x63ode\x18\x07 \x01(\x05\x12\x0b\n\x03msg\x18\x08 \x01(\t\"-\n\x14systemTmpCycleTx_msg\x12\x15\n\rcycle_tx_data\x18\x01 \x03(\x03\"%\n\nLoraCfgReq\x12\n\n\x02op\x18\x01 \x01(\x05\x12\x0b\n\x03\x63\x66g\x18\x02 \x01(\t\"F\n\nLoraCfgRsp\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\n\n\x02op\x18\x02 \x01(\x05\x12\x0b\n\x03\x63\x66g\x18\x03 \x01(\t\x12\x0f\n\x07\x66\x61\x63_cfg\x18\x04 \x01(\t\">\n\x0bmod_fw_info\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x10\n\x08identify\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\"L\n\x0e\x64\x65vice_fw_info\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x03mod\x18\x03 \x03(\x0b\x32\x0c.mod_fw_info\"@\n\x11mow_to_app_info_t\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0b\n\x03\x63md\x18\x02 \x01(\x05\x12\x10\n\x08mow_data\x18\x03 \x03(\x05\"a\n\x1a\x64\x65vice_product_type_info_t\x12\x0e\n\x06result\x18\x01 \x01(\x05\x12\x19\n\x11main_product_type\x18\x02 \x01(\t\x12\x18\n\x10sub_product_type\x18\x03 \x01(\t\"P\n\x0fQCAppTestExcept\x12\x13\n\x0b\x65xcept_type\x18\x01 \x01(\t\x12(\n\nconditions\x18\x02 \x03(\x0b\x32\x14.QCAppTestConditions\"t\n\x13QCAppTestConditions\x12\x11\n\tcond_type\x18\x01 \x01(\t\x12\x0f\n\x07int_val\x18\x02 \x01(\x05\x12\x11\n\tfloat_val\x18\x03 \x01(\x02\x12\x12\n\ndouble_val\x18\x04 \x01(\x01\x12\x12\n\nstring_val\x18\x05 \x01(\t\"\x99\x01\n\x19mow_to_app_qctools_info_t\x12\x1a\n\x04type\x18\x01 \x01(\x0e\x32\x0c.QCAppTestId\x12\x16\n\x0etimeOfDuration\x18\x02 \x01(\x05\x12\x0e\n\x06result\x18\x03 \x01(\x05\x12\x16\n\x0eresult_details\x18\x04 \x01(\t\x12 \n\x06\x65xcept\x18\x05 \x03(\x0b\x32\x10.QCAppTestExcept\"O\n\x16mCtrlSimulationCmdData\x12\x0e\n\x06subCmd\x18\x01 \x01(\x05\x12\x10\n\x08param_id\x18\x02 \x01(\x05\x12\x13\n\x0bparam_value\x18\x03 \x03(\x05\"\x8f\x01\n\x08rpt_lora\x12\x16\n\x0epair_code_scan\x18\x01 \x01(\x05\x12\x19\n\x11pair_code_channel\x18\x02 \x01(\x05\x12\x17\n\x0fpair_code_locid\x18\x03 \x01(\x05\x12\x17\n\x0fpair_code_netid\x18\x04 \x01(\x05\x12\x1e\n\x16lora_connection_status\x18\x05 \x01(\x05\"\xf1\x01\n\x07rpt_rtk\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x11\n\tpos_level\x18\x02 \x01(\x05\x12\x11\n\tgps_stars\x18\x03 \x01(\x05\x12\x0b\n\x03\x61ge\x18\x04 \x01(\x05\x12\x0f\n\x07lat_std\x18\x05 \x01(\x05\x12\x0f\n\x07lon_std\x18\x06 \x01(\x05\x12\x10\n\x08l2_stars\x18\x07 \x01(\x05\x12\x12\n\ndis_status\x18\x08 \x01(\x03\x12\x17\n\x0ftop4_total_mean\x18\t \x01(\x03\x12\x15\n\rco_view_stars\x18\n \x01(\x05\x12\r\n\x05reset\x18\x0b \x01(\x05\x12\x1c\n\tlora_info\x18\x0c \x01(\x0b\x32\t.rpt_lora\"\x86\x01\n\x10rpt_dev_location\x12\x12\n\nreal_pos_x\x18\x01 \x01(\x05\x12\x12\n\nreal_pos_y\x18\x02 \x01(\x05\x12\x13\n\x0breal_toward\x18\x03 \x01(\x05\x12\x10\n\x08pos_type\x18\x04 \x01(\x05\x12\x11\n\tzone_hash\x18\x05 \x01(\x03\x12\x10\n\x08\x62ol_hash\x18\x06 \x01(\x03\"4\n\x13vio_survival_info_t\x12\x1d\n\x15vio_survival_distance\x18\x01 \x01(\x02\";\n\x12\x63ollector_status_t\x12%\n\x1d\x63ollector_installation_status\x18\x01 \x01(\x05\"\"\n\x0clock_state_t\x12\x12\n\nlock_state\x18\x01 \x01(\r\"\xca\x02\n\x0erpt_dev_status\x12\x12\n\nsys_status\x18\x01 \x01(\x05\x12\x14\n\x0c\x63harge_state\x18\x02 \x01(\x05\x12\x13\n\x0b\x62\x61ttery_val\x18\x03 \x01(\x05\x12\x15\n\rsensor_status\x18\x04 \x01(\x05\x12\x13\n\x0blast_status\x18\x05 \x01(\x05\x12\x16\n\x0esys_time_stamp\x18\x06 \x01(\x03\x12\x14\n\x0cvslam_status\x18\x07 \x01(\x05\x12\x1c\n\tmnet_info\x18\x08 \x01(\x0b\x32\t.MnetInfo\x12/\n\x11vio_survival_info\x18\t \x01(\x0b\x32\x14.vio_survival_info_t\x12-\n\x10\x63ollector_status\x18\n \x01(\x0b\x32\x13.collector_status_t\x12!\n\nlock_state\x18\x0b \x01(\x0b\x32\r.lock_state_t\"\xaa\x01\n\x12rpt_connect_status\x12\x14\n\x0c\x63onnect_type\x18\x01 \x01(\x05\x12\x10\n\x08\x62le_rssi\x18\x02 \x01(\x05\x12\x11\n\twifi_rssi\x18\x03 \x01(\x05\x12\x11\n\tlink_type\x18\x04 \x01(\x05\x12\x11\n\tmnet_rssi\x18\x05 \x01(\x05\x12\x11\n\tmnet_inet\x18\x06 \x01(\x05\x12 \n\x08used_net\x18\x07 \x01(\x0e\x32\x0e.net_used_type\"\x9f\x03\n\x08rpt_work\x12\x0c\n\x04plan\x18\x01 \x01(\x05\x12\x11\n\tpath_hash\x18\x02 \x01(\x03\x12\x10\n\x08progress\x18\x03 \x01(\x05\x12\x0c\n\x04\x61rea\x18\x04 \x01(\x05\x12\x0f\n\x07\x62p_info\x18\x05 \x01(\x05\x12\x0f\n\x07\x62p_hash\x18\x06 \x01(\x03\x12\x10\n\x08\x62p_pos_x\x18\x07 \x01(\x05\x12\x10\n\x08\x62p_pos_y\x18\x08 \x01(\x05\x12\x15\n\rreal_path_num\x18\t \x01(\x03\x12\x12\n\npath_pos_x\x18\n \x01(\x05\x12\x12\n\npath_pos_y\x18\x0b \x01(\x05\x12\x14\n\x0cub_zone_hash\x18\x0c \x01(\x03\x12\x14\n\x0cub_path_hash\x18\r \x01(\x03\x12\x15\n\rinit_cfg_hash\x18\x0e \x01(\x03\x12\x15\n\rub_ecode_hash\x18\x0f \x01(\x03\x12\x14\n\x0cnav_run_mode\x18\x10 \x01(\x05\x12\x18\n\x10test_mode_status\x18\x11 \x01(\x03\x12\x15\n\rman_run_speed\x18\x12 \x01(\x05\x12\x17\n\x0fnav_edit_status\x18\x13 \x01(\x05\x12\x13\n\x0bknife_hight\x18\x14 \x01(\x05\"F\n\x0crpt_maintain\x12\x0f\n\x07mileage\x18\x01 \x01(\x03\x12\x11\n\twork_time\x18\x02 \x01(\x05\x12\x12\n\nbat_cycles\x18\x03 \x01(\x05\"\x8f\x01\n\x0freport_info_cfg\x12\x15\n\x03\x61\x63t\x18\x01 \x01(\x0e\x32\x08.rpt_act\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\x12\x0e\n\x06period\x18\x03 \x01(\x05\x12\x18\n\x10no_change_period\x18\x04 \x01(\x05\x12\r\n\x05\x63ount\x18\x05 \x01(\x05\x12\x1b\n\x03sub\x18\x06 \x03(\x0e\x32\x0e.rpt_info_type\"\x8c\x03\n\x10report_info_data\x12$\n\x07\x63onnect\x18\x01 \x01(\x0b\x32\x13.rpt_connect_status\x12\x1c\n\x03\x64\x65v\x18\x02 \x01(\x0b\x32\x0f.rpt_dev_status\x12\x15\n\x03rtk\x18\x03 \x01(\x0b\x32\x08.rpt_rtk\x12$\n\tlocations\x18\x04 \x03(\x0b\x32\x11.rpt_dev_location\x12\x17\n\x04work\x18\x05 \x01(\x0b\x32\t.rpt_work\x12 \n\x07\x66w_info\x18\x06 \x01(\x0b\x32\x0f.device_fw_info\x12\x1f\n\x08maintain\x18\x07 \x01(\x0b\x32\r.rpt_maintain\x12\x31\n\x11vision_point_info\x18\x08 \x03(\x0b\x32\x16.vision_point_info_msg\x12-\n\x0fvio_to_app_info\x18\t \x01(\x0b\x32\x14.vio_to_app_info_msg\x12\x39\n\x15vision_statistic_info\x18\n \x01(\x0b\x32\x1a.vision_statistic_info_msg\"\x9c\x0c\n\x07MctlSys\x12\"\n\rtoapp_batinfo\x18\x01 \x01(\x0b\x32\t.SysBatUpH\x00\x12)\n\x10toapp_work_state\x18\x02 \x01(\x0b\x32\r.SysWorkStateH\x00\x12*\n\x0ftodev_time_zone\x18\x03 \x01(\x0b\x32\x0f.SysSetTimeZoneH\x00\x12*\n\x0ftodev_data_time\x18\x04 \x01(\x0b\x32\x0f.SysSetDateTimeH\x00\x12\x1f\n\x08job_plan\x18\x06 \x01(\x0b\x32\x0b.SysJobPlanH\x00\x12(\n\x0etoapp_err_code\x18\x07 \x01(\x0b\x32\x0e.SysDevErrCodeH\x00\x12.\n\x13todev_job_plan_time\x18\n \x01(\x0b\x32\x0f.SysJobPlanTimeH\x00\x12%\n\x0etoapp_mow_info\x18\x0b \x01(\x0b\x32\x0b.SysMowInfoH\x00\x12&\n\x0f\x62idire_comm_cmd\x18\x0c \x01(\x0b\x32\x0b.SysCommCmdH\x00\x12\x16\n\x0cplan_job_del\x18\x0e \x01(\x03H\x00\x12\x1c\n\x06\x62order\x18\x0f \x01(\x0b\x32\n.SysBorderH\x00\x12.\n\x11toapp_plan_status\x18\x12 \x01(\x0b\x32\x11.SysPlanJobStatusH\x00\x12\x34\n\x12toapp_ul_fprogress\x18\x13 \x01(\x0b\x32\x16.SysUploadFileProgressH\x00\x12*\n\x10todev_deljobplan\x18\x14 \x01(\x0b\x32\x0e.SysDelJobPlanH\x00\x12\x1b\n\x11todev_mow_info_up\x18\x15 \x01(\x05H\x00\x12,\n\x10todev_knife_ctrl\x18\x16 \x01(\x0b\x32\x10.SysKnifeControlH\x00\x12\x1c\n\x12todev_reset_system\x18\x17 \x01(\x05H\x00\x12:\n\x19todev_reset_system_status\x18\x18 \x01(\x0b\x32\x15.SysResetSystemStatusH\x00\x12=\n\x16systemRapidStateTunnel\x18\x19 \x01(\x0b\x32\x1b.systemRapidStateTunnel_msgH\x00\x12;\n\x15systemTardStateTunnel\x18\x1a \x01(\x0b\x32\x1a.systemTardStateTunnel_msgH\x00\x12/\n\x0fsystemUpdateBuf\x18\x1b \x01(\x0b\x32\x14.systemUpdateBuf_msgH\x00\x12/\n\x15todev_time_ctrl_light\x18\x1c \x01(\x0b\x32\x0e.TimeCtrlLightH\x00\x12\x31\n\x10systemTmpCycleTx\x18\x1d \x01(\x0b\x32\x15.systemTmpCycleTx_msgH\x00\x12\x30\n\x14todev_off_chip_flash\x18\x1e \x01(\x0b\x32\x10.SysOffChipFlashH\x00\x12\x1f\n\x15todev_get_dev_fw_info\x18\x1f \x01(\x05H\x00\x12,\n\x11toapp_dev_fw_info\x18  \x01(\x0b\x32\x0f.device_fw_infoH\x00\x12)\n\x12todev_lora_cfg_req\x18! \x01(\x0b\x32\x0b.LoraCfgReqH\x00\x12)\n\x12toapp_lora_cfg_rsp\x18\" \x01(\x0b\x32\x0b.LoraCfgRspH\x00\x12-\n\x0fmow_to_app_info\x18# \x01(\x0b\x32\x12.mow_to_app_info_tH\x00\x12?\n\x18\x64\x65vice_product_type_info\x18$ \x01(\x0b\x32\x1b.device_product_type_info_tH\x00\x12=\n\x17mow_to_app_qctools_info\x18% \x01(\x0b\x32\x1a.mow_to_app_qctools_info_tH\x00\x12,\n\x10todev_report_cfg\x18& \x01(\x0b\x32\x10.report_info_cfgH\x00\x12.\n\x11toapp_report_data\x18\' \x01(\x0b\x32\x11.report_info_dataH\x00\x12\x31\n\x0esimulation_cmd\x18* \x01(\x0b\x32\x17.mCtrlSimulationCmdDataH\x00\x42\x0b\n\tSubSysMsg*+\n\tOperation\x12\t\n\x05WRITE\x10\x00\x12\x08\n\x04READ\x10\x01\x12\t\n\x05\x45RASE\x10\x02*\x8d\x02\n\tOffPartId\x12\x13\n\x0fOFF_PART_DL_IMG\x10\x00\x12\x19\n\x15OFF_PART_UPDINFO_BACK\x10\x01\x12\x14\n\x10OFF_PART_UPDINFO\x10\x02\x12\x13\n\x0fOFF_PART_NAKEDB\x10\x03\x12\x14\n\x10OFF_PART_FLASHDB\x10\x04\x12\x18\n\x14OFF_PART_UPD_APP_IMG\x10\x05\x12\x18\n\x14OFF_PART_UPD_BMS_IMG\x10\x06\x12\x18\n\x14OFF_PART_UPD_TMP_IMG\x10\x07\x12\x15\n\x11OFF_PART_DEV_INFO\x10\x08\x12\x18\n\x14OFF_PART_NAKEDB_BACK\x10\t\x12\x10\n\x0cOFF_PART_MAX\x10\n*\x95\x07\n\x0bQCAppTestId\x12!\n\x1dQC_APP_ITEM_ON_CHARGESATSTION\x10\x00\x12\x1a\n\x16QC_APP_TEST_X3_SPEAKER\x10\x01\x12)\n%QC_APP_TEST_STATIC_OBSTACLE_DETECTION\x10\x02\x12\"\n\x1eQC_APP_TEST_CHARGESTATION_TEMP\x10\x03\x12\x13\n\x0fQC_APP_ITEM_KEY\x10\x04\x12 \n\x1cQC_APP_TEST_BUMPER_FRONTLEFT\x10\x05\x12!\n\x1dQC_APP_TEST_BUMPER_FRONTRIGHT\x10\x06\x12\x14\n\x10QC_APP_TEST_STOP\x10\x07\x12\x16\n\x12QC_APP_TEST_UNLOCK\x10\x08\x12\x14\n\x10QC_APP_TEST_BUZZ\x10\t\x12\x14\n\x10QC_APP_TEST_LIFT\x10\n\x12\x16\n\x12QC_APP_ITEM_SENEOR\x10\x0b\x12\x19\n\x15QC_APP_TEST_ROLL_LEFT\x10\x0c\x12\x1a\n\x16QC_APP_TEST_ROLL_RIGHT\x10\r\x12\x1d\n\x19QC_APP_TEST_ULTRA_UNCOVER\x10\x0e\x12\x1c\n\x18QC_APP_TEST_ULTRA0_COVER\x10\x0f\x12\x1c\n\x18QC_APP_TEST_ULTRA1_COVER\x10\x10\x12\x1c\n\x18QC_APP_TEST_ULTRA2_COVER\x10\x11\x12\x14\n\x10QC_APP_TEST_RAIN\x10\x12\x12\x12\n\x0eQC_APP_ITEM_SQ\x10\x13\x12\x18\n\x14QC_APP_TEST_BLE_RSSI\x10\x14\x12 \n\x1cQC_APP_TEST_SATELLITES_ROVER\x10\x15\x12)\n%QC_APP_TEST_SATELLITES_REF_STATION_L1\x10\x16\x12)\n%QC_APP_TEST_SATELLITES_REF_STATION_L2\x10\x17\x12&\n\"QC_APP_TEST_SATELLITES_COMMON_VIEW\x10\x18\x12\x19\n\x15QC_APP_TEST_CNO_ROVER\x10\x19\x12\x1f\n\x1bQC_APP_TEST_CNO_REF_STATION\x10\x1a\x12\'\n#QC_APP_TEST_REF_STATION_LINK_STATUS\x10\x1b\x12\x1e\n\x1aQC_APP_TEST_LOCATION_STATE\x10\x1c\x12\x13\n\x0fQC_APP_TEST_MAX\x10\x1d*W\n\rnet_used_type\x12\x16\n\x12NET_USED_TYPE_NONE\x10\x00\x12\x16\n\x12NET_USED_TYPE_WIFI\x10\x01\x12\x16\n\x12NET_USED_TYPE_MNET\x10\x02*\xbf\x01\n\rrpt_info_type\x12\x0f\n\x0bRIT_CONNECT\x10\x00\x12\x0f\n\x0bRIT_DEV_STA\x10\x01\x12\x0b\n\x07RIT_RTK\x10\x02\x12\x11\n\rRIT_DEV_LOCAL\x10\x03\x12\x0c\n\x08RIT_WORK\x10\x04\x12\x0f\n\x0bRIT_FW_INFO\x10\x05\x12\x10\n\x0cRIT_MAINTAIN\x10\x06\x12\x14\n\x10RIT_VISION_POINT\x10\x07\x12\x0b\n\x07RIT_VIO\x10\x08\x12\x18\n\x14RIT_VISION_STATISTIC\x10\t*4\n\x07rpt_act\x12\r\n\tRPT_START\x10\x00\x12\x0c\n\x08RPT_STOP\x10\x01\x12\x0c\n\x08RPT_KEEP\x10\x02\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'pyluba.proto.mctrl_sys_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _OPERATION._serialized_start=6798
-  _OPERATION._serialized_end=6841
-  _OFFPARTID._serialized_start=6844
-  _OFFPARTID._serialized_end=7113
-  _RPTINFOTYPE._serialized_start=7116
-  _RPTINFOTYPE._serialized_end=7305
-  _MCTLSYS._serialized_start=61
-  _MCTLSYS._serialized_end=1621
-  _MCTRLSIMULATIONCMDDATA._serialized_start=1623
-  _MCTRLSIMULATIONCMDDATA._serialized_end=1700
-  _SYSKNIFECONTROL._serialized_start=1702
-  _SYSKNIFECONTROL._serialized_end=1761
-  _SYSBATUP._serialized_start=1763
-  _SYSBATUP._serialized_end=1789
-  _SYSWORKSTATE._serialized_start=1791
-  _SYSWORKSTATE._serialized_end=1881
-  _SYSSETTIMEZONE._serialized_start=1883
-  _SYSSETTIMEZONE._serialized_end=1936
-  _SYSSETDATETIME._serialized_start=1939
-  _SYSSETDATETIME._serialized_end=2097
-  _SYSJOBPLAN._serialized_start=2099
-  _SYSJOBPLAN._serialized_end=2185
-  _SYSDEVERRCODE._serialized_start=2187
-  _SYSDEVERRCODE._serialized_end=2221
-  _SYSBOARDTYPE._serialized_start=2223
-  _SYSBOARDTYPE._serialized_end=2256
-  _SYSSWVERSION._serialized_start=2258
-  _SYSSWVERSION._serialized_end=2311
-  _SYSDELJOBPLAN._serialized_start=2313
-  _SYSDELJOBPLAN._serialized_end=2362
-  _SYSJOBPLANTIME._serialized_start=2365
-  _SYSJOBPLANTIME._serialized_end=2590
-  _SYSMOWINFO._serialized_start=2592
-  _SYSMOWINFO._serialized_end=2699
-  _SYSOPTILINEACK._serialized_start=2701
-  _SYSOPTILINEACK._serialized_end=2760
-  _SYSCOMMCMD._serialized_start=2762
-  _SYSCOMMCMD._serialized_end=2815
-  _SYSUPLOADFILEPROGRESS._serialized_start=2817
-  _SYSUPLOADFILEPROGRESS._serialized_end=2889
-  _SYSERRORCODE._serialized_start=2891
-  _SYSERRORCODE._serialized_end=2921
-  _SYSBORDER._serialized_start=2923
-  _SYSBORDER._serialized_end=2953
-  _SYSPLANJOBSTATUS._serialized_start=2955
-  _SYSPLANJOBSTATUS._serialized_end=2996
-  _SYSRESETSYSTEMSTATUS._serialized_start=2998
-  _SYSRESETSYSTEMSTATUS._serialized_end=3040
-  _TIMECTRLLIGHT._serialized_start=3043
-  _TIMECTRLLIGHT._serialized_end=3181
-  _SYSTEMRAPIDSTATETUNNEL_MSG._serialized_start=3183
-  _SYSTEMRAPIDSTATETUNNEL_MSG._serialized_end=3237
-  _SYSTEMTARDSTATETUNNEL_MSG._serialized_start=3239
-  _SYSTEMTARDSTATETUNNEL_MSG._serialized_end=3291
-  _SYSTEMUPDATEBUF_MSG._serialized_start=3293
-  _SYSTEMUPDATEBUF_MSG._serialized_end=3339
-  _SYSOFFCHIPFLASH._serialized_start=3342
-  _SYSOFFCHIPFLASH._serialized_end=3476
-  _SYSTEMTMPCYCLETX_MSG._serialized_start=3478
-  _SYSTEMTMPCYCLETX_MSG._serialized_end=3523
-  _LORACFGREQ._serialized_start=3525
-  _LORACFGREQ._serialized_end=3563
-  _LORACFGRSP._serialized_start=3565
-  _LORACFGRSP._serialized_end=3635
-  _MOD_FW_INFO._serialized_start=3637
-  _MOD_FW_INFO._serialized_end=3699
-  _DEVICE_FW_INFO._serialized_start=3701
-  _DEVICE_FW_INFO._serialized_end=3777
-  _MOW_TO_APP_INFO_T._serialized_start=3779
-  _MOW_TO_APP_INFO_T._serialized_end=3843
-  _RPTCONNECTSTATUS._serialized_start=3846
-  _RPTCONNECTSTATUS._serialized_end=3998
-  _RPTWORK._serialized_start=4001
-  _RPTWORK._serialized_end=4416
-  _RPTMAINTAIN._serialized_start=4418
-  _RPTMAINTAIN._serialized_end=4487
-  _RPTDEVLOCATION._serialized_start=4490
-  _RPTDEVLOCATION._serialized_end=4622
-  _COLLECTORSTATUS._serialized_start=4624
-  _COLLECTORSTATUS._serialized_end=4680
-  _VIOSURVIVALINFO._serialized_start=4682
-  _VIOSURVIVALINFO._serialized_end=4730
-  _RPTDEVSTATUS._serialized_start=4733
-  _RPTDEVSTATUS._serialized_end=5019
-  _RPTLORA._serialized_start=5022
-  _RPTLORA._serialized_end=5164
-  _RPTRTK._serialized_start=5167
-  _RPTRTK._serialized_end=5406
-  _VIOTOAPPINFOMSG._serialized_start=5409
-  _VIOTOAPPINFOMSG._serialized_end=5559
-  _VISIONPOINTMSG._serialized_start=5561
-  _VISIONPOINTMSG._serialized_end=5610
-  _VISIONPOINTINFOMSG._serialized_start=5612
-  _VISIONPOINTINFOMSG._serialized_end=5699
-  _VISIONSTATISTICMSG._serialized_start=5701
-  _VISIONSTATISTICMSG._serialized_end=5748
-  _VISIONSTATISTICINFOMSG._serialized_start=5750
-  _VISIONSTATISTICINFOMSG._serialized_end=5854
-  _REPORTINFODATA._serialized_start=5857
-  _REPORTINFODATA._serialized_end=6232
-  _DEVICEPRODUCTTYPEINFO._serialized_start=6234
-  _DEVICEPRODUCTTYPEINFO._serialized_end=6326
-  _REPORTINFOCFG._serialized_start=6329
-  _REPORTINFOCFG._serialized_end=6458
-  _MOWTOAPPQCTOOLSINFO._serialized_start=6461
-  _MOWTOAPPQCTOOLSINFO._serialized_end=6596
-  _QCAPPTESTEXCEPT._serialized_start=6598
-  _QCAPPTESTEXCEPT._serialized_end=6678
-  _QCAPPTESTCONDITIONS._serialized_start=6680
-  _QCAPPTESTCONDITIONS._serialized_end=6796
+  _OPERATION._serialized_start=7188
+  _OPERATION._serialized_end=7231
+  _OFFPARTID._serialized_start=7234
+  _OFFPARTID._serialized_end=7503
+  _QCAPPTESTID._serialized_start=7506
+  _QCAPPTESTID._serialized_end=8423
+  _NET_USED_TYPE._serialized_start=8425
+  _NET_USED_TYPE._serialized_end=8512
+  _RPT_INFO_TYPE._serialized_start=8515
+  _RPT_INFO_TYPE._serialized_end=8706
+  _RPT_ACT._serialized_start=8708
+  _RPT_ACT._serialized_end=8760
+  _SYSBATUP._serialized_start=60
+  _SYSBATUP._serialized_end=86
+  _SYSWORKSTATE._serialized_start=88
+  _SYSWORKSTATE._serialized_end=178
+  _SYSSETTIMEZONE._serialized_start=180
+  _SYSSETTIMEZONE._serialized_end=233
+  _SYSSETDATETIME._serialized_start=236
+  _SYSSETDATETIME._serialized_end=394
+  _SYSJOBPLAN._serialized_start=396
+  _SYSJOBPLAN._serialized_end=482
+  _SYSDEVERRCODE._serialized_start=484
+  _SYSDEVERRCODE._serialized_end=518
+  _SYSBOARDTYPE._serialized_start=520
+  _SYSBOARDTYPE._serialized_end=553
+  _SYSSWVERSION._serialized_start=555
+  _SYSSWVERSION._serialized_end=608
+  _SYSDELJOBPLAN._serialized_start=610
+  _SYSDELJOBPLAN._serialized_end=659
+  _SYSJOBPLANTIME._serialized_start=662
+  _SYSJOBPLANTIME._serialized_end=898
+  _SYSMOWINFO._serialized_start=900
+  _SYSMOWINFO._serialized_end=1007
+  _SYSOPTILINEACK._serialized_start=1009
+  _SYSOPTILINEACK._serialized_end=1068
+  _SYSCOMMCMD._serialized_start=1070
+  _SYSCOMMCMD._serialized_end=1123
+  _SYSUPLOADFILEPROGRESS._serialized_start=1125
+  _SYSUPLOADFILEPROGRESS._serialized_end=1197
+  _SYSERRORCODE._serialized_start=1199
+  _SYSERRORCODE._serialized_end=1230
+  _SYSBORDER._serialized_start=1232
+  _SYSBORDER._serialized_end=1262
+  _SYSPLANJOBSTATUS._serialized_start=1264
+  _SYSPLANJOBSTATUS._serialized_end=1306
+  _SYSKNIFECONTROL._serialized_start=1308
+  _SYSKNIFECONTROL._serialized_end=1369
+  _SYSRESETSYSTEMSTATUS._serialized_start=1371
+  _SYSRESETSYSTEMSTATUS._serialized_end=1414
+  _TIMECTRLLIGHT._serialized_start=1417
+  _TIMECTRLLIGHT._serialized_end=1555
+  _VISION_POINT_MSG._serialized_start=1557
+  _VISION_POINT_MSG._serialized_end=1608
+  _VISION_POINT_INFO_MSG._serialized_start=1610
+  _VISION_POINT_INFO_MSG._serialized_end=1702
+  _VIO_TO_APP_INFO_MSG._serialized_start=1705
+  _VIO_TO_APP_INFO_MSG._serialized_end=1859
+  _VISION_STATISTIC_MSG._serialized_start=1861
+  _VISION_STATISTIC_MSG._serialized_end=1910
+  _VISION_STATISTIC_INFO_MSG._serialized_start=1912
+  _VISION_STATISTIC_INFO_MSG._serialized_end=2021
+  _SYSTEMRAPIDSTATETUNNEL_MSG._serialized_start=2024
+  _SYSTEMRAPIDSTATETUNNEL_MSG._serialized_end=2235
+  _SYSTEMTARDSTATETUNNEL_MSG._serialized_start=2237
+  _SYSTEMTARDSTATETUNNEL_MSG._serialized_end=2289
+  _SYSTEMUPDATEBUF_MSG._serialized_start=2291
+  _SYSTEMUPDATEBUF_MSG._serialized_end=2337
+  _SYSOFFCHIPFLASH._serialized_start=2340
+  _SYSOFFCHIPFLASH._serialized_end=2498
+  _SYSTEMTMPCYCLETX_MSG._serialized_start=2500
+  _SYSTEMTMPCYCLETX_MSG._serialized_end=2545
+  _LORACFGREQ._serialized_start=2547
+  _LORACFGREQ._serialized_end=2584
+  _LORACFGRSP._serialized_start=2586
+  _LORACFGRSP._serialized_end=2656
+  _MOD_FW_INFO._serialized_start=2658
+  _MOD_FW_INFO._serialized_end=2720
+  _DEVICE_FW_INFO._serialized_start=2722
+  _DEVICE_FW_INFO._serialized_end=2798
+  _MOW_TO_APP_INFO_T._serialized_start=2800
+  _MOW_TO_APP_INFO_T._serialized_end=2864
+  _DEVICE_PRODUCT_TYPE_INFO_T._serialized_start=2866
+  _DEVICE_PRODUCT_TYPE_INFO_T._serialized_end=2963
+  _QCAPPTESTEXCEPT._serialized_start=2965
+  _QCAPPTESTEXCEPT._serialized_end=3045
+  _QCAPPTESTCONDITIONS._serialized_start=3047
+  _QCAPPTESTCONDITIONS._serialized_end=3163
+  _MOW_TO_APP_QCTOOLS_INFO_T._serialized_start=3166
+  _MOW_TO_APP_QCTOOLS_INFO_T._serialized_end=3319
+  _MCTRLSIMULATIONCMDDATA._serialized_start=3321
+  _MCTRLSIMULATIONCMDDATA._serialized_end=3400
+  _RPT_LORA._serialized_start=3403
+  _RPT_LORA._serialized_end=3546
+  _RPT_RTK._serialized_start=3549
+  _RPT_RTK._serialized_end=3790
+  _RPT_DEV_LOCATION._serialized_start=3793
+  _RPT_DEV_LOCATION._serialized_end=3927
+  _VIO_SURVIVAL_INFO_T._serialized_start=3929
+  _VIO_SURVIVAL_INFO_T._serialized_end=3981
+  _COLLECTOR_STATUS_T._serialized_start=3983
+  _COLLECTOR_STATUS_T._serialized_end=4042
+  _LOCK_STATE_T._serialized_start=4044
+  _LOCK_STATE_T._serialized_end=4078
+  _RPT_DEV_STATUS._serialized_start=4081
+  _RPT_DEV_STATUS._serialized_end=4411
+  _RPT_CONNECT_STATUS._serialized_start=4414
+  _RPT_CONNECT_STATUS._serialized_end=4584
+  _RPT_WORK._serialized_start=4587
+  _RPT_WORK._serialized_end=5002
+  _RPT_MAINTAIN._serialized_start=5004
+  _RPT_MAINTAIN._serialized_end=5074
+  _REPORT_INFO_CFG._serialized_start=5077
+  _REPORT_INFO_CFG._serialized_end=5220
+  _REPORT_INFO_DATA._serialized_start=5223
+  _REPORT_INFO_DATA._serialized_end=5619
+  _MCTLSYS._serialized_start=5622
+  _MCTLSYS._serialized_end=7186
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pyluba-0.0.5/pyluba/utility/constant/device_constant.py` & `pyluba-0.0.6/pyluba/utility/constant/device_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/utility/periodic.py` & `pyluba-0.0.6/pyluba/utility/periodic.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyluba/utility/rocker_util.py` & `pyluba-0.0.6/pyluba/utility/rocker_util.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.5/pyproject.toml` & `pyluba-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name        = "pyluba"
-version     = "0.0.5"
+version     = "0.0.6"
 license     = "GNU-3.0"
 description = ""
 readme      = "README.md"
 authors     = [
     "Michael Arthur <michael@jumblesoft.co.nz>",
     "Jan Dalheimer <jan@dalheimer.de>"
 ]
@@ -12,33 +12,34 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 bleak = "^0.21.1"
 protobuf = "^5.26.1"
 py-jsonic = "^0.0.2"
-pydantic = "^2.5.3"
+pydantic = "^2.7.1"
 aliyun-python-sdk-iot = "^8.57.0"
 aliyun-iot-linkkit = "^1.2.12"
 aiohttp = "^3.9.1"
 paho-mqtt = "^1.6.1"
 alicloud-gateway-iot = "^1.0.0"
 alibabacloud-apigateway-util = "^0.0.2"
 alibabacloud-iot-api-gateway = "^0.0.4"
-twine = "^5.0.0"
-frida-tools = "^12.3.0"
-protobuf-to-pydantic = {version = "^0.2.6.2", extras = ["mypy-protobuf"]}
 grpcio-tools = "^1.63.0"
 bleak-retry-connector = "^3.5.0"
 jsonic = "^1.0.0"
-bumpver = "^2023.1129"
+
 
 [tool.poetry.group.dev.dependencies]
 types-protobuf = "^4.23.0.1"
 mypy-protobuf = "^3.4.0"
+twine = "^5.0.0"
+bumpver = "^2023.1129"
+frida-tools = "^12.3.0"
+protobuf-to-pydantic = {version = "^0.2.6.2", extras = ["mypy-protobuf"]}
 
 
 [tool.bumpver]
 current_version = "0.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
```

### Comparing `pyluba-0.0.5/PKG-INFO` & `pyluba-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyluba
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 License: GNU-3.0
 Author: Michael Arthur
 Author-email: michael@jumblesoft.co.nz
 Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,24 +14,20 @@
 Requires-Dist: alibabacloud-apigateway-util (>=0.0.2,<0.0.3)
 Requires-Dist: alibabacloud-iot-api-gateway (>=0.0.4,<0.0.5)
 Requires-Dist: alicloud-gateway-iot (>=1.0.0,<2.0.0)
 Requires-Dist: aliyun-iot-linkkit (>=1.2.12,<2.0.0)
 Requires-Dist: aliyun-python-sdk-iot (>=8.57.0,<9.0.0)
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
 Requires-Dist: bleak-retry-connector (>=3.5.0,<4.0.0)
-Requires-Dist: bumpver (>=2023.1129,<2024.0)
-Requires-Dist: frida-tools (>=12.3.0,<13.0.0)
 Requires-Dist: grpcio-tools (>=1.63.0,<2.0.0)
 Requires-Dist: jsonic (>=1.0.0,<2.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: protobuf (>=5.26.1,<6.0.0)
-Requires-Dist: protobuf-to-pydantic[mypy-protobuf] (>=0.2.6.2,<0.3.0.0)
 Requires-Dist: py-jsonic (>=0.0.2,<0.0.3)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
-Requires-Dist: twine (>=5.0.0,<6.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![SemVer 0.8.5][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
 [img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.0.1&color=blue
```

