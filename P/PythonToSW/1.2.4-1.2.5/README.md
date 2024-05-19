# Comparing `tmp/PythonToSW-1.2.4.tar.gz` & `tmp/PythonToSW-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.2.4.tar", last modified: Fri May 17 07:35:19 2024, max compression
+gzip compressed data, was "PythonToSW-1.2.5.tar", last modified: Sun May 19 10:58:28 2024, max compression
```

## Comparing `PythonToSW-1.2.4.tar` & `PythonToSW-1.2.5.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:35:19.370020 PythonToSW-1.2.4/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.4/LICENSE
--rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1803 2024-05-17 07:35:19.369256 PythonToSW-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.4/README.md
--rw-rw-rw-   0        0        0        5 2024-05-17 07:35:05.000000 PythonToSW-1.2.4/VERSION
--rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 07:35:19.370020 PythonToSW-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:35:19.224239 PythonToSW-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:35:19.251144 PythonToSW-1.2.4/src/PythonToSW/
--rw-rw-rw-   0        0        0     1136 2024-05-17 02:54:27.000000 PythonToSW-1.2.4/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:35:19.277704 PythonToSW-1.2.4/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.4/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.4/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    21012 2024-05-17 07:34:55.000000 PythonToSW-1.2.4/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     3176 2024-05-17 07:31:58.000000 PythonToSW-1.2.4/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1247 2024-05-17 03:19:53.000000 PythonToSW-1.2.4/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:35:19.366966 PythonToSW-1.2.4/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.4/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.2.4/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     7408 2024-05-17 07:31:58.000000 PythonToSW-1.2.4/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.4/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.4/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.4/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.4/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getAddonIndex.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getCurrency.py
--rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getGameSettings.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerLookDirection.py
--rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerName.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleGroup.py
--rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/moveGroup.py
--rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/moveGroupSafe.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/moveVehicle.py
--rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.4/src/PythonToSW/executions/moveVehicleSafe.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.4/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setCurrency.py
--rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setGameSetting.py
--rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setGroupPosSafe.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehiclePos.py
--rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehiclePosSafe.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnAddonVehicle.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnEquipment.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnObject.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnVehicle.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.4/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     2688 2024-05-17 07:20:38.000000 PythonToSW-1.2.4/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     2157 2024-05-17 07:25:51.000000 PythonToSW-1.2.4/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:35:19.367713 PythonToSW-1.2.4/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1803 2024-05-17 07:35:19.000000 PythonToSW-1.2.4/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4065 2024-05-17 07:35:19.000000 PythonToSW-1.2.4/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:35:19.000000 PythonToSW-1.2.4/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-17 07:35:19.000000 PythonToSW-1.2.4/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-17 07:35:19.000000 PythonToSW-1.2.4/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.137231 PythonToSW-1.2.5/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1865 2024-05-19 10:58:28.135735 PythonToSW-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-05-16 22:19:42.000000 PythonToSW-1.2.5/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-19 10:57:13.000000 PythonToSW-1.2.5/VERSION
+-rw-rw-rw-   0        0        0       62 2024-05-16 22:06:47.000000 PythonToSW-1.2.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 10:58:28.137231 PythonToSW-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2072 2024-05-19 10:58:18.000000 PythonToSW-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:58:27.996763 PythonToSW-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.008403 PythonToSW-1.2.5/src/PythonToSW/
+-rw-rw-rw-   0        0        0     6348 2024-05-17 09:46:54.000000 PythonToSW-1.2.5/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.036634 PythonToSW-1.2.5/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      315 2024-05-16 03:46:54.000000 PythonToSW-1.2.5/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   161117 2024-05-16 21:57:12.000000 PythonToSW-1.2.5/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    21012 2024-05-17 07:34:55.000000 PythonToSW-1.2.5/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     3176 2024-05-17 07:31:58.000000 PythonToSW-1.2.5/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1247 2024-05-17 03:19:53.000000 PythonToSW-1.2.5/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.133464 PythonToSW-1.2.5/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.2.5/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1732 2024-05-17 09:47:00.000000 PythonToSW-1.2.5/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     3893 2024-05-17 09:47:29.000000 PythonToSW-1.2.5/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.2.5/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.2.5/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1025 2024-05-16 04:08:52.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getAddonIndex.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getCurrency.py
+-rw-rw-rw-   0        0        0     1031 2024-05-16 22:21:02.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getGameSettings.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerLookDirection.py
+-rw-rw-rw-   0        0        0     1075 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerName.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleGroup.py
+-rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1080 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveGroup.py
+-rw-rw-rw-   0        0        0     1093 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveGroupSafe.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicle.py
+-rw-rw-rw-   0        0        0     1103 2024-05-16 00:02:01.000000 PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicleSafe.py
+-rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.2.5/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setCurrency.py
+-rw-rw-rw-   0        0        0     1120 2024-05-16 22:20:48.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setGameSetting.py
+-rw-rw-rw-   0        0        0     1100 2024-05-16 00:01:49.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setGroupPosSafe.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1110 2024-05-16 00:01:47.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePosSafe.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1122 2024-05-16 04:03:12.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnAddonVehicle.py
+-rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1157 2024-05-16 04:03:12.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnEquipment.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1090 2024-05-16 04:03:13.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnObject.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1089 2024-05-16 04:03:12.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnVehicle.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.2.5/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     2688 2024-05-17 07:20:38.000000 PythonToSW-1.2.5/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     2157 2024-05-17 07:25:51.000000 PythonToSW-1.2.5/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-19 10:58:28.134240 PythonToSW-1.2.5/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1865 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4065 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-19 10:58:27.000000 PythonToSW-1.2.5/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.2.4/LICENSE` & `PythonToSW-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/PKG-INFO` & `PythonToSW-1.2.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.4
+Version: 1.2.5
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
+Project-URL: Source code, https://github.com/cuh4/PythonToSW
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 Requires-Dist: requests
```

### Comparing `PythonToSW-1.2.4/README.md` & `PythonToSW-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/setup.py` & `PythonToSW-1.2.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,34 +24,40 @@
 # ---- // Imports
 import os
 from setuptools import setup, find_packages
 
 # ---- // Variables
 with open(os.path.join(os.path.dirname(__file__), "VERSION"), encoding = "utf-8") as file:
     version = file.read()
-    print(version)
     
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding = "utf-8") as file:
     long_description = file.read()
+    
+with open(os.path.join(os.path.dirname(__file__), "requirements.txt"), encoding = "utf-8") as file:
+    requirements = file.read().splitlines()
 
 # ---- // Main
 setup(
-    name= "PythonToSW",
+    name = "PythonToSW",
     version = version,
     author = "Cuh4",
     description = "A package that allows you to create addons in Stormworks with Python, handled through HTTP.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = find_packages(where = "src"),
     license = "Apache License 2.0",
     
     classifiers = [
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     
-    install_requires = open("requirements.txt").read().splitlines(),
+    project_urls = {
+        "Source code": "https://github.com/cuh4/PythonToSW"
+    },
+
+    install_requires = requirements,
 
     python_requires = ">=3.12",
     include_package_data = True,
     package_dir = {"": "src"}
 )
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/__init__.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # ----------------------------------------
-# [PythonToSW] Init
+# [PythonToSW] Set Vehicle Editable
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
-A Python package that allows you to make Stormworks addons with Python.
-The source code as well as examples can be found at https://github.com/Cuh4/PythonToSW
-
 Copyright (C) 2024 Cuh4
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
@@ -21,13 +18,16 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from .executions import *
-from .event import Event
-from .addon import Addon
-from . import exceptions
-from . import helpers
-from . import matrix
+from . import BaseExecution
+
+# ---- // Main
+class SetVehicleEditable(BaseExecution):
+    def __init__(self, vehicle_id: int, isEditable: bool):
+        super().__init__(
+            functionName = "setVehicleEditable",
+            arguments = [vehicle_id, isEditable]
+        )
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/addon/script.lua` & `PythonToSW-1.2.5/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/addon.py` & `PythonToSW-1.2.5/src/PythonToSW/addon.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/event.py` & `PythonToSW-1.2.5/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/exceptions.py` & `PythonToSW-1.2.5/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/__createExecution.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/__generateImportCode.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if content[pos] == "(":
             break
         
         className += content[pos]
         pos += 1
     
     # format into import statement
-    contents.append(f"from .{os.path.splitext(file)[0]} import {className}")
+    contents.append(f"from PythonToSW.executions.{os.path.splitext(file)[0]} import {className}")
     
 # convert contents to string
 contents = "\n".join(contents)
 
 # print and copy
 print(contents)
 pyperclip.copy(contents)
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.2.5/src/PythonToSW/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # [PythonToSW] Init
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
-A sub-package containing preset executions for you to use in your code.
+A Python package that allows you to make Stormworks addons with Python.
+The source code as well as examples can be found at https://github.com/Cuh4/PythonToSW
 
 Copyright (C) 2024 Cuh4
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -20,188 +21,94 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 # ---- // Imports
-from .. import exceptions
-
-from uuid import uuid4
-import time
-
-# ---- // Main
-class BaseExecution():
-    """
-    Represents an execution that can be sent to the in-game addon.
-
-    You never really need to use this directly. If there is an in-game
-    function that doesn't have an execution, create an execution that
-    inherits from this. Example:
-    
-    >>> class MoveGroup(BaseExecution):
-    >>>     def __init__(self, group_id: int, pos: list):
-    >>>         super().__init__(
-    >>>             functionName = "moveGroup",
-    >>>             arguments = [group_id, pos]
-    >>>         )
-    
-    Args:
-        functionName: (str) The name of the in-game function to call
-        arguments: (list) The arguments to pass to the in-game function
-    """
-
-    def __init__(self, functionName: str, arguments: list = []):
-        self.ID = str(uuid4())
-        self.functionName = functionName
-        self.arguments = arguments
-        
-        self.handled = False
-        self.returnValues = []
-        self.isWaiting = False
-        
-    def __str__(self):
-        return f"Execution-{self.ID} ({self.functionName})"
-        
-    def _toDict(self):
-        """
-        Converts this execution into a dictionary that can be sent to the addon
-        
-        Returns:
-            (dict) The dictionary representation of this execution
-        """
-
-        return {
-            "ID" : self.ID,
-            "functionName": self.functionName,
-            "arguments": self.arguments,
-            "handled": self.handled
-        }
-        
-    def _return(self, returnValues: list):
-        """
-        Marks this execution as handled and saves return values.
-        
-        Args:
-            returnValues: (list) The return values from the in-game function.
-            
-        Raises:
-            exceptions.InternalError: Raised if this method is called when the execution is already handled.
-        """
-
-        if self.handled:
-            raise exceptions.InternalError("Tried to return after already returning")
-        
-        self.handled = True
-        self.returnValues = returnValues
-    
-    def _halt(self):
-        """
-        Stops waiting on this execution via _wait() method.
-        """
-
-        self.isWaiting = False
-        
-    def _obsolete(self):
-        """
-        Returns whether this execution has been handled.
-        
-        Returns:
-            (bool) Whether this execution has been handled.
-        """
-
-        return not self.isWaiting
-        
-    def _wait(self) -> list:
-        """
-        Waits until this execution has been handled and returns the return values.
-        
-        Returns:
-            (list) The return values from the in-game function call.
-        """
-
-        self.isWaiting = True
-        
-        while not self.handled and self.isWaiting:
-            time.sleep(0.01)
-            
-        return self.returnValues
-    
-# ---- // Other Executions
-from .addAdmin import AddAdmin
-from .addAuth import AddAuth
-from .addMapLabel import AddMapLabel
-from .addMapLine import AddMapLine
-from .addMapObject import AddMapObject
-from .announce import Announce
-from .cancelGerstner import CancelGerstner
-from .clearOilSpills import ClearOilSpills
-from .clearRadiation import ClearRadiation
-from .clearVehicles import ClearVehicles
-from .despawnObject import DespawnObject
-from .despawnVehicle import DespawnVehicle
-from .despawnVehicleGroup import DespawnVehicleGroup
-from .getAddonIndex import GetAddonIndex
-from .getCharacterItem import GetCharacterItem
-from .getCurrency import GetCurrency
-from .getGameSettings import GetGameSettings
-from .getObjectData import GetObjectData
-from .getPlayerCharacter import GetPlayerCharacter
-from .getPlayerLookDirection import GetPlayerLookDirection
-from .getPlayerName import GetPlayerName
-from .getPlayerPos import GetPlayerPos
-from .getPlayers import GetPlayers
-from .getSeasonalEvent import GetSeasonalEvent
-from .getUniqueID import GetUniqueID
-from .getVehicleBatteryByName import GetVehicleBatteryByName
-from .getVehicleBatteryByVoxel import GetVehicleBatteryByVoxel
-from .getVehicleComponents import GetVehicleComponents
-from .getVehicleData import GetVehicleData
-from .getVehicleGroup import GetVehicleGroup
-from .getVehiclePos import GetVehiclePos
-from .getVehicleTankByName import GetVehicleTankByName
-from .getVehicleTankByVoxel import GetVehicleTankByVoxel
-from .isAridDLC import IsAridDLC
-from .isSpaceDLC import IsSpaceDLC
-from .isWeaponsDLC import IsWeaponsDLC
-from .moveGroup import MoveGroup
-from .moveGroupSafe import MoveGroupSafe
-from .moveVehicle import MoveVehicle
-from .moveVehicleSafe import MoveVehicleSafe
-from .notify import Notify
-from .removeAdmin import RemoveAdmin
-from .removeAuth import RemoveAuth
-from .removeMapLabel import RemoveMapLabel
-from .removeMapLine import RemoveMapLine
-from .removeMapObject import RemoveMapObject
-from .removePopup import RemovePopup
-from .setCharacterData import SetCharacterData
-from .setCharacterItem import SetCharacterItem
-from .setCharacterTooltip import SetCharacterTooltip
-from .setCreatureMoveTarget import SetCreatureMoveTarget
-from .setCurrency import SetCurrency
-from .setGameSetting import SetGameSetting
-from .setGroupPosSafe import SetGroupPosSafe
-from .setOilSpill import SetOilSpill
-from .setPlayerPos import SetPlayerPos
-from .setPopup import SetPopup
-from .setVehicleBatteryByName import SetVehicleBatteryByName
-from .setVehicleBatteryByVoxel import SetVehicleBatteryByName
-from .setVehicleEditable import SetVehicleEditable
-from .setVehicleInvulnerable import SetVehicleInvulnerable
-from .setVehiclePos import SetVehiclePos
-from .setVehiclePosSafe import SetVehiclePosSafe
-from .setVehicleShowOnMap import SetVehicleShowOnMap
-from .setVehicleTankByName import SetVehicleTankByName
-from .setVehicleTankByVoxel import SetVehicleTankByVoxel
-from .spawnAddonVehicle import SpawnAddonVehicle
-from .spawnCharacter import SpawnCharacter
-from .spawnCreature import SpawnCreature
-from .spawnEquipment import SpawnEquipment
-from .spawnExplosion import SpawnExplosion
-from .spawnMeteor import SpawnMeteor
-from .spawnMeteorShower import SpawnMeteorShower
-from .spawnObject import SpawnObject
-from .spawnTsunami import SpawnTsunami
-from .spawnVehicle import SpawnVehicle
-from .spawnVolcano import SpawnVolcano
-from .spawnWhirlpool import SpawnWhirlpool
+# Main
+from PythonToSW.event import Event
+from PythonToSW.addon import Addon
+from PythonToSW import exceptions
+from PythonToSW import helpers
+from PythonToSW import matrix
+
+# Executions
+from PythonToSW.executions import BaseExecution
+from PythonToSW.executions.addAdmin import AddAdmin
+from PythonToSW.executions.addAuth import AddAuth
+from PythonToSW.executions.addMapLabel import AddMapLabel
+from PythonToSW.executions.addMapLine import AddMapLine
+from PythonToSW.executions.addMapObject import AddMapObject
+from PythonToSW.executions.announce import Announce
+from PythonToSW.executions.cancelGerstner import CancelGerstner
+from PythonToSW.executions.clearOilSpills import ClearOilSpills
+from PythonToSW.executions.clearRadiation import ClearRadiation
+from PythonToSW.executions.clearVehicles import ClearVehicles
+from PythonToSW.executions.despawnObject import DespawnObject
+from PythonToSW.executions.despawnVehicle import DespawnVehicle
+from PythonToSW.executions.despawnVehicleGroup import DespawnVehicleGroup
+from PythonToSW.executions.getAddonIndex import GetAddonIndex
+from PythonToSW.executions.getCharacterItem import GetCharacterItem
+from PythonToSW.executions.getCurrency import GetCurrency
+from PythonToSW.executions.getGameSettings import GetGameSettings
+from PythonToSW.executions.getObjectData import GetObjectData
+from PythonToSW.executions.getPlayerCharacter import GetPlayerCharacter
+from PythonToSW.executions.getPlayerLookDirection import GetPlayerLookDirection
+from PythonToSW.executions.getPlayerName import GetPlayerName
+from PythonToSW.executions.getPlayerPos import GetPlayerPos
+from PythonToSW.executions.getPlayers import GetPlayers
+from PythonToSW.executions.getSeasonalEvent import GetSeasonalEvent
+from PythonToSW.executions.getUniqueID import GetUniqueID
+from PythonToSW.executions.getVehicleBatteryByName import GetVehicleBatteryByName
+from PythonToSW.executions.getVehicleBatteryByVoxel import GetVehicleBatteryByVoxel
+from PythonToSW.executions.getVehicleComponents import GetVehicleComponents
+from PythonToSW.executions.getVehicleData import GetVehicleData
+from PythonToSW.executions.getVehicleGroup import GetVehicleGroup
+from PythonToSW.executions.getVehiclePos import GetVehiclePos
+from PythonToSW.executions.getVehicleTankByName import GetVehicleTankByName
+from PythonToSW.executions.getVehicleTankByVoxel import GetVehicleTankByVoxel
+from PythonToSW.executions.isAridDLC import IsAridDLC
+from PythonToSW.executions.isSpaceDLC import IsSpaceDLC
+from PythonToSW.executions.isWeaponsDLC import IsWeaponsDLC
+from PythonToSW.executions.moveGroup import MoveGroup
+from PythonToSW.executions.moveGroupSafe import MoveGroupSafe
+from PythonToSW.executions.moveVehicle import MoveVehicle
+from PythonToSW.executions.moveVehicleSafe import MoveVehicleSafe
+from PythonToSW.executions.notify import Notify
+from PythonToSW.executions.removeAdmin import RemoveAdmin
+from PythonToSW.executions.removeAuth import RemoveAuth
+from PythonToSW.executions.removeMapLabel import RemoveMapLabel
+from PythonToSW.executions.removeMapLine import RemoveMapLine
+from PythonToSW.executions.removeMapObject import RemoveMapObject
+from PythonToSW.executions.removePopup import RemovePopup
+from PythonToSW.executions.setCharacterData import SetCharacterData
+from PythonToSW.executions.setCharacterItem import SetCharacterItem
+from PythonToSW.executions.setCharacterTooltip import SetCharacterTooltip
+from PythonToSW.executions.setCreatureMoveTarget import SetCreatureMoveTarget
+from PythonToSW.executions.setCurrency import SetCurrency
+from PythonToSW.executions.setGameSetting import SetGameSetting
+from PythonToSW.executions.setGroupPosSafe import SetGroupPosSafe
+from PythonToSW.executions.setOilSpill import SetOilSpill
+from PythonToSW.executions.setPlayerPos import SetPlayerPos
+from PythonToSW.executions.setPopup import SetPopup
+from PythonToSW.executions.setVehicleBatteryByName import SetVehicleBatteryByName
+from PythonToSW.executions.setVehicleBatteryByVoxel import SetVehicleBatteryByName
+from PythonToSW.executions.setVehicleEditable import SetVehicleEditable
+from PythonToSW.executions.setVehicleInvulnerable import SetVehicleInvulnerable
+from PythonToSW.executions.setVehiclePos import SetVehiclePos
+from PythonToSW.executions.setVehiclePosSafe import SetVehiclePosSafe
+from PythonToSW.executions.setVehicleShowOnMap import SetVehicleShowOnMap
+from PythonToSW.executions.setVehicleTankByName import SetVehicleTankByName
+from PythonToSW.executions.setVehicleTankByVoxel import SetVehicleTankByVoxel
+from PythonToSW.executions.spawnAddonVehicle import SpawnAddonVehicle
+from PythonToSW.executions.spawnCharacter import SpawnCharacter
+from PythonToSW.executions.spawnCreature import SpawnCreature
+from PythonToSW.executions.spawnEquipment import SpawnEquipment
+from PythonToSW.executions.spawnExplosion import SpawnExplosion
+from PythonToSW.executions.spawnMeteor import SpawnMeteor
+from PythonToSW.executions.spawnMeteorShower import SpawnMeteorShower
+from PythonToSW.executions.spawnObject import SpawnObject
+from PythonToSW.executions.spawnTsunami import SpawnTsunami
+from PythonToSW.executions.spawnVehicle import SpawnVehicle
+from PythonToSW.executions.spawnVolcano import SpawnVolcano
+from PythonToSW.executions.spawnWhirlpool import SpawnWhirlpool
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/announce.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/cancelGerstner.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/despawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getAddonIndex.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getAddonIndex.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getCurrency.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getGameSettings.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getGameSettings.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getObjectData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerLookDirection.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerLookDirection.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerName.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleGroup.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehiclePos.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/moveGroup.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/moveGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/moveGroupSafe.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/moveGroupSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/moveVehicle.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/moveVehicleSafe.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/moveVehicleSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/notify.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/notify.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setCurrency.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setCurrency.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setGameSetting.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setGameSetting.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setGroupPosSafe.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setGroupPosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Editable
+# [PythonToSW] Set Vehicle Show On Map
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -21,13 +21,13 @@
 limitations under the License.
 """
 
 # ---- // Imports
 from . import BaseExecution
 
 # ---- // Main
-class SetVehicleEditable(BaseExecution):
-    def __init__(self, vehicle_id: int, isEditable: bool):
+class SetVehicleShowOnMap(BaseExecution):
+    def __init__(self, vehicle_id: int, isShow: bool):
         super().__init__(
-            functionName = "setVehicleEditable",
-            arguments = [vehicle_id, isEditable]
+            functionName = "setVehicleShowOnMap",
+            arguments = [vehicle_id, isShow]
         )
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehiclePos.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehiclePosSafe.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehiclePosSafe.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnObject.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Set Vehicle Show On Map
+# [PythonToSW] Spawn Object
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -21,13 +21,13 @@
 limitations under the License.
 """
 
 # ---- // Imports
 from . import BaseExecution
 
 # ---- // Main
-class SetVehicleShowOnMap(BaseExecution):
-    def __init__(self, vehicle_id: int, isShow: bool):
+class SpawnObject(BaseExecution):
+    def __init__(self, pos: list, objectType: int):
         super().__init__(
-            functionName = "setVehicleShowOnMap",
-            arguments = [vehicle_id, isShow]
+            functionName = "spawnObject",
+            arguments = [pos, objectType]
         )
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnAddonVehicle.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnAddonVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnCreature.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnCreature.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnEquipment.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnEquipment.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnExplosion.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnExplosion.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnMeteor.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteor.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnObject.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ----------------------------------------
-# [PythonToSW] Spawn Object
+# [PythonToSW] Spawn Whirlpool
 # ----------------------------------------
 
 # A Python package that allows you to make Stormworks addons with Python.
 # Repo: https://github.com/Cuh4/PythonToSW
 
 """
 Copyright (C) 2024 Cuh4
@@ -21,13 +21,13 @@
 limitations under the License.
 """
 
 # ---- // Imports
 from . import BaseExecution
 
 # ---- // Main
-class SpawnObject(BaseExecution):
-    def __init__(self, pos: list, objectType: int):
+class SpawnWhirlpool(BaseExecution):
+    def __init__(self, pos: list, magnitude: float):
         super().__init__(
-            functionName = "spawnObject",
-            arguments = [pos, objectType]
+            functionName = "spawnWhirlpool",
+            arguments = [pos, magnitude]
         )
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnTsunami.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnTsunami.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnVehicle.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/executions/spawnVolcano.py` & `PythonToSW-1.2.5/src/PythonToSW/executions/spawnVolcano.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/helpers.py` & `PythonToSW-1.2.5/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW/matrix.py` & `PythonToSW-1.2.5/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.2.4/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.2.5/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.2.4
+Version: 1.2.5
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
+Project-URL: Source code, https://github.com/cuh4/PythonToSW
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyperclip
 Requires-Dist: requests
```

### Comparing `PythonToSW-1.2.4/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.2.5/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files identical despite different names*

