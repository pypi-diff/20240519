# Comparing `tmp/pyluba-0.0.7.tar.gz` & `tmp/pyluba-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyluba-0.0.7.tar", max compression
+gzip compressed data, was "pyluba-0.0.8.tar", max compression
```

## Comparing `pyluba-0.0.7.tar` & `pyluba-0.0.8.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.7/LICENSE
--rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.7/README.md
--rw-r--r--   0        0        0      903 2024-05-15 09:07:45.520662 pyluba-0.0.7/pyluba/__init__.py
--rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.7/pyluba/aliyun/cloud_gateway.py
--rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.7/pyluba/aliyun/cloud_service.py
--rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.7/pyluba/aliyun/test_alicloud_api_gateway.py
--rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/aliyun/tmp_constant.py
--rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.7/pyluba/bluetooth/__init__.py
--rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.7/pyluba/bluetooth/ble.py
--rw-r--r--   0        0        0    40473 2024-05-15 09:07:42.251526 pyluba-0.0.7/pyluba/bluetooth/ble_message.py
--rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/bluetooth/const.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/bluetooth/data/__init__.py
--rw-r--r--   0        0        0     4405 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/bluetooth/data/convert.py
--rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/bluetooth/data/framectrldata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/bluetooth/data/model/__init__.py
--rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/bluetooth/data/notifydata.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/__init__.py
--rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/__init__.py
--rw-r--r--   0        0        0     1359 2024-05-14 22:34:13.652444 pyluba-0.0.7/pyluba/data/model/excute_boarder_params.py
--rw-r--r--   0        0        0     1099 2024-05-14 22:35:28.648628 pyluba-0.0.7/pyluba/data/model/execute_boarder.py
--rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/generate_route_information.py
--rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/hash_list.py
--rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/mowing_modes.py
--rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/plan.py
--rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/rapid_state.py
--rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/model/region_data.py
--rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.7/pyluba/data/mqtt/__init__.py
--rw-r--r--   0        0        0     1669 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/data/mqtt/event.py
--rw-r--r--   0        0        0     2343 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/data/mqtt/properties.py
--rw-r--r--   0        0        0      924 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/data/mqtt/status.py
--rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/event/__init__.py
--rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.7/pyluba/event/event.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/http/_init_.py
--rw-r--r--   0        0        0     1832 2024-02-24 11:05:42.835293 pyluba-0.0.7/pyluba/http/http.py
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/luba/_init_.py
--rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/luba/base.py
--rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.7/pyluba/mammotion/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.7/pyluba/mammotion/commands/proto.py
--rw-r--r--   0        0        0       48 2024-05-14 22:27:59.597338 pyluba-0.0.7/pyluba/mammotion/devices/__init__.py
--rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.7/pyluba/mammotion/devices/luba.py
--rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.7/pyluba/mqtt/mqtt.py
--rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.7/pyluba/proto/common.proto
--rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.7/pyluba/proto/common_pb2.py
--rw-r--r--   0        0        0      460 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/common_pb2.pyi
--rw-r--r--   0        0        0     5502 2024-05-15 09:07:42.251526 pyluba-0.0.7/pyluba/proto/dev_net.proto
--rw-r--r--   0        0        0    12853 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/dev_net_pb2.py
--rw-r--r--   0        0        0    21825 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/dev_net_pb2.pyi
--rw-r--r--   0        0        0     1553 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/luba_msg.proto
--rw-r--r--   0        0        0     4215 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/luba_msg_pb2.py
--rw-r--r--   0        0        0     4031 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/luba_msg_pb2.pyi
--rw-r--r--   0        0        0     1114 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/luba_mul.proto
--rw-r--r--   0        0        0     3387 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/luba_mul_pb2.py
--rw-r--r--   0        0        0     3913 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/luba_mul_pb2.pyi
--rw-r--r--   0        0        0     1383 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/mctrl_driver.proto
--rw-r--r--   0        0        0     3770 2024-05-15 09:07:42.252526 pyluba-0.0.7/pyluba/proto/mctrl_driver_pb2.py
--rw-r--r--   0        0        0     5852 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/mctrl_driver_pb2.pyi
--rw-r--r--   0        0        0    10530 2024-05-15 09:07:42.253526 pyluba-0.0.7/pyluba/proto/mctrl_nav.proto
--rw-r--r--   0        0        0    21725 2024-05-15 09:07:42.253526 pyluba-0.0.7/pyluba/proto/mctrl_nav_pb2.py
--rw-r--r--   0        0        0    45951 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/mctrl_nav_pb2.pyi
--rw-r--r--   0        0        0      629 2024-05-15 09:07:42.253526 pyluba-0.0.7/pyluba/proto/mctrl_ota.proto
--rw-r--r--   0        0        0     2259 2024-05-15 09:07:42.254526 pyluba-0.0.7/pyluba/proto/mctrl_ota_pb2.py
--rw-r--r--   0        0        0     2821 2024-05-18 08:45:36.775444 pyluba-0.0.7/pyluba/proto/mctrl_ota_pb2.pyi
--rw-r--r--   0        0        0      664 2024-05-15 09:07:42.254526 pyluba-0.0.7/pyluba/proto/mctrl_pept.proto
--rw-r--r--   0        0        0     2121 2024-05-15 09:07:42.254526 pyluba-0.0.7/pyluba/proto/mctrl_pept_pb2.py
--rw-r--r--   0        0        0     2840 2024-05-18 08:45:36.776446 pyluba-0.0.7/pyluba/proto/mctrl_pept_pb2.pyi
--rw-r--r--   0        0        0    10186 2024-05-15 09:07:42.254526 pyluba-0.0.7/pyluba/proto/mctrl_sys.proto
--rw-r--r--   0        0        0    21469 2024-05-15 09:07:42.254526 pyluba-0.0.7/pyluba/proto/mctrl_sys_pb2.py
--rw-r--r--   0        0        0    38893 2024-05-18 08:45:36.776446 pyluba-0.0.7/pyluba/proto/mctrl_sys_pb2.pyi
--rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.7/pyluba/py.typed
--rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.7/pyluba/utility/constant/device_constant.py
--rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.7/pyluba/utility/periodic.py
--rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.7/pyluba/utility/rocker_util.py
--rw-r--r--   0        0        0     1498 2024-05-18 22:54:12.007966 pyluba-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 pyluba-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-24 00:10:17.430127 pyluba-0.0.8/LICENSE
+-rw-r--r--   0        0        0      742 2024-05-08 21:27:25.359942 pyluba-0.0.8/README.md
+-rw-r--r--   0        0        0      903 2024-05-15 09:07:45.520662 pyluba-0.0.8/pyluba/__init__.py
+-rw-r--r--   0        0        0     1983 2024-03-25 03:39:32.867946 pyluba-0.0.8/pyluba/aliyun/cloud_gateway.py
+-rw-r--r--   0        0        0     2233 2024-02-25 00:02:48.028073 pyluba-0.0.8/pyluba/aliyun/cloud_service.py
+-rw-r--r--   0        0        0     6460 2024-03-22 21:00:07.350463 pyluba-0.0.8/pyluba/aliyun/test_alicloud_api_gateway.py
+-rw-r--r--   0        0        0     6643 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/aliyun/tmp_constant.py
+-rw-r--r--   0        0        0       43 2024-05-08 22:13:38.998098 pyluba-0.0.8/pyluba/bluetooth/__init__.py
+-rw-r--r--   0        0        0     2495 2024-05-08 22:35:28.441708 pyluba-0.0.8/pyluba/bluetooth/ble.py
+-rw-r--r--   0        0        0    40473 2024-05-15 09:07:42.251526 pyluba-0.0.8/pyluba/bluetooth/ble_message.py
+-rw-r--r--   0        0        0     1748 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/const.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/__init__.py
+-rw-r--r--   0        0        0     4405 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/bluetooth/data/convert.py
+-rw-r--r--   0        0        0     1051 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/framectrldata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/model/__init__.py
+-rw-r--r--   0        0        0     2009 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/bluetooth/data/notifydata.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/__init__.py
+-rw-r--r--   0        0        0      265 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/__init__.py
+-rw-r--r--   0        0        0     1359 2024-05-14 22:34:13.652444 pyluba-0.0.8/pyluba/data/model/excute_boarder_params.py
+-rw-r--r--   0        0        0     1088 2024-05-18 23:22:44.570535 pyluba-0.0.8/pyluba/data/model/execute_boarder.py
+-rw-r--r--   0        0        0     3271 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/generate_route_information.py
+-rw-r--r--   0        0        0      480 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/hash_list.py
+-rw-r--r--   0        0        0      454 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/mowing_modes.py
+-rw-r--r--   0        0        0     1924 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/plan.py
+-rw-r--r--   0        0        0      986 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/rapid_state.py
+-rw-r--r--   0        0        0     2780 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/model/region_data.py
+-rw-r--r--   0        0        0        3 2024-02-24 00:10:17.431127 pyluba-0.0.8/pyluba/data/mqtt/__init__.py
+-rw-r--r--   0        0        0     1802 2024-05-18 23:15:54.054056 pyluba-0.0.8/pyluba/data/mqtt/event.py
+-rw-r--r--   0        0        0     2795 2024-05-18 23:17:51.762904 pyluba-0.0.8/pyluba/data/mqtt/properties.py
+-rw-r--r--   0        0        0     1064 2024-05-18 23:18:33.829029 pyluba-0.0.8/pyluba/data/mqtt/status.py
+-rw-r--r--   0        0        0      122 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/event/__init__.py
+-rw-r--r--   0        0        0     1485 2024-04-29 23:01:28.524663 pyluba-0.0.8/pyluba/event/event.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/http/_init_.py
+-rw-r--r--   0        0        0     1937 2024-05-18 23:19:47.517975 pyluba-0.0.8/pyluba/http/http.py
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/luba/_init_.py
+-rw-r--r--   0        0        0     3279 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/luba/base.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:38.823703 pyluba-0.0.8/pyluba/mammotion/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 09:24:22.155845 pyluba-0.0.8/pyluba/mammotion/commands/proto.py
+-rw-r--r--   0        0        0       48 2024-05-14 22:27:59.597338 pyluba-0.0.8/pyluba/mammotion/devices/__init__.py
+-rw-r--r--   0        0        0    14989 2024-05-14 08:49:20.985172 pyluba-0.0.8/pyluba/mammotion/devices/luba.py
+-rw-r--r--   0        0        0     5392 2024-02-24 08:01:33.605363 pyluba-0.0.8/pyluba/mqtt/mqtt.py
+-rw-r--r--   0        0        0       81 2024-02-24 00:10:17.432128 pyluba-0.0.8/pyluba/proto/common.proto
+-rw-r--r--   0        0        0     1015 2024-04-25 20:48:27.244814 pyluba-0.0.8/pyluba/proto/common_pb2.py
+-rw-r--r--   0        0        0      460 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/common_pb2.pyi
+-rw-r--r--   0        0        0     5502 2024-05-15 09:07:42.251526 pyluba-0.0.8/pyluba/proto/dev_net.proto
+-rw-r--r--   0        0        0    12853 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/dev_net_pb2.py
+-rw-r--r--   0        0        0    21825 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/dev_net_pb2.pyi
+-rw-r--r--   0        0        0     1553 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_msg.proto
+-rw-r--r--   0        0        0     4215 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_msg_pb2.py
+-rw-r--r--   0        0        0     4031 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/luba_msg_pb2.pyi
+-rw-r--r--   0        0        0     1114 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_mul.proto
+-rw-r--r--   0        0        0     3387 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/luba_mul_pb2.py
+-rw-r--r--   0        0        0     3913 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/luba_mul_pb2.pyi
+-rw-r--r--   0        0        0     1383 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/mctrl_driver.proto
+-rw-r--r--   0        0        0     3770 2024-05-15 09:07:42.252526 pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.py
+-rw-r--r--   0        0        0     5852 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.pyi
+-rw-r--r--   0        0        0    10530 2024-05-15 09:07:42.253526 pyluba-0.0.8/pyluba/proto/mctrl_nav.proto
+-rw-r--r--   0        0        0    21725 2024-05-15 09:07:42.253526 pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.py
+-rw-r--r--   0        0        0    45951 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.pyi
+-rw-r--r--   0        0        0      629 2024-05-15 09:07:42.253526 pyluba-0.0.8/pyluba/proto/mctrl_ota.proto
+-rw-r--r--   0        0        0     2259 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.py
+-rw-r--r--   0        0        0     2821 2024-05-18 08:45:36.775444 pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.pyi
+-rw-r--r--   0        0        0      664 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_pept.proto
+-rw-r--r--   0        0        0     2121 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.py
+-rw-r--r--   0        0        0     2840 2024-05-18 08:45:36.776446 pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.pyi
+-rw-r--r--   0        0        0    10186 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_sys.proto
+-rw-r--r--   0        0        0    21469 2024-05-15 09:07:42.254526 pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.py
+-rw-r--r--   0        0        0    38893 2024-05-18 08:45:36.776446 pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.pyi
+-rw-r--r--   0        0        0        0 2024-02-24 00:10:17.433127 pyluba-0.0.8/pyluba/py.typed
+-rw-r--r--   0        0        0     5306 2024-05-13 23:09:11.573598 pyluba-0.0.8/pyluba/utility/constant/device_constant.py
+-rw-r--r--   0        0        0     1073 2024-02-24 00:10:17.433127 pyluba-0.0.8/pyluba/utility/periodic.py
+-rw-r--r--   0        0        0     5097 2024-02-24 00:10:17.433127 pyluba-0.0.8/pyluba/utility/rocker_util.py
+-rw-r--r--   0        0        0     1443 2024-05-18 23:25:34.314790 pyluba-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 pyluba-0.0.8/PKG-INFO
```

### Comparing `pyluba-0.0.7/LICENSE` & `pyluba-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/README.md` & `pyluba-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/__init__.py` & `pyluba-0.0.8/pyluba/__init__.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/aliyun/cloud_gateway.py` & `pyluba-0.0.8/pyluba/aliyun/cloud_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/aliyun/cloud_service.py` & `pyluba-0.0.8/pyluba/aliyun/cloud_service.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/aliyun/test_alicloud_api_gateway.py` & `pyluba-0.0.8/pyluba/aliyun/test_alicloud_api_gateway.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/aliyun/tmp_constant.py` & `pyluba-0.0.8/pyluba/aliyun/tmp_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/bluetooth/ble.py` & `pyluba-0.0.8/pyluba/bluetooth/ble.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/bluetooth/ble_message.py` & `pyluba-0.0.8/pyluba/bluetooth/ble_message.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/bluetooth/const.py` & `pyluba-0.0.8/pyluba/bluetooth/const.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/bluetooth/data/convert.py` & `pyluba-0.0.8/pyluba/bluetooth/data/convert.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/bluetooth/data/framectrldata.py` & `pyluba-0.0.8/pyluba/bluetooth/data/framectrldata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/bluetooth/data/notifydata.py` & `pyluba-0.0.8/pyluba/bluetooth/data/notifydata.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/data/model/excute_boarder_params.py` & `pyluba-0.0.8/pyluba/data/model/excute_boarder_params.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/data/model/execute_boarder.py` & `pyluba-0.0.8/pyluba/data/model/execute_boarder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from jsonic.serializable import serialize, Serializable
+from jsonic.serializable import Serializable
 from .excute_boarder_params import ExecuteBorderParams
 
 
 class ExecuteBorder(Serializable):
     """ generated source for class ExecuteBorderBean """
     cmd = int()
     params = ExecuteBorderParams(None, None, None)
```

### Comparing `pyluba-0.0.7/pyluba/data/model/generate_route_information.py` & `pyluba-0.0.8/pyluba/data/model/generate_route_information.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/data/model/plan.py` & `pyluba-0.0.8/pyluba/data/model/plan.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/data/model/rapid_state.py` & `pyluba-0.0.8/pyluba/data/model/rapid_state.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/data/model/region_data.py` & `pyluba-0.0.8/pyluba/data/model/region_data.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/data/mqtt/event.py` & `pyluba-0.0.8/pyluba/data/mqtt/event.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from base64 import b64decode
+from dataclasses import dataclass
 from typing import Literal, Any, Union
 
-from pydantic import BaseModel
-
 from pyluba.proto import luba_msg_pb2
 
+from mashumaro.mixins.orjson import DataClassORJSONMixin
 
 class Base64EncodedProtobuf:
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
@@ -16,26 +16,26 @@
         if not isinstance(v, str):
             raise TypeError("string required")
         binary = b64decode(v, validate=True)
         data = luba_msg_pb2.LubaMsg()
         data.ParseFromString(binary)
         return data
 
-
-class DeviceProtobufMsgEventValue(BaseModel):
+@dataclass
+class DeviceProtobufMsgEventValue(DataClassORJSONMixin):
     content: Base64EncodedProtobuf
 
-
-class DeviceWarningEventValue(BaseModel):
+@dataclass
+class DeviceWarningEventValue(DataClassORJSONMixin):
     # TODO: enum for error codes
     # (see resources/res/values-en-rUS/strings.xml in APK)
     code: int
 
 
-class GeneralParams(BaseModel):
+class GeneralParams(DataClassORJSONMixin):
     identifier: str
     groupIdList: list[str]
     groupId: str
     categoryKey: Literal["LawnMower"]
     batchId: str
     gmtCreate: int
     productKey: str
@@ -59,13 +59,13 @@
 
 
 class DeviceWarningEventParams(GeneralParams):
     identifier: Literal["device_warning_event"]
     type: Literal["alert"]
     value: DeviceWarningEventValue
 
-
-class ThingEventMessage(BaseModel):
+@dataclass
+class ThingEventMessage(DataClassORJSONMixin):
     method: Literal["thing.events"]
     id: str
     params: Union[DeviceProtobufMsgEventParams, DeviceWarningEventParams]
     version: Literal["1.0"]
```

### Comparing `pyluba-0.0.7/pyluba/event/event.py` & `pyluba-0.0.8/pyluba/event/event.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/http/http.py` & `pyluba-0.0.8/pyluba/http/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
+from dataclasses import dataclass
 from typing import TypeVar, Generic, Literal
 
 from aiohttp import ClientSession
-from pydantic import BaseModel
-from pydantic.generics import GenericModel
-
+from mashumaro import DataClassDictMixin
+from mashumaro.mixins.orjson import DataClassORJSONMixin
 
 DataT = TypeVar("DataT")
 
 
-class Response(GenericModel, Generic[DataT]):
+class Response(DataClassDictMixin, Generic[DataT]):
     data: DataT
     code: int
     msg: str
 
-
-class LoginResponseUserInformation(BaseModel):
+@dataclass
+class LoginResponseUserInformation(DataClassORJSONMixin):
     areaCode: str
     domainAbbreviation: str
     email: str
     userId: str
     userAccount: str
     authType: str
 
-
-class LoginResponseData(BaseModel):
+@dataclass
+class LoginResponseData(DataClassORJSONMixin):
     access_token: str
     token_type: Literal["bearer"]
     refresh_token: str
     expires_in: int
     scope: Literal["read"]
     grant_type: Literal["password"]
     authorization_code: str
```

### Comparing `pyluba-0.0.7/pyluba/luba/base.py` & `pyluba-0.0.8/pyluba/luba/base.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/mammotion/devices/luba.py` & `pyluba-0.0.8/pyluba/mammotion/devices/luba.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/mqtt/mqtt.py` & `pyluba-0.0.8/pyluba/mqtt/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/common_pb2.py` & `pyluba-0.0.8/pyluba/proto/common_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/dev_net.proto` & `pyluba-0.0.8/pyluba/proto/dev_net.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/dev_net_pb2.py` & `pyluba-0.0.8/pyluba/proto/dev_net_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/dev_net_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/dev_net_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/luba_msg.proto` & `pyluba-0.0.8/pyluba/proto/luba_msg.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/luba_msg_pb2.py` & `pyluba-0.0.8/pyluba/proto/luba_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/luba_msg_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/luba_msg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/luba_mul.proto` & `pyluba-0.0.8/pyluba/proto/luba_mul.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/luba_mul_pb2.py` & `pyluba-0.0.8/pyluba/proto/luba_mul_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/luba_mul_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/luba_mul_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_driver.proto` & `pyluba-0.0.8/pyluba/proto/mctrl_driver.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_driver_pb2.py` & `pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_driver_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/mctrl_driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_nav.proto` & `pyluba-0.0.8/pyluba/proto/mctrl_nav.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_nav_pb2.py` & `pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_nav_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/mctrl_nav_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_ota.proto` & `pyluba-0.0.8/pyluba/proto/mctrl_ota.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_ota_pb2.py` & `pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_ota_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/mctrl_ota_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_pept.proto` & `pyluba-0.0.8/pyluba/proto/mctrl_pept.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_pept_pb2.py` & `pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_pept_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/mctrl_pept_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_sys.proto` & `pyluba-0.0.8/pyluba/proto/mctrl_sys.proto`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_sys_pb2.py` & `pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/proto/mctrl_sys_pb2.pyi` & `pyluba-0.0.8/pyluba/proto/mctrl_sys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/utility/constant/device_constant.py` & `pyluba-0.0.8/pyluba/utility/constant/device_constant.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/utility/periodic.py` & `pyluba-0.0.8/pyluba/utility/periodic.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyluba/utility/rocker_util.py` & `pyluba-0.0.8/pyluba/utility/rocker_util.py`

 * *Files identical despite different names*

### Comparing `pyluba-0.0.7/pyproject.toml` & `pyluba-0.0.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name        = "pyluba"
-version     = "0.0.7"
+version     = "0.0.8"
 license     = "GNU-3.0"
 description = ""
 readme      = "README.md"
 authors     = [
     "Michael Arthur <michael@jumblesoft.co.nz>",
     "Jan Dalheimer <jan@dalheimer.de>"
 ]
@@ -12,34 +12,34 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
 bleak = "^0.21.1"
 protobuf = ">=4.23.1"
 py-jsonic = "^0.0.2"
-pydantic = "^2.7.1"
 aliyun-python-sdk-iot = "^8.57.0"
 aliyun-iot-linkkit = "^1.2.12"
 aiohttp = "^3.9.1"
 paho-mqtt = "^1.6.1"
 alicloud-gateway-iot = "^1.0.0"
 alibabacloud-apigateway-util = "^0.0.2"
 alibabacloud-iot-api-gateway = "^0.0.4"
 bleak-retry-connector = "^3.5.0"
 jsonic = "^1.0.0"
+mashumaro = "^3.13"
+orjson = "^3.10.3"
 
 
 [tool.poetry.group.dev.dependencies]
 types-protobuf = "^4.23.0.1"
 mypy-protobuf = "^3.4.0"
 twine = "^5.0.0"
 bumpver = "^2023.1129"
 frida-tools = "^12.3.0"
 grpcio-tools = "^1.63.0"
-protobuf-to-pydantic = {version = "^0.2.6.2", extras = ["mypy-protobuf"]}
 
 
 [tool.bumpver]
 current_version = "0.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
```

### Comparing `pyluba-0.0.7/PKG-INFO` & `pyluba-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyluba
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 License: GNU-3.0
 Author: Michael Arthur
 Author-email: michael@jumblesoft.co.nz
 Requires-Python: >=3.11,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -15,18 +15,19 @@
 Requires-Dist: alibabacloud-iot-api-gateway (>=0.0.4,<0.0.5)
 Requires-Dist: alicloud-gateway-iot (>=1.0.0,<2.0.0)
 Requires-Dist: aliyun-iot-linkkit (>=1.2.12,<2.0.0)
 Requires-Dist: aliyun-python-sdk-iot (>=8.57.0,<9.0.0)
 Requires-Dist: bleak (>=0.21.1,<0.22.0)
 Requires-Dist: bleak-retry-connector (>=3.5.0,<4.0.0)
 Requires-Dist: jsonic (>=1.0.0,<2.0.0)
+Requires-Dist: mashumaro (>=3.13,<4.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: protobuf (>=4.23.1)
 Requires-Dist: py-jsonic (>=0.0.2,<0.0.3)
-Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![SemVer 0.8.5][img_version]][url_version]
 [![PyPI Releases][img_pypi]][url_pypi]
 [![Supported Python Versions][img_pyversions]][url_pyversions]
 
 [img_version]: https://img.shields.io/static/v1.svg?label=SemVer&message=0.0.1&color=blue
```

