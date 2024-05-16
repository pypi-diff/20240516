# Comparing `tmp/PythonToSW-1.1.1.tar.gz` & `tmp/PythonToSW-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.1.1.tar", last modified: Wed May 15 22:18:07 2024, max compression
+gzip compressed data, was "PythonToSW-1.1.2.tar", last modified: Wed May 15 22:30:08 2024, max compression
```

## Comparing `PythonToSW-1.1.1.tar` & `PythonToSW-1.1.2.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.585254 PythonToSW-1.1.1/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1731 2024-05-15 22:18:07.584507 PythonToSW-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.1.1/README.md
--rw-rw-rw-   0        0        0        5 2024-05-15 22:18:04.000000 PythonToSW-1.1.1/VERSION
--rw-rw-rw-   0        0        0       52 2024-05-15 22:15:14.000000 PythonToSW-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 22:18:07.585254 PythonToSW-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.504328 PythonToSW-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.511925 PythonToSW-1.1.1/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.540181 PythonToSW-1.1.1/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.1.1/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.1.1/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    11081 2024-05-15 22:13:20.000000 PythonToSW-1.1.1/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.583015 PythonToSW-1.1.1/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.1.1/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.1.1/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     4946 2024-05-15 22:09:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.1.1/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.1.1/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.1.1/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehiclePos.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.1.1/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.1.1/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.583761 PythonToSW-1.1.1/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3277 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 22:30:08.523331 PythonToSW-1.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1731 2024-05-15 22:30:08.521839 PythonToSW-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.1.2/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-15 22:30:04.000000 PythonToSW-1.1.2/VERSION
+-rw-rw-rw-   0        0        0       52 2024-05-15 22:15:14.000000 PythonToSW-1.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:30:08.523331 PythonToSW-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:30:08.446117 PythonToSW-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 22:30:08.454275 PythonToSW-1.1.2/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:30:08.475009 PythonToSW-1.1.2/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.1.2/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.1.2/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    11087 2024-05-15 22:27:06.000000 PythonToSW-1.1.2/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:30:08.520344 PythonToSW-1.1.2/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.1.2/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.1.2/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     5068 2024-05-15 22:29:25.000000 PythonToSW-1.1.2/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.1.2/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.1.2/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.1.2/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.1.2/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1018 2024-05-15 22:28:57.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getCurrency.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1083 2024-05-15 22:28:49.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleGroup.py
+-rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.1.2/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1115 2024-05-15 22:28:48.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setCurrency.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.1.2/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.1.2/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.1.2/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:30:08.521091 PythonToSW-1.1.2/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-05-15 22:30:08.000000 PythonToSW-1.1.2/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3404 2024-05-15 22:30:08.000000 PythonToSW-1.1.2/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:30:08.000000 PythonToSW-1.1.2/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 22:30:08.000000 PythonToSW-1.1.2/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 22:30:08.000000 PythonToSW-1.1.2/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.1.1/LICENSE` & `PythonToSW-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/PKG-INFO` & `PythonToSW-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.1.1/README.md` & `PythonToSW-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/setup.py` & `PythonToSW-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/__init__.py` & `PythonToSW-1.1.2/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/addon/script.lua` & `PythonToSW-1.1.2/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/addon.py` & `PythonToSW-1.1.2/src/PythonToSW/addon.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         
         self.pendingExecutions: dict[str, executions.BaseExecution] = {}
         self.callbacks: dict[str, Event] = {}
         
         self.showStartupMessage = showStartupMessage
         
     # Start the addon
-    def start(self, codeFunc: "function"):
+    def start(self, target: "function"):
         if self.running:
             raise exceptions.FailedStartAttempt("Addon is already running")
         
         # set running
         self.running = True
         
         # setup addon
@@ -72,18 +72,18 @@
         self.__setupRoutes()
         
         # hide flask output
         self.__hideFlaskOutput()
         
         # show message
         if self.showStartupMessage:
-            print(f"[PythonToSW] {self.addonName} has started, listening on port {self.port}. Create a save with your addon enabled in Stormworks and keep this running.")
+            print(f"[PythonToSW] '{self.addonName}' (addon) has started, listening on port {self.port}. Create a save with your addon enabled in Stormworks and keep this running.")
         
         # start server
-        threading.Thread(target = codeFunc).start()
+        threading.Thread(target = target).start()
         self.app.run(host = "127.0.0.1", port = self.port, threaded = True)
         
     # Execute a server function in the addon
     def execute(self, execution: executions.BaseExecution):
         # check if addon is running
         if not self.running:
             raise exceptions.FailedExecutionAttempt("Attempted to execute server function when addon is not running")
```

### Comparing `PythonToSW-1.1.1/src/PythonToSW/event.py` & `PythonToSW-1.1.2/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/exceptions.py` & `PythonToSW-1.1.2/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/__createExecution.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/__generateImportCode.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,24 +83,26 @@
 from .clearOilSpills import ClearOilSpills
 from .clearRadiation import ClearRadiation
 from .clearVehicles import ClearVehicles
 from .despawnObject import DespawnObject
 from .despawnVehicle import DespawnVehicle
 from .despawnVehicleGroup import DespawnVehicleGroup
 from .getCharacterItem import GetCharacterItem
+from .getCurrency import GetCurrency
 from .getObjectData import GetObjectData
 from .getPlayerCharacter import GetPlayerCharacter
 from .getPlayerPos import GetPlayerPos
 from .getPlayers import GetPlayers
 from .getSeasonalEvent import GetSeasonalEvent
 from .getUniqueID import GetUniqueID
 from .getVehicleBatteryByName import GetVehicleBatteryByName
 from .getVehicleBatteryByVoxel import GetVehicleBatteryByVoxel
 from .getVehicleComponents import GetVehicleComponents
 from .getVehicleData import GetVehicleData
+from .getVehicleGroup import GetVehicleGroup
 from .getVehiclePos import GetVehiclePos
 from .getVehicleTankByName import GetVehicleTankByName
 from .getVehicleTankByVoxel import GetVehicleTankByVoxel
 from .isAridDLC import IsAridDLC
 from .isSpaceDLC import IsSpaceDLC
 from .isWeaponsDLC import IsWeaponsDLC
 from .notify import Notify
@@ -110,14 +112,15 @@
 from .removeMapLine import RemoveMapLine
 from .removeMapObject import RemoveMapObject
 from .removePopup import RemovePopup
 from .setCharacterData import SetCharacterData
 from .setCharacterItem import SetCharacterItem
 from .setCharacterTooltip import SetCharacterTooltip
 from .setCreatureMoveTarget import SetCreatureMoveTarget
+from .setCurrency import SetCurrency
 from .setOilSpill import SetOilSpill
 from .setPlayerPos import SetPlayerPos
 from .setPopup import SetPopup
 from .setVehicleBatteryByName import SetVehicleBatteryByName
 from .setVehicleBatteryByVoxel import SetVehicleBatteryByName
 from .setVehicleEditable import SetVehicleEditable
 from .setVehicleInvulnerable import SetVehicleInvulnerable
```

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/announce.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/cancelGerstner.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/despawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/despawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getObjectData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehiclePos.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/notify.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/notify.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setCharacterData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehiclePos.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehiclePos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnCreature.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnCreature.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnExplosion.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnExplosion.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteor.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnMeteor.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnTsunami.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnTsunami.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnVolcano.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnVolcano.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/executions/spawnWhirlpool.py` & `PythonToSW-1.1.2/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/helpers.py` & `PythonToSW-1.1.2/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW/matrix.py` & `PythonToSW-1.1.2/src/PythonToSW/matrix.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.1/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.1.2/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.1.1
+Version: 1.1.2
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.1.1/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.1.2/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,24 +30,26 @@
 src/PythonToSW/executions/clearOilSpills.py
 src/PythonToSW/executions/clearRadiation.py
 src/PythonToSW/executions/clearVehicles.py
 src/PythonToSW/executions/despawnObject.py
 src/PythonToSW/executions/despawnVehicle.py
 src/PythonToSW/executions/despawnVehicleGroup.py
 src/PythonToSW/executions/getCharacterItem.py
+src/PythonToSW/executions/getCurrency.py
 src/PythonToSW/executions/getObjectData.py
 src/PythonToSW/executions/getPlayerCharacter.py
 src/PythonToSW/executions/getPlayerPos.py
 src/PythonToSW/executions/getPlayers.py
 src/PythonToSW/executions/getSeasonalEvent.py
 src/PythonToSW/executions/getUniqueID.py
 src/PythonToSW/executions/getVehicleBatteryByName.py
 src/PythonToSW/executions/getVehicleBatteryByVoxel.py
 src/PythonToSW/executions/getVehicleComponents.py
 src/PythonToSW/executions/getVehicleData.py
+src/PythonToSW/executions/getVehicleGroup.py
 src/PythonToSW/executions/getVehiclePos.py
 src/PythonToSW/executions/getVehicleTankByName.py
 src/PythonToSW/executions/getVehicleTankByVoxel.py
 src/PythonToSW/executions/isAridDLC.py
 src/PythonToSW/executions/isSpaceDLC.py
 src/PythonToSW/executions/isWeaponsDLC.py
 src/PythonToSW/executions/notify.py
@@ -57,14 +59,15 @@
 src/PythonToSW/executions/removeMapLine.py
 src/PythonToSW/executions/removeMapObject.py
 src/PythonToSW/executions/removePopup.py
 src/PythonToSW/executions/setCharacterData.py
 src/PythonToSW/executions/setCharacterItem.py
 src/PythonToSW/executions/setCharacterTooltip.py
 src/PythonToSW/executions/setCreatureMoveTarget.py
+src/PythonToSW/executions/setCurrency.py
 src/PythonToSW/executions/setOilSpill.py
 src/PythonToSW/executions/setPlayerPos.py
 src/PythonToSW/executions/setPopup.py
 src/PythonToSW/executions/setVehicleBatteryByName.py
 src/PythonToSW/executions/setVehicleBatteryByVoxel.py
 src/PythonToSW/executions/setVehicleEditable.py
 src/PythonToSW/executions/setVehicleInvulnerable.py
```

