# Comparing `tmp/bttc-0.0.77.4.tar.gz` & `tmp/bttc-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.77.4.tar", last modified: Thu May  9 02:38:52 2024, max compression
+gzip compressed data, was "bttc-0.0.79.tar", last modified: Sun May 19 04:06:50 2024, max compression
```

## Comparing `bttc-0.0.77.4.tar` & `bttc-0.0.79.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77.4/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-09 02:38:52.019067 bttc-0.0.77.4/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-06 13:58:19.000000 bttc-0.0.77.4/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6838 2024-05-09 02:38:42.000000 bttc-0.0.77.4/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77.4/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77.4/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77.4/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77.4/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-08 02:00:40.000000 bttc-0.0.77.4/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    36150 2024-05-06 14:42:05.000000 bttc-0.0.77.4/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.011067 bttc-0.0.77.4/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9130 2024-05-09 02:36:08.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6497 2024-05-09 02:35:18.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77.4/bttc/utils/device_factory.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-07 06:26:37.000000 bttc-0.0.77.4/bttc/utils/dialer_simulator.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77.4/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-08 03:08:22.000000 bttc-0.0.77.4/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.77.4/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77.4/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    17093 2024-05-06 13:58:19.000000 bttc-0.0.77.4/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-09 02:38:52.023067 bttc-0.0.77.4/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77.4/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.79/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2765 2024-05-19 04:06:50.516775 bttc-0.0.79/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2037 2024-05-19 04:05:38.000000 bttc-0.0.79/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6836 2024-05-19 04:06:38.000000 bttc-0.0.79/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    10830 2024-05-19 04:05:38.000000 bttc-0.0.79/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.79/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.79/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.79/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    36248 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.508775 bttc-0.0.79/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9163 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7155 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.79/bttc/utils/device_factory.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/utils/dialer_simulator.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.79/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-11 11:42:51.000000 bttc-0.0.79/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.79/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.516775 bttc-0.0.79/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.79/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    17165 2024-05-19 04:05:38.000000 bttc-0.0.79/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.79/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.79/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-19 04:06:50.512775 bttc-0.0.79/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2765 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-19 04:06:50.000000 bttc-0.0.79/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-19 04:06:50.516775 bttc-0.0.79/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.79/setup.py
```

### Comparing `bttc-0.0.77.4/LICENSE` & `bttc-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/PKG-INFO` & `bttc-0.0.79/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: bttc
-Version: 0.0.77.4
-Summary: A package to provide common utilities for BT testing.
-Home-page: https://github.com/johnklee/bt_test_common
-Author: John Lee/Yuan Long Luo/Denny Chai
-Author-email: puremonkey2007@gmail.com
-License: MIT License
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Common utilities used in BT testing
 This package is used to hold common utilities for BT testing.
 
 ## Installation
 You can install the released package from pip:
 
 ```shell
@@ -60,15 +41,30 @@
 ```shell
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
+### `dut.gm`: Utility used in general operations of device.
+The `dut.gm` utility, loaded automatically when you access your device, streamlines common actions like:
+- Getting/setting device properties
+- Searching logcat messages
+- Managing airplane mode
+- Taking screenshots
+- Dumping system information (build number, model, etc.)
+- And more!
+
+
+### `dut.mc`: Utility to support common Media control operations/methods.
+The `dut.mc` utility, loaded automatically when you access your device, lets you control music playback and get its current state.
+
+
 ## Release info
+* Release v0.0.78: #207, #209, #212, #213, #215, #217
 * Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
```

### Comparing `bttc-0.0.77.4/README.md` & `bttc-0.0.79/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: bttc
+Version: 0.0.79
+Summary: A package to provide common utilities for BT testing.
+Home-page: https://github.com/johnklee/bt_test_common
+Author: John Lee/Yuan Long Luo/Denny Chai
+Author-email: puremonkey2007@gmail.com
+License: MIT License
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Common utilities used in BT testing
 This package is used to hold common utilities for BT testing.
 
 ## Installation
 You can install the released package from pip:
 
 ```shell
@@ -41,15 +60,30 @@
 ```shell
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
+### `dut.gm`: Utility used in general operations of device.
+The `dut.gm` utility, loaded automatically when you access your device, streamlines common actions like:
+- Getting/setting device properties
+- Searching logcat messages
+- Managing airplane mode
+- Taking screenshots
+- Dumping system information (build number, model, etc.)
+- And more!
+
+
+### `dut.mc`: Utility to support common Media control operations/methods.
+The `dut.mc` utility, loaded automatically when you access your device, lets you control music playback and get its current state.
+
+
 ## Release info
+* Release v0.0.78: #207, #209, #212, #213, #215, #217
 * Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
```

### Comparing `bttc-0.0.77.4/bttc/__init__.py` & `bttc-0.0.79/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.77.4'
+__version__ = '0.0.79'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.77.4/bttc/apk_utils.py` & `bttc-0.0.79/bttc/apk_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 AndroidLike = typing_utils.AndroidLike
 BINDING_KEYWORD = 'apk'
 DEFAULT_TIMEOUT_INSTALL_APK_SEC = 300
 MBS_PACKAGE_NAME = 'com.google.android.mobly.snippet.bundled'
 SL4A_PACKAGE_NAME = 'com.googlecode.android_scripting'
 UIAUTOMATOR_PACKAGE_NAME = 'com.google.android.mobly.snippet.uiautomator'
 
+# Error messages from adb.
+ADB_UNINSTALL_INTERNAL_ERROR_MSG = 'DELETE_FAILED_INTERNAL_ERROR'
+
 
 class ApkModule(core.UtilBase):
   """Apk module to hold apk related functions."""
 
   NAME = BINDING_KEYWORD
   DESCRIPTION = 'Utility to support Apk related operations.'
 
@@ -50,14 +53,15 @@
     self._bind(install_mbs)
     self._bind(install_sl4a)
     self._bind(is_package_installed)
     self._bind(is_mbs_installed)
     self._bind(is_sl4a_installed)
     self._bind(is_uiautomator_installed)
     self._bind(list_packages)
+    self._bind(uninstall)
 
 
 def bind(
     ad: AndroidLike | str,
     init_mbs: bool = False,
     init_sl4a: bool = False,
     init_snippet_uiautomator: bool = False,
@@ -324,7 +328,40 @@
   installed_package_set = set()
   for installed_pkg in ad.adb.shell(
       'pm list packages').decode().strip().split('\n'):
     if installed_pkg.startswith('package:'):
       installed_package_set.add(installed_pkg[8:])
 
   return installed_package_set
+
+
+def uninstall(ad: AndroidLike, package_name: str) -> None:
+  """Uninstall an apk on an given device if it is installed.
+
+  Works for regular app and OEM pre-installed non-system app.
+
+  Args:
+    ad: Android like device.
+    package_name: string, package name of the app.
+  """
+  if not is_package_installed(ad, package_name):
+    ad.log.info('Package:%s has been installed!', package_name)
+    return
+
+  try:
+    ad.adb.uninstall([package_name])
+    ad.log.info('Package:%s has been uninstalled successfully!')
+  except adb.AdbError as e1:
+    # This error can happen if the package to uninstall is non-system and
+    # pre-loaded by OEM. Try removing it via PackageManager (pm) under UID 0.
+    if ADB_UNINSTALL_INTERNAL_ERROR_MSG in str(e1):
+      ad.log.debug(
+          'Encountered uninstall internal error, try pm remove '
+          'with UID 0.')
+      try:
+        ad.adb.shell(
+            ['pm', 'uninstall', '-k', '--user', '0', package_name])
+        return
+      except adb.AdbError as e2:
+        ad.log.exception('Second attempt to uninstall failed: %s', e2)
+
+      raise e1
```

### Comparing `bttc-0.0.77.4/bttc/ble_data.py` & `bttc-0.0.79/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/ble_utils.py` & `bttc-0.0.79/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/bt_data.py` & `bttc-0.0.79/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/bt_utils.py` & `bttc-0.0.79/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/cli/__init__.py` & `bttc-0.0.79/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/cli/constants.py` & `bttc-0.0.79/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/cli/main.py` & `bttc-0.0.79/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/common_data.py` & `bttc-0.0.79/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/constants.py` & `bttc-0.0.79/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/core.py` & `bttc-0.0.79/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/errors.py` & `bttc-0.0.79/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/general_data.py` & `bttc-0.0.79/bttc/general_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/general_utils.py` & `bttc-0.0.79/bttc/general_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import bttc
 from bttc import bt_utils
 from bttc import constants
 from bttc import core
 from bttc import errors
 from bttc import general_data
 from bttc.cli.constants import warning
+from bttc.profiles.hfp import hfp_data
 from bttc.utils import device_factory
 from bttc.utils import key_events_handler
 from bttc.utils import log_parser
 from bttc.utils import typing_utils
 from mobly import utils
 
 from mobly.controllers import android_device
@@ -562,15 +563,15 @@
   try:
     return bool(int(shell_output))
   except ValueError as ex:
     device.log.warning("Unknown adb output=%s", ex)
     raise
 
 
-def get_call_state(device: typing_utils.AdbDevice) -> str:
+def get_call_state(device: typing_utils.AdbDevice) -> hfp_data.CallStateEnum:
   """Gets call state from dumpsys telecom log.
 
   For this function to work, we expect below log snippet from given log
   content:
 
   Call state is IDLE:
   ```
@@ -622,15 +623,16 @@
   """
   output = dumpsys(device, "telecom", "mCallAudioManager", "-A11")
   pattern = r"(Ringing) calls:\n\s+TC@\d|Call id=.+state=(\w+)|null"
   match = re.search(pattern, output)
   if match is None:
     raise adb.Error("Failed to execute command for dumpsys telecom")
 
-  return (match.group(1) or match.group(2) or "IDLE").upper()
+  return hfp_data.CallStateEnum.from_str(
+      (match.group(1) or match.group(2) or "IDLE").upper())
 
 
 def get_device_time(
   device: typing_utils.AdbDevice, to_datetime: bool = False
 ) -> str | datetime.datetime:
   """Gets device epoch time and transfer to logcat timestamp format."""
   device_time_str = (
```

### Comparing `bttc-0.0.77.4/bttc/mc_data.py` & `bttc-0.0.79/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/mc_utils.py` & `bttc-0.0.79/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.79/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.79/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.79/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.79/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.79/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.79/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/avrcp/errors.py` & `bttc-0.0.79/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/__init__.py` & `bttc-0.0.79/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/constants.py` & `bttc-0.0.79/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/errors.py` & `bttc-0.0.79/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.79/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.79/bttc/profiles/hfp/hfp_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,16 @@
 
     Args:
       audio_route: Audio route to switch to.
     """
     self._device.sl4a.telecomCallSetAudioRoute(audio_route.value)
 
 
-class AndroidPhoneWithDialerSimulator(AndroidPhone):
+class AndroidPhoneWithDialerSimulator(
+    AndroidPhone, hfp_facade.DialerSimulator):
   """Android with dialer simulator apk installed."""
 
   def __init__(self, device: typing_utils.AndroidLike,
                phone_number: str | None = None):
     super().__init__(device, phone_number)
     self._ds = dialer_simulator.DialerSimulator(device)
```

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.79/bttc/profiles/hfp/hfp_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,40 @@
 from bttc.profiles.hfp import hfp_data
 from bttc.utils import typing_utils
 
 
 _CALL_IDLE = hfp_data.CallStateEnum.IDLE
 
 
+class DialerSimulator(Protocol):
+  """Abstract class for dialer simulator behaviors."""
+
+  def incoming_call(self) -> CallResult:
+    """Simulates incoming call.
+
+    This method is only valid with dialer simulator available in DUT.
+    For details, please refer to go/dialer-simulator
+
+    Returns:
+      dataclass CallResult to represent calling result.
+    """
+    ...
+
+  def outgoing_call(self) -> CallResult:
+    """Simulates outgoing call.
+
+    This method is only valid with dialer simulator available in DUT.
+    For details, please refer to go/dialer-simulator
+
+    Returns:
+      dataclass CallResult to represent calling result.
+    """
+    ...
+
+
 class PhoneDevice(abc.ABC):
   """Abstract phone device for HFP testing.
 
   Attributes:
     phone_number: Phone number of device.
     log: Logger object.
   """
```

### Comparing `bttc-0.0.77.4/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.79/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/strategy.py` & `bttc-0.0.79/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/ad_checker.py` & `bttc-0.0.79/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/device_factory.py` & `bttc-0.0.79/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/dialer_simulator.py` & `bttc-0.0.79/bttc/utils/dialer_simulator.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/iperf/__init__.py` & `bttc-0.0.79/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/iperf/errors.py` & `bttc-0.0.79/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/key_events_handler.py` & `bttc-0.0.79/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/log_parser.py` & `bttc-0.0.79/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/logcat.py` & `bttc-0.0.79/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.79/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.79/bttc/utils/media_player/yt_player_agent.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/retry.py` & `bttc-0.0.79/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/typing_utils.py` & `bttc-0.0.79/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.79/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/ui_pages/errors.py` & `bttc-0.0.79/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.79/bttc/utils/ui_pages/ui_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """UI core module for UI page operations."""
 from __future__ import annotations
 import itertools
+import logging
 import shlex
 from typing import Any, Callable, Generator, Iterable, TypeAlias
 
 from mobly.controllers import android_device
 
 from bttc.utils import ui_pages
 from bttc.utils.ui_pages import errors
@@ -38,14 +39,15 @@
 class UIPage:
   """Object to represent the current UI page."""
 
   def __init__(
       self,
       device: AndroidDevice,
       parsed_ui: ui_pages.ParsedUI | None = None) -> None:
+    self.log = logging.getLogger(self.__class__.__name__)
     self._ad = device
     self._parsed_ui = parsed_ui
     if self._parsed_ui is None:
       self.refresh()
 
   @property
   def ad(self):
@@ -103,15 +105,15 @@
 
     Returns:
       The transformed page object.
     """
     if self.ui_device:
       self.log.debug('Back to previous page by uiautomator...')
       self.ui_device.press.back()
-      return self.get_page()
+      return self.refresh()
 
     self.log.debug('Back to previous page by keycode "BACK"...')
     self.ad.ke.key_back()
     return self.refresh()
 
   def refresh(self) -> UIPage:
     """Refreshes current page with obtained latest page.
```

### Comparing `bttc-0.0.77.4/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.79/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils/ui_pages/utils.py` & `bttc-0.0.79/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/utils_loader.py` & `bttc-0.0.79/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc/wifi_utils.py` & `bttc-0.0.79/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/bttc.egg-info/PKG-INFO` & `bttc-0.0.79/bttc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77.4
+Version: 0.0.79
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -60,15 +60,30 @@
 ```shell
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
+### `dut.gm`: Utility used in general operations of device.
+The `dut.gm` utility, loaded automatically when you access your device, streamlines common actions like:
+- Getting/setting device properties
+- Searching logcat messages
+- Managing airplane mode
+- Taking screenshots
+- Dumping system information (build number, model, etc.)
+- And more!
+
+
+### `dut.mc`: Utility to support common Media control operations/methods.
+The `dut.mc` utility, loaded automatically when you access your device, lets you control music playback and get its current state.
+
+
 ## Release info
+* Release v0.0.78: #207, #209, #212, #213, #215, #217
 * Release v0.0.77: #202
 * Release v0.0.76: #198, #196, #194, #192
 * Release v0.0.75: #64
 * Release v0.0.74: #125, #159, #171, #173, #176, #178, #180
 * Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
```

### Comparing `bttc-0.0.77.4/bttc.egg-info/SOURCES.txt` & `bttc-0.0.79/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.4/setup.py` & `bttc-0.0.79/setup.py`

 * *Files identical despite different names*

