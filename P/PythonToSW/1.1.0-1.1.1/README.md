# Comparing `tmp/PythonToSW-1.1.0.tar.gz` & `tmp/PythonToSW-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToSW-1.1.0.tar", last modified: Tue May 14 23:52:12 2024, max compression
+gzip compressed data, was "PythonToSW-1.1.1.tar", last modified: Wed May 15 22:18:07 2024, max compression
```

## Comparing `PythonToSW-1.1.0.tar` & `PythonToSW-1.1.1.tar`

### file list

```diff
@@ -1,87 +1,90 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 23:52:12.298868 PythonToSW-1.1.0/
--rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       66 2024-05-14 18:04:45.000000 PythonToSW-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1731 2024-05-14 23:52:12.298009 PythonToSW-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.1.0/README.md
--rw-rw-rw-   0        0        0        5 2024-05-14 23:52:02.000000 PythonToSW-1.1.0/VERSION
--rw-rw-rw-   0        0        0       42 2024-05-14 23:52:12.298868 PythonToSW-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1967 2024-05-14 18:02:21.000000 PythonToSW-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:52:12.213220 PythonToSW-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 23:52:12.221277 PythonToSW-1.1.0/src/PythonToSW/
--rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:52:12.251273 PythonToSW-1.1.0/src/PythonToSW/addon/
--rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.1.0/src/PythonToSW/addon/playlist.xml
--rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.1.0/src/PythonToSW/addon/script.lua
--rw-rw-rw-   0        0        0    10866 2024-05-14 18:06:38.000000 PythonToSW-1.1.0/src/PythonToSW/addon.py
--rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/event.py
--rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:52:12.295487 PythonToSW-1.1.0/src/PythonToSW/executions/
--rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.1.0/src/PythonToSW/executions/__createExecution.py
--rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.1.0/src/PythonToSW/executions/__generateImportCode.py
--rw-rw-rw-   0        0        0     4862 2024-05-14 23:51:04.000000 PythonToSW-1.1.0/src/PythonToSW/executions/__init__.py
--rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/addAdmin.py
--rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/addAuth.py
--rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/addMapLabel.py
--rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/addMapLine.py
--rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/addMapObject.py
--rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/announce.py
--rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.1.0/src/PythonToSW/executions/cancelGerstner.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/clearOilSpills.py
--rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/clearRadiation.py
--rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/clearVehicles.py
--rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.1.0/src/PythonToSW/executions/despawnObject.py
--rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.1.0/src/PythonToSW/executions/despawnVehicle.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.1.0/src/PythonToSW/executions/despawnVehicleGroup.py
--rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getCharacterItem.py
--rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getObjectData.py
--rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getPlayerCharacter.py
--rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getPlayerPos.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getPlayers.py
--rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getSeasonalEvent.py
--rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getUniqueID.py
--rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleComponents.py
--rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleData.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleTankByName.py
--rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/isAridDLC.py
--rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/isSpaceDLC.py
--rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/isWeaponsDLC.py
--rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.1.0/src/PythonToSW/executions/notify.py
--rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/removeAdmin.py
--rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/removeAuth.py
--rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/removeMapLabel.py
--rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/removeMapLine.py
--rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/removeMapObject.py
--rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/removePopup.py
--rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setCharacterData.py
--rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setCharacterItem.py
--rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setCharacterTooltip.py
--rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setCreatureMoveTarget.py
--rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setOilSpill.py
--rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setPlayerPos.py
--rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setPopup.py
--rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleBatteryByName.py
--rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
--rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleEditable.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleInvulnerable.py
--rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleShowOnMap.py
--rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleTankByName.py
--rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleTankByVoxel.py
--rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnCharacter.py
--rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnCreature.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnExplosion.py
--rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnMeteor.py
--rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnMeteorShower.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnTsunami.py
--rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnVolcano.py
--rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.1.0/src/PythonToSW/executions/spawnWhirlpool.py
--rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.1.0/src/PythonToSW/helpers.py
--rw-rw-rw-   0        0        0     1058 2024-05-14 16:56:07.000000 PythonToSW-1.1.0/src/PythonToSW/matrix.py
-drwxrwxrwx   0        0        0        0 2024-05-14 23:52:12.296990 PythonToSW-1.1.0/src/PythonToSW.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-05-14 23:52:12.000000 PythonToSW-1.1.0/src/PythonToSW.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3174 2024-05-14 23:52:12.000000 PythonToSW-1.1.0/src/PythonToSW.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 23:52:12.000000 PythonToSW-1.1.0/src/PythonToSW.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-14 23:52:12.000000 PythonToSW-1.1.0/src/PythonToSW.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-14 23:52:12.000000 PythonToSW-1.1.0/src/PythonToSW.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.585254 PythonToSW-1.1.1/
+-rw-rw-rw-   0        0        0    11558 2024-01-17 15:06:42.000000 PythonToSW-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       92 2024-05-15 22:14:52.000000 PythonToSW-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1731 2024-05-15 22:18:07.584507 PythonToSW-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1197 2024-05-14 16:49:00.000000 PythonToSW-1.1.1/README.md
+-rw-rw-rw-   0        0        0        5 2024-05-15 22:18:04.000000 PythonToSW-1.1.1/VERSION
+-rw-rw-rw-   0        0        0       52 2024-05-15 22:15:14.000000 PythonToSW-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 22:18:07.585254 PythonToSW-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1878 2024-05-15 22:15:23.000000 PythonToSW-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.504328 PythonToSW-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.511925 PythonToSW-1.1.1/src/PythonToSW/
+-rw-rw-rw-   0        0        0      973 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.540181 PythonToSW-1.1.1/src/PythonToSW/addon/
+-rw-rw-rw-   0        0        0      143 2024-05-13 00:11:11.000000 PythonToSW-1.1.1/src/PythonToSW/addon/playlist.xml
+-rw-rw-rw-   0        0        0   159991 2024-05-14 16:56:49.000000 PythonToSW-1.1.1/src/PythonToSW/addon/script.lua
+-rw-rw-rw-   0        0        0    11081 2024-05-15 22:13:20.000000 PythonToSW-1.1.1/src/PythonToSW/addon.py
+-rw-rw-rw-   0        0        0     1868 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/event.py
+-rw-rw-rw-   0        0        0     1064 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.583015 PythonToSW-1.1.1/src/PythonToSW/executions/
+-rw-rw-rw-   0        0        0     2809 2024-05-14 23:36:22.000000 PythonToSW-1.1.1/src/PythonToSW/executions/__createExecution.py
+-rw-rw-rw-   0        0        0     1711 2024-05-14 23:24:00.000000 PythonToSW-1.1.1/src/PythonToSW/executions/__generateImportCode.py
+-rw-rw-rw-   0        0        0     4946 2024-05-15 22:09:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/__init__.py
+-rw-rw-rw-   0        0        0     1059 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addAdmin.py
+-rw-rw-rw-   0        0        0     1056 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addAuth.py
+-rw-rw-rw-   0        0        0     1216 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addMapLabel.py
+-rw-rw-rw-   0        0        0     1220 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addMapLine.py
+-rw-rw-rw-   0        0        0     1582 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/addMapObject.py
+-rw-rw-rw-   0        0        0     1107 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/announce.py
+-rw-rw-rw-   0        0        0     1027 2024-05-14 23:48:22.000000 PythonToSW-1.1.1/src/PythonToSW/executions/cancelGerstner.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/clearOilSpills.py
+-rw-rw-rw-   0        0        0     1028 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/clearRadiation.py
+-rw-rw-rw-   0        0        0     1025 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/clearVehicles.py
+-rw-rw-rw-   0        0        0     1106 2024-05-14 23:49:23.000000 PythonToSW-1.1.1/src/PythonToSW/executions/despawnObject.py
+-rw-rw-rw-   0        0        0     1111 2024-05-14 23:49:25.000000 PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicle.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:49:26.000000 PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicleGroup.py
+-rw-rw-rw-   0        0        0     1105 2024-05-14 18:26:42.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getCharacterItem.py
+-rw-rw-rw-   0        0        0     1079 2024-05-14 18:24:19.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getObjectData.py
+-rw-rw-rw-   0        0        0     1092 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerCharacter.py
+-rw-rw-rw-   0        0        0     1072 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerPos.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getPlayers.py
+-rw-rw-rw-   0        0        0     1035 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getSeasonalEvent.py
+-rw-rw-rw-   0        0        0     1017 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getUniqueID.py
+-rw-rw-rw-   0        0        0     1138 2024-05-14 23:44:48.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1172 2024-05-14 23:44:45.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1102 2024-05-14 18:30:01.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleComponents.py
+-rw-rw-rw-   0        0        0     1084 2024-05-14 18:29:46.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleData.py
+-rw-rw-rw-   0        0        0     1162 2024-05-15 22:08:55.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:44:59.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1163 2024-05-14 23:45:28.000000 PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1012 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/isAridDLC.py
+-rw-rw-rw-   0        0        0     1015 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/isSpaceDLC.py
+-rw-rw-rw-   0        0        0     1021 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/isWeaponsDLC.py
+-rw-rw-rw-   0        0        0     1135 2024-05-14 23:47:34.000000 PythonToSW-1.1.1/src/PythonToSW/executions/notify.py
+-rw-rw-rw-   0        0        0     1068 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeAdmin.py
+-rw-rw-rw-   0        0        0     1065 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeAuth.py
+-rw-rw-rw-   0        0        0     1097 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLabel.py
+-rw-rw-rw-   0        0        0     1094 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLine.py
+-rw-rw-rw-   0        0        0     1100 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removeMapObject.py
+-rw-rw-rw-   0        0        0     1087 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/removePopup.py
+-rw-rw-rw-   0        0        0     1171 2024-05-14 18:25:00.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterData.py
+-rw-rw-rw-   0        0        0     1222 2024-05-14 18:26:10.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterItem.py
+-rw-rw-rw-   0        0        0     1120 2024-05-14 18:25:27.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterTooltip.py
+-rw-rw-rw-   0        0        0     1115 2024-05-14 23:49:29.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setCreatureMoveTarget.py
+-rw-rw-rw-   0        0        0     1089 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setOilSpill.py
+-rw-rw-rw-   0        0        0     1088 2024-05-14 16:56:13.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setPlayerPos.py
+-rw-rw-rw-   0        0        0     1299 2024-05-14 18:18:44.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setPopup.py
+-rw-rw-rw-   0        0        0     1161 2024-05-14 23:43:28.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByName.py
+-rw-rw-rw-   0        0        0     1194 2024-05-14 23:42:27.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByVoxel.py
+-rw-rw-rw-   0        0        0     1126 2024-05-14 23:39:49.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleEditable.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:39:47.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleInvulnerable.py
+-rw-rw-rw-   0        0        0     1097 2024-05-15 22:08:43.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehiclePos.py
+-rw-rw-rw-   0        0        0     1123 2024-05-14 23:39:52.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleShowOnMap.py
+-rw-rw-rw-   0        0        0     1146 2024-05-14 23:43:54.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByName.py
+-rw-rw-rw-   0        0        0     1186 2024-05-14 23:44:14.000000 PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByVoxel.py
+-rw-rw-rw-   0        0        0     1095 2024-05-14 23:46:38.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnCharacter.py
+-rw-rw-rw-   0        0        0     1143 2024-05-14 23:47:06.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnCreature.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:47:30.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnExplosion.py
+-rw-rw-rw-   0        0        0     1128 2024-05-14 23:46:36.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteor.py
+-rw-rw-rw-   0        0        0     1147 2024-05-14 23:45:56.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteorShower.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:58.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnTsunami.py
+-rw-rw-rw-   0        0        0     1093 2024-05-14 23:45:54.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnVolcano.py
+-rw-rw-rw-   0        0        0     1099 2024-05-14 23:45:59.000000 PythonToSW-1.1.1/src/PythonToSW/executions/spawnWhirlpool.py
+-rw-rw-rw-   0        0        0     1618 2024-05-14 17:19:17.000000 PythonToSW-1.1.1/src/PythonToSW/helpers.py
+-rw-rw-rw-   0        0        0     1428 2024-05-15 22:17:00.000000 PythonToSW-1.1.1/src/PythonToSW/matrix.py
+drwxrwxrwx   0        0        0        0 2024-05-15 22:18:07.583761 PythonToSW-1.1.1/src/PythonToSW.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3277 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 22:18:07.000000 PythonToSW-1.1.1/src/PythonToSW.egg-info/top_level.txt
```

### Comparing `PythonToSW-1.1.0/LICENSE` & `PythonToSW-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/PKG-INFO` & `PythonToSW-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.1.0/README.md` & `PythonToSW-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/setup.py` & `PythonToSW-1.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 # ---- // Variables
 with open(os.path.join(os.path.dirname(__file__), "VERSION"), encoding = "utf-8") as file:
     version = file.read()
     print(version)
     
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding = "utf-8") as file:
     long_description = file.read()
-    
 
 # ---- // Main
 setup(
     name= "PythonToSW",
     version = version,
     author = "Cuh4",
     description = "A package that allows you to create addons in Stormworks with Python, handled through HTTP.",
@@ -46,20 +45,13 @@
     license = "Apache License 2.0",
     
     classifiers = [
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     
-    install_requires = [
-        "pyperclip",
-        "requests",
-        "urllib3",
-        "uuid",
-        "xmltodict",
-        "flask"
-    ],
+    install_requires = open("requirements.txt").read().splitlines(),
 
     python_requires = ">=3.12",
     include_package_data = True,
     package_dir = {"": "src"}
 )
```

### Comparing `PythonToSW-1.1.0/src/PythonToSW/__init__.py` & `PythonToSW-1.1.1/src/PythonToSW/__init__.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/addon/script.lua` & `PythonToSW-1.1.1/src/PythonToSW/addon/script.lua`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/addon.py` & `PythonToSW-1.1.1/src/PythonToSW/addon.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,27 +34,27 @@
 from . import helpers
 from . import exceptions
 from . import executions
 from . import Event
 
 # ---- // Main
 class Addon():
-    def __init__(self, addonName: str, port: int, *, showStartupMessage: bool = True):
+    def __init__(self, addonName: str, port: int, *, showStartupMessage: bool = True, destinationAddonPath: str = None):
         self.addonName = addonName
         self.port = port
         self.app = flask.Flask(__name__)
         self.running = False
         self.addonPath = os.path.join(os.path.dirname(__file__), "addon")
-        self.destinationAddonPath = os.path.join(os.getenv("APPDATA"), "Stormworks", "data", "missions")
+        self.destinationAddonPath = destinationAddonPath or os.path.join(os.getenv("APPDATA"), "Stormworks", "data", "missions")
         
         if not os.path.exists(self.addonPath):
             raise exceptions.InternalError(f"Addon path does not exist: {os.path.abspath(self.addonPath)}")
         
         if not os.path.exists(self.destinationAddonPath):
-            raise exceptions.InternalError(f"Addon destination path does not exist: {os.path.abspath(self.destinationAddonPath)}. Please install and run Stormworks: Build and Rescue.")
+            raise exceptions.InternalError(f"Addon destination path does not exist: {os.path.abspath(self.destinationAddonPath)}. Please install and run Stormworks: Build and Rescue.\nIf you are on a non-Windows OS, please provide the destinationAddonPath argument and set it to the location of Stormworks' Stormworks/data/missions folder.")
         
         self.pendingExecutions: dict[str, executions.BaseExecution] = {}
         self.callbacks: dict[str, Event] = {}
         
         self.showStartupMessage = showStartupMessage
         
     # Start the addon
```

### Comparing `PythonToSW-1.1.0/src/PythonToSW/event.py` & `PythonToSW-1.1.1/src/PythonToSW/event.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/exceptions.py` & `PythonToSW-1.1.1/src/PythonToSW/exceptions.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/__createExecution.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/__createExecution.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/__generateImportCode.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/__generateImportCode.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/__init__.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 from .getPlayers import GetPlayers
 from .getSeasonalEvent import GetSeasonalEvent
 from .getUniqueID import GetUniqueID
 from .getVehicleBatteryByName import GetVehicleBatteryByName
 from .getVehicleBatteryByVoxel import GetVehicleBatteryByVoxel
 from .getVehicleComponents import GetVehicleComponents
 from .getVehicleData import GetVehicleData
+from .getVehiclePos import GetVehiclePos
 from .getVehicleTankByName import GetVehicleTankByName
 from .getVehicleTankByVoxel import GetVehicleTankByVoxel
 from .isAridDLC import IsAridDLC
 from .isSpaceDLC import IsSpaceDLC
 from .isWeaponsDLC import IsWeaponsDLC
 from .notify import Notify
 from .removeAdmin import RemoveAdmin
@@ -116,14 +117,15 @@
 from .setOilSpill import SetOilSpill
 from .setPlayerPos import SetPlayerPos
 from .setPopup import SetPopup
 from .setVehicleBatteryByName import SetVehicleBatteryByName
 from .setVehicleBatteryByVoxel import SetVehicleBatteryByName
 from .setVehicleEditable import SetVehicleEditable
 from .setVehicleInvulnerable import SetVehicleInvulnerable
+from .setVehiclePos import SetVehiclePos
 from .setVehicleShowOnMap import SetVehicleShowOnMap
 from .setVehicleTankByName import SetVehicleTankByName
 from .setVehicleTankByVoxel import SetVehicleTankByVoxel
 from .spawnCharacter import SpawnCharacter
 from .spawnCreature import SpawnCreature
 from .spawnExplosion import SpawnExplosion
 from .spawnMeteor import SpawnMeteor
```

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/addAdmin.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/addAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/addAuth.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/addAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/addMapLabel.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/addMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/addMapLine.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/addMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/addMapObject.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/addMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/announce.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/announce.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/cancelGerstner.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/cancelGerstner.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/clearOilSpills.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/clearOilSpills.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/clearRadiation.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/clearRadiation.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/clearVehicles.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/clearVehicles.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/despawnObject.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/despawnObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/despawnVehicle.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicle.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/despawnVehicleGroup.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/despawnVehicleGroup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getCharacterItem.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getObjectData.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getObjectData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getPlayerCharacter.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getPlayerPos.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getPlayers.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getPlayers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getSeasonalEvent.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getSeasonalEvent.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getUniqueID.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getUniqueID.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleBatteryByName.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleBatteryByVoxel.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleComponents.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleComponents.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleData.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleTankByName.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/getVehicleTankByVoxel.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/getVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/isAridDLC.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/isAridDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/isSpaceDLC.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/isSpaceDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/isWeaponsDLC.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/isWeaponsDLC.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/notify.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/notify.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/removeAdmin.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/removeAdmin.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/removeAuth.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/removeAuth.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/removeMapLabel.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLabel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/removeMapLine.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/removeMapLine.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/removeMapObject.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/removeMapObject.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/removePopup.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/removePopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setCharacterData.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterData.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setCharacterItem.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterItem.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setCharacterTooltip.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setCharacterTooltip.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setCreatureMoveTarget.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setCreatureMoveTarget.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setOilSpill.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setOilSpill.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setPlayerPos.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setPlayerPos.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setPopup.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setPopup.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleBatteryByName.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleBatteryByVoxel.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleBatteryByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleEditable.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleEditable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleInvulnerable.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleInvulnerable.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleShowOnMap.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleShowOnMap.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleTankByName.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByName.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/setVehicleTankByVoxel.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/setVehicleTankByVoxel.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnCharacter.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnCharacter.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnCreature.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnCreature.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnExplosion.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnExplosion.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnMeteor.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteor.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnMeteorShower.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnMeteorShower.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnTsunami.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnTsunami.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnVolcano.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnVolcano.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/executions/spawnWhirlpool.py` & `PythonToSW-1.1.1/src/PythonToSW/executions/spawnWhirlpool.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW/helpers.py` & `PythonToSW-1.1.1/src/PythonToSW/helpers.py`

 * *Files identical despite different names*

### Comparing `PythonToSW-1.1.0/src/PythonToSW.egg-info/PKG-INFO` & `PythonToSW-1.1.1/src/PythonToSW.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToSW
-Version: 1.1.0
+Version: 1.1.1
 Summary: A package that allows you to create addons in Stormworks with Python, handled through HTTP.
 Author: Cuh4
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
```

### Comparing `PythonToSW-1.1.0/src/PythonToSW.egg-info/SOURCES.txt` & `PythonToSW-1.1.1/src/PythonToSW.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
+requirements.txt
 setup.py
 src/PythonToSW/__init__.py
 src/PythonToSW/addon.py
 src/PythonToSW/event.py
 src/PythonToSW/exceptions.py
 src/PythonToSW/helpers.py
 src/PythonToSW/matrix.py
@@ -39,14 +40,15 @@
 src/PythonToSW/executions/getPlayers.py
 src/PythonToSW/executions/getSeasonalEvent.py
 src/PythonToSW/executions/getUniqueID.py
 src/PythonToSW/executions/getVehicleBatteryByName.py
 src/PythonToSW/executions/getVehicleBatteryByVoxel.py
 src/PythonToSW/executions/getVehicleComponents.py
 src/PythonToSW/executions/getVehicleData.py
+src/PythonToSW/executions/getVehiclePos.py
 src/PythonToSW/executions/getVehicleTankByName.py
 src/PythonToSW/executions/getVehicleTankByVoxel.py
 src/PythonToSW/executions/isAridDLC.py
 src/PythonToSW/executions/isSpaceDLC.py
 src/PythonToSW/executions/isWeaponsDLC.py
 src/PythonToSW/executions/notify.py
 src/PythonToSW/executions/removeAdmin.py
@@ -62,14 +64,15 @@
 src/PythonToSW/executions/setOilSpill.py
 src/PythonToSW/executions/setPlayerPos.py
 src/PythonToSW/executions/setPopup.py
 src/PythonToSW/executions/setVehicleBatteryByName.py
 src/PythonToSW/executions/setVehicleBatteryByVoxel.py
 src/PythonToSW/executions/setVehicleEditable.py
 src/PythonToSW/executions/setVehicleInvulnerable.py
+src/PythonToSW/executions/setVehiclePos.py
 src/PythonToSW/executions/setVehicleShowOnMap.py
 src/PythonToSW/executions/setVehicleTankByName.py
 src/PythonToSW/executions/setVehicleTankByVoxel.py
 src/PythonToSW/executions/spawnCharacter.py
 src/PythonToSW/executions/spawnCreature.py
 src/PythonToSW/executions/spawnExplosion.py
 src/PythonToSW/executions/spawnMeteor.py
```

